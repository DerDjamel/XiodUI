# Timeline

```tsx
import { Timeline, TimelineContent, TimelineDate, TimelineHeader, TimelineIndicator, TimelineItem, TimelineSeparator, TimelineTitle, useTimeline } from "xiod-ui/timeline";
```

## Timeline

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| defaultValue | `number \| undefined` | — |
| onValueChange | `((value: number) => void) \| undefined` | — |
| orientation | `"horizontal" \| "vertical" \| undefined` | `"vertical"` |
| value | `number \| undefined` | — |

- `defaultValue` — The step that is active at first, when it isn't controlled. Items before it show as completed and items after it as pending.
- `onValueChange` — Called with the new step when the active step changes through `setActiveStep` from `useTimeline`.
- `value` — The active step. Items before it show as completed and items after it as pending.

## TimelineContent

Renders a `<div>` and takes its props. Pass `render` to render a different element.

## TimelineDate

Renders a `<time>` and takes its props. Pass `render` to render a different element.

## TimelineHeader

Renders a `<div>` and takes its props. Pass `render` to render a different element.

## TimelineIndicator

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| size | `"sm" \| "default" \| "lg" \| null \| undefined` | `"default"` |
| variant | `"default" \| "solid" \| null \| undefined` | `"default"` |

## TimelineItem

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| status | `"completed" \| "active" \| "pending" \| undefined` |
| step | `number \| undefined` |

- `status` — The item's status. Overrides the one worked out from `step`.
- `step` — The item's position in the timeline, compared with the `Timeline`'s value to work out its status.

## TimelineSeparator

Renders a `<div>` and takes its props. Pass `render` to render a different element.

## TimelineTitle

Renders a `<h3>` and takes its props. Pass `render` to render a different element.

## useTimeline

```tsx
useTimeline()
```

Returns `undefined | { activeStep?: number | undefined; setActiveStep: (step: number) => void }`.

Required props are bold. Full docs: https://ui.xiod.dev/docs
