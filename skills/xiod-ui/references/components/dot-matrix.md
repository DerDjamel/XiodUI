# DotMatrix

```tsx
import { DotMatrix } from "xiod-ui/dot-matrix";
```

## DotMatrix

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| ariaLabel | `string \| undefined` | `"Dot matrix loader"` |
| autoplay | `boolean \| undefined` | `true` |
| bloom | `boolean \| undefined` | `true` |
| bloomIntensity | `number \| undefined` | `1.8` |
| color | `string \| undefined` | `"currentColor"` |
| colorOff | `string \| undefined` | `"var(--muted-foreground)"` |
| colorPreset | `DotMatrixColorPreset \| undefined` | `"solid"` |
| cols | `number \| undefined` | `5` |
| dotSize | `number \| undefined` | `8` |
| fps | `number \| undefined` | `12` |
| frames | `number[][][] \| undefined` | — |
| gap | `number \| undefined` | `3` |
| halo | `boolean \| undefined` | `false` |
| isPlaying | `boolean \| undefined` | `true` |
| levels | `number[] \| undefined` | — |
| loop | `boolean \| undefined` | `true` |
| mode | `"animation" \| "static" \| "vu" \| undefined` | `"animation"` |
| onFrame | `((index: number) => void) \| undefined` | — |
| pattern | `number[][] \| boolean[][] \| undefined` | — |
| preset | `DotMatrixPreset \| undefined` | `"ripple"` |
| rows | `number \| undefined` | `5` |
| shape | `DotMatrixShape \| undefined` | `"circle"` |
| speed | `number \| undefined` | `1` |

- `ariaLabel` — The name screen readers announce for the matrix.
- `autoplay` — Whether the animation plays on its own. Animations never play when the user prefers reduced motion.
- `bloom` — Whether lit dots glow.
- `bloomIntensity` — How far the glow spreads. Higher values give a softer, wider glow.
- `color` — The colour of lit dots, as a CSS colour.
- `colorOff` — The colour of unlit dots, as a CSS colour.
- `colorPreset` — A gradient to colour the lit dots with. `solid` uses `color`.
- `cols` — The number of columns of dots.
- `dotSize` — The size of each dot, in pixels.
- `fps` — How many custom `frames` to show per second.
- `frames` — Your own animation for `animation` mode: a list of frames, each one array per row of brightness values from 0 to 1. Takes the place of `preset`.
- `gap` — The space between dots, in pixels.
- `halo` — Whether to add a soft glow behind the whole matrix.
- `isPlaying` — Whether the animation is playing. Set it to `false` to pause.
- `levels` — The height of each column in `vu` mode, from 0 to 1, left to right.
- `loop` — Whether custom `frames` start over after the last one. When `false`, the animation stops on the last frame.
- `mode` — What the dots show: an animation (a `preset` or your own `frames`), a fixed `pattern`, or level bars from `levels`.
- `onFrame` — Called with the index of each custom frame as it is shown.
- `pattern` — The dots to light in `static` mode, one array per row. Each value is `true`/`false`, or a brightness from 0 to 1.
- `preset` — The built-in animation to play in `animation` mode when no `frames` are given. `none` shows every dot lit.
- `rows` — The number of rows of dots.
- `shape` — The shape of each dot.
- `speed` — How fast a `preset` animation plays, as a multiple of its normal speed.

Required props are bold. Full docs: https://ui.xiod.dev/docs
