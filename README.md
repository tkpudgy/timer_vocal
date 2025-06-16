# Race Timer Flow

A lightweight, single-page HTML/JavaScript stopwatch designed for race timing drills:
- **Prep**, **Ready**, **Random Delay**, then **Go**
- Spoken cues and high-speed numeric readouts via the Web Speech API
- Visual flowchart layout for clarity on all stages

---

## 🚀 Features

- **Configurable timings** for:
  - Prep time
  - Ready time
  - Minimum & maximum random delay
  - Stopwatch duration
- **Spoken prompts**:
  - "Get ready"
  - "On your marks"
  - "Set"
  - "Go"
  - Numeric seconds announced at high speed
- **Beep** just before the final "Go" cue
- **Drift‑compensated** 1 Hz timer for accuracy
- **No external dependencies**—pure HTML/CSS/JS

---

## 💻 Installation & Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/<YOUR-USERNAME>/race-timer.git
   cd race-timer
   ```

2. **Open locally**
   - Double-click `index.html` in your file explorer, or
   - Serve via a local HTTP server:
     ```bash
     # Python 3
     python3 -m http.server 8000
     ```
     Then visit `http://localhost:8000/`.

3. **Configure timings**
   - Adjust the input boxes for each stage:
     - **Prep Time** (seconds)
     - **Ready Time** (seconds)
     - **Min Delay** / **Max Delay** (seconds)
     - **Stopwatch Duration** (seconds)

4. **Start the timer**
   - Click **Start** and follow the spoken cues.

---

## 🌐 Deploying via GitHub Pages

1. Push your code to a GitHub repo (e.g. `race-timer`).
2. In **Settings → Pages**, set **Source** to the `main` branch root.
3. Your app will be live at:
   ```
   https://<YOUR-USERNAME>.github.io/race-timer/
   ```

---

## ⚙️ Customization

- **Speech rate**: adjust `msg.rate` in `speakText()` / `speakNumber()`
- **Beep length**: modify the duration passed to `beep()`
- **Styling**: tweak the CSS in the `<style>` block

---

## 🤝 Contributing

Feel free to open issues or submit pull requests for enhancements, bug fixes, or new features.

---

## 📄 License

This project is released under the [MIT License](LICENSE). Feel free to use and adapt.
