# Input

```tsx
import { Input } from "xiod-ui/input";
```

## Input

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| className | `string \| undefined` | — |
| defaultValue | `string \| number \| readonly string[] \| undefined` | — |
| nativeInput | `boolean \| undefined` | `false` |
| onValueChange | `((value: string, eventDetails: { reason: "none"; event: Event; cancel: () => void; allowPropagation: () => void; isCanceled: boolean; isPropagationAllowed: boolean; trigger: Element \| undefined; }) => void) \| undefined` | — |
| size | `number \| "sm" \| "default" \| "lg" \| undefined` | `"default"` |
| style | `CSSProperties \| undefined` | — |
| unstyled | `boolean \| undefined` | `false` |
| value | `string \| number \| readonly string[] \| undefined` | — |

- `defaultValue` — The default value of the input. Use when uncontrolled.
- `nativeInput` — Whether to render a plain `<input>` instead of Base UI's `Input`. A plain input doesn't register with a surrounding `Field`.
- `onValueChange` — Callback fired when the `value` changes. Use when controlled.
- `unstyled` — Whether to drop the border, background and focus ring, leaving only the text field. Use inside your own styled container.
- `value` — The value of the input. Use when controlled.

Required props are bold. Full docs: https://ui.xiod.dev/docs
