# Stack - Guidelines

## Guidelines

**Use Stack when**: Building layouts with flex containers using design tokens. Two primitives:
- **XStack**: Horizontal row (flex row)
- **YStack**: Vertical column (flex column)

Both automatically use design token spacing (8px, 16px, 24px, etc.) — no magic numbers or inline styles.

**XStack (Horizontal) use cases**:
- **Icon + label rows** → check icon + "Payment confirmed" text
- **Side-by-side elements** → label on left, value on right
- **Toolbar buttons** → multiple buttons in a horizontal row
- **Form field rows** → multiple inputs on same row (on web; stack on mobile)
- **Card headers** → title + action button side-by-side
- **Price display** → currency icon + amount + unit

**YStack (Vertical) use cases**:
- **Form fields** → stacked input fields with consistent spacing
- **Card content** → stacked sections (title, description, footer)
- **List items** → vertical list of related items
- **Modal/dialog body** → stacked content sections
- **Section layout** → stacked content blocks

**Key principles**:
- Always use `gap` prop with design tokens (8, 12, 16, 24, 32)
- Never use inline `style` with magic numbers
- Align items with `align` prop (center, start, end, stretch)
- Justify content with `justify` prop (start, end, center, space-between, space-around)

**Common patterns**:
```tsx
// Icon + label (centered vertically)
<XStack gap={8} align="center">
  <Icon />
  <Text />
</XStack>

// Form fields (vertical stack)
<YStack gap={16}>
  <TextField />
  <TextField />
  <Button />
</YStack>

// Card layout (nested stacks)
<YStack gap={12} padding={16}>
  <Typography.Header>Title</Typography.Header>
  <XStack justify="space-between">
    <Text>Label</Text>
    <Text weight="bold">Value</Text>
  </XStack>
</YStack>
```

**Web vs Mobile**:
- Web: XStack for horizontal layouts that fit
- Mobile: often convert XStack to YStack for full-width single column
- Always test that spacing tokens work at mobile viewport

---

## Do / Don't

| ✅ Do | ❌ Don't |
|---|---|
| `<XStack gap={8} align="center">` for icon + label rows | `<div style={{display:'flex',gap:'8px'}}>` — inline styles bypass token system |
| `<YStack gap={16}>` for form field stacking | Nest `<div>` with `flexDirection: column` manually |
| Compose stacks — `<YStack>` containing `<XStack>` items | Use one-off flex wrappers for every layout |

---

---

### Imports

**Web**:
```tsx
import { Stack (XStack / YStack) } from '@shinetools/lumen-react';
```

**Mobile**:
```tsx
import { Stack (XStack / YStack) } from '@shinetools/lumen-native';
```

### Basic Usage

```tsx
import { XStack, YStack } from '@shinetools/lumen-react';

// Icon + label row
<XStack gap={8} align="center">
  <Icon icon={CheckCircle} size="small" />
  <Typography.Text>Payment confirmed</Typography.Text>
</XStack>

// Form field column
<YStack gap={16}>
  <TextField label="First name" />
  <TextField label="Last name" />
  <TextField label="Email" type="email" />
</YStack>

// Card layout
<YStack gap={12} padding={20}>
  <Typography.Header as="h3">Invoice #1042</Typography.Header>
  <XStack gap={8} justify="space-between">
    <Typography.Text variant="secondary">Total</Typography.Text>
    <Typography.Text weight="semibold">1 250,00 €</Typography.Text>
  </XStack>
</YStack>
```

---

---

## Do / Don't

| ✅ Do | ❌ Don't |
|---|---|
| `<XStack gap={8} align="center">` for icon + label rows | `<div style={{display:'flex',gap:'8px'}}>` — inline styles bypass token system |
| `<YStack gap={16}>` for form field stacking | Nest `<div>` with `flexDirection: column` manually |
| Compose stacks — `<YStack>` containing `<XStack>` items | Use one-off flex wrappers for every layout |

---
