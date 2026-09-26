# Waveform

```tsx
import { useWaveform, Waveform, WaveformHandle, WaveformScrubber, WaveformVisual } from "xiod-ui/waveform";
```

## useWaveform

```tsx
useWaveform()
```

Returns `{ value: number; duration: number; onValueChange?: ((value: number) => void) | undefined; active: boolean; processing: boolean; mode: "static" | "scrolling" | "live"; barWidth: number; barGap: number; barRadius: number; barColor?: string | undefined; progressColor?: string | undefined; fadeEdges: boolean; fadeWidth: number; sensitivity: number; updateRate: number; seed: number; data?: number[] | undefined; canvasRef: RefObject<HTMLCanvasElement | null>; containerRef: RefObject<HTMLDivElement | null>; isDragging: boolean; setIsDragging: (dragging: boolean) => void; seekTo: (clientX: number) => void; liveDataRef: MutableRefObject<number[]>; needsRedrawRef: MutableRefObject<boolean>; requestDrawRef: MutableRefObject<(() => void) | null>; triggerRedraw: () => void }`.

## Waveform

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| active | `boolean \| undefined` | `false` |
| barColor | `string \| undefined` | — |
| barGap | `number \| undefined` | `2` |
| barRadius | `number \| undefined` | `1.5` |
| barWidth | `number \| undefined` | `3` |
| data | `number[] \| undefined` | — |
| defaultValue | `number \| undefined` | — |
| deviceId | `string \| undefined` | — |
| duration | `number \| undefined` | `1` |
| fadeEdges | `boolean \| undefined` | `true` |
| fadeWidth | `number \| undefined` | `24` |
| microphone | `boolean \| undefined` | `false` |
| mode | `"static" \| "scrolling" \| "live" \| undefined` | `"static"` |
| onValueChange | `((value: number) => void) \| undefined` | — |
| processing | `boolean \| undefined` | `false` |
| progressColor | `string \| undefined` | — |
| seed | `number \| undefined` | `42` |
| sensitivity | `number \| undefined` | `1` |
| updateRate | `number \| undefined` | `30` |
| value | `number \| undefined` | — |

- `active` — Whether the waveform shows live input instead of a recording. With `microphone`, the microphone is recorded while this is `true`.
- `barColor` — The colour of bars not yet played, as a CSS colour. Defaults to the `--border` token.
- `barGap` — The space between bars, in pixels.
- `barRadius` — The corner radius of each bar, in pixels. `0` gives square bars.
- `barWidth` — The width of each bar, in pixels.
- `data` — The bar heights to draw, each from 0 to 1. They are stretched to fill the width.
- `defaultValue` — The playback position at first, when it isn't controlled.
- `deviceId` — The microphone to record from, as a `deviceId` from `navigator.mediaDevices.enumerateDevices()`. Uses the default microphone when unset.
- `duration` — The total length, in the same unit as `value`. Leave it at 1 to use `value` as a fraction from 0 to 1.
- `fadeEdges` — Whether the bars fade out towards the left and right edges.
- `fadeWidth` — How far the fade reaches in from each edge, in pixels.
- `microphone` — Whether to record from the microphone while `active`. The browser asks the user for permission first.
- `mode` — How live input is drawn: `scrolling` adds each sample at the right edge and moves older ones left; `static` and `live` redraw the bars across the full width.
- `onValueChange` — Called with the new position when the user clicks or drags to seek.
- `processing` — Whether to show a gently moving wave, for example while an assistant is thinking. Ignored while `active`.
- `progressColor` — The colour of played bars and of live input, as a CSS colour. Defaults to the `--primary` token.
- `seed` — A number that picks the placeholder waveform drawn when there's no `data`. The same seed always draws the same shape.
- `sensitivity` — How strongly microphone input moves the bars. Raise it for quiet input.
- `updateRate` — How often to sample the microphone, in milliseconds.
- `value` — The playback position, in the same unit as `duration`. Use with `onValueChange` to control it.

## WaveformHandle

Takes the DOM props of the element it renders. Pass `render` to render a different element.

## WaveformScrubber

Takes the DOM props of the element it renders. Pass `render` to render a different element.

## WaveformVisual

No props of its own. Takes the DOM props of the element it renders.

Required props are bold. Full docs: https://ui.xiod.dev/docs
