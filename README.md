# Social Media Data Analysis and Visualization System
### BCA Final Year Project &bull; Academic Year 2025–2026

A modern, responsive, and beginner-friendly web application for analyzing, visualizing, and deriving actionable insights from multi-platform social media datasets. Built entirely with **HTML5, Vanilla CSS3, and Vanilla JavaScript (ES6+)** with **Chart.js** integration.

---

## 📌 Project Overview & Abstract

In today's digital economy, social media platforms generate massive volumes of user interaction data every second. For digital marketers, content creators, and academic researchers, analyzing this data is vital to understanding audience behavior and optimizing content strategy.

This project delivers a **Social Media Data Analysis and Visualization System** designed to:
1. Ingest social media performance metrics across **Instagram, Facebook, YouTube, LinkedIn, and X (formerly Twitter)**.
2. Calculate engagement rates using standard digital marketing algorithms.
3. Visualize metrics through interactive charts (doughnut, grouped bar, smooth trend line, horizontal ranking).
4. Provide multi-criteria search, dynamic filtering (by platform, format, date range, and engagement threshold).
5. Support client-side **CSV file uploads** with automated parsing and data export.
6. Run seamlessly in any modern web browser **without requiring external backends or database setups**, making it ideal for BCA project demonstrations and evaluations.

---

## 🎯 Key Objectives

- **Cross-Platform Analytics:** Compare metrics across Instagram, YouTube, LinkedIn, Facebook, and X in a unified dashboard.
- **Engagement Modeling:** Automate the calculation of engagement percentages:
  $$\text{Engagement Rate (\%)} = \left( \frac{\text{Total Likes} + \text{Total Comments} + \text{Total Shares}}{\text{Total Views}} \right) \times 100$$
- **Interactive Visualizations:** Provide multi-dimensional charts with dynamic updates upon filtering.
- **Automated Algorithmic Insights:** Identify top-performing platforms, winning content formats, and viral posts automatically.
- **Data Portability:** Enable seamless import and export of social media datasets in standard CSV format.

---

## 🚀 Features Matrix

| Feature | Description | Status |
| :--- | :--- | :--- |
| **Executive KPI Cards** | Real-time counters for Total Views, Likes, Comments, Shares, Filtered Posts, and Avg Engagement Rate | ✅ Completed |
| **Platform-Wise Cards** | Dedicated interactive cards for Instagram, Facebook, YouTube, LinkedIn, and X with 1-click filtering | ✅ Completed |
| **Interactive Charts** | 5 Chart.js visual models: Platform Share, Metrics Comparison, Chronological Trend, Content Format, and Top 5 Posts | ✅ Completed |
| **Automated Insights** | Smart algorithm highlighting best platform, winning format, and peak viral reach | ✅ Completed |
| **CSV File Ingestion** | Drag-and-drop or file upload parser with quote-handling and error validation | ✅ Completed |
| **CRUD Operations** | Add new posts with live engagement calculation and delete existing posts | ✅ Completed |
| **Post Breakdown Modal** | Click any post to inspect the exact mathematical step-by-step formula and engagement classification | ✅ Completed |
| **Search & Filters** | Real-time text search, platform filter, format filter, date range, and minimum engagement slider | ✅ Completed |
| **Sortable Data Table** | Column sorting for all metrics (Date, Views, Likes, Comments, Shares, Engagement %) with pagination | ✅ Completed |
| **CSV Export** | Export filtered dataset back to CSV with 1 click | ✅ Completed |
| **Light & Dark Theme** | Smooth theme switcher with persistent preferences stored in `localStorage` | ✅ Completed |
| **Academic Report Print** | Clean print stylesheet formatted for PDF generation or physical project reports | ✅ Completed |

---

## 📐 Mathematical Formulation

### 1. Engagement Rate (ER)
The proportion of active interactions relative to overall reach:

$$\text{ER} = \left( \frac{L + C + S}{V} \right) \times 100$$

Where:
- $L$ = Total Likes / Reactions
- $C$ = Total Comments / Replies
- $S$ = Total Shares / Reposts / Retweets
- $V$ = Total Views / Impressions / Reach

### 2. Performance Classification Tiers
- **Viral ($\ge 8.0\%$):** Outstanding community amplification.
- **High ($5.0\% - 7.9\%$):** Excellent audience interaction.
- **Moderate ($2.5\% - 4.9\%$):** Healthy industry benchmark.
- **Low ($< 2.5\%$):** Optimization or format adjustment recommended.

---

## 📂 Project Directory Structure

