# CHANGELOG

All notable changes to this project are documented in this file.

## [2.6.1] - 2025-10-19 ⚡ Performance & Bug Fixes
### Performance Optimizations
- **Deferred Display Updates:** Moved `_update_display()` from `mark_canvas_dirty()` to `_draw()` 
  - Eliminates double-rendering (was rendering twice per operation)
  - Display updates once per frame when needed instead of immediately
- **Cache Invalidation Optimization:** Removed duplicate `mark_display_dirty()` calls
  - `_draw_line_pixels()` no longer invalidates cache (tool handles it)
  - Removed from custom brush line drawing
  - Result: 60-100× fewer cache invalidations
- **Queue Redraw Loop Prevention:** Added `in_draw_call` flag
  - Prevents infinite loop: `_draw() → _update_display() → queue_redraw() → _draw()`
  - `_update_display()` only calls `queue_redraw()` when NOT inside `_draw()`
- **Line Tool Preview Performance:** 20-100× improvement
  - Apply symmetry to line endpoints instead of every brush pixel
  - Reduces draw calls from 10,000+ to ~100-500 per frame
- **Cache Reuse Optimization:** `composite_cache` no longer destroyed on every invalidation
  - Image object reused instead of recreated
  - Significant memory allocation reduction

### Bug Fixes
- **Line Tool Mirroring Bug:** Fixed lines drawing mirrored/inverted in certain directions
  - Disabled buggy pixel-perfect line algorithm
  - Restored reliable Bresenham line drawing for all directions
  - Pixel-perfect algorithm had coordinate swapping issues with diagonal lines
- **Drawing Functionality Restored:** Fixed complete drawing failure after optimization
  - Restored `_update_display()` call while keeping cache reuse optimization
  - Balance between performance and functionality
- **Line Tool with Symmetry:** Now works correctly with all symmetry modes
  - Proper endpoint symmetry application
  - No more double-mirroring artifacts

### Technical Details
- 8 commits: 5 performance optimizations + 3 bug fixes
- Console spam "[CACHE] Rendering new composite" eliminated
- Smooth Line tool operation even with large brush sizes
- All tools tested and working correctly

### Known Issues
- Pixel-perfect line algorithm disabled (will be fixed in future release)
- Currently using standard Bresenham algorithm (reliable but less smooth)

## [2.6.0] - 2025-10-19 🎨 Reference Images & Pixel Perfect Lines
### Added
- **Reference Image System:** Load PNG/JPEG images as non-destructive reference sketches
  - View → Load Reference Image... to import reference
  - Adjustable opacity slider (0-100%, default 50%)
  - Show/Hide toggle for quick visibility control
  - Reference drawn behind canvas (non-destructive)
  - Clear reference when done
- **Pixel Perfect Lines:** Improved line rendering algorithm for pixel art
  - Minimizes "jaggies" (stepped appearance) in lines
  - Smooth, aesthetically pleasing lines for pixel art
  - Better than standard Bresenham algorithm
  - Uses interpolation with rounding for optimal results
  - Toggle on/off via View → Pixel Perfect Lines
- **Mirror Drawing Mode Improvements:**
  - Dashed guide lines for symmetry axes (more professional appearance)
  - Improved radial symmetry visualization
  - Show/Hide symmetry axes toggle (View → Show Symmetry Axes)
  - API for axis position control
- **UI Enhancements:**
  - View menu items for all drawing aids
  - Status notifications for feature toggles
  - FileDialog configuration fix for "Open PNG"

### Technical
- Reference image rendering in _draw() with opacity support
- _pixel_perfect_line() algorithm with steep/shallow line handling
- _draw_dashed_line() and _draw_dashed_circle() for guide visualization
- Symmetry axes control functions: set_symmetry_axis_position(), reset_symmetry_axes()
- ~300 lines of new code for reference and drawing improvements

