# 🔊 Random Noise Generator Web Tool

A minimalist web interface that generates randomized high-pitch sounds at adjustable intervals, designed for attention training or sound sensitivity testing. Works on both desktop and mobile browsers.

![Demo Screenshot](https://via.placeholder.com/800x500/2c2c2e/FFFFFF?text=Noise+Generator+Demo) *(Replace with actual screenshot)*

## 🌟 Features

- **iPhone-style scroll wheel timer** (0-60 minutes/seconds)
- **Tactile control knobs** for volume and frequency adjustment
- **Randomized sound algorithm**:
  - High-frequency noise (3000-5000Hz)
  - Random durations (0.1-2 seconds)
  - Adjustable frequency intervals (5s-2min)
- **Dark mode UI** with iOS-inspired design
- **Cross-platform** (Mac, iPhone, Windows, Android)

## 🛠️ How It Works

The tool uses:
- Web Audio API for sound generation
- Custom scroll picker with snap-to-center logic
- CSS transforms for knob rotation effects
- Touch/mouse event handling for cross-device support

## 🚀 Usage

1. **Set duration** using the scroll wheels
2. **Adjust controls**:
   - Left knob: Output volume
   - Right knob: Sound frequency
3. **Start/Stop** with dedicated buttons

```html
<!-- Key implementation snippet -->
<script>
  function playNoise() {
    const frequency = 3000 + Math.random() * 2000;
    const duration = 0.1 + Math.random() * 1.9;
    // Audio generation code...
  }
</script>
