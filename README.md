# Android Espion 2.0 🔍

![Android Espion Banner](https://img.shields.io/badge/Android-Espion-brightgreen.svg?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-3.7+-blue.svg?style=for-the-badge&logo=python)
![License](https://img.shields.io/badge/License-Educational-yellow.svg?style=for-the-badge)

**Android Espion 2.0** is a powerful Android device management and monitoring tool built with Python and CustomTkinter. It provides a sleek GUI interface for remotely controlling and monitoring Android devices through ADB (Android Debug Bridge).

## ⚠️ Disclaimer

This tool is designed for **educational purposes only**. It should only be used on devices you own or have explicit permission to access. Unauthorized use of this software may violate local, state, federal, or international laws. The developers are not responsible for any misuse of this tool.

## ✨ Features

### 🔗 Device Connection
- **Wireless ADB Connection**: Connect to Android devices over Wi-Fi using IP address
- **Device Status Monitoring**: Real-time connection status updates
- **Smart Connection Handling**: Automatic ADB server management

### 📱 Device Information
- **Comprehensive Device Details**: Model, manufacturer, chipset information
- **System Information**: Android version, security patch level
- **Hardware Details**: SIM operator, encryption state, build date
- **Real-time Updates**: Refresh device information on demand

### 📸 Screen Capture & Mirroring
- **Screenshot Capture**: Take and automatically open device screenshots
- **Real-time Screen Mirroring**: Live screen mirroring with scrcpy integration
- **Quality Options**: Normal and low-resolution mirroring modes
- **Instant Preview**: Screenshots automatically open after capture

### 📁 File Management
- **Interactive File Browser**: Navigate device storage with tree view
- **File Transfer**: Push files to device and pull files from device
- **Directory Navigation**: Browse /sdcard/ and subdirectories
- **Batch Operations**: Select and transfer multiple files

### 🎵 Audio Monitoring
- **Microphone Streaming**: Listen to device microphone audio
- **Device Audio Streaming**: Stream device's internal audio
- **Android 11+ Support**: Compatible with modern Android versions
- **Real-time Audio**: Live audio streaming with minimal latency

### 🌐 Remote Control
- **Image Display**: Push and display images on device screen
- **URL Opening**: Open web links directly on the device
- **Remote App Launch**: Launch applications through intent system

### 🎨 User Interface
- **Modern Dark Theme**: Sleek CustomTkinter interface
- **ASCII Art Backgrounds**: Dynamic randomized backgrounds
- **Status Indicators**: Real-time status updates with colored text
- **Responsive Design**: Adaptive layout for different screen sizes

## 🛠️ Prerequisites

### Required Software
- **Python 3.7+** with the following packages:
  - `customtkinter`
  - `Pillow (PIL)`
  - `tkinter` (usually included with Python)

### Android Tools
- **ADB (Android Debug Bridge)**: Must be installed and added to system PATH
- **Scrcpy**: For screen mirroring functionality ([Download here](https://github.com/Genymobile/scrcpy))

### Android Device Setup
1. Enable **Developer Options** on your Android device
2. Enable **USB Debugging** in Developer Options
3. Enable **Wireless ADB** (Android 11+) or connect via USB initially
4. Ensure device and computer are on the same network

## 📦 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Ak-shay-n/Android-Espion-2.O.git
   cd Android-Espion-2.O
   ```

2. **Install Python dependencies:**
   ```bash
   pip install customtkinter Pillow
   ```

3. **Install ADB:**
   - **Windows**: Download Android SDK Platform Tools
   - **macOS**: `brew install android-platform-tools`
   - **Linux**: `sudo apt install adb` (Ubuntu/Debian)

4. **Install Scrcpy:**
   - **Windows**: Download from GitHub releases
   - **macOS**: `brew install scrcpy`
   - **Linux**: `sudo apt install scrcpy`

## 🚀 Usage

### Basic Usage
1. **Launch the application:**
   ```bash
   python androidEspion.py
   ```

2. **Connect to your device:**
   - Enter your Android device's IP address
   - Click "Connect" or press Enter
   - Wait for successful connection confirmation

3. **Explore features:**
   - Use the function selection menu to access different tools
   - Navigate through various monitoring and control options

### Feature Guide

#### 📱 Device Information
- Access comprehensive device details
- View system specifications and security information
- Monitor device status and configuration

#### 📸 Screenshots
- Capture device screen instantly
- Images are saved to `files/` directory
- Screenshots open automatically for viewing

#### 🖥️ Screen Mirroring
- Choose between normal and low-resolution mirroring
- Real-time display of device screen
- Interactive control through scrcpy

#### 📁 File Operations
- Browse device storage structure
- Transfer files between device and computer
- Navigate directories with intuitive tree view

#### 🎵 Audio Streaming
- Stream microphone or device audio
- Compatible with Android 11 and newer
- Real-time audio monitoring capabilities

## 📁 Project Structure

```
Android-Espion-2.O/
├── androidEspion.py          # Main GUI application
├── anndroidEspionageproto.py # Command-line prototype
├── files/                    # Directory for transferred files
├── newVid.mp4               # Sample media file
└── README.md                # This file
```

## 🔧 Configuration

### ADB Setup
Ensure ADB is properly configured and accessible from command line:
```bash
adb version
```

### Device IP Discovery
Find your Android device's IP address:
1. Go to Settings → About Phone → Status
2. Look for "IP Address" or check Wi-Fi settings
3. Use the IP address in the connection field

## 🐛 Troubleshooting

### Common Issues

**Connection Failed:**
- Verify device and computer are on same network
- Ensure USB debugging is enabled
- Try running `adb tcpip 5555` manually
- Restart ADB server: `adb kill-server && adb start-server`

**Scrcpy Not Working:**
- Verify scrcpy is installed and in PATH
- Check Android version compatibility
- Ensure sufficient device permissions

**Audio Streaming Issues:**
- Requires Android 11 or higher
- Check device audio permissions
- Verify scrcpy supports audio on your device

### File Permission Issues
If you encounter permission errors:
```bash
# Linux/macOS
chmod +x androidEspion.py

# Windows (Run as Administrator if needed)
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

### Development Guidelines
1. Follow PEP 8 style guidelines
2. Add comments for complex functionality
3. Test thoroughly on different Android versions
4. Update documentation for new features

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⚖️ Legal Notice

This tool is intended for:
- **Educational purposes**
- **Authorized penetration testing**
- **Personal device management**
- **Security research with proper authorization**

**Unauthorized access to devices is illegal and unethical. Always obtain proper permission before using this tool.**

## 🔗 Related Projects

- [Scrcpy](https://github.com/Genymobile/scrcpy) - Display and control Android devices
- [ADB](https://developer.android.com/studio/command-line/adb) - Android Debug Bridge
- [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter) - Modern GUI framework

## 🙏 Acknowledgments

- CustomTkinter team for the modern GUI framework
- Scrcpy developers for screen mirroring capabilities
- Android development community for ADB documentation
- Open source contributors who made this project possible

---

**⭐ If you find this project useful, please consider giving it a star!**

*Remember: With great power comes great responsibility. Use this tool ethically and legally.*
