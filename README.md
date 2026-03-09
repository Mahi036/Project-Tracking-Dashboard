# 📊 Global Delivery Feedback Dashboard – Houston Office

A **100% local, privacy-first** dashboard for visualizing the Global Delivery Feedback Form data (Knowcraft × Stout).

> **🔒 No data ever leaves your device.** Everything runs in your browser. No server. No upload. No tracking.

---

## 🚀 How to Use

1. **Download** `global_delivery_dashboard.html`
2. **Open** it directly in any browser (Chrome, Firefox, Edge, Safari)
3. **Upload** your CSV or Excel file (`.csv`, `.xlsx`, `.xls`)
4. Instantly see your dashboard!

> You don't need to install anything. No Node.js. No Python. No internet after the first load.

---

## 📁 Supported File Formats

| Format | Extension |
|--------|-----------|
| Excel  | `.xlsx`, `.xls` |
| CSV    | `.csv` |

The dashboard auto-detects your column names — it works even if column headers are slightly different.

---

## 📈 What You Get

### KPI Cards
- Total Projects
- Open / Closed counts (with %)
- PCS vs CVA counts
- Unique Team Members

### Charts
| Chart | Description |
|-------|-------------|
| Open vs Closed | Donut chart of project status |
| CVA vs PCS | Breakdown of project type |
| Project Types | Bar chart (Hourly, Full Project, QC, etc.) |
| Projects per Team Member | Horizontal bar, top contributors |
| Projects Over Time | Line chart by due date (monthly) |

### Filters
- **Quarter** (Q1 2024, Q2 2024, etc. — auto-detected from Due Date)
- **CVA / PCS**
- **Project Type**
- **Open / Closed status**
- **Team Member** (any of Member 1, 2, or 3)

### Data Table
- Paginated to 200 rows (apply filters to narrow down)
- Color-coded badges for status and CVA/PCS
- Auto-populated Quarter column

---

## 🔐 Privacy & Security

- **Zero network requests** after page load
- **No cookies, no localStorage** — data only lives in memory during your session
- **No analytics, no tracking**
- Safe to use with confidential project data

---

## 🌐 Hosting on GitHub (for your team)

1. Create a new **GitHub repository** (can be private)
2. Upload `global_delivery_dashboard.html`
3. Go to **Settings → Pages → Deploy from branch → main**
4. Share the GitHub Pages URL with your team

Each user opens the dashboard in their browser and uploads their own local file. **Nothing is shared or stored.**

Alternatively, team members can just download the `.html` file and open it locally — no GitHub Pages needed.

---

## 🧩 Column Mapping

The dashboard looks for these column names (case-insensitive):

| Dashboard Field | Expected Column Name |
|-----------------|----------------------|
| Project Name | `Project Code / Name` |
| Date Assigned | `Date Assigned` |
| Due Date | `Due Date` |
| CVA/PCS | `CVA/PCS` |
| Project Type | `Project Type` |
| Scope | `Scope` |
| Tasks | `Brief Description of Tasks` |
| Status | `Open/Closed` |
| Team Member 1 | `Knowcraft Team Member #1` |
| Team Member 2 | `Knowcraft Team Member #2 (as applicable)` |
| Team Member 3 | `Knowcraft Team Member #3 (as applicable)` |
| Stout POC | `Stout Point of Contact` |
| Knowcraft Feedback | `Knowcraft Comment and Feedback` |
| Stout Feedback | `Stout Comment and Feedback` |

---

*Built with Chart.js, PapaParse, and SheetJS. Single HTML file. No build step.*
