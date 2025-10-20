# PIXO v2.3 - Custom Brushes System 🖌️
**Release Date:** October 19, 2025  
**Status:** Stable Release

---

## 🎨 What's New

### Custom Brushes System (Feature #1 of v2.3 Roadmap)

PIXO now includes a powerful custom brush system that allows you to paint with predefined patterns and create your own brushes!

#### ✨ Key Features

- **8 Built-in Brushes:**
  - Square - Classic blocky pixel brush
  - Circle (default) - Smooth rounded brush with soft edges
  - Cross - + pattern for textures
  - Diagonal - \ pattern for diagonal textures
  - Noise - Random noise texture (16x16)
  - Soft Circle - Airbrushed gradient effect (16x16)
  - Grass - Vertical lines for vegetation (12x12)
  - Star - 5-pointed star for decorative elements (12x12)

- **Brush Panel UI:**
  - Toggle with Ctrl+B keyboard shortcut
  - Visual thumbnails for all brushes
  - Real-time parameter controls
  - Organized grid layout

- **Adjustable Parameters:**
  - **Size:** 1-32 pixels (affects stamp size)
  - **Spacing:** 0.5-2.0 (controls distance between stamps)
  - **Jitter:** 0.0-0.5 (adds randomness to position)

- **Tool Integration:**
  - Works with Pencil tool (P) for freehand drawing
  - Works with Line tool (L) for straight lines
  - Works with Rectangle tool (R) for outlines
  - Works with Circle tool (C) for circular outlines
  - Works with Eraser tool (E) for pattern erasing

- **Import/Export:**
  - Import PNG/JPG images as custom brushes
  - Save custom brushes to disk
  - Automatic loading of saved brushes
  - Brushes stored in `user://brushes/` directory

---

## 🐛 Bug Fixes

During integration testing, we discovered and fixed **7 critical bugs** that prevented the brush system from working correctly:

### Bug #1: BrushPanel Node Missing
- **Fixed:** Added BrushPanel instance to main.tscn
- **Impact:** System is now functional

### Bug #2: No Immediate Visual Feedback
- **Fixed:** Added `queue_redraw()` to all state change functions
- **Impact:** Tool/brush/color changes now visible immediately

### Bug #3: Bucket Fill Multiple Triggers
- **Fixed:** Implemented one-shot tool pattern with `is_drawing` check
- **Impact:** Bucket fill now executes only once per click

### Bug #4: Bucket Fill Not Visible
- **Fixed:** Set `display_needs_update = true` in bucket handler
- **Impact:** Bucket fill results now appear immediately

### Bug #5: First Pixel Not Visible
- **Fixed:** Added `_update_display()` call after first pixel drawn
- **Impact:** Single clicks with custom brushes now visible immediately

### Bug #6: Cache Not Invalidating
- **Fixed:** Added `composite_cache = null` in `mark_display_dirty()`
- **Impact:** Display updates correctly after drawing

### Bug #7: Line Drawing Not Visible ⭐
- **Fixed:** Added `mark_display_dirty()` to `_draw_line_pixels()` for custom brush path
- **Impact:** Dragging mouse now shows brush strokes in real-time

---

## 🔧 Technical Details

### Architecture
- **CustomBrush Resource:** GDScript Resource class for brush data
- **CustomBrushManager:** Singleton for brush loading/saving
- **BrushPanel:** Scene-based UI with GridContainer layout
- **Integration:** Signals and callbacks connect brush system to main canvas

### Performance
- Brush stamps use efficient pixel-by-pixel blending
- Display caching system with hash-based validation
- Explicit cache invalidation for pixel-level changes
- No performance degradation with large brushes (32px tested)

### Files Modified
- `main.tscn` - Added BrushPanel integration
- `scripts/main.gd` - Signal connections and keyboard shortcuts
- `scripts/drawing_canvas.gd` - Custom brush drawing integration
- `scripts/custom_brush.gd` - Brush Resource implementation (NEW)
- `scripts/custom_brush_manager.gd` - Brush management (NEW)
- `ui/brush_panel.tscn` - Brush selection UI (NEW)
- `ui/brush_panel.gd` - UI logic and parameters (NEW)

---

## 📚 Documentation

New documentation added:
- `docs/features/custom_brushes/CUSTOM_BRUSHES_BUGFIX_SESSION.md` - Detailed bug analysis
- `docs/features/custom_brushes/CUSTOM_BRUSHES_TESTING_GUIDE.md` - Testing procedures

---

## 🎯 How to Use

### Quick Start
1. Press **Ctrl+B** to open brush panel
2. Click any brush thumbnail to select it
3. Press **P** for pencil tool
4. Draw on canvas with custom brush!

### Parameters
- **Size:** Adjust brush stamp size
- **Spacing:** Control distance between stamps (1.0 = no gaps)
- **Jitter:** Add randomness (0.0 = perfect alignment)

### Import Custom Brush
1. Click "Import Brush" button
2. Select PNG or JPG file (16x16 to 32x32 recommended)
3. Brush appears in custom brushes list
4. Draw with your imported brush!

### Save/Load Brushes
- Custom brushes automatically save to `user://brushes/`
- Restart Godot to load saved brushes
- Delete brushes from brush panel

---

## 🚀 What's Next (v2.4 Roadmap)

Planned enhancements:
- [ ] Brush rotation control
- [ ] Color variation per stamp
- [ ] Tablet pressure sensitivity
- [ ] Brush presets/favorites
- [ ] Advanced blend modes
- [ ] Animated brushes

---

## ⚠️ Known Issues

- None currently! All integration bugs have been fixed.

---

## 🙏 Credits

- **Development:** BitVit (mjojo GLK Dev)
- **Testing:** Community feedback
- **Engine:** Godot 4.5

---

## 📄 License

Copyright © 2024-2025 BitVit (mjojo GLK Dev). All Rights Reserved.  
See LICENSE and COPYRIGHT.md for details.

---

## 🎉 Conclusion

Custom Brushes System v2.3 brings professional brush tools to PIXO, enabling more creative and expressive pixel art creation. With 8 builtin brushes, adjustable parameters, and import/export capabilities, artists now have powerful tools at their fingertips.

**Enjoy creating with custom brushes!** 🎨

---

**Previous Releases:**
- v2.2 - Tile Animation System
- v2.1 - Performance Optimizations
- v2.0 - Layer System & Blend Modes
