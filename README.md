# Petra Brands — Retail Command Center

A comprehensive retail sales analytics dashboard for House of Party (HOP), PixlePop, and Muddies brands.

## 🚀 Live Dashboard

**https://alikaaba-bit.github.io/petra-retail-dashboard/**

## 📊 Features

### Brand Hierarchy
- **House of Party** (parent brand)
  - Party Hero (HOP-PH) — balloon & decor kits
  - Table Hero (HOP-TH) — tableware & party supplies
  - Balloon Creations (HOP-BC) — balloon garland sets
- **PixlePop** (HOP-PXL) — puzzles, stickers, coasters, 3D displays
- **Muddies** (HOP-MUD) — art & craft kits

### Dashboard Tabs

1. **Overview**
   - KPIs (revenue, GP, margin, units)
   - Brand cards with sub-line drill-down
   - Retailer bars + donut chart
   - Monthly revenue/GP trend
   - YOY comparison
   - Annual summary
   - Payment terms breakdown

2. **Retailers**
   - Full retailer breakdown with brand tags
   - Stacked monthly chart
   - Retailer × brand matrix table
   - Brand-split horizontal bars

3. **SKU Intel**
   - Sortable SKU table (revenue/units/margin)
   - Performance signals (🔥/✅/⚠️)
   - Top 10 SKUs chart
   - Pagination

4. **Forecast**
   - Inventory velocity for high-volume SKUs
   - Trend detection (📈/📉/→)
   - Reorder planning calculator (8-week China lead time)

### Filters
- **Brand**: House of Party / PixlePop / Muddies
- **HOP Sub-line**: Party Hero / Table Hero / Balloon Creations
- **Retailer**: Dropdown with all 11 retailers
- **Year**: All / 2025 / 2026
- **Status**: All / Confirmed / Cancelled

## 📈 Data Stats

- **1,330** order line items
- **88** SKUs with COG data
- **11** retailers (Target 84.8% dominant)
- **42** unique POs
- **$2.06M** revenue (2025), **$46.7K** (2026 Jan-Feb)

## 🛠️ Tech Stack

- **React 18** + **Vite**
- **Recharts** for visualizations
- **GitHub Pages** for hosting
- **GitHub Actions** for auto-deploy

## 🚀 Development

```bash
# Install dependencies
npm install

# Run dev server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## 📦 Deployment

Automatically deploys to GitHub Pages on push to `main` branch via GitHub Actions.

## 🔄 Updating Data

1. Export new PO tracker Excel file
2. Run data parser to generate JSON
3. Update embedded data in `src/App.jsx`
4. Push to main branch
5. Dashboard auto-deploys in ~2 minutes

## 📝 Notes

- Data embedded as compressed JSON (~245KB)
- No backend required
- Dark theme (#0C0A14) with HOP brand colors
- Fully responsive design
- Custom scrollbars

## 🐛 Known Limitations

- Endcap C3 Target POs (~1,100 items) lack COG data
- Threadies brand not yet in tracker
- Retail only (no Amazon/DTC data)

## 📄 License

Proprietary - Petra Brands
