---
name: Alert
category: Feedback
status: stable
---
# Alert

## How to use

Persistent page-level messages that require user acknowledgment. Specifically:
- **Warning state** → "Account balance below €100" (user should act but can delay)
- **Blocking error** → "VAT number invalid — fix before submitting form" (requires action)
- **Info/context** → "This invoice is overdue" (informational, not blocking)
- **Action required** → "Payment method expired — update before checkout"
- **Page-level notices** → "Read-only mode" (affects entire page behavior)

**Source Code**:
**Source Code**:
- 🌐 **Web (lumen-react)**: https://github.com/shinetools/shine-ui/tree/main/libs/lumen-react/src/lib/alert
- 📱 **Mobile (lumen-native)**: https://github.com/shinetools/shine-ui/tree/main/libs/lumen-native/src/lib/alert

---

## Status & Availability

| Platform | Status | Version | Notes |
|----------|--------|---------|-------|
| 🌐 Web (lumen-react) | 🟡 WIP | — | Not yet released, coming soon |
| 📱 Mobile (lumen-native) | 🟡 WIP | — | Not yet released, coming soon |

**Recommendation**: Use [[Banner]] component instead. Alert is vault-only at this time.
