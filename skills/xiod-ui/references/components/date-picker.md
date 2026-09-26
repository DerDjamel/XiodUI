# DatePicker

```tsx
import { DatePicker } from "xiod-ui/date-picker";
```

## DatePicker

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| defaultValue | `Date \| DateRange \| undefined` | — |
| disabled | `boolean \| Date \| Date[] \| ((date: Date) => boolean) \| undefined` | — |
| disableOutsideDays | `boolean \| undefined` | `false` |
| fixedWeeks | `boolean \| undefined` | `true` |
| formatStr | `"PPP" \| "LLL dd, y" \| "yyyy-MM-dd" \| undefined` | `"PPP"` |
| icon | `ReactNode` | — |
| maxDate | `Date \| undefined` | — |
| minDate | `Date \| undefined` | — |
| mode | `"single" \| "range" \| undefined` | `"single"` |
| numberOfMonths | `number \| undefined` | `1` |
| onSelect | `((value: Date \| DateRange \| undefined) => void) \| undefined` | — |
| placeholder | `string \| undefined` | — |
| showOutsideDays | `boolean \| undefined` | `true` |
| triggerClassName | `string \| undefined` | — |
| triggerSize | `"sm" \| "default" \| "lg" \| "xs" \| undefined` | `"default"` |
| triggerType | `"button" \| "input" \| undefined` | `"button"` |
| triggerVariant | `"default" \| "secondary" \| "ghost" \| "outline" \| undefined` | `"outline"` |
| value | `Date \| DateRange \| undefined` | — |
| weekStartsOn | `0 \| 1 \| 2 \| 3 \| 4 \| 5 \| 6 \| undefined` | `0` |

- `defaultValue` — The date, or `{ from, to }` range, selected at first, when it isn't controlled.
- `disabled` — Days that can't be selected: `true` for all, a date, a list of dates, or a function that returns `true` for a date.
- `disableOutsideDays` — Whether days from the previous and next months can't be selected.
- `fixedWeeks` — Whether every month shows six weeks, so the calendar's height doesn't change between months.
- `formatStr` — How the button shows a single date: `"PPP"` for September 26, 2026, `"LLL dd, y"` for Sep 26, 2026, or `"yyyy-MM-dd"` for 2026-09-26.
- `icon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `maxDate` — The latest date that can be selected.
- `minDate` — The earliest date that can be selected.
- `mode` — Whether the user picks one date (`single`) or a start and end date (`range`).
- `numberOfMonths` — How many months the calendar shows side by side.
- `onSelect` — Called with the new date, or the new `{ from, to }` range, when the user picks or types one.
- `placeholder` — The text shown when no date is selected.
- `showOutsideDays` — Whether the calendar shows the days of the previous and next months that fill the first and last weeks.
- `triggerClassName` — Classes for the button or input that opens the calendar.
- `triggerSize` — The `Button` size of the trigger, when `triggerType` is `button`.
- `triggerType` — What opens the calendar: a `button` showing the formatted date, or an `input` the user can also type a date into as YYYY-MM-DD.
- `triggerVariant` — The `Button` variant of the trigger, when `triggerType` is `button`.
- `value` — The selected date, or `{ from, to }` in `range` mode. Use with `onSelect` to control it.
- `weekStartsOn` — The first day of the week, from 0 for Sunday to 6 for Saturday.

Required props are bold. Full docs: https://ui.xiod.dev/docs
