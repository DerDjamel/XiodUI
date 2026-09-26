# Draggable

```tsx
import { Draggable, DraggableBody, DraggableControls, DraggableFooter, DraggableHandle, DraggableHeader, DraggableResizeHandle, DraggableTitle } from "xiod-ui/draggable";
```

## Draggable

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| bounds | `DraggableBounds \| undefined` | `"viewport"` |
| defaultHeight | `number \| undefined` | `300` |
| defaultOpen | `boolean \| undefined` | `true` |
| defaultWidth | `number \| undefined` | `360` |
| defaultX | `number \| undefined` | `40` |
| defaultY | `number \| undefined` | `40` |
| isDraggable | `boolean \| undefined` | `true` |
| isResizable | `boolean \| undefined` | `true` |
| maxHeight | `number \| undefined` | `600` |
| maxWidth | `number \| undefined` | `800` |
| minHeight | `number \| undefined` | `160` |
| minWidth | `number \| undefined` | `240` |
| onOpenChange | `((open: boolean) => void) \| undefined` | — |
| open | `boolean \| undefined` | — |
| variant | `"default" \| "expressive" \| "flat" \| null \| undefined` | `"default"` |

- `bounds` — What the panel can't be moved out of: the `viewport`, its `parent` element, or `none` to move freely.
- `defaultHeight` — The panel's starting height, in pixels.
- `defaultOpen` — Whether the panel is shown at first, when it isn't controlled.
- `defaultWidth` — The panel's starting width, in pixels.
- `defaultX` — The panel's starting distance from the left edge of the viewport, in pixels.
- `defaultY` — The panel's starting distance from the top edge of the viewport, in pixels.
- `isDraggable` — Whether the panel can be moved, by its header or handle.
- `isResizable` — Whether the panel can be resized from its corner.
- `maxHeight` — The tallest the panel can be resized to, in pixels.
- `maxWidth` — The widest the panel can be resized to, in pixels.
- `minHeight` — The shortest the panel can be resized to, in pixels.
- `minWidth` — The narrowest the panel can be resized to, in pixels.
- `onOpenChange` — Called with `false` when the panel's close button is pressed.
- `open` — Whether the panel is shown. Use with `onOpenChange` to control it.

## DraggableBody

Takes the DOM props of the element it renders. Pass `render` to render a different element.

## DraggableControls

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| closeIcon | `ReactNode` |
| maximizeIcon | `ReactNode` |
| minimizeIcon | `ReactNode` |
| restoreIcon | `ReactNode` |

- `closeIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `maximizeIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `minimizeIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `restoreIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.

## DraggableFooter

Takes the DOM props of the element it renders. Pass `render` to render a different element.

## DraggableHandle

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| icon | `ReactNode` |

- `icon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.

## DraggableHeader

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| icon | `ReactNode` |

- `icon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.

## DraggableResizeHandle

Takes the DOM props of the element it renders. Pass `render` to render a different element.

## DraggableTitle

Takes the DOM props of the element it renders. Pass `render` to render a different element.

Required props are bold. Full docs: https://ui.xiod.dev/docs
