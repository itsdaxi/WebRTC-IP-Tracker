# WebRTC Leak & IP Tracker - Real-Time OSINT Dashboard

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Security: OSINT](https://img.shields.io/badge/Security-OSINT-red.svg)]()
[![Platform: Tampermonkey](https://img.shields.io/badge/Platform-Tampermonkey-green.svg)]()

**WebRTC-IP-Tracker** is an advanced security research tool designed to monitor, intercept, and visualize **WebRTC leaks** in real-time. By hooking into the `RTCPeerConnection` API, this tool exposes public IP addresses that often remain hidden behind VPNs, Proxies, or NAT gateways.



---

## 🚀 Core Features
- **WebRTC Interception**: Automatically catches ICE candidates by monitoring STUN/TURN requests.
- **Instant Geolocation**: Provides detailed Country, City, ISP, and Geographic Coordinates via `ipgeolocation.io` integration.
- **"Immortal" UI**: High-priority overlay panel (Maximum Z-Index) that remains visible regardless of site-specific CSS or Content Security Policies (CSP).
- **Draggable Interface**: Customizable positioning with a simple drag-and-drop header.
- **Hotkey Support**: Press `R` to instantly reset the tracker and clear cached session data.

## 🎭 Showcase
<div align="center">
  <img width="350" alt="WebRTC IP Tracker Detection" src="https://github.com/user-attachments/assets/8a62c046-20fb-4cf7-be15-6a3e9b4581f6" />
  <img width="350" alt="IP Geolocation Details" src="https://github.com/user-attachments/assets/b592f860-fee0-4f7a-8cd1-9d0cb2051104" />
</div>

---

## 🛠 Prerequisites (Mandatory)
To ensure the script functions correctly across all domains, you must configure your browser and Tampermonkey as follows:

1. **Allow Access to File URLs**: 
   - Open your browser's **Extensions** page (e.g., `chrome://extensions`).
   - Find **Tampermonkey** and click **Details**.
   - Enable the toggle: **"Allow access to file URLs"**.
2. **Developer Mode**:
   - Ensure "Developer Mode" is turned **ON** in your browser's extension settings.
3. **Script Permissions**:
   - For Brave or Safari users, ensure "Allow User Scripts" is enabled in your global security/privacy settings.

---

## 📖 Installation Guide
1. **Install Manager**: Download [Tampermonkey](https://www.tampermonkey.net/) for your specific browser.
2. **Create New Script**: Click the Tampermonkey icon -> **"Create a new script..."**.
3. **Paste Code**: Delete the default template and paste the content of `webrtc_ip_tracker.user.js`.
4. **Configure API Key**: 
   - Sign up at [ipgeolocation.io](https://ipgeolocation.io/) for a free API key.
   - Replace `YOUR_API_KEY_HERE` with your actual key in the script code.
5. **Save**: Click `File` -> `Save` (or `Ctrl+S`).
6. **Verification**: Visit a WebRTC-enabled site (e.g., [BrowserLeaks WebRTC Test](https://browserleaks.com/webrtc)) to see the tracker in action.

---

## 🎯 Use Cases
- **Privacy Auditing**: Real-world verification of VPN "WebRTC Leak Protection" claims.
- **OSINT Research**: Gathering network intelligence and identifying entry points during security audits.
- **Network Analysis**: Monitoring how modern web applications initialize Peer-to-Peer (P2P) connections.

---

## ⚖️ Disclaimer
**For Educational and Ethical Research Purposes Only.**
This project was developed to demonstrate privacy vulnerabilities related to WebRTC leaks. The author is not responsible for any misuse, illegal activities, or violations of third-party Terms of Service performed with this tool. Users assume all responsibility for its application in security auditing and research.

## 📜 License
Distributed under the [MIT License](LICENSE).
