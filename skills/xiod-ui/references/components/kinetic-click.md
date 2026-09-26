# KineticClick

```tsx
import { KineticClick } from "xiod-ui/kinetic-click";
```

## KineticClick

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| children | `ReactNode` | — |
| color | `string \| undefined` | `"currentColor"` |
| colorFrom | `"text" \| "auto" \| "background" \| "border" \| undefined` | `"auto"` |
| count | `number \| undefined` | — |
| duration | `number \| undefined` | — |
| size | `number \| undefined` | — |
| trigger | `KineticClickTrigger \| undefined` | `"mousedown"` |
| variant | `KineticClickVariant \| undefined` | `"spark"` |

- `color` — The colour of the effect, as a CSS colour. `currentColor` takes it from the clicked element, as `colorFrom` sets.
- `colorFrom` — Which colour of the clicked element to use when `color` is `currentColor`. `auto` uses the first of its text, background and border colours that isn't a neutral grey, so a white-text button still gets a coloured effect.
- `count` — How many particles, ripples or shapes each click creates. Each effect has its own default.
- `duration` — How long the effect lasts, in milliseconds. Each effect has its own default.
- `size` — How large the effect is, in pixels: a particle's size, or a ripple's largest radius. Each effect has its own default.
- `trigger` — When the effect plays: as soon as the button is pressed (`mousedown`), or when it is released (`click`).
- `variant` — The effect that plays where the user clicks.

Required props are bold. Full docs: https://ui.xiod.dev/docs
