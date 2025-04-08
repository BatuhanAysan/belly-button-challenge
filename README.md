# 🧬 Belly Button Biodiversity Dashboard

## 📌 Overview

This project is an interactive data visualization dashboard that explores the *Belly Button Biodiversity* dataset. The dataset catalogs the microbial species (OTUs) found in human navels. The dashboard allows users to select test subjects and view:

- The top 10 bacterial cultures found.
- A full OTU distribution per sample in a bubble chart.
- Demographic metadata associated with each individual.

The app is built using **JavaScript**, **D3.js**, and **Plotly.js**, and is deployed via **GitHub Pages**.

---

## 🚀 Live Demo

🔗 [GitHub Pages Link](https://batuhanaysan.github.io/belly-button-challenge/)  

🔗 [GitHub Repository](https://github.com/BatuhanAysan/belly-button-challenge)

---

## 📁 Project Structure

```text
belly-button-challenge/
├── index.html              # Main HTML page
├── samples.json            # Dataset (reference only - loaded externally)
├── README.md               # Project documentation
├── static/
│   └── js/
│       └── app.js          # JavaScript logic for fetching data and building charts
```
---

## 📈 Features

- **Dropdown menu** to select test subject IDs.
- **Horizontal bar chart** of top 10 bacterial OTUs per individual.
- **Bubble chart** showing all bacteria with dynamic marker size and color.
- **Metadata panel** with demographic info per subject.
- **Fully dynamic interactivity** on selection changes.
- **Responsive Plotly visualizations** using external JSON data.

---

## ⚙️ How It Works

### 1. `init()`  
Initializes the dashboard:
- Loads data from external JSON.
- Populates dropdown with test subject IDs.
- Renders default charts and metadata (first sample in the list).

### 2. `buildCharts(sample)`  
Creates:
- A **bar chart** (Top 10 OTUs for selected individual).
- A **bubble chart** (all sample OTUs).

Uses `Plotly.newPlot()` to render visualizations.

### 3. `buildMetadata(sample)`  
Updates the metadata panel with key-value pairs for the selected individual.

### 4. `optionChanged(newSample)`  
Fired when user selects a different ID from the dropdown. Triggers both chart and metadata updates.

---

## 📊 Libraries & Tools

- [D3.js](https://d3js.org/) – For data loading and DOM manipulation  
- [Plotly.js](https://plotly.com/javascript/) – For building interactive charts  
- [GitHub Pages](https://pages.github.com/) – For hosting the project

---

## ✅ Requirements Met

✔️ Bar chart with top 10 OTUs (dynamic)  
✔️ Bubble chart with full data (interactive)  
✔️ Metadata panel updates on selection  
✔️ GitHub Pages deployment (optional if not yet deployed)

---

## 🧠 Notes

- Data is loaded from this URL:  
  `https://static.bc-edx.com/data/dl-1-2/m14/lms/starter/samples.json`
- Project follows best practices for code readability and component structure.
- `console.log()` was used during development for debugging.

---

## 🙏 Acknowledgements

- This project was inspired by the *Belly Button Biodiversity* study conducted by the [Rob Dunn Lab](http://robdunnlab.com/projects/belly-button-biodiversity/results-and-data/).
- The dataset and starter code were provided by the instructional team of the Data Analytics Bootcamp.
- Minor code references and troubleshooting solutions were adapted from community resources such as Stack Overflow.


