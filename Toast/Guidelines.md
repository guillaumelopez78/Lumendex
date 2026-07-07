# Toast - Guidelines

## Guidelines

**Behavior**:
- Auto-dismiss after **5 seconds** (standard duration in Shine)
- Optional action button: `{ label: 'Undo', onClick: () => ... }`
- Position: **bottom-right** on web, **bottom center** on mobile
- Tone: past-tense, factual. "Invoice sent" not "Your invoice has been successfully sent!" (no congratulations)

**Web vs Mobile**: Same 5-second duration. Position changes: web (bottom-right), mobile (bottom-center).

---

## Do / Don't

### React (Web)


| ✅ Do | ❌ Don't |
|---|---|
| Action confirmation + optional "View" link | Persistent error → auto-dismiss before user can act |
| States what happened. Object + past-tense verb. Full stop. | Congratulatory tone is patronising for business software. Exclamation marks add noise. |
| Auto-dismiss after **5 seconds** — standard duration in Shine | Use durations under 3s or over 10s — 5s is the confirmed default |
| Display Toasts in the **bottom-right** corner of the screen | Place Toasts at the top or centered — bottom-right is the established position in Shine |

### Native (Mobile)


| ✅ Do | ❌ Don't |
|---|---|
| Auto-dismiss after 5 seconds on mobile — same duration as React | |
| Display Toast at the bottom of the screen on mobile | Place Toast at the top — bottom is the confirmed position |

---

---

### Imports

**Web**:
```tsx
import { Toast } from '@shinetools/lumen-react';
```

**Mobile**:
```tsx
import { Toast } from '@shinetools/lumen-native';
```

### Basic Usage

```tsx
import { toast } from '@shinetools/lumen-react';

toast.success('Invoice sent', {
  action: { label: 'View', onClick: () => navigate('/invoices/123') }
});
toast.danger('Export failed — try again');
```

---

---

## Do / Don't

### React (Web)


| ✅ Do | ❌ Don't |
|---|---|
| Action confirmation + optional "View" link | Persistent error → auto-dismiss before user can act |
| States what happened. Object + past-tense verb. Full stop. | Congratulatory tone is patronising for business software. Exclamation marks add noise. |
| Auto-dismiss after **5 seconds** — standard duration in Shine | Use durations under 3s or over 10s — 5s is the confirmed default |
| Display Toasts in the **bottom-right** corner of the screen | Place Toasts at the top or centered — bottom-right is the established position in Shine |

### Native (Mobile)


| ✅ Do | ❌ Don't |
|---|---|
| Auto-dismiss after 5 seconds on mobile — same duration as React | |
| Display Toast at the bottom of the screen on mobile | Place Toast at the top — bottom is the confirmed position |

---
