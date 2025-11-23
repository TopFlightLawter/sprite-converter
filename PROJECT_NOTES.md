# ESP32 Sprite Converter - Project Notes

## Project Overview
Built: 2025-01-18
Tool for converting pixel art to RGB565 C arrays for ESP32 displays

## Live URL
https://TopFlightLawter.github.io/sprite-converter/

## What We Built

### Version 1.0 Features
- ✅ Dark mode UI (black, neon blue, lime green, yellow accents)
- ✅ PNG/JPG upload with drag & drop
- ✅ RGB565 conversion with live preview
- ✅ C++ code generation for ESP32
- ✅ Gallery system with localStorage
- ✅ Template library with actual pixel art
- ✅ PWA support (installable on iPad)
- ✅ Offline functionality

### Templates Included
**Characters:**
- Character Front (32x32)
- Character Side (32x32)
- Chibi Character (32x32)
- Character Front 64x64

**Items:**
- Coin, Heart, Sword, Potion Bottle, Treasure Chest, Key

**UI Elements:**
- Buttons (small/medium)
- Icons (16x16)

**Backgrounds:**
- Full Screen (480x320)

## Workflow
1. Download template from app
2. Edit in ArtStudio Pro on iPad
3. Upload customized sprite
4. Generate C++ code or save to gallery
5. Copy code into ESP32 sketch

## Version 2.0 Ideas (Future)
- Animation timeline system
- Batch processing
- Built-in pixel editor
- WebSerial device integration
- Sprite sheet packer/unpacker
- Advanced code generation (complete sketches)
- AI background removal
- Display simulator

## Files Location
Local: `C:\Users\topfl\OneDrive\Documents\AI Transfers\Prompt Storage\Here\sprite-converter-pwa\`

Files:
- index.html (main app)
- manifest.json (PWA config)
- service-worker.js (offline support)
- README.md (deployment instructions)

## GitHub Repository
Owner: TopFlightLawter
Repo: sprite-converter
Branch: main

## Updating the App
1. Edit local files
2. Commit to GitHub
3. GitHub Pages auto-deploys (~1 min)
4. Clear iPad Safari cache to see changes
5. Rerun "AppMaker" shortcut if needed

## Technical Details
- RGB565 format (16-bit color)
- Transparent pixels → white
- PROGMEM arrays for ESP32
- localStorage limit: ~5-10MB
- Works with: ST7796, ILI9341, ILI9488 displays

## Support
- GitHub Issues: https://github.com/TopFlightLawter/sprite-converter/issues
- This conversation saved in Claude Code history
