# 🔒 Steganography Playground

[![Live Demo](https://img.shields.io/badge/Live-Demo-brightgreen)](https://curiousboey.github.io/steganography-playground)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/curiousboey/steganography-playground.svg)](https://github.com/curiousboey/steganography-playground/stargazers)

A professional, interactive web application for demonstrating LSB (Least Significant Bit) steganography techniques. Hide secret messages within images and learn how steganography works through hands-on interactive tutorials.

## 🚀 Features

### Core Functionality
- **🔐 Hide Messages**: Embed secret text messages into images using advanced LSB steganography
- **🔓 Extract Messages**: Retrieve hidden messages from steganographic images
- **🖼️ Format Support**: Compatible with PNG, JPG, JPEG, and other standard image formats
- **💾 Download Results**: Save encoded images with embedded messages

### Interactive Education System
- **🎓 4-Step Learning Process**: Interactive tutorials explaining steganography concepts
- **🔢 Binary Conversion Demo**: Real-time text-to-binary conversion visualization
- **🎨 Pixel Modification Viewer**: See how LSB changes affect image pixels
- **👁️ Visual Comparison**: Side-by-side comparison of original vs steganographic images
- **🔓 Extraction Process**: Step-by-step message retrieval demonstration

### Professional Design
- **🌟 Glass Morphism UI**: Modern, professional design with backdrop blur effects
- **📱 Responsive Layout**: Optimized for all device sizes and screen resolutions
- **🎯 Accessibility**: Full keyboard navigation and screen reader support
- **⚡ Performance**: Optimized for fast loading and smooth interactions

## 🎯 Live Demo

Experience the steganography playground: [**Live Demo**](https://curiousboey.github.io/steganography-playground)

## 🛠️ Technology Stack

- **Frontend**: Pure HTML5, CSS3, JavaScript (ES6+)
- **Styling**: CSS Grid, Flexbox, Custom Properties
- **Fonts**: Google Fonts (Inter, Fira Code)
- **Canvas API**: For image processing and steganography operations
- **No Dependencies**: Completely self-contained, no external libraries required

## 📋 Quick Start

### Method 1: Direct Download
1. Download or clone this repository
2. Open `index.html` in any modern web browser
3. Start hiding and extracting messages!

### Method 2: GitHub Pages
1. Fork this repository
2. Enable GitHub Pages in repository settings
3. Access your live version at `https://curiousboey.github.io/steganography-playground`

### Method 3: Local Development
```bash
git clone https://github.com/curiousboey/steganography-playground.git
cd steganography-playground
# Open index.html in your preferred browser
```

## 📖 How It Works

### LSB Steganography Algorithm

The application uses **Least Significant Bit (LSB) steganography** to hide messages:

1. **Text Encoding**: Secret message is converted to binary format
2. **Pixel Modification**: Binary data is embedded into the least significant bits of image pixels
3. **Imperceptible Changes**: Modifications are so small they're invisible to human eyes
4. **Message Extraction**: Hidden data is retrieved by reading LSBs from pixels

### Technical Implementation

```javascript
// Example: Hiding a message
const binaryMessage = textToBinary(secretMessage);
for (let i = 0; i < binaryMessage.length; i++) {
    imageData[i * 4] = (imageData[i * 4] & 0xFE) | parseInt(binaryMessage[i]);
}
```

## 🎮 Usage Guide

### Hiding a Message
1. **Upload Image**: Click "Choose Image File" and select your cover image
2. **Enter Message**: Type your secret message in the text area
3. **Process**: Click "Encrypt & Hide Message" to embed the data
4. **Download**: Save the resulting steganographic image

### Extracting a Message
1. **Upload Encoded Image**: Select an image containing hidden data
2. **Extract**: Click "Decrypt & Extract Message" to reveal the secret
3. **View Result**: The hidden message will be displayed

### Interactive Learning
1. **Explore Demos**: Click on the 4 educational cards to learn each step
2. **Text-to-Binary**: Type in the interactive input to see binary conversion
3. **Pixel Visualization**: Click pixels to see LSB modifications
4. **Step Through Process**: Use the extraction demo to understand retrieval

## 🔧 Customization

### Embedding in Other Sites
The application is designed to be easily embedded:

```html
<iframe src="path/to/index.html" width="100%" height="800px" frameborder="0"></iframe>
```

### Color Scheme Customization
Modify CSS custom properties in the `:root` selector:

```css
:root {
    --primary-color: #64ffda;    /* Accent color */
    --secondary-color: #82b1ff;  /* Secondary accent */
    --primary-bg: #0a0f1c;       /* Main background */
    /* ... more variables */
}
```

## 🔒 Security Considerations

- **Educational Purpose**: This tool is designed for learning and demonstration
- **No Encryption**: Messages are hidden but not encrypted
- **Format Limitations**: Some image formats may not preserve hidden data
- **Detection**: Advanced steganalysis tools can detect LSB steganography

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### Development Guidelines
- Follow existing code style and conventions
- Test all functionality across different browsers
- Ensure responsive design works on all screen sizes
- Add comments for complex algorithms

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Steganography Research**: Based on academic research in digital steganography
- **Design Inspiration**: Modern glass morphism and cyberpunk aesthetics
- **Educational Focus**: Inspired by interactive learning platforms

## 📞 Support

- **Issues**: [GitHub Issues](https://github.com/curiousboey/steganography-playground/issues)
- **Discussions**: [GitHub Discussions](https://github.com/curiousboey/steganography-playground/discussions)
- **Documentation**: This README and inline code comments

## 🌟 Star History

If you find this project useful, please consider giving it a star! ⭐

---

**Made with ❤️ for cybersecurity education and digital privacy awareness**
