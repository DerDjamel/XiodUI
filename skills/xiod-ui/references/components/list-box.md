# ListBox

```tsx
import { ListBox, ListBoxGroup, ListBoxItem, ListBoxLabel, ListBoxSeparator } from "xiod-ui/list-box";
```

## ListBox

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| defaultValue | `ListBoxValue \| undefined` |
| multiple | `boolean \| undefined` |
| name | `string \| undefined` |
| onValueChange | `((value: ListBoxValue) => void) \| undefined` |
| value | `ListBoxValue \| undefined` |

- `defaultValue` — The value selected at first, when the selection isn't controlled.
- `multiple` — Whether more than one item can be selected. The value is then an array.
- `name` — Submits the selection with a form: one hidden input per selected value.
- `onValueChange` — Called with the new value when the selection changes.
- `value` — The selected value: a string, or an array of strings when `multiple` is set. Use with `onValueChange` to control the selection.

## ListBoxGroup

Renders a `<div>` and takes its props. Pass `render` to render a different element.

## ListBoxItem

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| disabled | `boolean \| undefined` |
| **value** | `string` |

- `value` — The value this item selects. Must be unique within the list.

## ListBoxLabel

Renders a `<div>` and takes its props. Pass `render` to render a different element.

## ListBoxSeparator

Renders a `<div>` and takes its props. Pass `render` to render a different element.

Required props are bold. Full docs: https://ui.xiod.dev/docs
