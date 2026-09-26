# DashboardGrid

```tsx
import { DashboardGrid, DashboardTile, DashboardTileControls, DashboardTileHandle, DashboardTileHeader, DashboardTileResizeHandle, DashboardTileTitle } from "xiod-ui/dashboard-grid";
```

## DashboardGrid

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| breakpoints | `Breakpoints \| undefined` | `defaultBreakpoints` |
| cols | `number \| BreakpointCols \| undefined` | `12` |
| compactType | `CompactType \| undefined` | `"vertical"` |
| containerPadding | `[number, number] \| undefined` | `DEFAULT_CONTAINER_PADDING` |
| isDraggable | `boolean \| undefined` | `true` |
| isResizable | `boolean \| undefined` | `true` |
| **layout** | `DashboardTileData[]` | — |
| margin | `[number, number] \| undefined` | `DEFAULT_GRID_MARGIN` |
| onLayoutChange | `((layout: DashboardTileData[]) => void) \| undefined` | — |
| onTileRemove | `((id: string) => void) \| undefined` | — |
| preventCollision | `boolean \| undefined` | `false` |
| rowHeight | `number \| undefined` | `60` |
| showGridLines | `boolean \| undefined` | `false` |
| variant | `"canvas" \| "default" \| "ghost" \| "bordered" \| null \| undefined` | `"default"` |

- `breakpoints` — The smallest grid width, in pixels, at which each breakpoint applies. Only used when `cols` is an object.
- `cols` — The number of columns: one number for every width, or an object with a count per breakpoint (`lg`, `md`, `sm`, `xs`, `xxs`).
- `compactType` — Which way tiles move to fill gaps: `vertical` pulls them up, `horizontal` pulls them left, and `null` leaves them where they are dropped.
- `containerPadding` — The space between the tiles and the edge of the grid, in pixels, as `[horizontal, vertical]`.
- `isDraggable` — Whether tiles can be moved, by pointer or keyboard.
- `isResizable` — Whether tiles can be resized, by pointer or keyboard.
- `layout` — The position and size of every tile. Keep it in state and update it from `onLayoutChange`.
- `margin` — The space between tiles, in pixels, as `[horizontal, vertical]`.
- `onLayoutChange` — Called with the new layout after a tile is moved or resized.
- `onTileRemove` — Called with a tile's id when its remove button is pressed. The remove button only shows when this is set.
- `preventCollision` — Whether a tile can't be dropped on top of another. When `false`, the other tiles move out of the way.
- `rowHeight` — The height of one row, in pixels.
- `showGridLines` — Whether to draw the column and row lines behind the tiles.

## DashboardTile

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| **id** | `string` | — |
| variant | `"default" \| "expressive" \| "flat" \| null \| undefined` | `"default"` |

- `id` — The tile's id, matching an `i` in the grid's `layout`.

## DashboardTileControls

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| icon | `ReactNode` |
| id | `string \| undefined` |

- `icon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `id` — The id of the tile these controls belong to. With it, and the grid's `onTileRemove` set, they show a remove button by default.

## DashboardTileHandle

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| icon | `ReactNode` |
| id | `string \| undefined` |

- `icon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `id` — The id of the tile this handle moves, by dragging or with the arrow keys.

## DashboardTileHeader

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| icon | `ReactNode` |
| id | `string \| undefined` |

- `icon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `id` — The id of the tile this header belongs to. With it, the header moves the tile when dragged and shows its remove button.

## DashboardTileResizeHandle

Takes the DOM props of the element it renders. Pass `render` to render a different element.

## DashboardTileTitle

Takes the DOM props of the element it renders. Pass `render` to render a different element.

Required props are bold. Full docs: https://ui.xiod.dev/docs
