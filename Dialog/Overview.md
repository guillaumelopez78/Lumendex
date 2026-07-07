---
name: Dialog
category: Overlay
status: stable
---
# Dialog

## How to use

Critical confirmations that BLOCK user flow. Specifically:
- **Destructive confirmations** → delete invoice, revoke API key, close account (must be explicit)
- **Blocking errors** → payment failed, insufficient balance, invalid VAT (user can't proceed without action)
- **Rare critical dialogs** → account suspension warning (very limited use)
- **Permission blocking** → 2FA verification before sensitive action (only when required)

**Source Code**:
**Source Code**:
- 🌐 **Web (lumen-react)**: https://github.com/shinetools/shine-ui/tree/main/libs/lumen-react/src/lib/dialog
- 📱 **Mobile (lumen-native)**: https://github.com/shinetools/shine-ui/tree/main/libs/lumen-native/src/lib/dialog

---

## Status & Availability

| Platform | Status | Version | Notes |
|----------|--------|---------|-------|
| 🌐 Web (lumen-react) | 🟢 Stable | v0.0.1 | Production-ready |
| 📱 Mobile (lumen-native) | 🟢 Stable | v0.0.1 | Production-ready |

**Note**: Modal in vault maps to Dialog in repository.