## [2.5.0] - 2025-10-19 🔧 Tool System Refactoring
### Added
- **Tool System Architecture:** Extracted 6 drawing tools into dedicated classes
  - ToolBase: Base class with common tool interface
  - PencilTool, EraserTool, BucketTool: Basic drawing tools
  - LineTool, RectangleTool, CircleTool: Shape tools
  - Total: ~708 lines in 7 new files
- **Tile Animation Tab:** Moved Tile Animation Editor from popup window to TabContainer
  - Better UX consistency with other panels
  - Always accessible without menu navigation
  - ~30 lines added, ~170 lines removed (window code)

### Fixed
- 12 bugs fixed during Tool System integration:
  - Tool switching and state management
  - Preview rendering for shapes
  - Symmetry modes with all tools
  - Brush sizes consistency
  - Undo/Redo integration
  - Cursor preview for eraser
  - Tool activation feedback
  - And more...

### Removed
- Deprecated code cleanup (~240 lines):
  - Old preview functions (_draw_preview_line, _draw_preview_rectangle, _draw_preview_circle)
  - Old shape functions (_finalize_shape, _draw_rectangle, _draw_circle, _draw_circle_points)
  - Tile Animation window code (moved to tab)

### Technical
- Tool System integration in drawing_canvas.gd (~50 lines)
- Each tool handles own input, preview, and drawing logic
- Cleaner separation of concerns
- Better maintainability for future tool additions

## [2.3.0] - 2025-10-19 🖌️ Custom Brushes
### Added
- **Custom Brushes System:** Complete brush system with 8 builtin brushes (Square, Circle, Cross, Diagonal, Noise, Soft Circle, Grass, Star)
- Brush Panel UI with visual thumbnails (toggle with Ctrl+B)
- Adjustable brush parameters: Size (1-32), Spacing (0.5-2.0), Jitter (0.0-0.5)
- Import custom brushes from PNG/JPG images
- Save/Load custom brushes to user://brushes/
- Integration with all drawing tools (Pencil, Line, Rectangle, Circle, Eraser)
- Real-time brush preview and immediate visual feedback

### Fixed
- BrushPanel node integration in main scene
- Immediate visual feedback for tool/brush/color changes (queue_redraw)
- Bucket fill multiple trigger issue (one-shot tool pattern)
- Bucket fill display not updating immediately
- First pixel not visible with custom brushes
- Display cache not invalidating after pixel changes
- Line drawing not visible when dragging with custom brushes

### Technical
- New CustomBrush Resource class for brush data
- CustomBrushManager singleton for brush management
- Hash-based display caching with explicit invalidation
- Performance optimized for brushes up to 32px

## [2.2.0] - 2025-10-18 🎬 Tile Animation
### Added
- Tile Animation System for animated tiles/sprites
- Animation timeline and keyframe editor
- Multiple animations per tileset
- Real-time preview in canvas

## [2.1.1] - 2025-10-18
### Added
- Resource-based project persistence: new Godot Resource classes `PixelLayer`, `PixelFrame`, `PixelProject` and support for saving/loading projects as `.tres`.
- "Save as Resource (.tres)" UI action (File → Save as Resource) and file dialog.
- Multi-frame project save/load via `.tres` (preserves frames/layers and Image data).
- Quick Wins sprint selection added to roadmap (Recent files, Quick Open, Export selected area, Drag & Drop improvements).
- Godot integration proposals added to roadmap: Godot Editor Plugin, Live Importer/Auto-sync, Runtime PIXO Loader, Godot Tileset Exporter, CLI exporter and One-click "Open in Godot".

### Changed
- The roadmap (`ROADMAP.md`) has been consolidated and expanded with roadmap expansion items; project is now tracking v2.2 in-progress.

### Notes / Migration
- Legacy `.pixo` JSON format remains supported; loader includes migration to internal resource structures when opening legacy projects. When possible, save projects as `.tres` to take advantage of Godot-native inspection and editor features.

---

_For full development notes and design decisions see `ROADMAP.md` and commit history._
