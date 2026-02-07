# 🛠 Full Setup Guide: WebRTC Leak & IP Tracker

Follow this step-by-step guide to correctly install and configure the tracker. This process takes approximately 5 minutes.

---

## 1. Environment Preparation
Before installing the script, your browser needs specific permissions to allow Tampermonkey to interact with the networking layer and the UI.

### For Chrome, Edge, and Brave users:
1. Open your browser and go to the **Extensions** page:
   - Chrome/Brave: `chrome://extensions`
   - Edge: `edge://extensions`
2. Find the **Tampermonkey** extension and click **Details**.
3. Scroll down and enable the toggle: **"Allow access to file URLs"**.
4. Ensure **"Developer Mode"** is turned **ON** (usually a toggle in the top-right corner of the page).

---

## 2. Obtain your API Key
The script requires a connection to a geolocation database to translate IP addresses into physical locations.

1. Go to [ipgeolocation.io](https://ipgeolocation.io/).
2. Sign up for a **Free Plan** (which provides 1,000 requests per day).
3. Confirm your email address.
4. Log in to your Dashboard and copy your **API Key**.

---

## 3. Script Installation
1. Click the **Tampermonkey icon** in your browser toolbar and select **"Create a new script..."**.
2. A new editor window will open. Delete any existing template code.
3. Copy the entire content of the file `webrtc_ip_tracker.user.js` from this repository.
4. Paste it into the Tampermonkey editor.
5. **Configuration**: Find the following line (usually near the top):
   ```javascript
   const apiKey = "YOUR_API_KEY_HERE";
