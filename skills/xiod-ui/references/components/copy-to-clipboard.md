# CopyToClipboard

```tsx
import { CopyToClipboard } from "xiod-ui/copy-to-clipboard";
```

## CopyToClipboard

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| copiedIcon | `ReactNode` | — |
| copiedText | `string \| undefined` | `"Copied!"` |
| copyIcon | `ReactNode` | — |
| disableTooltip | `boolean \| undefined` | `false` |
| size | `"sm" \| "default" \| "lg" \| null \| undefined` | `"default"` |
| **text** | `string` | — |
| textToCopy | `string \| undefined` | — |
| tooltipText | `string \| undefined` | `"Copy"` |

- `copiedIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `copiedText` — The message in the toast shown after copying.
- `copyIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `disableTooltip` — Whether to hide the copy button's tooltip.
- `text` — The text shown in the field. It is also what gets copied, unless you set `textToCopy`.
- `textToCopy` — The text to copy, when it differs from what the field shows.
- `tooltipText` — The copy button's tooltip, also used as its accessible name.

Required props are bold. Full docs: https://ui.xiod.dev/docs
