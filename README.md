# 🕒 Digital Clock

A simple, responsive digital clock built with plain HTML, CSS, and JavaScript. It displays the live time, date, and day of the week, and updates every second.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## ✨ Features

- Live time in 12-hour format with AM/PM
- Current day of the week
- Full date (day, month, year)
- Updates every second
- Responsive layout for desktop and mobile
- Dark theme with a glowing time display
- No libraries or dependencies

## 📸 Preview

> Add a screenshot or GIF of your clock here.
>
> `![Digital Clock Preview](screenshot.png)`

## 🚀 Getting Started

### Option 1: Run locally

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/digital-clock.git
   ```
2. Go into the project folder:
   ```bash
   cd digital-clock
   ```
3. Open `index.html` in your browser.

### Option 2: Use GitHub Pages

1. Go to **Settings → Pages** in your repository.
2. Under **Source**, select the `main` branch and the `/ (root)` folder.
3. Save, and your clock will be live at `https://your-username.github.io/digital-clock/`.

## 📁 Project Structure

```
digital-clock/
├── index.html    # Markup, styles, and script
└── README.md
```

## ⚙️ How It Works

- `setInterval` calls `updateClock()` every 1000 ms.
- `new Date()` provides the current hours, minutes, seconds, day, and date.
- Hours are converted to 12-hour format, and `padStart(2, "0")` keeps two digits (e.g., `07:05:09`).
- Day and month names come from lookup arrays, so the output is the same in every browser.

## 🎨 Customization

**Switch to 24-hour format:** in `updateClock()`, remove the AM/PM conversion:

```js
let h = now.getHours();
```

**Change the colors:** edit these values in the CSS:

```css
background: #0f172a;   /* page background */
color: #38bdf8;        /* day text accent */
text-shadow: 0 0 20px rgba(56, 189, 248, 0.6); /* time glow */
```

## 🛠️ Built With

- HTML5
- CSS3
- Vanilla JavaScript

## 🗺️ Future Ideas

- [ ] 12/24-hour toggle
- [ ] Light/dark theme switch
- [ ] Timezone selector
- [ ] Alarm feature

## 🤝 Contributing

Contributions are welcome!

1. Fork the project
2. Create your feature branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -m "Add new feature"`)
4. Push to the branch (`git push origin feature/new-feature`)
5. Open a Pull Request

## 👤 Author

**Parth**
