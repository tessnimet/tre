# Option 3: HTML Custom Visual & Export Template

This option provides two approaches:
1. **Option 3A**: Use the HTML template for exports, reports, or web viewing
2. **Option 3B**: Create a custom Power BI visual (advanced, requires development)

---

## Option 3A: HTML Template for Export/Reporting ✅

### Use Cases:
- Export Power BI data as HTML reports
- Create web-based versions of your dashboard
- Share dashboard outside Power BI
- Create printable versions
- Use for mobile-friendly viewing

### How to Use:

#### Step 1: Export Data from Power BI
1. In Power BI, go to each table/chart
2. Click **More options** (...) → **Export data**
3. Save as CSV file
4. Repeat for all data sources

#### Step 2: Update the HTML Template
1. Open `WayUp_Medical_Dashboard_Demo.html` in a text editor
2. Find the `<script>` section at the bottom (around line 819)
3. Replace the hardcoded data with your exported CSV data

**Example - Update the Line Chart Data:**
```javascript
// BEFORE (Hardcoded):
labels: ['Juin','Juil','Août','Sep','Oct','Nov','Déc','Jan','Fév','Mar','Avr','Mai'],
data: [210,245,189,267,298,312,278,334,289,356,321,342],

// AFTER (From your CSV):
labels: ['Jan','Feb','Mar','Apr','May','Jun'],
data: [245,189,267,298,312,278],
```

#### Step 3: View Your Dashboard
1. Open the updated HTML file in a web browser
2. Your data is now displayed in the beautiful WayUp Medical template
3. Save as PNG or PDF from your browser (Ctrl+P / Cmd+P)

### Advantages:
✅ Exact replica of the HTML design
✅ No Power BI licensing needed to view
✅ Highly portable (just send HTML file)
✅ Great for reports and presentations
✅ Mobile responsive

### Limitations:
✗ Static (doesn't update Power BI in real-time)
✗ Requires manual data updates
✗ Need to know where to find data in HTML

---

## Option 3B: Create a Custom Power BI Visual (Advanced)

### Prerequisites:
- Node.js installed
- Basic JavaScript knowledge
- Power BI Visuals SDK knowledge

### What You'll Get:
- A custom visual that loads directly in Power BI
- Dynamic data binding (updates with your data)
- Full interactivity

### Setup Steps:

#### Step 1: Install Power BI Visuals CLI
```bash
npm install -g powerbi-visuals-tools
pbiviz new WayUpMedicalVisual
cd WayUpMedicalVisual
```

#### Step 2: Get the Visual Files
1. Copy HTML content from `WayUp_Medical_Dashboard_Demo.html`
2. Copy CSS from the `<style>` section
3. Copy JavaScript from the `<script>` section

#### Step 3: Update the Visual Package
Edit `src/visual.ts`:
```typescript
import powerbiVisualsApi from "powerbi-visuals-api";
import DataView = powerbiVisualsApi.DataView;

export class Visual implements IVisual {
    // Your HTML template logic here
    // Map Power BI data to the template
}
```

#### Step 4: Build and Package
```bash
pbiviz package
```

#### Step 5: Import into Power BI
1. In Power BI, click the three dots (...)
2. Select **Import a custom visual**
3. Upload the `.pbix` file created in Step 4

### Resources:
- [Power BI Visuals SDK Documentation](https://learn.microsoft.com/en-us/power-bi/developer/visuals/custom-visual-develop-tutorial)
- [Power BI Visuals GitHub](https://github.com/Microsoft/PowerBI-visuals)
- [Sample Custom Visuals](https://github.com/Microsoft/PowerBI-visuals-sampleBarChart)

### Time Estimate:
- Learning: 2-4 hours
- Development: 4-8 hours
- Testing: 2-3 hours
- **Total: 8-15 hours** (if you're new to custom visuals)

---

## Comparison: Option 3A vs 3B

| Feature | 3A (HTML Export) | 3B (Custom Visual) |
|---------|------------------|-------------------|
| Setup Time | 5-10 min | 8-15 hours |
| Skill Required | Basic | Intermediate/Advanced |
| Power BI Integration | No (Export only) | Yes (Native) |
| Real-time Updates | No | Yes |
| Portability | High | Low |
| Customization | Easy (Edit HTML) | Very flexible |
| Maintenance | Simple | Complex |
| Best For | Reports/Exports | Production dashboards |

---

## Quick Start: Option 3A

### Fastest Way to Get Started:

#### 1. Export Your Data
```
In Power BI:
1. Click on a chart
2. More (...) → Export data
3. Save as CSV
```

#### 2. Open HTML File
```
In your browser:
1. Open WayUp_Medical_Dashboard_Demo.html
2. View the beautiful template
```

#### 3. Update Sample Data (Optional)
```
Edit the chart data section in the HTML to match your data
```

#### 4. Export/Share
```
Right-click in browser → Save as HTML
Or Ctrl+P → Print to PDF
```

---

## Example: Updating Chart Data in HTML

### Find this section:
```javascript
// LINE CHART
new Chart(document.getElementById('lineChart'), {
  type: 'line',
  data: {
    labels: ['Juin','Juil','Août','Sep','Oct','Nov','Déc','Jan','Fév','Mar','Avr','Mai'],
    datasets: [{
      label: 'RDV',
      data: [210,245,189,267,298,312,278,334,289,356,321,342],
      // ... rest of config
    }]
  }
});
```

### Replace with your data:
```javascript
// LINE CHART
new Chart(document.getElementById('lineChart'), {
  type: 'line',
  data: {
    labels: ['Jan','Feb','Mar','Apr','May','Jun'],  // ← Your months
    datasets: [{
      label: 'Appointments',  // ← Your label
      data: [245, 312, 289, 356, 298, 321],  // ← Your numbers
      // ... rest of config
    }]
  }
});
```

---

## Video Tutorial (for Option 3B)
- [Power BI Custom Visuals Development](https://www.youtube.com/watch?v=5Kb_mNRTLiI)
- [Building Your First Custom Visual](https://www.youtube.com/watch?v=SgR6i50pJxo)

---

## Support for Option 3B
If building a custom visual, you'll need:
1. Intermediate JavaScript/TypeScript skills
2. Understanding of Power BI data model
3. Familiarity with D3.js or Chart.js
4. Time to debug and test

**Recommendation**: Start with Option 1 or 2 first. Only use Option 3B if you need custom functionality not available in standard Power BI visuals.

---

## Summary

| Approach | Ease | Speed | Quality | Recommendation |
|----------|------|-------|---------|-----------------|
| Option 1 (Theme) | ⭐⭐⭐⭐⭐ | ⚡ 5 min | ⭐⭐⭐⭐ | **START HERE** ✅ |
| Option 2 (Manual) | ⭐⭐⭐ | ⏱️ 30-60 min | ⭐⭐⭐⭐⭐ | If Option 1 not enough |
| Option 3A (HTML) | ⭐⭐⭐⭐ | ⏱️ 15 min | ⭐⭐⭐⭐⭐ | For exports/reports |
| Option 3B (Custom) | ⭐ | 📅 Hours | ⭐⭐⭐⭐⭐ | If you need native integration |

**Recommendation Order**:
1. **Try Option 1** first (easiest, fastest)
2. **Then Option 2** if you need fine-tuning
3. **Then Option 3A** if you need HTML exports
4. **Only Option 3B** if you need a production custom visual

---

**Ready? Start with Option 1 in `QUICK_SETUP_OPTION1.md`! 🚀**
