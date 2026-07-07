---
name: Loader
category: Feedback
status: stable
---
# Loader

## How to use

Operation with **unknown duration** or **no determinable progress**. Specifically:
- **Button states during action** → saving invoice, sending email, processing payment (show in button)
- **Page section loading** → fetching customer details, loading transaction history, rendering dashboard
- **Full-page load** → initial app load, heavy data fetch (full-page overlay with spinner)
- **File operations** → uploading CSV, exporting PDF (unknown completion time)
- **Async operations** → API calls, background processing, webhook waiting

**Source Code**:
**Source Code**:
- 🌐 **Web (lumen-react)**: https://github.com/shinetools/shine-ui/tree/main/libs/lumen-react/src/lib/loader
- 📱 **Mobile (lumen-native)**: https://github.com/shinetools/shine-ui/tree/main/libs/lumen-native/src/lib/loader

---

## Status & Availability

| Platform | Status | Version | Notes |
|----------|--------|---------|-------|
| 🌐 Web (lumen-react) | 🟢 Stable | v0.0.1 | Production-ready |
| 📱 Mobile (lumen-native) | 🟢 Stable | v0.0.1 | Production-ready |
