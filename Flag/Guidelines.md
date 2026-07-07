# Flag - Guidelines

---

## Do / Don't

### React (Web)


| ✅ Do | ❌ Don't |
|---|---|
| Pair with visible country name text for full context | Use flag alone without a country name label — accessibility risk |
| Use `alt="France"` (full name) rather than `alt="FR"` when writing explicit alt text | Use the raw ISO code as `alt` when the full name is available |

---

---

### Imports

**Web**:
```tsx
import { Flag } from '@shinetools/lumen-react';
```

**Mobile**:
```tsx
import { Flag } from '@shinetools/lumen-native';
```

### Basic Usage

```tsx
import { Flag } from '@shinetools/lumen-react';

<Flag code="FR" />
<Flag code="DE" size="small" />
<Flag code="US" size="large" alt="United States" />

// Decorative (country name already visible)
<Flag code="GB" alt="" />
```

---

---

## Do / Don't

### React (Web)


| ✅ Do | ❌ Don't |
|---|---|
| Pair with visible country name text for full context | Use flag alone without a country name label — accessibility risk |
| Use `alt="France"` (full name) rather than `alt="FR"` when writing explicit alt text | Use the raw ISO code as `alt` when the full name is available |

---
