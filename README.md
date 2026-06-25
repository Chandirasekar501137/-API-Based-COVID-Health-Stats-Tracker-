# 🦠 COVID-19 Tracker

A responsive web application built with **React.js** that allows users to search and view COVID-19 statistics for any country worldwide, along with global pandemic totals.

> Data sourced from WHO COVID-19 Dashboard & Johns Hopkins University · Final pandemic totals as of May 2023

---

## 🚀 Features

- 🌍 **Global Stats** — View worldwide total cases, deaths, and recoveries at a glance
- 🔍 **Country Search** — Search any country by name and view its detailed stats instantly
- 📋 **Country Table** — Browse and click through a complete list of all countries
- 📜 **Smooth Scroll** — Automatically scrolls to results after search
- ❌ **Not Found Handling** — Friendly message shown for invalid country searches
- 🔄 **Clear Search** — Reset results and return to top with one click
- 📱 **Responsive Design** — Works across desktop and mobile devices

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| React.js (v19) | Frontend UI library |
| JavaScript (ES6+) | Application logic |
| HTML5 | Component structure |
| CSS3 | Styling & responsive layout |
| React Hooks (`useState`, `useRef`) | State & DOM management |
| Create React App | Project setup & build tool |
| Static JSON Dataset | COVID-19 country data |
| Git & GitHub | Version control |

---

## 📁 Project Structure

```
covid-tracker/
├── public/
│   └── index.html
├── src/
│   ├── components/
│   │   ├── Header.js
│   │   ├── Hero.js
│   │   ├── SearchBar.js
│   │   ├── GlobalStats.js
│   │   ├── CountryResult.js
│   │   ├── CountryTable.js
│   │   └── NotFound.js
│   ├── data/
│   │   └── covidData.js
│   ├── App.js
│   ├── App.css
│   └── index.css
├── package.json
└── README.md
```

---

## ⚙️ Getting Started

### Prerequisites

Make sure you have the following installed:
- [Node.js](https://nodejs.org/) (v14 or above)
- npm (comes with Node.js)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/covid-tracker.git
   cd covid-tracker
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm start
   ```

4. Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## 🏗️ Build for Production

```bash
npm run build
```

This creates an optimized production build in the `build/` folder, ready for deployment.

---

## 🔄 Application Flow

```
Launch App
    ↓
Header + Hero Section displayed
    ↓
Global Stats loaded automatically
    ↓
User types country name → Search
    ↓
Country Found?
  ✅ YES → CountryResult displayed
  ❌ NO  → NotFound message shown
    ↓
Page scrolls smoothly to result
    ↓
User can browse CountryTable
    ↓
Click Clear → Reset & scroll to top
```

---

## ⚛️ Key React Concepts Used

- **Functional Components** — All UI sections are independent reusable components
- **useState** — Manages search result state (`null` / found / not-found)
- **useRef** — Smooth scroll to result section after search
- **Props** — `onSearch`, `onSelect`, `onClear` passed from App to child components
- **Conditional Rendering** — Result section renders only when a search is made
- **Event Handling** — Search, select, and clear actions handled via functions

---

## 📊 Data Source

- [WHO COVID-19 Dashboard](https://www.who.int/emergencies/diseases/novel-coronavirus-2019)
- Johns Hopkins University COVID-19 Data Repository
- **Note:** Data reflects final pandemic totals as of **May 2023**

---

## 🔮 Future Enhancements

- [ ] Live API integration for real-time statistics
- [ ] Line/bar charts showing case trends over time
- [ ] State and region-level data
- [ ] Dark mode toggle
- [ ] Multilingual support

---

## 📄 License

This project was built for the **Naan Mudhalvan Arts Internship Program 2026** — Frontend Web Development using React.

---

## 👨‍💻 Author

Built with ❤️ for health awareness.
