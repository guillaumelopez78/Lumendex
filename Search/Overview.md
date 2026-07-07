---
name: Search
category: Forms
status: stable
---
# Search

## How to use

Filtering/searching content with optional autocomplete. Specifically:
- **Invoice list filtering** → search by invoice number, customer name, date range
- **Dashboard search** → find transactions, customers, documents across pages
- **Lightweight autocomplete** → search + show suggestions as user types
- **Filtering tables/lists** → search within visible data (not global search)
- **Not full-text search** → use Search component for scoped filtering, not app-wide search

**Source Code**:
**Source Code**:
- 🌐 **Web (lumen-react)**: https://github.com/shinetools/shine-ui/tree/main/libs/lumen-react/src/lib/search
- 📱 **Mobile (lumen-native)**: https://github.com/shinetools/shine-ui/tree/main/libs/lumen-native/src/lib/search

---

## Status & Availability

| Platform | Status | Version | Notes |
|----------|--------|---------|-------|
| 🌐 Web (lumen-react) | 🟡 WIP | — | Not yet released, coming soon |
| 📱 Mobile (lumen-native) | 🟡 WIP | — | Not yet released, coming soon |

**Recommendation**: Use [[TextField]] with Icon pattern. Search is vault-only at this time.
