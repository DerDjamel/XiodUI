# Resizable

```tsx
import { ResizableHandle, ResizablePanel, ResizablePanelGroup } from "xiod-ui/resizable";
```

## ResizableHandle

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| disabled | `boolean \| undefined` | `false` |
| disableDoubleClick | `boolean \| undefined` | `false` |
| icon | `ReactNode` | — |
| withHandle | `boolean \| undefined` | `false` |

- `disabled` — Whether the user is prevented from dragging this handle.
- `disableDoubleClick` — Whether double-clicking the handle leaves the panel before it as it is, instead of collapsing or expanding it.
- `icon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `withHandle` — Whether to show a grip in the middle of the handle, so it's easier to see and grab.

## ResizablePanel

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| collapsedSize | `string \| number \| undefined` | `"0%"` |
| collapsible | `boolean \| undefined` | `false` |
| defaultSize | `string \| number \| undefined` | — |
| disabled | `boolean \| undefined` | `false` |
| groupResizeBehavior | `"preserve-relative-size" \| "preserve-pixel-size" \| undefined` | `"preserve-relative-size"` |
| id | `string \| undefined` | — |
| maxSize | `string \| number \| undefined` | `"100%"` |
| minSize | `string \| number \| undefined` | `"0%"` |
| onCollapse | `(() => void) \| undefined` | — |
| onExpand | `(() => void) \| undefined` | — |
| onResize | `((size: { asPercentage: number; inPixels: number; }) => void) \| undefined` | — |
| panelRef | `RefObject<ImperativePanelHandle \| null> \| undefined` | — |

- `collapsedSize` — The panel's size when collapsed. A number is in pixels; a string can use `%`, `px`, `rem`, `em`, `vh` or `vw`.
- `collapsible` — Whether the panel collapses to `collapsedSize` when dragged well below `minSize` (past halfway to `collapsedSize`), or when the handle after it is double-clicked.
- `defaultSize` — The panel's size at first. When no panel sets one, the space is split evenly. A number is in pixels; a string can use `%`, `px`, `rem`, `em`, `vh` or `vw`.
- `disabled` — Whether the user is prevented from resizing this panel. `panelRef` can still resize it.
- `groupResizeBehavior` — What happens to the panel when the whole group changes size: `preserve-relative-size` keeps its share of the group, `preserve-pixel-size` keeps its width or height in pixels.
- `id` — A stable id for the panel. Set it when the group has a `storageKey`, so the saved layout is matched to the right panels.
- `maxSize` — The largest size the user can drag the panel to. A number is in pixels; a string can use `%`, `px`, `rem`, `em`, `vh` or `vw`.
- `minSize` — The smallest size the user can drag the panel to. A number is in pixels; a string can use `%`, `px`, `rem`, `em`, `vh` or `vw`.
- `onCollapse` — Called when the panel collapses.
- `onExpand` — Called when the panel expands from collapsed.
- `onResize` — Called with the panel's new size, as a percentage of the group and in pixels, whenever it changes.
- `panelRef` — A ref to control the panel from code: `collapse()`, `expand()`, `resize(size)`, `isCollapsed()`, `isExpanded()` and `getSize()`.

## ResizablePanelGroup

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| defaultLayout | `(string \| number)[] \| undefined` | — |
| direction | `"horizontal" \| "vertical" \| undefined` | `"horizontal"` |
| disabled | `boolean \| undefined` | `false` |
| groupRef | `RefObject<ImperativeGroupHandle \| null> \| undefined` | — |
| onLayoutChange | `((layout: number[]) => void) \| undefined` | — |
| onLayoutChanged | `((layout: number[]) => void) \| undefined` | — |
| storage | `{ getItem: (key: string) => string \| null; setItem: (key: string, value: string) => void; } \| undefined` | — |
| storageKey | `string \| undefined` | — |

- `defaultLayout` — The size of each panel at first, in order. Takes precedence over each panel's `defaultSize`. A number is in pixels; a string can use `%`, `px`, `rem`, `em`, `vh` or `vw`.
- `direction` — Whether the panels sit side by side (`horizontal`) or stacked (`vertical`).
- `disabled` — Whether the user is prevented from resizing any panel.
- `groupRef` — A ref to read and set the whole layout from code, with `getLayout()` and `setLayout(layout)`. Sizes are percentages.
- `onLayoutChange` — Called with each panel's size, as a percentage of the group, whenever the layout changes, including on every step of a drag.
- `onLayoutChanged` — Called with each panel's size, as a percentage of the group, once the user finishes a resize: at the end of a drag, on a key press or on a double-click.
- `storage` — Where to save the layout when `storageKey` is set, instead of localStorage.
- `storageKey` — A key to save the layout under, so it comes back on the next visit. Saved to localStorage unless you pass `storage`. Give each panel an `id` so the saved layout survives changes to the page.

Required props are bold. Full docs: https://ui.xiod.dev/docs
