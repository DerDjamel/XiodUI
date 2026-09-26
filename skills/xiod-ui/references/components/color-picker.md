# ColorPicker

```tsx
import { BlossomColorPicker, ColorPicker } from "xiod-ui/color-picker";
```

## BlossomColorPicker

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| adaptivePositioning | `boolean \| undefined` | `true` |
| animationDuration | `number \| undefined` | `300` |
| circularBarWidth | `number \| undefined` | `BAR_WIDTH` |
| collapsible | `boolean \| undefined` | `true` |
| colors | `ColorInput[] \| undefined` | — |
| coreSize | `number \| undefined` | `32` |
| defaultValue | `BlossomColorPickerValue \| undefined` | — |
| disabled | `boolean \| undefined` | `false` |
| initialExpanded | `boolean \| undefined` | `false` |
| onChange | `((color: BlossomColorPickerColor) => void) \| undefined` | — |
| onCollapse | `((color: BlossomColorPickerColor) => void) \| undefined` | — |
| openOnHover | `boolean \| undefined` | `false` |
| petalSize | `number \| undefined` | `32` |
| showAlphaSlider | `boolean \| undefined` | `true` |
| showCoreColor | `boolean \| undefined` | `true` |
| showOpacitySlider | `boolean \| undefined` | `true` |
| sliderOffset | `number \| undefined` | `SLIDER_OFFSET` |
| sliderPosition | `SliderPosition \| undefined` | — |
| sliderWidth | `number \| undefined` | `BAR_WIDTH` |
| value | `BlossomColorPickerValue \| undefined` | — |

- `adaptivePositioning` — Whether the open picker shifts to stay inside the window, and places its sliders where there is room when `sliderPosition` is unset.
- `animationDuration` — How long the petals take to open and close, in milliseconds.
- `circularBarWidth` — The thickness of the ring that shows the selected colour around the petals, in pixels.
- `collapsible` — Whether the picker closes to its centre button. When `false`, it stays open.
- `colors` — The petal colours, as hex, `rgb()` or `hsl()` strings or `{ h, s, l }` objects. Up to 10 sit in one ring; more are split into rings by lightness.
- `coreSize` — The diameter of the centre button, in pixels.
- `defaultValue` — The colour selected at first, when it isn't controlled.
- `disabled` — Whether the picker ignores input.
- `initialExpanded` — Whether the picker starts open.
- `onChange` — Called with the new colour, in every format, whenever it changes.
- `onCollapse` — Called with the selected colour when the picker closes.
- `openOnHover` — Whether hovering the picker opens it, as well as clicking. Only applies when `collapsible`.
- `petalSize` — The diameter of each petal, in pixels.
- `showAlphaSlider` — Whether to show the Lightness arc slider beside the petals while open.
- `showCoreColor` — Whether the centre shows the selected colour while open. When `false`, it turns white while open.
- `showOpacitySlider` — Whether to show the Opacity arc slider, on the side opposite the Lightness slider, while open.
- `sliderOffset` — The distance between the colour ring and the arc sliders, in pixels.
- `sliderPosition` — The side the Lightness slider sits on. The Opacity slider takes the opposite side. When unset, the picker picks the side with the most room.
- `sliderWidth` — The thickness of the arc sliders, in pixels.
- `value` — The selected colour. Use with `onChange` to control it.

## ColorPicker

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| adaptivePositioning | `boolean \| undefined` | `true` |
| animationDuration | `number \| undefined` | `300` |
| circularBarWidth | `number \| undefined` | `BAR_WIDTH` |
| className | `string \| undefined` | — |
| collapsible | `boolean \| undefined` | `false` |
| colors | `ColorInput[] \| undefined` | — |
| coreSize | `number \| undefined` | `36` |
| darkMode | `boolean \| undefined` | — |
| defaultValue | `BlossomColorPickerValue \| undefined` | — |
| disabled | `boolean \| undefined` | `false` |
| initialExpanded | `boolean \| undefined` | `true` |
| onChange | `((color: BlossomColorPickerColor) => void) \| undefined` | — |
| onCollapse | `((color: BlossomColorPickerColor) => void) \| undefined` | — |
| openOnHover | `boolean \| undefined` | `false` |
| petalSize | `number \| undefined` | `32` |
| showAlphaSlider | `boolean \| undefined` | `true` |
| showCoreColor | `boolean \| undefined` | `true` |
| sliderOffset | `number \| undefined` | `SLIDER_OFFSET` |
| sliderPosition | `SliderPosition \| undefined` | — |
| sliderWidth | `number \| undefined` | `BAR_WIDTH` |
| triggerIcon | `ReactNode` | — |
| value | `BlossomColorPickerValue \| undefined` | — |

- `adaptivePositioning` — Whether the open picker shifts to stay inside the window, and places its sliders where there is room when `sliderPosition` is unset.
- `animationDuration` — How long the petals take to open and close, in milliseconds.
- `circularBarWidth` — The thickness of the ring that shows the selected colour around the petals, in pixels.
- `collapsible` — Whether the picker closes to its centre button. When `false`, it stays open.
- `colors` — The petal colours, as hex, `rgb()` or `hsl()` strings or `{ h, s, l }` objects. Up to 10 sit in one ring; more are split into rings by lightness.
- `coreSize` — The diameter of the centre button, in pixels.
- `darkMode` — Whether the panel always uses dark colours, whatever the page's theme.
- `defaultValue` — The colour selected at first, when it isn't controlled.
- `disabled` — Whether the picker ignores input.
- `initialExpanded` — Whether the picker starts open.
- `onChange` — Called with the new colour, in every format, whenever it changes.
- `onCollapse` — Called with the selected colour when the picker closes.
- `openOnHover` — Whether hovering the picker opens it, as well as clicking. Only applies when `collapsible`.
- `petalSize` — The diameter of each petal, in pixels.
- `showAlphaSlider` — Whether to show the Lightness arc slider beside the petals while open.
- `showCoreColor` — Whether the centre shows the selected colour while open. When `false`, it turns white while open.
- `sliderOffset` — The distance between the colour ring and the arc sliders, in pixels.
- `sliderPosition` — The side the Lightness slider sits on. The Opacity slider takes the opposite side. When unset, the picker picks the side with the most room.
- `sliderWidth` — The thickness of the arc sliders, in pixels.
- `triggerIcon` — Replaces the icon on the colour format switch. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `value` — The selected colour. Use with `onChange` to control it.

Required props are bold. Full docs: https://ui.xiod.dev/docs
