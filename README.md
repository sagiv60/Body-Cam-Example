# 🎥 Body-Cam Overlay for OBS

Create a realistic **body-cam style overlay** in OBS, inspired by law enforcement footage. Ideal for roleplay servers, immersive content creation, or stylized video edits.

🔗 [Video Example](https://www.youtube.com/watch?v=9HtMRLDxdI4)

---

## 🧰 Features

* ✅ Authentic body-cam aesthetic
* ✅ Customizable text (e.g., officer name, unit ID, timestamp)
* ✅ Easy integration with OBS via Browser Source
* ✅ Built-in periodic **beep sound** for added realism
* ✅ Compatible with live streams and recorded footage

---

## 📦 What's Included

* `BodyCamMain.html` – Main overlay file (HTML/CSS/JS)
* `axoncamsound.html` – Beep sound player (use with `AXON_BODY_CAM_BEEP.mp3`)
* `AXON_BODY_CAM_BEEP.mp3` – Looping beep audio
* `README.md` – This instruction file

---

## 🚀 How to Use

### 1. Download the Files

Clone or download the repository to your local machine.

### 2. Customize Overlay Information

Open `BodyCamMain.html` in a text editor and edit the following section:

```html
        const player = "Lieutenant A. Halstead";
        const agency = "Atlanta Police Department";
        const callsign = "[232]";
```

Change the text values as desired.

---

### 3. Integrate with OBS (Overlay Only)

1. Open **OBS Studio**.
2. Click the "+" in the **Sources** panel → choose **Browser**.
3. Name it e.g. `BodyCam Overlay` and click **OK**.
4. In the **Browser Source settings**:

   * ✅ Check **"Local File"**
   * Browse and select `BodyCamMain.html`
   * Set width & height (e.g. `1920x1080`)
   * Click **OK**

---

### 4. Add Body-Cam Beep Sound (Optional)

To simulate the authentic **Axon-style beep**:

1. In OBS, add **another Browser Source**

2. Name it e.g. `BodyCam Beep`

3. In the properties window:

   * ✅ Check **"Local File"**
   * Select `axoncamsound.html`
   * Set width & height (e.g., `400x100`) – size doesn't matter
   * ✅ Check **"Control audio via OBS"** (important!)
   * Click **OK**

4. In the **Audio Mixer**, ensure:

   * You can control the beep's volume
   * Mute/unmute as needed

💡 The `axoncamsound.html` file plays `AXON_BODY_CAM_BEEP.mp3` in a loop to match real-world body cam audio feedback.

---

## ✏️ Customization Tips

* **Fonts** – Use monospaced fonts like “Klartext Mono”
* **Timestamp** – Uses system clock for real-time display
* **Opacity** – You can fade the overlay using OBS filters
* **Sounds** – Replace `AXON_BODY_CAM_BEEP.mp3` with your own if desired
* **CSS** – Adjust styles in the HTML file to tweak layout and colors

---

## 🧠 Credits

* **Original Concept** – Inspired by real-world bodycam UIs
* **Video Demo** – [YouTube: Body-Cam Overlay Example](https://www.youtube.com/watch?v=9HtMRLDxdI4)
* **Additional Resources**:

  * [SWRP619/Axon-3-Body-Cam](https://github.com/SWRP619/Axon-3-Body-Cam)
  * [PeterSethaphan/Bodycam-overlay-Edit-by-Alex\_Dubbler](https://github.com/PeterSethaphan/Bodycam-overlay-Edit-by-Alex_Dubbler)