```
SocialMediaProject/
│
├── index.html                           # Main dashboard & UI markup
│
├── css/
│   └── style.css                        # Modern CSS styling (Dark/Light themes, Glassmorphism, Responsive Grid)
│
├── js/
│   ├── data.js                          # 30+ default sample multi-platform social media posts
│   ├── utils.js                         # CSV parser/exporter, engagement calculator, formatters
│   ├── charts.js                        # Chart.js initialization & dynamic theme-aware updates
│   └── app.js                           # State manager, event listeners, filters, table & modal logic
│
├── data/
│   └── sample_social_media_data.csv     # Downloadable/uploadable sample dataset for examiner testing
│
└── README.md                            # BCA Final Year Project documentation
```

---

## 💻 Supported Social Media Platforms

1. **Instagram:** Reels, Carousels, Static Images (`#tech`, `#coding`, `@techpulse_official`)
2. **YouTube:** Long-form Videos, YouTube Shorts (`CodeCraft Academy`, `ByteSize Shorts`)
3. **LinkedIn:** Professional Carousels, Industry Surveys, Thought Leadership Posts (`Satya Dev`, `Career Catalyst`)
4. **Facebook:** Community Videos, Infographics, Small Business Updates (`Digital Creators Hub`)
5. **X (Twitter):** Tech Announcements, Fast-breaking Threads, Infographics (`@TechRadarNow`, `@FrontendNinja`)

---

## 🛠️ Technology Stack

- **HTML5:** Semantic architecture (`<header>`, `<main>`, `<section>`, `<table>`, `<canvas>`).
- **CSS3:** Custom Variables, Flexbox, CSS Grid, Glassmorphism backdrop blur, CSS micro-animations, Print media queries.
- **JavaScript (ES6+):** Arrow functions, Template literals, Array methods (`filter`, `reduce`, `map`, `sort`), FileReader API, Blob/URL API.
- **Chart.js 4.4.1 (CDN):** Responsive canvas-based data visualizations.
- **FontAwesome 6.5.1 (CDN):** Vector iconography for platform branding and UI controls.
- **Google Fonts:** `Inter` (body copy) & `Outfit` (display headers and KPI metrics).

---

## 📖 How to Run the Application

### Option 1: Direct Browser Launch (Simplest)
1. Navigate to the project folder: `c:\Users\ELCOT\Desktop\SocialMediaProject`.
2. Double-click **`index.html`** or right-click and select **Open with Google Chrome / Microsoft Edge / Mozilla Firefox**.
3. The application will start immediately with all 30 sample social posts pre-loaded!

### Option 2: Using Any Local Server (e.g., VS Code Live Server or Python)
If you prefer running through HTTP localhost:
- **Python 3:** Run `python -m http.server 8000` in the project folder and open `http://localhost:8000`.
- **Node.js:** Run `npx serve .` or use the VS Code Live Server extension.

---

## 🧪 Testing the CSV Upload Feature

1. Click the **"Sample CSV"** button in the filter toolbar (or locate `data/sample_social_media_data.csv`).
2. Open the file in Excel or Notepad to add your own test rows.
3. In the application, click **"Upload CSV"** in the top navigation bar.
4. Drag and drop your `.csv` file or browse to select it.
5. Choose whether to **Replace** the existing records or **Append** to them.
6. The dashboard KPI cards, platform cards, table, and charts will immediately refresh with your new data!

---

## 🎓 BCA Viva Voce Questions & Answers

**Q1: What is the main objective of this project?**  
*Answer:* To provide an automated, multi-platform social media data analysis and visualization dashboard that measures audience engagement rates, compares platform performance, and helps creators optimize their digital content strategy without relying on heavy backend infrastructure.

**Q2: How is the Engagement Rate calculated in this system?**  
*Answer:* Using the standard formula:  
`Engagement Rate (%) = ((Likes + Comments + Shares) / Views) * 100`.  
This measures active user engagement relative to total audience exposure.

**Q3: How does the CSV parser handle fields with commas inside quotation marks?**  
*Answer:* In `js/utils.js`, the `parseCSV()` function implements a character-by-character scanner tracking an `insideQuotes` boolean flag. Commas encountered while `insideQuotes` is `true` are treated as literal text rather than column delimiters.

**Q4: How do the filters interact with Chart.js?**  
*Answer:* When any filter (platform, format, date, or search) is changed, `applyFilters()` updates `AppState.filteredPosts`. It then calls `updateAllCharts()`, which recalculates platform aggregations, destroys the previous Chart.js instances if necessary, and re-renders new graphs with smooth animations.

**Q5: Can the application work completely offline?**  
*Answer:* Yes. `js/data.js` contains a complete bundled dataset of 30 multi-platform posts, so all table rendering, mathematical operations, and search functions run entirely in the browser client without server calls.

---

## 📄 License & Credits
Developed as a BCA Final Year Project. Open-source under the MIT License for educational and demonstration purposes.
