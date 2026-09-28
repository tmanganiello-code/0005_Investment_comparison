# InvestCompare

**InvestCompare** is an interactive, single-page web application designed to help users simulate, analyze, and compare two financial investment strategies side-by-side. It provides detailed nominal and inflation-adjusted (real) growth projections by accounting for compound interest, capital gains tax, stamp duty, recurring fees, and periodic contributions.

---

## Key Features

* **Side-by-Side Comparison:** Model two distinct investments (**Investment A** vs. **Investment B**) under identical global simulation timelines.
* **Realistic Financial Engine:**
  * **Compounding Options:** Flexible annual or monthly compounding schedules.
  * **Tax & Stamp Duty Handling:** Support for standard tax rates (26%, 12.5%, custom) applied strictly to capital profits, plus flexible stamp duty calculations (asset-based, average value, or disabled).
  * **Fee Structures:** Multi-tiered fee configurations including initial, recurring annual, and final liquidation fees (percentage or fixed amounts).
  * **Periodic Contributions:** Option to simulate ongoing monthly contributions.
  * **Variable Annual Returns:** Set distinct year-by-year return rates under advanced settings.
* **Inflation-Adjusted Real Growth:** Dynamically adjusts nominal balances against expected annual inflation to calculate true purchasing power over time.
* **Visual Analytics & Reporting:**
  * Dynamic charts powered by [Chart.js](https://www.chartjs.org/) illustrating capital evolution and cumulative net vs. real growth.
  * Side-by-side KPI metrics and numeric comparison summary tables.
* **Localization & Usability:**
  * **CSV Data Export:** Export detailed year-end breakdowns for further spreadsheet analysis.
  * **Multilingual:** On-the-fly toggling between Italian and English UI languages.
  * **Theme Preferences:** Built-in dark/light mode toggle with system color scheme detection.

---

## Tech Stack

* **Frontend:** Standalone **HTML5**, **CSS3** (Custom Properties, Flexbox, Grid), and vanilla **JavaScript (ES6+)**.
* **Visualization:** [Chart.js](https://cdn.jsdelivr.net/npm/chart.js) (loaded via CDN).
* **State Management:** Browser `localStorage` for persisting user inputs and preference settings across sessions.

---

## Getting Started

Because **InvestCompare** is a lightweight, fully client-side application, no node dependencies, build steps, or server setups are required.

### Quick Start

1. Clone or download this repository:
   ```bash
   git clone https://github.com/your-username/invest-compare.git
   ```
2. Open `index.html` directly in any modern web browser.

---

## How to Use

1. **Global Parameters:** Set the overall duration (in years), expected annual inflation rate, compounding frequency, and optional monthly contributions.
2. **Investment Parameters:** Configure the initial capital, expected returns, tax rates, stamp duties, and fee structures for **Investment A** and **Investment B**.
3. **Simulate:** Click **Recalculate** (*Ricalcola*) to update results, charts, and key performance metrics.
4. **Export:** Click **Export CSV** (*Esporta CSV*) to download the complete year-by-year financial table.

---

## Disclaimer

*This application performs mathematical simulations based on parameters provided by the user and does not constitute financial, tax, or legal advice. Real-world fiscal regimes, fees, and tax mechanisms depend on specific financial instruments and local legislation.*
