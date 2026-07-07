# Button

**Source Code:**
- 🌐 [Web (lumen-react)](https://github.com/shinetools/shine-ui/tree/main/libs/lumen-react/src/lib/button)
- 📱 [Mobile (lumen-native)](https://github.com/shinetools/shine-ui/tree/main/libs/lumen-native/src/lib/button)
- 🎨 [Figma Design](https://www.figma.com/design/qe7lyEyFHlsrzacfeKtW9y/%F0%9F%92%A1-Lumen-DS?node-id=1422-12814)

| Platform | Status | Version |
|----------|--------|---------|
| 🌐 Web | 🟢 Stable | v0.0.1 |
| 📱 Mobile | 🟢 Stable | v0.0.1 |

---

## Code Example

```jsx
import { Button } from '@shinetools/lumen-react';
import { Plus, Download, X } from 'lucide-react';

// Primary action
<Button variant="filled" color="accent">
  Save changes
</Button>

// Secondary action
<Button variant="outlined" color="primary">
  Cancel
</Button>

// With icon
<Button variant="filled" icon={<Plus />}>
  Add item
</Button>

// Loading state
<Button loading variant="filled">
  Saving...
</Button>

// Disabled
<Button disabled>
  Unavailable
</Button>

// Icon only (requires aria-label)
<Button variant="text" aria-label="Close" icon={<X />} />
```
