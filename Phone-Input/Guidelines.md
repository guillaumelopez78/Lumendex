# Phone-Input - Guidelines

## Guidelines

**Context by page**:
- **Signup form** → phone field (optional or required) with country selector
- **Checkout** → billing/shipping phone with country code
- **Profile/settings** → user contact phone number
- **Customer creation** → phone field with country code (business customer)
- **API integrations** → phone field for webhook callbacks

**Behavior**:
- Country dropdown on left, phone number field on right
- Country defaults to user's locale (browser language) if available
- Auto-formats based on selected country (different countries have different formats)
- Validates international phone format (optional on your component)
- Returns full phone number with country code

**Web vs Mobile**:
- Web: country dropdown + text field side-by-side, comfortable spacing
- Mobile: country dropdown stacked above or full-height above phone field
- Mobile: phone keyboard appears when typing (tel input type)
- Mobile: country search might be search + dropdown or native select

---

## Do / Don't

### React (Web)

| ✅ Do | ❌ Don't |
|---|---|
| [Good practice] | [Bad practice] |
| [Good practice] | [Bad practice] |

### Native (Mobile)

| ✅ Do | ❌ Don't |
|---|---|
| [Good practice] | [Bad practice] |
| [Good practice] | [Bad practice] |

---

---

### Imports

**Web**:
```tsx
import { Input Phone Number } from '@shinetools/lumen-react';
```

**Mobile**:
```tsx
import { Input Phone Number } from '@shinetools/lumen-native';
```

### Basic Usage

```tsx
<Input Phone Number />
```

---

---

## Do / Don't

### React (Web)

| ✅ Do | ❌ Don't |
|---|---|
| [Good practice] | [Bad practice] |
| [Good practice] | [Bad practice] |

### Native (Mobile)

| ✅ Do | ❌ Don't |
|---|---|
| [Good practice] | [Bad practice] |
| [Good practice] | [Bad practice] |

---
