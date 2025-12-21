# Smart Construction Cost Predictor and Market Analyzer

This is a front-end based analytics dashboard that estimates construction project costs and shows how different project parameters affect overall cost, risk, and planning decisions.

The project was built to explore **how cost estimation can be structured analytically**, rather than relying only on rough thumb rules or isolated spreadsheets.

---

## Why I Built This
During my civil engineering coursework and personal learning, I noticed that cost discussions often depend heavily on experience and approximations. While that works on site, I wanted to see if the same thinking could be converted into a simple analytical system where inputs and assumptions are clearly visible.

This project is my attempt to **model cost trade-offs and planning factors in a structured way**, using code instead of manual calculations.

---

## What the Application Does
The dashboard takes basic project details such as:
- project type
- built-up area
- city/location tier
- construction quality
- timeline and labor availability

Based on these inputs, it:
- estimates total project cost and cost per square foot
- splits cost into materials, labor, equipment, overhead, and contingency
- highlights possible risks related to cost, time, and quality
- shows charts and trends to make comparisons easier

The goal is not perfect accuracy, but **clear understanding of how changes in inputs impact results**.

---

## How the Cost Logic Works (High Level)
- Each project type starts with a base cost
- Multipliers are applied for:
  - location tier
  - quality grade
  - labor availability
  - market conditions
  - season
  - number of floors, basements, and timeline pressure
- Costs are then distributed using fixed ratios to represent materials, labor, equipment, and overhead
- An additional contingency buffer is added to account for uncertainty

This approach is similar to how early-stage feasibility or planning discussions are done.

---

## Outputs Generated
- **Key metrics**: total cost, unit cost, contingency buffer
- **Visuals**:
  - cost breakup chart
  - material price trend chart
- **Risk indicators**:
  - cost overrun risk
  - timeline risk
  - quality risk
- **Text insights** that explain why costs or risks increase under certain conditions

---

## Tech Stack
- HTML & CSS for layout and styling
- JavaScript for cost calculations and logic
- Chart.js for visualizations

This project is fully client-side and runs in the browser.

---

## Limitations
- Cost values and ratios are based on assumed industry averages
- Material price trends are simulated, not live market data
- The estimates should not be used as final BOQs or tender values

The intent is analytical learning, not professional estimation.

---

## What I Learned
- How to convert domain assumptions into structured logic
- How dashboards help in comparing scenarios quickly
- How small changes in inputs (location, timeline, labor) can significantly impact cost and risk
- How to present numerical results in a way that supports decision-making

---

## Possible Improvements
- Storing historical project data using a database
- Adding export options (Excel / PDF)
- Connecting to live commodity price APIs
- Rebuilding the dashboard in Power BI or a backend-based system

---

## Author
**Priyanshu Aryan**  
B.Tech Civil Engineering, IIT Patna  
2022-2026

This project reflects my interest in analytics, dashboards, and data-driven decision systems.
