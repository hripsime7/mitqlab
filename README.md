# 🧠 MitqLab — Տվյալագիտություն հայերեն

> **Free Armenian-language data science education for children and teenagers.**
> Անվճար հայկական կրթական հարթակ՝ տվյալագիտության, Python-ի և Machine Learning-ի համար։

[![Live Site](https://img.shields.io/badge/Live%20Site-mitqlab.am-415A77?style=flat-square)](https://mitqlab.am)
[![License: MIT](https://img.shields.io/badge/License-MIT-778DA9?style=flat-square)](LICENSE)
[![Language](https://img.shields.io/badge/Language-Armenian%20🇦🇲-E0E1DD?style=flat-square)]()
[![Made for Kids](https://img.shields.io/badge/Audience-Ages%2012--18-1B263B?style=flat-square)]()

---

## 🌍 What is MitqLab?

MitqLab (**Միտք** = *Mind*) is a free, open-source, browser-based learning platform that teaches data science and programming to Armenian-speaking children and teenagers — entirely in Armenian, with no installation required.

Every lesson runs directly in the browser. Students write and execute real Python code — powered by **Pyodide** — without installing anything.

---

## ✨ Features

- 🇦🇲 **Fully in Armenian** — lessons, UI, examples, and feedback
- 🐍 **Real Python in the browser** — powered by Pyodide (no install needed)
- 📊 **numpy + matplotlib + pandas** — real data science libraries, not simulations
- 📝 **Interactive code editors** — edit and run code on every lesson page
- 📈 **Live chart rendering** — matplotlib plots appear inline in the browser
- 🏆 **15-question quiz** — with instant feedback and explanations
- 🎓 **Downloadable certificate** — generated on canvas after passing the quiz
- 📱 **Mobile-friendly** — works on phones and tablets
- 💸 **Completely free** — no login, no paywall, no ads

---

## 📚 Curriculum (v1.0)

| Module | Topic | Duration |
|--------|-------|----------|
| 01 | Մաթեմատիկա & Վիճակագրություն — Mean, Median, Mode, Correlation | 20 min |
| 02 | Տվյալներ & Pandas — DataFrames, cleaning, NaN handling | 25 min |
| 03 | Machine Learning — Linear Regression, Decision Tree, KNN | 30 min |
| 04 | Վիզուալիզացիա — Matplotlib line, bar, scatter charts | 20 min |
| 05 | Կիրառություններ — Medicine, Finance, Engineering, Governance | 15 min |
| 06 | Ավարտական Թեստ — 15 questions, 80% passing threshold | 15 min |
| 07 | Վկայական — Personalized downloadable certificate | — |

**Total: ~2 hours · Beginner level · Ages 12–18**

---

## 🚀 Getting Started

No build tools, no dependencies, no server required.

```bash
git clone https://github.com/YOUR-USERNAME/mitqlab.git
cd mitqlab
open index.html   # or just double-click it
```

Or visit the live site: **[mitqlab.am](https://mitqlab.am)**

> ⚠️ On first load, Pyodide downloads ~10 MB of WebAssembly to enable real Python in the browser. This takes 5–15 seconds depending on connection speed. After that, all code runs instantly.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| HTML / CSS / JS | Single-file app, zero build step |
| [Pyodide v0.27](https://pyodide.org) | CPython compiled to WebAssembly |
| numpy | Array math, statistics, linear regression |
| pandas | DataFrames, data cleaning |
| matplotlib (Agg backend) | Chart rendering → base64 PNG inline |
| Canvas API | Certificate generation |
| GitHub Pages | Free hosting |

---

## 🗺️ Roadmap

- [ ] More courses — Statistics II, Web Scraping, SQL
- [ ] Armenian NLP lesson (working with Armenian text data)
- [ ] Teacher dashboard — assign lessons, track class progress
- [ ] Mobile app (PWA)
- [ ] Offline mode
- [ ] Localization support for Diaspora Armenian dialects

---

## 🤝 Contributing

Contributions are very welcome — especially from Armenian developers and educators.

```bash
# Fork the repo, make your changes, open a pull request
git checkout -b feature/your-lesson-name
```

Ways to contribute:
- **New lessons** — add a module on a new topic
- **Translations** — improve the Armenian text
- **Bug fixes** — report or fix issues
- **Design** — improve the UI for younger audiences

Please open an issue first to discuss major changes.

---

## 📬 Contact & Partners

We are actively looking for:
- 🏫 **Schools and teachers** to pilot the platform
- 💰 **Grants and sponsors** — TUMO, Teach for Armenia, SmartGate, USAID
- 👩‍💻 **Volunteer developers** and content creators

**Email:** hello@mitqlab.am
**Website:** [mitqlab.am](https://mitqlab.am)

---

## 📄 License

MIT License — free to use, modify, and distribute.
See [LICENSE](LICENSE) for details.

---

<div align="center">
  <strong>Տվյալագիտություն — հայերեն, անվճար, բոլորի համար։</strong><br>
  <em>Data science — in Armenian, free, for everyone.</em><br><br>
  Made with ❤️ for Armenian kids everywhere 🇦🇲
</div>
