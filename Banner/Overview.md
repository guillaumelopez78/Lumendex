---
name: Banner
category: Feedback
status: stable
---
# Banner

## How to use

Full-width persistent messages at the **very top of the page**. Specifically:
- **System-level warnings** → "Maintenance window 2pm-3pm CET tomorrow" (affects all users/page)
- **Critical page-blocking errors** → "Database backup in progress, read-only mode until 14:00" (affects entire page)
- **Account status alerts** → "Trial expires in 2 days — upgrade now", "Payment failed, service suspended"
- **Persistent status** → "You are in demo mode" (stays visible until dismissed or resolved)
- **Action required (critical)** → "Security verification needed before checkout" (must be acknowledged)

**Source Code**:
**Source Code**:
- 🌐 **Web (lumen-react)**: https://github.com/shinetools/shine-ui/tree/main/libs/lumen-react/src/lib/banner
- 📱 **Mobile (lumen-native)**: https://github.com/shinetools/shine-ui/tree/main/libs/lumen-native/src/lib/banner

---

## Status & Availability

| Platform | Status | Version | Notes |
|----------|--------|---------|-------|
| 🌐 Web (lumen-react) | 🟢 Stable | v0.0.1 | Production-ready |
| 📱 Mobile (lumen-native) | 🟢 Stable | v0.0.1 | Production-ready |
