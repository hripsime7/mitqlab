# 🧠 MitqLab — Տվյալագիտություն հայերեն

> **Free Armenian-language data science education for children and teenagers.**
> Անվճար հայկական կրթական հարթակ՝ տվյալագիտության, Python-ի և Machine Learning-ի համար։

[![License: MIT](https://img.shields.io/badge/License-MIT-778DA9?style=flat-square)](LICENSE)
[![Language](https://img.shields.io/badge/Language-Armenian%20🇦🇲-E0E1DD?style=flat-square)]()
[![Made for Kids](https://img.shields.io/badge/Audience-Ages%209--14-1B263B?style=flat-square)]()
[![Try it now](https://img.shields.io/badge/Try%20it%20now-GitHub-415A77?style=flat-square)](https://github.com/hripsime7/mitqlab)

---

## 🌍 What is MitqLab?

MitqLab (**Միտք** = *Mind*) is a free, open-source, browser-based learning platform that teaches data science and programming to Armenian-speaking children and teenagers — entirely in Armenian, with no installation required.

Every lesson runs directly in the browser. Students write and execute real Python code — powered by **Pyodide** — without installing anything.

---

## 🚀 Try it now

**No installation needed!** Just click the link below:

👉 **[https://github.com/hripsime7/mitqlab](https://github.com/hripsime7/mitqlab)**

1. Clone or download the repository
2. Open `index.html` in any modern browser (Chrome, Firefox, Edge, Safari)
3. Start learning!

> ⚠️ On first load, Pyodide downloads ~10 MB of WebAssembly to enable real Python in the browser. This takes 5–15 seconds depending on connection speed. After that, all code runs instantly.

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

**Total: ~2 hours · Beginner level · Ages 9–14**

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

---

## 📥 Download & Run

```bash
# Clone the repository
git clone https://github.com/hripsime7/mitqlab.git

# Open the file
cd mitqlab
open index.html   # or just double-click it
