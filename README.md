# PS5 Websrv Payload Menu

A clean, modern, and offline-capable payload menu designed to work specifically with **WebSrv** on the PlayStation 5. This menu allows you to inject `.bin` and `.elf` payloads directly from the browser to your console's `elfldr`.

## 🚀 Live Host

You can use the live host here (HTTP):
### [🌐 Open PS5 Websrv Menu](http://sinajet.wuaze.com/PS5-Websrv-Payload-Menu/index.html)

---

## ✨ Features

- **Offline Caching:** The menu caches itself automatically. Once loaded, you can use it completely offline.
- **Auto-Update:** If you are connected to the internet, the cache will automatically update to the latest version in the background.
- **Dynamic Injection:** Automatically detects and sends payloads via WebSrv (port 8080).
- **Firmware Detection:** Shows compatible payloads based on your selected firmware.

---

## ⚠️ Important: Self-Hosting Guide

If you plan to host this menu on your own server, please read this carefully:

1.  **NO SSL / HTTPS:** You **MUST** host this on a server that supports **HTTP**.
2.  **Why?** The PS5 WebSrv runs on `http://127.0.0.1:8080`. Modern browsers (including PS5 WebKit) block requests sent from a Secure (HTTPS) website to an Insecure (HTTP) service (Mixed Content Blocking).
3.  **Do NOT use GitHub Pages:** GitHub Pages enforces HTTPS, so payload injection **will not work**. Use alternatives cheap HTTP hosting, or a local server (IIS, Apache, Python, ESP32).

---

## 📥 Shortcut App (PKG)

For easier access, you can download the **Itemzflow/Store Shortcut PKG** from the releases page:

[**⬇️ Download Latest Release**](https://github.com/sinajet/PS5-Websrv-Payload-Menu/releases/)

---

## ⚙️ Requirements

To use this menu, you must have **WebSrv** running on your PS5.
This menu communicates with `elfldr` listening on port `8080`.

- **WebSrv Repository:** [ps5-payload-dev/websrv](https://github.com/ps5-payload-dev/websrv)

---

## ❤️ Credits & Acknowledgments

This project wouldn't be possible without the hard work of the scene developers:

- **[ps5-payload-dev Team](https://github.com/ps5-payload-dev):** For creating **WebSrv**, the backbone of this project.
- **[idlesauce](https://github.com/idlesauce):** Huge thanks for the offline caching mechanism and inspiration.
- **All Scene Developers:** A massive thank you to every developer contributing to keeping the PS5 scene alive and thriving.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/sinajet/PS5-Websrv-Payload-Menu/blob/main/LICENSE) file for details.
