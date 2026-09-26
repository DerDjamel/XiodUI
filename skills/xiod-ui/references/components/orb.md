# Orb

```tsx
import { Orb, OrbBadge, OrbLabel } from "xiod-ui/orb";
```

## Orb

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| aria-label | `string \| undefined` | — |
| color | `string \| undefined` | — |
| glow | `"none" \| "subtle" \| "intense" \| null \| undefined` | `"none"` |
| intent | `"default" \| "primary" \| "secondary" \| "success" \| "warning" \| "destructive" \| "info" \| null \| undefined` | `"default"` |
| interactive | `boolean \| undefined` | `false` |
| paused | `boolean \| undefined` | `false` |
| pixelSize | `number \| undefined` | — |
| size | `"sm" \| "lg" \| "xs" \| "md" \| "xl" \| "2xl" \| null \| undefined` | `"lg"` |
| speed | `number \| undefined` | `1` |
| state | `OrbState \| undefined` | `"working"` |
| theme | `OrbTheme \| undefined` | `"auto"` |
| variant | `"default" \| "expressive" \| "classic" \| "sharp" \| "diamond" \| "ring" \| "cross" \| null \| undefined` | `"default"` |

- `aria-label` — The name screen readers announce. Defaults to a label for the `state`, such as "Thinking…".
- `color` — The colour of the dots, as a hex (`#f60`, `#ff6600`) or `rgb()` colour with comma-separated values. The dots are neutral when unset.
- `glow` — How strongly the orb glows in its own colour.
- `intent` — The theme colour of the glow around the orb. The dots stay neutral unless you set `color`.
- `interactive` — Whether the orb speeds up while the pointer is over it.
- `paused` — Whether the animation is paused. It also stays still when the user prefers reduced motion.
- `pixelSize` — The orb's width and height in pixels. Takes precedence over `size`.
- `speed` — How fast the orb animates, as a multiple of its normal speed.
- `state` — What the orb is doing, which picks its animation. Some names share an animation, such as `thinking` and `working`.
- `theme` — Whether the orb is drawn for a dark or light background. `auto` follows the nearest `dark` or `light` class or `data-theme`, then the system setting.

## OrbBadge

Takes the DOM props of the element it renders. Pass `render` to render a different element.

## OrbLabel

Takes the DOM props of the element it renders. Pass `render` to render a different element.

Required props are bold. Full docs: https://ui.xiod.dev/docs
