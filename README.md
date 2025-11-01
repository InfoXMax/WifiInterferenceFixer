# Wi-Fi Network Analyzer (Local Netsh Parser)



This project provides a simple, client-side tool for parsing and displaying the detailed Wi-Fi network information gathered by the Windows command-line utility `netsh`. It helps users quickly visualize the SSIDs, channels, and signal strengths of nearby access points for troubleshooting interference and optimizing their network settings.

---

## 🚀 Features

* **Command Copy:** One-click copy of the required `netsh` command for easy use in the terminal.
* **Offline Analysis:** Runs entirely within the browser—no backend or internet connection needed after the file is loaded.
* **Data Parsing:** Accurately extracts SSID, Channel, Signal (converted to dBm), Band (2.4 GHz or 5 GHz), and MAC Address (BSSID).
* **Clean Visualization:** Presents raw network data in an easy-to-read table.

---

## 💻 How to Use

The application is designed specifically to process the output from a single Windows command.

### The Command

The key command to generate the necessary data is:

```cmd
netsh wlan show networks mode=bssid
```
---

# Step-by-Step Guide:
Run the command:

* Open your Windows Command Prompt or PowerShell as an administrator.

* Click the Copy Command button in the app and paste the command into your terminal, then press Enter.

Capture the output:

* Copy the entire output text from the terminal (right-click and select "Mark", then select the text and press Enter to copy).

Analyze:

* Paste the copied text into the large text area in the application.

Click the Analyze button.

The results table will populate with the parsed data, allowing you to easily view the channel usage and signal quality of all detected Wi-Fi networks.

# 🛠️ Technology Stack
This is a minimal, single-file web application designed for maximum portability and ease of use.

HTML5: Structure and content.

Tailwind CSS: Used via CDN for modern, fully responsive styling.

Vanilla JavaScript: For clipboard manipulation, parsing the text input, performing the dBm calculation, and rendering the results table.

# ⚙️ Running Locally
Since this is a single HTML file (Wifi.html), there are no complex build steps required.

Clone this repository or download the Wifi.html file.

Open Wifi.html directly in any modern web browser (Chrome, Firefox, Edge, Safari).