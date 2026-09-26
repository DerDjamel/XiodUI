# Sortable

```tsx
import { Sortable, SortableColumn, SortableColumnHeader, SortableColumnTitle, SortableItem, SortableItemHandle, SortableItemRemove } from "xiod-ui/sortable";
```

## Sortable

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| handleIcon | `ReactNode` | — |
| **items** | `string[]` | — |
| onRemove | `((id: string) => void) \| undefined` | — |
| **onReorder** | `(newItems: string[]) => void` | — |
| orientation | `SortableOrientation \| undefined` | `"vertical"` |
| variant | `"default" \| "ghost" \| "bordered" \| null \| undefined` | `"default"` |

- `handleIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `items` — The ids of the items, in their current order. Each `SortableItem` finds its place by its `id`.
- `onRemove` — Called with an item's id when its `SortableItemRemove` button is pressed.
- `onReorder` — Called with the ids in their new order whenever an item moves: on drop with a pointer, or on each arrow key while moving one with the keyboard. Escape during a keyboard move calls it again with the original order.

## SortableColumn

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| **id** | `string` |

- `id` — The column's id. It also names the column for screen readers unless you pass `aria-label`.

## SortableColumnHeader

Takes the DOM props of the element it renders. Pass `render` to render a different element.

## SortableColumnTitle

Takes the DOM props of the element it renders. Pass `render` to render a different element.

## SortableItem

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| **id** | `string` | — |
| variant | `"default" \| "flat" \| "accent" \| null \| undefined` | `"default"` |

- `id` — The item's id, as listed in the `Sortable`'s `items`.

## SortableItemHandle

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| icon | `ReactNode` |

- `icon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.

## SortableItemRemove

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| icon | `ReactNode` |
| **id** | `string` |

- `icon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `id` — The id of the item to remove, passed to the `Sortable`'s `onRemove`.

Required props are bold. Full docs: https://ui.xiod.dev/docs
