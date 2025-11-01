# Professional Image Resizer 🎨

A powerful, feature-rich web application for resizing, editing, and converting images - all processed locally in your browser with zero server uploads!

![Version](https://img.shields.io/badge/version-2.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![JavaScript](https://img.shields.io/badge/javascript-ES6+-yellow.svg)

## ✨ Features

### 🖼️ Image Upload & Management
- **Drag & Drop Support** - Simply drag images into the browser
- **File Browser** - Traditional file selection
- **Multiple Format Support** - JPG, PNG, WebP, GIF
- **Large File Handling** - Support for files up to 50MB
- **Real-time Preview** - Instant visual feedback

### 📏 Advanced Resizing
- **Percentage Scaling** - Resize from 1% to 200% of original size
- **Custom Dimensions** - Set exact width and height in pixels
- **Aspect Ratio Lock** - Maintain proportions or resize freely
- **Preset Dimensions** - Quick access to common sizes:
  - 1080p (1920×1080)
  - 4K (3840×2160)
  - Square (1080×1080)
  - Instagram (1080×1350)
  - Facebook (1200×630)
  - Twitter (1024×512)

### ✂️ Crop Tools
- **Visual Crop Mode** - Interactive crop overlay
- **Aspect Ratio Presets**:
  - Free (no constraints)
  - 1:1 (Square)
  - 4:3 (Standard)
  - 16:9 (Widescreen)
  - 9:16 (Story/Vertical)
  - 4:5 (Portrait)

### 🎨 Image Filters
- **Original** - No filter
- **Grayscale** - Classic black & white
- **Sepia** - Vintage brown tone
- **Invert** - Negative colors
- **Vintage** - Old photo effect
- **Cool** - Blue-tinted
- **Warm** - Orange-tinted
- **Vibrant** - Enhanced saturation

### 🎚️ Fine-tune Adjustments
- **Brightness** - 0% to 200%
- **Contrast** - 0% to 200%
- **Saturation** - 0% to 200%
- **Blur** - 0px to 20px
- **Hue Rotation** - 0° to 360°
- **One-click Reset** - Restore all adjustments

### 🔄 Transform Tools
- **Rotate** - 90° left or right
- **Flip** - Horizontal or vertical mirroring
- **Non-destructive** - All transformations are reversible

### 💾 Export Options
- **Multiple Formats**:
  - JPEG (best for photos)
  - PNG (lossless, transparency support)
  - WebP (modern, efficient compression)
- **Quality Control** - Adjust compression from 1% to 100%
- **File Size Comparison** - See before/after file sizes
- **Custom Naming** - Automatic "_resized" suffix

### 🎭 User Interface
- **Dark Mode** - Toggle between light and dark themes
- **Responsive Design** - Works on desktop, tablet, and mobile
- **Tab Organization** - Resize, Crop, Filters, Adjust, Transform
- **Toast Notifications** - Helpful feedback messages
- **Loading Indicators** - Visual processing feedback
- **Keyboard Shortcuts**:
  - `Ctrl/Cmd + D` - Download image
  - `Ctrl/Cmd + Z` - Reset all changes

### 🔒 Privacy & Security
- **100% Client-Side** - No server uploads, all processing in browser
- **No Data Collection** - Your images never leave your device
- **Offline Capable** - Works without internet after initial load
- **Secure** - No third-party services or tracking

## 🚀 Getting Started

### Quick Start
Simply open `index.html` in a modern web browser!

### Using a Local Server
For the best experience, use a local server:

```bash
# Using Python 3
python -m http.server 8080

# Using Python 2
python -m SimpleHTTPServer 8080

# Using Node.js http-server
npx http-server -p 8080

# Using the package.json script
npm start
```

Then open `http://localhost:8080` in your browser.

### Using Live Server (Recommended for Development)
```bash
npm run dev
```

## 📖 How to Use

1. **Upload an Image**
   - Drag and drop an image onto the upload area
   - Or click "Browse Files" to select an image

2. **Edit Your Image**
   - Use the **Resize** tab to change dimensions
   - Switch to **Crop** for cropping tools
   - Apply **Filters** for instant effects
   - Fine-tune with **Adjust** sliders
   - Use **Transform** for rotation/flipping

3. **Download**
   - Choose your export format (JPEG/PNG/WebP)
   - Adjust quality settings
   - Click "Download Image"

## 🛠️ Technical Details

### Technologies Used
- **HTML5** - Semantic markup
- **CSS3** - Modern styling with CSS variables
- **Vanilla JavaScript** - No frameworks, pure ES6+
- **Canvas API** - Image processing and rendering
- **LocalStorage** - Theme preference persistence

### Browser Compatibility
- ✅ Chrome/Edge 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Opera 76+

### File Structure
```
Image-resizer/
├── index.html          # Main HTML structure
├── index.css           # Comprehensive styles with dark mode
├── index.js            # Full-featured JavaScript
├── package.json        # Project configuration
├── README.md           # Documentation
├── background.jpg      # Background image
└── upload_icon.svg     # Upload icon
```

## 🎯 Use Cases

- **Social Media** - Resize images for different platforms
- **Web Development** - Optimize images for websites
- **Photography** - Quick edits and filters
- **Design** - Prepare assets with exact dimensions
- **Compression** - Reduce file sizes without quality loss
- **Format Conversion** - Convert between JPEG, PNG, WebP

## 🌟 Highlights

### Performance
- Efficient canvas-based processing
- Smooth 60fps UI animations
- Lazy loading and optimized rendering

### Accessibility
- Keyboard navigation support
- Focus indicators
- Screen reader friendly
- Semantic HTML

### Responsive
- Mobile-first design
- Touch-friendly controls
- Adaptive layouts
- Flexible grid system

## 📝 Features Breakdown

| Feature | Description | Status |
|---------|-------------|--------|
| Drag & Drop Upload | Upload images by dragging | ✅ |
| Multiple Formats | JPG, PNG, WebP, GIF | ✅ |
| Percentage Resize | Scale 1-200% | ✅ |
| Custom Dimensions | Exact pixel control | ✅ |
| Aspect Ratio Lock | Maintain proportions | ✅ |
| Preset Sizes | Quick common dimensions | ✅ |
| Visual Crop | Interactive cropping | ✅ |
| 8 Image Filters | Instant effects | ✅ |
| 5 Adjustments | Fine-tune controls | ✅ |
| Rotate & Flip | Transform tools | ✅ |
| Format Conversion | JPEG/PNG/WebP export | ✅ |
| Quality Control | 1-100% compression | ✅ |
| Dark Mode | Theme toggle | ✅ |
| File Size Stats | Before/after comparison | ✅ |
| Keyboard Shortcuts | Quick actions | ✅ |
| Toast Notifications | User feedback | ✅ |
| Responsive Design | All devices | ✅ |

## 🔧 Customization

### Change Default Settings
Edit `index.js` to modify default values:

```javascript
// Default quality
elements.qualitySlider.value = 90; // Change to your preference

// Default aspect ratio lock
state.isAspectRatioLocked = true; // true or false

// Max file size (in bytes)
if (file.size > 50 * 1024 * 1024) // Change 50 to your limit
```

### Add Custom Presets
In `index.html`, add new preset buttons:

```html
<button class="preset-btn" data-width="1280" data-height="720">720p</button>
```

### Modify Theme Colors
Edit CSS variables in `index.css`:

```css
:root {
  --bg-primary: #your-color;
  --text-accent: #your-color;
  /* ... */
}
```

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests
- Improve documentation

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👨‍💻 Author

**Abhay Gupta**
- GitHub: [@Abs6187](https://github.com/Abs6187)
- Repository: [Image-resizer](https://github.com/Abs6187/Image-resizer)

## 🙏 Acknowledgments

- Font Awesome for icons
- Google Fonts for Inter typeface
- Canvas API documentation
- Web development community

## 📊 Statistics

- **Lines of Code**: 1800+
- **File Size**: ~45KB (uncompressed)
- **Features**: 30+
- **Supported Formats**: 4 (JPG, PNG, WebP, GIF)
- **Export Formats**: 3 (JPG, PNG, WebP)

## 🔮 Future Enhancements

Potential features for future versions:
- [ ] Batch processing for multiple images
- [ ] Advanced crop with freehand selection
- [ ] More filter presets
- [ ] Text and watermark overlay
- [ ] Image comparison slider
- [ ] History/Undo system
- [ ] Cloud storage integration
- [ ] PWA support for offline use
- [ ] Image format metadata preservation

## 📞 Support

If you encounter any issues or have questions:
1. Check the [Issues](https://github.com/Abs6187/Image-resizer/issues) page
2. Create a new issue with details
3. Contact via GitHub

---

**Made with ❤️ by Abhay Gupta**

*Star ⭐ this repository if you find it helpful!*
