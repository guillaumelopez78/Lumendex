# Design Assets Hub

Design files, components, and visual systems for **Cash Pilot**.

---

## 🎨 Figma & Prototypes

| Asset | Status | Link |
|-------|--------|------|
| **MVP Prototype** | Complete | [Figma] (see Figma link in MVP brief) |
| **Design System** | In Use | [Lumen Design System] |
| **Component Library** | Active | [Figma Components] |

**Figma File:** Cash Pilot MVP - [See project brief for link]

---

## 🎯 Visual Design System

**Design Tokens:**
- **Colors:** Primary (brand), Secondary, Semantic (success/warning/error), Neutral
- **Typography:** Primary typeface, sizing hierarchy, line heights
- **Spacing:** 8px base unit, grid structure, padding standards
- **Shadows:** Component depth, elevation system

**See:** Lumen Design System documentation

---

## 🧩 Component Library

### Core Components
- **KPI Display** - Large number + label + context
- **Chart (Balance Curve + Histogram)** - Main visualization
- **Transaction List** - Grouped by type, expandable
- **Summary Cards** - Cash In/Out/Net/Balance
- **Date Range Picker** - Week/month selection

### UI Elements
- **Buttons** - Primary action, secondary, tertiary
- **Cards** - Container with shadow/border
- **Modals** - Dialog for What-If scenarios
- **Badges** - Status indicators (Pending, Overdue, Paid)
- **Tooltips** - Hover details on chart

---

## 📐 Layout & Responsive

### Desktop Layout
**Above-the-fold:**
- Primary KPI (Projected Balance)
- Secondary KPI (Cash Runway)
- Chart

**Below-the-fold:**
- Tax Reserves section
- Transaction list with filters

### Mobile Layout (Future)
- Simplified KPIs
- Chart with swipe navigation
- Full-screen transaction details
- Stacked layout (no side panels)

---

## 🎭 Design Specs

**Visual Hierarchy:**
- Large numbers (KPIs) at top
- Chart as main focal point
- Actions below the fold

**Color Palette:**
- Cash In: Green (positive)
- Cash Out: Gray/Blue (neutral)
- Tax Reserves: Outlined box with warning color
- Warnings: Red when balance approaches negative

**Typography:**
- Primary KPI: Large, Bold, Primary color
- Secondary: Medium, Semi-Bold
- Body: Regular weight, readable contrast
- Metadata: Small, Light gray

---

## 📋 Design Checklist

- [x] MVP design complete
- [x] Figma prototype tested (Maze test - 7 users)
- [x] Component library documented
- [ ] Design system tokens finalized
- [ ] Mobile designs (post-MVP)
- [ ] Accessibility audit (WCAG AA)

---

## 🔗 Related Categories

- [[../04_TECHNICAL/Technical Hub.md|Technical]] - Implementation details
- [[../06_DISCOVERY/Discovery Hub.md|Discovery]] - Maze test results & feedback

---

## 📌 Project Hub

- [[../Cash Pilot - Overview.md|Cash Pilot - Overview]]

---

**Last Updated:** June 2026  
**Owner:** Martin Albrecht Kvien (Designer)  
**Design Tool:** Figma  
**Status:** MVP complete, post-MVP in planning
