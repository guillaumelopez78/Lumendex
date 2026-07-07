# Radio-Button - Guidelines

## Guidelines

**Context by page**:
- Signup/onboarding → account type radio selection
- Billing settings → plan frequency (monthly/annual) selection
- Invoice editor → template/design selection
- Settings → preference selection (auto-save behavior, notification frequency)

**Web vs Mobile**:
- Web: inline radio options if 3-4 fit in one row, otherwise stack vertically
- Mobile: always stack vertically (one radio per row) for touch targets
- Mobile: increase touch area with `comfortArea` prop

---

## Do / Don't

### React (Web)


| ✅ Do | ❌ Don't |
|---|---|
| All options + hints visible — easy to compare | Select hides hint text — user can't compare |
| Switch to Select when the group exceeds 4–5 options — keep radio groups short so options fit without scrolling | Stack more than 5 radio options — switch to Select when list grows beyond 4–5 |

### Native (Mobile)


> 🔴 To define — Native RadioButton guidelines not yet documented.

---

---

### Imports

**Web**:
```tsx
import { RadioButton } from '@shinetools/lumen-react';
```

**Mobile**:
```tsx
import { RadioButton } from '@shinetools/lumen-native';
```

### Basic Usage

```tsx
import { RadioButton } from '@shinetools/lumen-react';

const [freq, setFreq] = useState('monthly');

<fieldset>
  <legend>Billing frequency</legend>
  <RadioButton label="Monthly" name="freq" value="monthly"
    checked={freq === 'monthly'} onChange={() => setFreq('monthly')} comfortArea />
  <RadioButton label="Quarterly" name="freq" value="quarterly"
    checked={freq === 'quarterly'} onChange={() => setFreq('quarterly')} comfortArea />
  <RadioButton label="Annual" name="freq" value="annual"
    checked={freq === 'annual'} onChange={() => setFreq('annual')} comfortArea />
</fieldset>
```

---

---

## Do / Don't

### React (Web)


| ✅ Do | ❌ Don't |
|---|---|
| All options + hints visible — easy to compare | Select hides hint text — user can't compare |
| Switch to Select when the group exceeds 4–5 options — keep radio groups short so options fit without scrolling | Stack more than 5 radio options — switch to Select when list grows beyond 4–5 |

### Native (Mobile)


> 🔴 To define — Native RadioButton guidelines not yet documented.

---
