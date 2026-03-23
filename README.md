# 📊 Playwright Test Dashboard

A simple, visual dashboard for viewing Playwright test results with charts and export options.

![Playwright](https://img.shields.io/badge/Playwright-Testing-blue)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 🎯 What It Does

- 📈 **Shows test statistics** - Total tests, passed, failed
- 🥧 **Pie chart visualization** - Quick pass/fail ratio view
- 📋 **Detailed test table** - Test names, status, duration, file
- 💾 **Export options** - Copy to Excel or download CSV
- 📁 **Load JSON reports** - Import any Playwright test results

---

## 🚀 Quick Start

1. **Open the dashboard** - Just open the HTML file in any browser
2. **Load your test results** - Click "Load JSON File" and select your Playwright report
3. **View results** - See stats, chart, and detailed table instantly

> 💡 **Sample data included** - The dashboard loads with example data so you can see how it works!

---

## 📖 How to Get Your Test Data

### Method 1: From Playwright HTML Report
```bash
# Run tests with HTML reporter
npx playwright test --reporter=html

# Open report, press F12 → Console, type:
copy(JSON.stringify(window.playwrightReport))

# Save as results.json and load in dashboard
Method 2: JSON Reporter
bash
npx playwright test --reporter=json > results.json
✨ Features
Feature	What It Does
Statistics Cards	Color-coded cards showing totals
Pie Chart	Visual pass/fail distribution
Test Table	All tests with status and duration
Copy to Excel	One-click copy to clipboard
Export CSV	Download results as CSV file
🛠️ Troubleshooting
No data loading?

Ensure your JSON file has the correct format

Check browser console (F12) for errors

Chart not showing?

Refresh the page

Check internet connection (Chart.js loads from CDN)

📁 JSON Format Example
json
{
  "suites": [{
    "specs": [{
      "file": "test.spec.ts",
      "tests": [{
        "title": "Test name",
        "results": [{
          "status": "passed",
          "duration": 1234
        }]
      }]
    }]
  }]
}
🎨 Customization
Change Colors
Edit the CSS to match your brand:

css
.stat-card.passed { background: linear-gradient(135deg, #28a745, #20c997); }
button { background-color: #007bff; }
📄 License
MIT - Free to use and modify

Made for test automation teams 🚀

text

This README is:
- ✅ **Short and simple** - Easy to read
- ✅ **Large text** - Clear headings and sections
- ✅ **Visually appealing** - Emojis and badges
- ✅ **GitHub ready** - Proper markdown formatting
- ✅ **Practical** - Quick start and troubleshooting



The "🗑️ Clear All Data" button will remove all existing data from the dashboard. After clearing, when you upload new test results, only your uploaded data will be displayed.

Here's how it works:

📋 Data Management
✅ Clear All Data Button
Click 🗑️ Clear All Data to remove ALL existing test results

This clears:

🤖 Automated tests

✍️ Manual tests

🎮 Maths quiz results

All statistics and charts

Dashboard will show zero results

📁 Uploading New Data
After clearing, you can upload:

🤖 Automated Tests - Load JSON file from Playwright

✍️ Manual Testing - Add manual test entries

🎮 Maths Quiz Game - Import quiz results

💡 Quick Steps
Clear current data → Click 🗑️ Clear All Data

Upload your data → Use the appropriate import/upload button

View results → Only your uploaded data appears

⚠️ Important Notes
Action	Result
Clear All Data	Removes EVERYTHING (automated, manual, quiz results)
Upload Automated Tests	Adds to existing data (unless you cleared first)
Manual Testing	Adds to existing data
Maths Quiz	Adds to existing data
🎯 Best Practice
If you want ONLY your uploaded data:

Click 🗑️ Clear All Data first

Then upload your test results

Dashboard will show ONLY what you uploaded

Tip: The sample data (Emma, Liam, Sophia, Oliver's quizzes) is just demo data. You can clear it before adding your data or JSON file and so it will then show just your real test results! 🚀
