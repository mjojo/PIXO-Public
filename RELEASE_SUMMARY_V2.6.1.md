# PIXO v2.6.1 Release Summary ⚡

**Release Date:** October 19, 2025  
**Tag:** v2.6.1  
**Type:** Patch Release (Performance + Bug Fixes)

---

## Quick Stats
- **8 commits** (5 performance + 3 bug fixes)
- **60-100× performance improvement** in cache invalidation
- **20-100× faster** Line tool preview
- **3 critical bugs fixed** (Line mirroring, drawing failure, symmetry)
- **0 breaking changes**

---

## What's Fixed

### Performance 🚀
- Deferred display updates (no more double-rendering)
- Removed duplicate cache invalidations
- Prevented queue_redraw infinite loops
- Optimized Line tool preview rendering
- Cache reuse instead of recreation

### Bugs 🐛
- Line tool no longer draws mirrored/inverted
- Drawing functionality fully restored
- Symmetry works correctly with all tools

---

## Files to Push
```bash
# Push commits
git push origin main

# Push tag
git push origin v2.6.1
```

---

## GitHub Release
1. Go to: https://github.com/mjojo/PIXO/releases/new
2. Tag: `v2.6.1`
3. Title: `v2.6.1 - Performance & Bug Fixes ⚡`
4. Description: Copy from `RELEASE_V2.6.1.md`
5. Attach binaries (if built)
6. Publish release

---

## Announcement Text

```
🎉 PIXO v2.6.1 is out!

This patch release brings massive performance improvements and critical bug fixes:

⚡ Performance:
• 60-100× fewer cache invalidations
• 20-100× faster Line tool preview
• Eliminated render loop spam

🐛 Bug Fixes:
• Fixed Line tool mirroring bug
• Restored drawing functionality
• Fixed symmetry issues

Download: https://github.com/mjojo/PIXO/releases/tag/v2.6.1
Full notes: RELEASE_V2.6.1.md

#pixelart #gamedev #opensource
```

---

## Next Steps
- [ ] Push commits and tag to GitHub
- [ ] Create GitHub Release
- [ ] Build binaries (Windows, Linux, macOS)
- [ ] Update project.godot version number
- [ ] Announce on social media
- [ ] Update documentation if needed
- [ ] Start v2.7 development (Filter System)

---

Made with ❤️ by mjojo GLK Dev
