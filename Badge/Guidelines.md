# Badge - Guidelines

## Guidelines

**Context by page**:
- **Invoice list**: status badge (Paid, Pending, Overdue) on each row
- **Sidebar**: count badge on "Messages" (shows unread count)
- **Header**: count badge on notification icon (shows alert count)
- **Profile card**: status badges (Premium, Verified) below name
- **Tab/section header**: count badge showing items in section

**Behavior**:
- Non-interactive (no click handler)
- No close/dismiss button
- Position: typically top-right or inline with related item
- Updates automatically when state changes (no user action needed)

**Web vs Mobile**:
- Web: inline with text or element it describes
- Mobile: same positioning, badges remain small and scannable
- Count badge might increase slightly for touch readability but stay compact

---

## Do / Don't

### React (Web)


| ✅ Do | ❌ Don't |
|---|---|
| One semantic badge per row — status at a glance | 4 badge variants on one row — priority unclear |
| Use `count` mode with a number for unread notifications (messages, alerts) — shows the exact count | Use `dot` mode for unread counts — the dot gives no quantity information |
| Leave status badge colors unforced for now — no global convention defined yet, align per-feature | Invent new color meanings without cross-team alignment — wait for the global convention |

### Native (Mobile)


| ✅ Do | ❌ Don't |
|---|---|
| Use count mode for unread notifications on mobile — same as React | Use dot mode for unread counts on mobile |

---

---

### Imports

**Web**:
```tsx
import { Badge } from '@shinetools/lumen-react';
```

**Mobile**:
```tsx
import { Badge } from '@shinetools/lumen-native';
```

### Basic Usage

```tsx
import { Badge } from '@shinetools/lumen-react';

// Digit badge
<Badge count={3} color="neutral" />
<Badge count={3} color="accent" />
<Badge count={12} color="danger" />

// Solid fill (default)
<Badge count={5} color="warning" mode="primary" />

// Tinted subtle fill
<Badge count={5} color="warning" mode="subtle" />

// Dot (status indicator)
<Badge color="success" /* no count or icon = dot */ />
<Badge color="danger" />
```

---

---

## Do / Don't

### React (Web)


| ✅ Do | ❌ Don't |
|---|---|
| One semantic badge per row — status at a glance | 4 badge variants on one row — priority unclear |
| Use `count` mode with a number for unread notifications (messages, alerts) — shows the exact count | Use `dot` mode for unread counts — the dot gives no quantity information |
| Leave status badge colors unforced for now — no global convention defined yet, align per-feature | Invent new color meanings without cross-team alignment — wait for the global convention |

### Native (Mobile)


| ✅ Do | ❌ Don't |
|---|---|
| Use count mode for unread notifications on mobile — same as React | Use dot mode for unread counts on mobile |

---
