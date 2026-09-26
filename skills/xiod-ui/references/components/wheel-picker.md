# WheelPicker

```tsx
import { useWheelPickerGroup, WheelPicker, WheelPickerGroup } from "xiod-ui/wheel-picker";
```

## useWheelPickerGroup

```tsx
useWheelPickerGroup()
```

Returns `null | { activeIndex: number; setActiveIndex: (index: number) => void; register: (existingIndex: number | null, ref: HTMLDivElement) => number; getPickerRef: (index: number) => HTMLDivElement | null; getPickerIndices: () => number[] }`.

## WheelPicker

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| classNames | `WheelPickerClassNames \| undefined` | — |
| defaultValue | `T \| undefined` | — |
| dragSensitivity | `number \| undefined` | `3` |
| infinite | `boolean \| undefined` | `false` |
| onValueChange | `((value: T) => void) \| undefined` | — |
| optionItemHeight | `number \| undefined` | — |
| **options** | `WheelPickerOption<T>[]` | — |
| scrollSensitivity | `number \| undefined` | `5` |
| size | `"sm" \| "lg" \| "md" \| null \| undefined` | `"md"` |
| value | `T \| undefined` | — |
| visibleCount | `number \| undefined` | `20` |

- `classNames` — Classes for the parts of the wheel.
- `defaultValue` — The value selected at first, when it isn't controlled.
- `dragSensitivity` — How quickly the wheel slows after a flick. Higher values stop it sooner.
- `infinite` — Whether the options repeat, so the wheel turns endlessly in either direction.
- `onValueChange` — Called with the new value when the wheel settles on an option.
- `optionItemHeight` — The height of each option, in pixels. Defaults to 28, 36 or 44 depending on `size`.
- `options` — The options on the wheel.
- `scrollSensitivity` — How far and fast the wheel turns for mouse-wheel and keyboard scrolling. Higher values turn it further and faster.
- `value` — The selected value. Use with `onValueChange` to control it.
- `visibleCount` — The number of options around the whole wheel, which sets how sharply it curves. A quarter of them show on each side of the selected option. Use a multiple of 4.

## WheelPickerGroup

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| children | `ReactNode` |

Required props are bold. Full docs: https://ui.xiod.dev/docs
