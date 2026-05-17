# 🎨 Option 2: Manual Formatting Guide (30-60 minutes)

## Fine-Tuned Control Over Every Visual

This option gives you **complete control** over how each element looks. Use this if:
- Option 1 applied the theme but you want to customize further
- You need specific colors for certain visuals
- You want precise control over styling
- You need to match different elements differently

---

## 📊 What You'll Format

1. **KPI Cards** - Large number displays
2. **Line Charts** - Trend lines
3. **Bar Charts** - Comparisons
4. **Donut/Pie Charts** - Distributions
5. **Tables** - Data grids
6. **Slicers** - Filters
7. **Text Boxes** - Labels

---

## 🎨 Color Palette Reference

Copy these hex codes as needed:

```
Primary:
- Navy:        #0D2137
- Blue:        #1A5FA8
- Blue Mid:    #2E75B6
- Blue Light:  #4A9FE0

Status:
- Green:       #0D9E6E (Good/Success)
- Orange:      #E8850A (Warning)
- Red:         #D63B3B (Alert/Bad)
- Purple:      #6C3FC5 (Accent)

Backgrounds:
- Blue Pale:   #E8F3FB
- Green Pale:  #E6F7F2
- Orange Pale: #FEF3E2
- Red Pale:    #FDE8E8
- Page BG:     #F0F5FB
- Border:      #D8E6F3
```

---

## 🚀 Step-by-Step Formatting

### Part 1: KPI Cards (10 minutes)

#### Setup:
1. Create a card visual with your data
2. Click the card to select it
3. Click the **Format visual** icon (paint brush) on the right

#### Formatting:
1. Go to **Format visual** panel
2. Expand **Card**
3. Set:
   - **Background**: #FFFFFF (white)
   - **Border**: On, color #D8E6F3, width 1px
   - **Shadow**: On, with 2px offset

#### Value Styling:
1. Expand **Data label** or **Value**
2. Set:
   - **Color**: #0D2137 (navy)
   - **Font**: DM Sans, size 26, weight 700

#### Label Styling:
1. Expand **Category label** or **Label**
2. Set:
   - **Color**: #7A9AB8 (light gray)
   - **Font**: DM Sans, size 11, weight 500

**Expected Result**: Professional white card with navy values and gray labels

---

### Part 2: Line Charts (10 minutes)

#### Setup:
1. Click your line chart
2. Go to **Format visual**

#### Lines:
1. Expand **Lines**
2. Set:
   - **Color**: #1A5FA8 (blue)
   - **Stroke width**: 2.5
   - **Style**: Solid

#### Points:
1. Expand **Data points**
2. Set:
   - **Color**: #1A5FA8 (blue)
   - **Size**: 3-4px
   - **Show**: On

#### Axes:
1. Expand **X-axis**
   - **Color**: #7A9AB8
   - **Title size**: 10px
2. Expand **Y-axis**
   - **Grid lines color**: #F0F5FB (light)
   - **Color**: #7A9AB8

#### Legend:
1. Expand **Legend**
2. Set:
   - **Position**: Bottom
   - **Text color**: #3A5A7A
   - **Font size**: 11px

**Expected Result**: Professional blue line with points, light grid

---

### Part 3: Bar Charts (10 minutes)

#### Setup:
1. Click your bar chart
2. Go to **Format visual**

#### Data Colors:
1. Expand **Data colors**
2. For each bar series:
   - **Primary**: #1A5FA8 (blue)
   - Or use status colors:
     - Good → #0D9E6E (green)
     - Warning → #E8850A (orange)
     - Alert → #D63B3B (red)

#### Bars:
1. Expand **Bars**
2. Set:
   - **Radius**: 6px (rounded corners)
   - **Outline**: #D8E6F3
   - **Width**: 70%

#### Axes:
1. Expand **X-axis**
   - **Text color**: #3A5A7A
   - **Font size**: 10px
2. Expand **Y-axis**
   - **Grid lines**: On, color #F0F5FB
   - **Text color**: #7A9AB8

**Expected Result**: Professional rounded bars with consistent colors

---

### Part 4: Donut/Pie Charts (8 minutes)

#### Setup:
1. Click your donut chart
2. Go to **Format visual**

#### Data Colors:
Use this color sequence:
1. #1A5FA8 (blue)
2. #0D9E6E (green)
3. #E8850A (orange)
4. #D63B3B (red)
5. #6C3FC5 (purple)

#### Chart:
1. Expand **Chart**
2. Set:
   - **Inner radius** (for donut): 68-72%
   - **Data label color**: #0D2137 (navy)

#### Legend:
1. Expand **Legend**
2. Set:
   - **Position**: Bottom
   - **Text color**: #3A5A7A
   - **Font size**: 10px

**Expected Result**: Beautiful multicolor donut with professional legend

---

### Part 5: Tables (12 minutes)

#### Setup:
1. Click your table
2. Go to **Format visual**

#### General:
1. Expand **Grid**
2. Set:
   - **Grid color**: #D8E6F3
   - **Outline color**: #D8E6F3
   - **Text size**: 12px

#### Header:
1. Expand **Column headers**
2. Set:
   - **Background**: #0D2137 (navy)
   - **Text color**: #FFFFFF (white)
   - **Text size**: 11px, weight 600
   - **Alignment**: Left

#### Rows:
1. Expand **Values**
2. Set:
   - **Text color**: #0D2137 (navy)
   - **Alternating row colors**: Off (keep white)
   - **Text size**: 12px

#### Hover Effect (Optional):
1. Expand **Row hover**
2. Set:
   - **Background**: #E8F3FB (light blue)

