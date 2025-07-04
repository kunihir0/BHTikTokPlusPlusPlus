# BHTikTok++

An awesome tweak for TikTok!

[![Documentation](https://img.shields.io/badge/docs-comprehensive-blue.svg)](docs/)
[![Platform](https://img.shields.io/badge/platform-iOS-lightgrey.svg)](https://developer.apple.com/ios/)
[![Language](https://img.shields.io/badge/language-Objective--C-orange.svg)](https://developer.apple.com/library/archive/documentation/Cocoa/Conceptual/ProgrammingWithObjectiveC/Introduction/Introduction.html)
[![Framework](https://img.shields.io/badge/framework-Theos-red.svg)](https://theos.dev/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Documentation](#documentation)
- [Installation](#installation)
- [Configuration](#configuration)
- [Development](#development)
- [Contributing](#contributing)

## 🎯 Overview

BHTikTok++ is a comprehensive iOS tweak that enhances the TikTok experience by providing additional features such as ad blocking, video downloading, UI customization, and various privacy and convenience features. Built using the Theos framework, it integrates seamlessly with TikTok's existing functionality while adding powerful new capabilities.

### Key Highlights

- 🚫 **Complete Ad Removal** - Eliminate all advertisements from your TikTok feed
- 📥 **Advanced Download System** - Download videos, photos, and music in various formats
- 🎨 **UI Customization** - Hide elements, adjust transparency, and customize the interface
- 🔒 **Privacy & Security** - App lock, jailbreak detection bypass, and privacy controls
- 🌍 **Region Spoofing** - Access content from different regions and countries
- ⚡ **Performance Enhancements** - Auto-play controls, speed adjustments, and optimization
- 👤 **Profile Modifications** - Fake verification, follower counts, and enhanced profiles

## ✨ Features

### 📱 Feed Enhancements
- **No Ads** - Complete advertisement removal from feed and UI
- **Download Videos** - Download videos in standard and HD quality
- **Download Photos** - Save photo albums and individual images
- **Download Music** - Extract and save audio content
- **Upload Region Display** - Show country flags next to usernames
- **Show Username** - Display actual usernames instead of display names
- **Disable Pull-to-refresh** - Prevent accidental feed refreshes
- **Disable Sensitive Content Warnings** - Bypass content sensitivity filters
- **Disable Warnings** - Hide TikTok warning messages
- **Disable Live Broadcast** - Filter out live streaming content
- **Skip Recommendations** - Auto-skip recommendation cards
- **Remove Watermark** - Remove TikTok watermarks from videos
- **Show/Hide UI Button** - Toggle interface elements visibility
- **Copy Video Description** - Copy video captions and descriptions
- **Copy Video Link** - Copy direct video URLs
- **Copy Music Link** - Copy audio track URLs
- **Auto Play Next Video** - Automatically advance to next video
- **Show Progress Bar** - Display video progress indicators
- **Transparent Comments** - Make comment overlays semi-transparent

### 👤 Profile Features
- **Save Profile Image** - Long-press to save profile pictures
- **Copy Profile Information** - Copy user bio and profile details
- **Profile Video Count** - Display total number of uploaded videos
- **Video Like Count** - Show like counts on profile videos
- **Video Upload Date** - Display when videos were uploaded
- **Fake Verification** - Add verification badges to profiles
- **Fake Follower Count** - Customize displayed follower numbers
- **Fake Following Count** - Customize displayed following numbers
- **Extended Bio** - Increase bio character limits
- **Extended Comments** - Increase comment length limits

### ⚙️ Interaction Controls
- **Confirm Like** - Confirmation dialog before liking videos
- **Confirm Comment Like** - Confirmation before liking comments
- **Confirm Comment Dislike** - Confirmation before disliking comments
- **Confirm Follow** - Confirmation dialog before following users

### 🌍 Advanced Features
- **Always Open in Safari** - Redirect links to Safari browser
- **Region Changing** - Spoof location to access region-locked content
- **Live Button Customization** - Repurpose live button for custom actions
- **Playback Speed Control** - Adjust video playback speed (0.5x to 2.0x)
- **Always Upload in HD** - Force high-definition video uploads
- **App Lock** - Biometric/passcode protection for the app

### 🔧 Developer Features
- **FLEX Integration** - Runtime debugging and exploration tools
- **Comprehensive Logging** - Detailed operation logging for development

## 📚 Documentation

Comprehensive technical documentation is available in the [`docs/`](docs/) directory:

### 🏗️ Core Components
- [**Main Tweak Implementation**](docs/core/tweak.md) - Primary hook system and functionality
- [**Manager System**](docs/core/bhi-manager.md) - Centralized settings and utility management
- [**TikTok Headers**](docs/core/tiktok-headers.md) - Interface declarations for TikTok classes
- [**Security System**](docs/core/security.md) - App lock and authentication features

### 📥 Download System
- [**Single File Downloads**](docs/download/bh-download.md) - Individual file download handling
- [**Multiple File Downloads**](docs/download/bh-multiple-download.md) - Batch download operations

### ⚙️ Settings Interface
- [**Main Settings Controller**](docs/settings/main-settings.md) - Primary configuration interface
- [**Region Selection**](docs/settings/country-table.md) - Country/region picker
- [**Live Button Actions**](docs/settings/live-actions.md) - Live button customization
- [**Playback Speed Control**](docs/settings/playback-speed.md) - Video speed adjustment

### 📦 Third-Party Libraries
- [**JGProgressHUD Integration**](docs/libraries/jgprogresshud.md) - Progress indication system

### 🔧 Configuration
- [**Build System**](docs/configuration/build-system.md) - Makefile and build configuration
- [**Bundle Configuration**](docs/configuration/bundle-config.md) - App targeting and filtering

## 🚀 Installation

### Prerequisites

- Jailbroken iOS device (iOS 12.0+)
- Cydia, Sileo, or compatible package manager
- MobileSubstrate installed

### From Package Manager

1. Add the repository to your package manager
2. Search for "BHTikTok++"
3. Install the package
4. Restart SpringBoard if prompted

### Manual Installation

1. Download the latest `.deb` file from releases
2. Install using your preferred method:
   ```bash
   # Via SSH
   dpkg -i BHTikTok++.deb
   
   # Via Filza
   # Navigate to the .deb file and tap to install
   ```
3. Restart TikTok application

## ⚙️ Configuration

### Accessing Settings

1. Open TikTok
2. Navigate to **Profile** → **Settings**
3. Look for **"BHTikTok++ settings"** in the Account section
4. Configure desired features

### Key Settings Categories

- **Feed Settings** - Download buttons, ad blocking, UI modifications
- **Profile Settings** - Profile enhancements and customizations
- **Confirmation Settings** - User action confirmations
- **Region Settings** - Location spoofing configuration
- **Speed Settings** - Video playback speed control
- **Security Settings** - App lock and privacy features

### First Run Setup

On first installation, the following features are enabled by default:
- Hide Ads
- Download Button
- Show/Hide UI Button
- Show Progress Bar
- Profile Save and Copy features
- Extended Bio and Comments

## 🛠️ Development

### Build Requirements

- **macOS** with Xcode Command Line Tools
- **Theos** development framework
- **iOS SDK** (iOS 16.5+)
- **Device** or **Simulator** for testing

### Build Process

```bash
# Clone the repository
git clone https://github.com/user/BHTikTokPlusPlusPlus.git
cd BHTikTokPlusPlusPlus

# Clean and build
make clean && make

# Install to device
make install

# Create package
make package
```

### Development Setup

```bash
# Configure Theos environment
export THEOS=/opt/theos

# Set device IP for installation
export THEOS_DEVICE_IP=192.168.1.100
export THEOS_DEVICE_USER=root
```

### Project Structure

```
BHTikTokPlusPlusPlus/
├── Tweak.x                    # Main tweak implementation
├── BHIManager.[h|m]          # Settings and utility manager
├── TikTokHeaders.h           # TikTok class interfaces
├── SecurityViewController.[h|m] # App lock functionality
├── BH*Download.[h|m]         # Download system
├── Settings/                 # Settings interface controllers
├── JGProgressHUD/           # Progress indicator library
├── docs/                    # Comprehensive documentation
├── Makefile                 # Build configuration
├── control                  # Package metadata
└── BHTikTok.plist          # Bundle filter configuration
```

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details.

### Development Areas

- **Feature Development** - New TikTok enhancements
- **Bug Fixes** - Stability and compatibility improvements
- **Documentation** - Code documentation and user guides
- **Testing** - Compatibility testing across iOS versions
- **Localization** - Translation support for multiple languages

### Contribution Process

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 TODO

### High Priority
- [ ] Add Localization for the tweak interface
- [x] Add HD Download functionality
- [ ] Story Download capability
- [ ] Enhanced error handling and user feedback
- [ ] Performance optimizations

### Medium Priority
- [ ] Custom download quality selection
- [ ] Batch download management
- [ ] Download history and management
- [ ] Enhanced region spoofing options
- [ ] Additional UI customization options

### Low Priority
- [ ] Theme system for settings interface
- [ ] Advanced download scheduling
- [ ] Cloud sync for settings
- [ ] Plugin system for extensions

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **TikTok** - For the amazing platform
- **Theos Team** - For the excellent development framework
- **JGProgressHUD** - For the beautiful progress indicators
- **Community** - For feedback, testing, and support
- **Contributors** - For making this project better

## ⚠️ Disclaimer

This tweak is for educational and personal use only. Users are responsible for complying with TikTok's Terms of Service and applicable laws. The developers are not responsible for any misuse or violations.

---

**Made with ❤️ by the BHTikTok++ Team**

For more information, visit our [Documentation](docs/).