# Aura-Pal Web Dashboard ✨

A cute, minimalistic, and modern tech dashboard designed as the web interface for the **Aura-Pal** mini AI assistant robot. It features a responsive layout, beautiful animated backgrounds, and interactive fidget toys.

This dashboard is designed to connect to an ESP32 robot equipped with OpenCV to display FER2013 emotion analysis.

## 📂 Project Files

- **`index.html`**
  The main HTML document defining the physical structure of the dashboard. It features a large, dynamic central Reacting Face (`#bigFace`), a hidden hover-reveal stats panel for the 7 standard FER2013 emotions, and compact input feeds tucked into the corner.

- **`style.css`**
  The custom stylesheet responsible for the "modern cozy vibe". It uses pastel CSS variables for theming, implements a frosted glassmorphism design system (`.glass-panel`), and defines extensive CSS `@keyframes` that map to Javascript intensity classes to dynamically scale miniature emotion decorations based on confidence rates.

- **`script.js`**
  The logic powerhouse of the dashboard. It handles:
  1. **ESP32 Mock Stream**: Simulates receiving emotion payloads from a WebSocket. 
  2. **Emotion Rendering**: Dynamically updates the central face shape, quotes, and scales decoration intensity based on the primary emotion confidence.
  3. **Webcam Integration**: Can access the user's local webcam for standalone interactive testing.
  4. **Image Uploading**: Allows the user to upload a static image to be "analyzed".
  5. **Interactive Fidget Features**: Drives the global particle click effect system.

## 🚀 Usage

You can launch this project simply by opening `index.html` in any modern web browser. No complex build tools or local servers are required to test the UI thanks to the built-in standalone mock modes!

### To Connect to a Real Backend:
Refer to the commented-out section at the bottom of `script.js` titled `--- HOW TO CONNECT TRUE BACKEND ---` for an example of how to link this frontend to a real WebSocket streaming from the ESP32.

<a href="https://ayushman-pyne.github.io/Aura-Pal/" style="display: inline-block; padding: 12px 24px; background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; text-decoration: none; border-radius: 8px; font-weight: 600; font-size: 16px; box-shadow: 0 4px 15px rgba(102, 126, 234, 0.4); transition: transform 0.2s, box-shadow 0.2s;">
    Go to Website →
  </a>
