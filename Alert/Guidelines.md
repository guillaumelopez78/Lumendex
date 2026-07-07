# Alert - Guidelines

## Guidelines

**Behavior**:
- Stays visible until dismissed (by user or automatic resolution)
- Includes action button when user can take immediate action
- Position: inline on page where context matters
- At top of section if page-level, or near affected field if field-level

**Web vs Mobile**: Same behavior. On mobile, alert takes full width and wraps text.

---

## Do / Don't

| ✅ Do | ❌ Don't |
|---|---|
| Use `danger` for blocking errors that prevent progression | Use `danger` for mild warnings |
| Include a resolution path (`action`) when applicable | Show an error with no way to fix it |
| Keep body copy concise | Write long paragraphs inside an Alert |

---

---

### Imports

**Web**:
```tsx
import { Alert } from '@shinetools/lumen-react';
```

**Mobile**:
```tsx
import { Alert } from '@shinetools/lumen-native';
```

### Basic Usage

```tsx
<Alert />
```

---

---

## Do / Don't

| ✅ Do | ❌ Don't |
|---|---|
| Use `danger` for blocking errors that prevent progression | Use `danger` for mild warnings |
| Include a resolution path (`action`) when applicable | Show an error with no way to fix it |
| Keep body copy concise | Write long paragraphs inside an Alert |

---
