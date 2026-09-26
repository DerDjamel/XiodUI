# RulerPicker

```tsx
import { RulerPicker } from "xiod-ui/ruler-picker";
```

## RulerPicker

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| defaultValue | `number \| undefined` | — |
| itemWidth | `number \| undefined` | `80` |
| max | `number \| undefined` | `100` |
| min | `number \| undefined` | `0` |
| onChange | `((value: number) => void) \| undefined` | — |
| size | `"sm" \| "lg" \| "md" \| null \| undefined` | `"md"` |
| subDivisions | `number \| undefined` | `4` |
| value | `number \| undefined` | — |

- `defaultValue` — The value selected at first, when it isn't controlled. Defaults to `min`.
- `itemWidth` — The distance between two whole-number marks, in pixels.
- `max` — The highest value on the ruler.
- `min` — The lowest value on the ruler.
- `onChange` — Called with the new value as the ruler settles on a mark, by scrolling, dragging or the arrow keys.
- `subDivisions` — The number of small ticks drawn between two whole-number marks. With `9`, the middle tick is drawn longer.
- `value` — The selected whole number. Use with `onChange` to control it.

Required props are bold. Full docs: https://ui.xiod.dev/docs
