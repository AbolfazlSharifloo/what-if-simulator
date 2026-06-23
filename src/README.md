# What If? Simulator

[![Live Demo](https://img.shields.io/badge/demo-live-green.svg)](https://sharifloo-net.github.io/what-if-simulator/)

## Overview
A Progressive Web App (PWA) that explores hypothetical "What If?" scenarios and their structured consequences of six key categories: Daily Life, Economy, Technology, Social Structure, Advantages, and Problems. The application allows users to explore preloaded scenarios, create custom ones, and even generate new scenarios using AI.

## 🚀 Features

### Core Functionality
- **Preloaded Scenarios**: Explore thought-provoking scenarios with detailed consequences
- **Custom Scenarios**: Create and save your own "What If?" scenarios
- **AI-Powered Generation**: Generate new scenarios using external LLM integration (with fallback to built-in generator)
- **Favorites System**: Bookmark your favorite scenarios for quick access
- **Data Management**: Import/export scenarios as JSON files
- **Search & Filter**: Quickly find scenarios by title or content
- **Keyboard Navigation**: Intuitive controls (arrows to navigate, 'F' to favorite)
- **Offline Support**: Full PWA functionality with service worker caching
- **Responsive Design**: Optimized for both desktop and mobile devices

### Technical Highlights
- **Progressive Web App**: Installable on devices with offline support
- **Zero Dependencies**: Built with vanilla JavaScript, HTML5, and CSS3
- **Lightweight**: Fast loading with minimal resource usage
- **Data Persistence**: All scenarios saved in browser's localStorage
- **Accessibility**: Keyboard navigation and semantic HTML

## 📁 Project Structure

```
what-if-sim/
├── index.html          # Main application entry point
├── styles.css          # Responsive styling with CSS custom properties
├── app.js              # Core application logic and functionality
├── service-worker.js   # Service worker for offline capabilities
├── manifest.json       # PWA configuration
├── icons/              # App icons for various platforms
└── README.md           # This documentation
```

## 🛠️ Installation & Setup

### Local Development
1. Clone the repository
2. Open `index.html` directly in a modern web browser
   - Or serve using a local server:
     ```bash
     # Using Python (any version)
     python -m http.server 5000
     ```
     Then visit `http://localhost:5000`

### PWA Installation
1. Deploy the app to a web server (HTTPS required for service worker)
2. Visit the deployed URL in a modern browser
3. Click the install prompt (browser-dependent) or use the browser's "Add to Home Screen" option

### APK Generation (Android)
1. Deploy to an HTTPS server
2. Visit [PWABuilder](https://www.pwabuilder.com/)
3. Enter your deployed URL
4. Click "Build My PWA" and select Android
5. Download and sign the generated APK

## 🔍 Usage Guide

### Exploring Scenarios
- Use the sidebar to browse available scenarios
- Click on any scenario to view its details
- Use the search bar to filter scenarios
- Press 'F' to toggle favorite status
- Use keyboard arrows to navigate between scenarios

### Creating Custom Scenarios
1. Click "Create New Scenario"
2. Fill in the scenario title and description
3. Add bullet points to each category
4. Save to add to your collection

### AI-Powered Generation
1. Click "Generate with AI"
2. Enter a scenario idea
3. (Optional) Provide an API key for enhanced generation
4. Review and save the generated scenario

## 🔄 Data Management

### Exporting Scenarios
1. Click "Export Scenarios"
2. A JSON file will be downloaded containing all your scenarios

### Importing Scenarios
1. Click "Import Scenarios"
2. Select a previously exported JSON file
3. Choose whether to merge or replace existing scenarios

## 🗄️ Data Storage
- Scenarios are stored in the browser's localStorage with the key: `whatif-scenarios-v1`
- AI API key (if provided) is stored with the key: `whatif-ai-apikey-v1`
- Favorites and quick access preferences are stored in localStorage

## 🌐 Browser Support
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile Safari (iOS 13+)
- Chrome for Android

## 📝 License
This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## 📬 Contact
For feature requests or bug reports, please open an issue on the repository.