**Expected Result**: Professional table with navy header and white rows

---

### Part 6: Status Badge Styling (5 minutes)

If you have status indicators (Good/Bad/Warning):

#### For "Good" Status:
- **Background**: #E6F7F2 (green pale)
- **Text**: #0D9E6E (green)
- **Border**: #0D9E6E (optional)

#### For "Warning" Status:
- **Background**: #FEF3E2 (orange pale)
- **Text**: #E8850A (orange)
- **Border**: #E8850A (optional)

#### For "Alert" Status:
- **Background**: #FDE8E8 (red pale)
- **Text**: #D63B3B (red)
- **Border**: #D63B3B (optional)

**Example**: In a table, format status column cells with these colors

---

### Part 7: Slicers (5 minutes)

#### Setup:
1. Click your slicer
2. Go to **Format visual**

#### Styling:
1. Expand **Selection controls**
2. Set:
   - **Background (selected)**: #E8F3FB (light blue)
   - **Text (selected)**: #1A5FA8 (blue)
   - **Background (unselected)**: #FFFFFF (white)
   - **Text (unselected)**: #3A5A7A (dark gray)

#### Border:
1. Set:
   - **Outline**: #D8E6F3
   - **Width**: 1px

**Expected Result**: Professional filter controls with blue highlight

---

### Part 8: Text Boxes & Titles (5 minutes)

#### Large Titles:
1. **Font**: Plus Jakarta Sans (if available), else DM Sans
2. **Size**: 18px
3. **Weight**: 700 (bold)
4. **Color**: #0D2137 (navy)

#### Section Titles:
1. **Font**: Plus Jakarta Sans, else DM Sans
2. **Size**: 13px
3. **Weight**: 700 (bold)
4. **Color**: #7A9AB8 (light gray)
5. **Transform**: UPPERCASE (optional)

#### Body Text:
1. **Font**: DM Sans
2. **Size**: 12px
3. **Weight**: 400 (regular)
4. **Color**: #3A5A7A (dark gray)

**Expected Result**: Professional text hierarchy

---

## 📋 Formatting Checklist

- [ ] KPI Cards - White with navy text
- [ ] Line Charts - Blue lines with points
- [ ] Bar Charts - Blue/status colors with rounded bars
- [ ] Donut Charts - Multicolor with proper legend
- [ ] Tables - Navy headers, white rows
- [ ] Status Badges - Green/Orange/Red backgrounds
- [ ] Slicers - Blue selection state
- [ ] Text - Proper hierarchy and colors
- [ ] Overall - Consistent medical design system

---

## 🎨 Before & After

### Before (Default):
- ❌ Gray background
- ❌ Black text
- ❌ Standard blue charts
- ❌ Generic tables
- ❌ Inconsistent styling

### After (Manual Formatting):
- ✅ Light blue background (#F0F5FB)
- ✅ Navy text (#0D2137)
- ✅ Professional blue/status colors
- ✅ Professional tables with navy headers
- ✅ Consistent medical design system

---

## 💡 Pro Tips

### Tip 1: Copy Formatting
Once you format one visual, copy that format to similar visuals:
1. Select formatted visual
2. Copy format (Ctrl+Alt+C or Format Painter)
3. Paste to other visuals

### Tip 2: Use Conditional Formatting
For status columns, use conditional formatting instead of manual coloring:
1. Select data column
2. Right-click → Conditional formatting
3. Set color rules

### Tip 3: Create a Master Template
Once you have one page perfectly styled, copy the entire page to reuse styling:
1. Right-click page tab
2. Duplicate page
3. Replace data/visuals

### Tip 4: Save as Template
Once styled, save as a template for future dashboards:
1. File → Save as template
2. Name it "Medical Dashboard Template"
3. Reuse for future projects

---

## ❓ Common Issues & Fixes

### Issue: Colors look different than in the HTML template
**Fix**: Double-check you're using exact hex codes. Copy/paste them to avoid typos.

### Issue: Text is too small/large
**Fix**: Go to Format visual → Text properties, adjust font size.

### Issue: Table header won't change color
**Fix**: Make sure you're in the "Column headers" section, not "Values".

### Issue: Slicer selection isn't visible
**Fix**: Check that "Selection controls" background color is different from unselected color.

### Issue: Chart colors aren't consistent
**Fix**: Check each series individually in "Data colors" section.

---

## 🚀 Next Steps

After manual formatting:

1. **Satisfied?** → Done! Save your file. 🎉
2. **Need to export?** → See `OPTION3_HTML_CUSTOM_VISUAL.md` (3A)
3. **Want custom visual?** → See `OPTION3_HTML_CUSTOM_VISUAL.md` (3B)
4. **Done with styling?** → Share your dashboard!

---

## 📁 Reference Files

| File | Purpose |
|------|---------|
| `QUICK_SETUP_OPTION1.md` | Apply theme automatically (5 min) |
| `OPTION2_MANUAL_FORMATTING.md` | This file (fine-tune) |
| `OPTION3_HTML_CUSTOM_VISUAL.md` | Export or custom visual |
| `STYLING_GUIDE.md` | Overview of all options |

---

## 📊 Estimated Time Breakdown

| Component | Time |
|-----------|------|
| KPI Cards | 10 min |
| Line Charts | 10 min |
| Bar Charts | 10 min |
| Donut Charts | 8 min |
| Tables | 12 min |
| Badges | 5 min |
| Slicers | 5 min |
| Text/Titles | 5 min |
| **Total** | **~60 min** |

Or ~30 minutes if you skip some components.

---

**You've got this! Take your time and create a beautiful dashboard! 🏥✨**
