# InputGroup

```tsx
import { InputGroup, InputGroupAddon, InputGroupInput, InputGroupText, InputGroupTextarea } from "xiod-ui/input-group";
```

## InputGroup

Renders a `<div>` and takes its props. Pass `render` to render a different element.

## InputGroupAddon

Renders a `<div>` and takes its props. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| align | `"inline-start" \| "block-end" \| "block-start" \| "inline-end" \| null \| undefined` | `"inline-start"` |

- `align` — Where the addon sits: before or after the text on the same line (`inline-*`), or on its own row above or below it (`block-*`).

## InputGroupInput

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| className | `string \| undefined` |
| defaultValue | `string \| number \| readonly string[] \| undefined` |
| nativeInput | `boolean \| undefined` |
| onValueChange | `((value: string, eventDetails: { reason: "none"; event: Event; cancel: () => void; allowPropagation: () => void; isCanceled: boolean; isPropagationAllowed: boolean; trigger: Element \| undefined; }) => void) \| undefined` |
| size | `number \| "sm" \| "default" \| "lg" \| undefined` |
| style | `CSSProperties \| undefined` |
| unstyled | `boolean \| undefined` |
| value | `string \| number \| readonly string[] \| undefined` |

- `defaultValue` — The default value of the input. Use when uncontrolled.
- `nativeInput` — Whether to render a plain `<input>` instead of Base UI's `Input`. A plain input doesn't register with a surrounding `Field`.
- `onValueChange` — Callback fired when the `value` changes. Use when controlled.
- `unstyled` — Whether to drop the border, background and focus ring, leaving only the text field. Use inside your own styled container.
- `value` — The value of the input. Use when controlled.

## InputGroupText

Renders a `<span>` and takes its props. Pass `render` to render a different element.

## InputGroupTextarea

| Prop | Type |
| :--- | :--- |
| size | `number \| "sm" \| "default" \| "lg" \| undefined` |
| unstyled | `boolean \| undefined` |

- `unstyled` — Whether to drop the border, background and focus ring, leaving only the text field. Use inside your own styled container.

Required props are bold. Full docs: https://ui.xiod.dev/docs
