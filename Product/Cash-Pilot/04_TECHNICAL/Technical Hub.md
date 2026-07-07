# Technical Hub

Technical architecture, data sources, and integrations for **Cash Pilot**.

---

## 🏗️ Architecture Overview

| Component | Source | Status |
|-----------|--------|--------|
| **Bank Data** | Open Banking API | Active |
| **Invoices** | Invoice Core | Integrated |
| **Expenses** | Expense Module | Integrated |
| **Tax Data** | Bookkeeping | Integrated |

---

## 📊 Data Sources & Integration

### 1. Banking Data (Open Banking API)
**Purpose:** Current balance, transaction history  
**Refresh Rate:** Multiple times daily  
**Data Quality:** High (reconciled transactions)

### 2. Invoicing System
**Purpose:** Sent invoices (receivables), payment tracking  
**Integration:** Native to Shine  
**Data Quality:** High (source of truth)

### 3. Expenses Module
**Purpose:** Recurring expenses, one-time costs  
**Integration:** Native to Shine  
**Data Quality:** High

### 4. Bookkeeping System
**Purpose:** Tax calculations, historical data  
**Integration:** Native to Shine  
**Data Quality:** High

---

## ⚙️ Forecast Calculation

### Accuracy Levels

**0-60 Days: High Accuracy**
- Uses actual invoices + bank transactions
- Reconciled against real data
- Minimal estimation

**60+ Days: High Estimation**
- Based on Year-over-Year trends
- Recurring expense patterns
- Seasonal averages

### Tax Calculation
- VAT: Aggregated from invoicing system
- Income Tax: Based on earnings + country thresholds
- Corporate Tax: Annual thresholds
- **Updated:** Annually to reflect regulations

---

## 🔄 Data Refresh & Recalculation

**Real-time Triggers:**
- User marks invoice as "Sent" → Recalculate immediately
- User records expense → Recalculate immediately
- Bank transaction arrives → Recalculate next refresh cycle

**Scheduled Refresh:**
- Open Banking API: Multiple times daily
- Bookkeeping data: Daily sync
- User actions: Real-time

---

## 🛡️ Technical Constraints

| Constraint | Impact | Solution |
|-----------|--------|----------|
| Data Freshness | Accuracy | API refresh x/day + real-time triggers |
| Tax Law Changes | Reliability | Annual thresholds update |
| Multi-currency | Complexity | Convert to base currency + display |
| Data Privacy | Security | GDPR compliance, encrypted storage |

---

## 📚 Technical Documentation

**See Also:**
- [[Infrastructure.md]] - Azure infrastructure
- [[API Integrations.md]] - Detailed API specs
- [[Data Models.md]] - Entity relationships

---

## 🔗 Related Categories

- [[../03_STRATEGY/Strategy Hub.md|Strategy]] - Feature feasibility
- [[../05_DESIGN_ASSETS/Design Hub.md|Design Assets]] - Design implications

---

## 📌 Project Hub

- [[../Cash Pilot - Overview.md|Cash Pilot - Overview]]

---

**Last Updated:** June 2026  
**Owner:** Bogdan Posea (Tech Lead)  
**Status:** MVP complete, monitoring production
