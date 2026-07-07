# Dialog - Guidelines

---

## Do / Don't

### React (Web)


| ✅ Do | ❌ Don't |
|---|---|
| 1 cancel + 1 danger CTA — clear destructive action | 3 equal-weight accent buttons — user can't prioritize |
| Affirmative title naming the object · consequence in body · Return not Cancel | Question title · vague body · "Yes, delete" adds nothing |
| Modal footer: secondary (`text`/`outlined`) on the left, primary `filled` on the right (inline, auto-width) | Place the primary button on the left — visual weight and reading order both point right |
| Allow closing by clicking the overlay — it's always enabled in Shine | Block overlay close for destructive modals — the overlay always closes the modal in Shine |
| Default to **600px** width (`md`) — the standard modal size in Shine | Use custom widths without a design reason — 600px is the confirmed default |

### Native (Mobile)


| ✅ Do | ❌ Don't |
|---|---|
| Overlay click always closes the Modal on mobile — same as React | Block overlay close on mobile |
| Use fullscreen Modal on mobile for complex flows | Use a 600px-wide modal on mobile — use fullscreen instead |

---

---

### Imports

**Web**:
```tsx
import { Dialog } from '@shinetools/lumen-react';
```

**Mobile**:
```tsx
import { Dialog (Modal) } from '@shinetools/lumen-native';
```

### Basic Usage

```tsx
import { Modal } from '@shinetools/lumen-react';

<Modal open={open} onClose={() => setOpen(false)}
  title="Delete invoice" size="sm"
  footer={<>
    <Button variant="text" onClick={() => setOpen(false)}>Cancel</Button>
    <Button variant="filled" color="danger" onClick={del}>Delete</Button>
  </>}
>This action cannot be undone.</Modal>
```

---

---

## Do / Don't

### React (Web)


| ✅ Do | ❌ Don't |
|---|---|
| 1 cancel + 1 danger CTA — clear destructive action | 3 equal-weight accent buttons — user can't prioritize |
| Affirmative title naming the object · consequence in body · Return not Cancel | Question title · vague body · "Yes, delete" adds nothing |
| Modal footer: secondary (`text`/`outlined`) on the left, primary `filled` on the right (inline, auto-width) | Place the primary button on the left — visual weight and reading order both point right |
| Allow closing by clicking the overlay — it's always enabled in Shine | Block overlay close for destructive modals — the overlay always closes the modal in Shine |
| Default to **600px** width (`md`) — the standard modal size in Shine | Use custom widths without a design reason — 600px is the confirmed default |

### Native (Mobile)


| ✅ Do | ❌ Don't |
|---|---|
| Overlay click always closes the Modal on mobile — same as React | Block overlay close on mobile |
| Use fullscreen Modal on mobile for complex flows | Use a 600px-wide modal on mobile — use fullscreen instead |

---
