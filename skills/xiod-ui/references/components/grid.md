# Grid

```tsx
import { Grid, GridItem } from "xiod-ui/grid";
```

## Grid

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| align | `"center" \| "start" \| "end" \| "stretch" \| "baseline" \| null \| undefined` | — |
| columns | `1 \| "none" \| 2 \| 3 \| 4 \| 5 \| 6 \| "subgrid" \| 7 \| 8 \| 9 \| 10 \| 11 \| 12 \| null \| undefined` | — |
| flow | `"col" \| "row" \| "dense" \| "row-dense" \| "col-dense" \| null \| undefined` | — |
| gap | `"base" \| "none" \| "sm" \| "lg" \| "md" \| "xl" \| null \| undefined` | `"base"` |
| justify | `"center" \| "start" \| "end" \| "stretch" \| "between" \| null \| undefined` | — |
| rows | `1 \| "none" \| 2 \| 3 \| 4 \| 5 \| 6 \| "subgrid" \| 7 \| 8 \| 9 \| 10 \| 11 \| 12 \| null \| undefined` | — |

- `align` — How items line up vertically within their cells.
- `columns` — The number of equal columns. `subgrid` lines up with the columns of a parent grid.
- `flow` — How items fill the grid: along rows or columns. The `dense` options fill earlier gaps with later, smaller items.
- `gap` — The space between rows and columns. `base` is 1rem on phones and 1.5rem from the `sm` breakpoint up.
- `justify` — How items line up horizontally within their cells. `between` spreads the columns out with the space between them.
- `rows` — The number of equal rows. `subgrid` lines up with the rows of a parent grid.

## GridItem

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| colEnd | `1 \| 2 \| 3 \| 4 \| 5 \| 6 \| 7 \| 8 \| 9 \| 10 \| 11 \| 12 \| 13 \| null \| undefined` |
| colSpan | `1 \| "auto" \| 2 \| 3 \| 4 \| 5 \| 6 \| 7 \| 8 \| 9 \| 10 \| 11 \| 12 \| "full" \| null \| undefined` |
| colStart | `1 \| 2 \| 3 \| 4 \| 5 \| 6 \| 7 \| 8 \| 9 \| 10 \| 11 \| 12 \| 13 \| null \| undefined` |
| rowEnd | `1 \| 2 \| 3 \| 4 \| 5 \| 6 \| 7 \| 8 \| 9 \| 10 \| 11 \| 12 \| 13 \| null \| undefined` |
| rowSpan | `1 \| "auto" \| 2 \| 3 \| 4 \| 5 \| 6 \| 7 \| 8 \| 9 \| 10 \| 11 \| 12 \| "full" \| null \| undefined` |
| rowStart | `1 \| 2 \| 3 \| 4 \| 5 \| 6 \| 7 \| 8 \| 9 \| 10 \| 11 \| 12 \| 13 \| null \| undefined` |

- `colEnd` — The column line the item ends at, counting from 1 at the left edge.
- `colSpan` — How many columns the item spans. `full` spans every column.
- `colStart` — The column line the item starts at, counting from 1 at the left edge.
- `rowEnd` — The row line the item ends at, counting from 1 at the top.
- `rowSpan` — How many rows the item spans. `full` spans every row.
- `rowStart` — The row line the item starts at, counting from 1 at the top.

Required props are bold. Full docs: https://ui.xiod.dev/docs
