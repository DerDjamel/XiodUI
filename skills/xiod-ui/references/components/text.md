# Text

```tsx
import { Text } from "xiod-ui/text";
```

## Text

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| size | `"none" \| "sm" \| "default" \| "lg" \| "xs" \| "xl" \| null \| undefined` | `"default"` |
| truncate | `boolean \| null \| undefined` | — |
| variant | `"body" \| "secondary" \| "success" \| "warning" \| "info" \| "error" \| "heading1" \| "heading2" \| "heading3" \| "heading4" \| "mono" \| "mono-secondary" \| null \| undefined` | `"body"` |
| weight | `"normal" \| "medium" \| "semibold" \| "bold" \| null \| undefined` | — |

- `truncate` — Whether to keep the text on one line and cut it off with an ellipsis.
- `weight` — The font weight. When unset, the variant's own weight applies.

Required props are bold. Full docs: https://ui.xiod.dev/docs
