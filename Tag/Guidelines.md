# Tag - Guidelines

## Guidelines

**Behavior**:
- Click tag → if `isSelected` or `onClick` provided, toggles state
- Click X (clear button) → fires `onClear()`, removes tag from view
- Tag can be selected or unselected (visual distinction)
- No destructive actions (tag is a filter/label, not a button)

**Web vs Mobile**:
- Web: inline tags in toolbar, flexible wrapping
- Mobile: single-row scrollable tags or wrap to multiple rows
- Mobile: larger touch targets (44px minimum height with `size="large"`)
- Mobile: clear button (X) more prominent on touch

---

## Do / Don't

### React (Web)


| ✅ Do | ❌ Don't |
|---|---|
| Removable filter chips + interactive category selector | Tags as non-interactive status labels → use Badge |
| Use Tag for both interactive filtering (`isSelected`, `onClear`) and static metadata labels — both are valid in Shine | Force Tag into one role — filtering tags and metadata display tags coexist in the product |
| Use `size="large"` for filter tags in table toolbars — it's the standard size for table filters in Shine | Use `small` or `medium` for filter tags in tables — `large` is the confirmed default for this context |

### Native (Mobile)


> 🔴 To define — Native Tag guidelines not yet documented.

---

---

### Imports

**Web**:
```tsx
import { Tag } from '@shinetools/lumen-react';
```

**Mobile**:
```tsx
import { Tag } from '@shinetools/lumen-native';
```

### Basic Usage

```tsx
import { Tag, TagGroup } from '@shinetools/lumen-react';

// Applied filters (clearable)
<TagGroup>
  <Tag label="Invoice" color="blue" onClear={() => removeFilter('invoice')} />
  <Tag label="Q4 2025" color="neutral" onClear={() => removeFilter('q4')} />
</TagGroup>

// Interactive (selected state)
{categories.map(cat => (
  <Tag
    key={cat.id}
    label={cat.name}
    color="blue"
    isSelected={selected === cat.id}
    onClick={() => setSelected(cat.id)}
  />
))}
```

---

---

## Do / Don't

### React (Web)


| ✅ Do | ❌ Don't |
|---|---|
| Removable filter chips + interactive category selector | Tags as non-interactive status labels → use Badge |
| Use Tag for both interactive filtering (`isSelected`, `onClear`) and static metadata labels — both are valid in Shine | Force Tag into one role — filtering tags and metadata display tags coexist in the product |
| Use `size="large"` for filter tags in table toolbars — it's the standard size for table filters in Shine | Use `small` or `medium` for filter tags in tables — `large` is the confirmed default for this context |

### Native (Mobile)


> 🔴 To define — Native Tag guidelines not yet documented.

---
