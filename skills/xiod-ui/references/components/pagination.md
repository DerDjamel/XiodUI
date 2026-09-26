# Pagination

```tsx
import { Pagination, PaginationContent, PaginationEllipsis, PaginationFirst, PaginationInput, PaginationItem, PaginationLast, PaginationLink, PaginationNext, PaginationPrevious } from "xiod-ui/pagination";
```

## Pagination

Renders a `<nav>` and takes its props. Pass `render` to render a different element.

## PaginationContent

Renders a `<ul>` and takes its props. Pass `render` to render a different element.

## PaginationEllipsis

Renders a `<span>` and takes its props. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| icon | `ReactNode` |

- `icon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.

## PaginationFirst

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| icon | `ReactNode` |
| isActive | `boolean \| undefined` |
| size | `"sm" \| "default" \| "lg" \| "xs" \| "xl" \| "icon" \| "icon-lg" \| "icon-sm" \| "icon-xl" \| "icon-xs" \| null \| undefined` |

- `icon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `isActive` — Whether the link is the current page. Highlights it and marks it with `aria-current="page"`.

## PaginationInput

| Prop | Type |
| :--- | :--- |
| onChange | `((page: number) => void) \| undefined` |
| totalPages | `number \| undefined` |
| value | `number \| undefined` |

- `onChange` — Called with the page number when the user presses Enter or leaves the input. The number is clamped between 1 and `totalPages`.
- `totalPages` — The number of pages. Entries above it are clamped to it.
- `value` — The current page number.

## PaginationItem

Renders a `<li>` and takes its props. Pass `render` to render a different element.

## PaginationLast

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| icon | `ReactNode` |
| isActive | `boolean \| undefined` |
| size | `"sm" \| "default" \| "lg" \| "xs" \| "xl" \| "icon" \| "icon-lg" \| "icon-sm" \| "icon-xl" \| "icon-xs" \| null \| undefined` |

- `icon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `isActive` — Whether the link is the current page. Highlights it and marks it with `aria-current="page"`.

## PaginationLink

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| isActive | `boolean \| undefined` | — |
| size | `"sm" \| "default" \| "lg" \| "xs" \| "xl" \| "icon" \| "icon-lg" \| "icon-sm" \| "icon-xl" \| "icon-xs" \| null \| undefined` | `"icon"` |

- `isActive` — Whether the link is the current page. Highlights it and marks it with `aria-current="page"`.

## PaginationNext

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| icon | `ReactNode` |
| isActive | `boolean \| undefined` |
| size | `"sm" \| "default" \| "lg" \| "xs" \| "xl" \| "icon" \| "icon-lg" \| "icon-sm" \| "icon-xl" \| "icon-xs" \| null \| undefined` |

- `icon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `isActive` — Whether the link is the current page. Highlights it and marks it with `aria-current="page"`.

## PaginationPrevious

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| icon | `ReactNode` |
| isActive | `boolean \| undefined` |
| size | `"sm" \| "default" \| "lg" \| "xs" \| "xl" \| "icon" \| "icon-lg" \| "icon-sm" \| "icon-xl" \| "icon-xs" \| null \| undefined` |

- `icon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `isActive` — Whether the link is the current page. Highlights it and marks it with `aria-current="page"`.

Required props are bold. Full docs: https://ui.xiod.dev/docs
