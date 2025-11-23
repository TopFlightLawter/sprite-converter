# ESP32 Sprite Converter PWA

Convert your pixel art to RGB565 C arrays for ESP32 displays - installable as a Progressive Web App!

## Features

- 🎨 **Dark Mode UI** - Easy on the eyes with neon blue, lime green, and yellow accents
- 📱 **PWA Ready** - Install on your iPad as a standalone app
- 🖼️ **Template Library** - Download pre-sized templates for ArtStudio Pro
- 🔄 **Live Preview** - See original vs RGB565 conversion side-by-side
- 💾 **Gallery System** - Save all your sprites with localStorage
- 📋 **Copy Code** - One-click copy of generated C arrays
- ⚡ **Offline Support** - Works without internet once installed

## Deployment to GitHub Pages

### Option 1: Using GitHub Web Interface (Easiest)

1. **Create a new repository on GitHub:**
   - Go to https://github.com/new
   - Name it `sprite-converter` (or any name you like)
   - Make it Public
   - Don't add README, .gitignore, or license
   - Click "Create repository"

2. **Upload files:**
   - Click "uploading an existing file"
   - Drag and drop these 3 files:
     - `index.html`
     - `manifest.json`
     - `service-worker.js`
   - Commit changes

3. **Enable GitHub Pages:**
   - Go to repository Settings → Pages
   - Under "Source", select "main" branch
   - Click Save
   - Your site will be live at: `https://yourusername.github.io/sprite-converter/`

### Option 2: Using Git (If you have Git installed on laptop)

```bash
# Navigate to the sprite-converter-pwa folder
cd "C:\Users\topfl\OneDrive\Documents\AI Transfers\Prompt Storage\Here\sprite-converter-pwa"

# Initialize git repository
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit - ESP32 Sprite Converter PWA"

# Add your GitHub repository as remote
git remote add origin https://github.com/YOUR_USERNAME/sprite-converter.git

# Push to GitHub
git branch -M main
git push -u origin main
```

Then enable GitHub Pages in repository settings (step 3 above).

## Installing on iPad

Once deployed to GitHub Pages:

1. **Open Safari on your iPad**
2. **Navigate to your GitHub Pages URL**
3. **Tap the Share button** (square with arrow)
4. **Scroll down and tap "Add to Home Screen"**
5. **Tap "Add"**

The app will now appear on your iPad home screen like a native app!

## Usage

1. **Download a template** from the Templates tab
2. **Edit in ArtStudio Pro** - create your pixel art
3. **Upload your finished art** in the Converter tab
4. **Save to Gallery** or immediately copy the generated code
5. **Paste into your ESP32 sketch** and use with `sprite.pushImage()`

## Technical Details

- **RGB565 Conversion** - Optimized for ESP32 TFT displays
- **Transparent Pixels** - Automatically converted to white
- **Memory Calculation** - Shows exact bytes needed for PROGMEM
- **C Array Format** - Ready to paste into Arduino/ESP32 sketches

## Browser Compatibility

- ✅ Safari (iOS/iPadOS)
- ✅ Chrome (Desktop/Mobile)
- ✅ Edge
- ✅ Firefox

## License

Free to use for personal and commercial projects!
