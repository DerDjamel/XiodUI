# Calendar

```tsx
import { Calendar } from "xiod-ui/calendar";
```

## Calendar

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| classNames | `CalendarClassNames \| undefined` | — |
| disabled | `Matcher \| Matcher[] \| undefined` | — |
| disableOutsideDays | `boolean \| undefined` | `false` |
| fixedWeeks | `boolean \| undefined` | `true` |
| localeMonths | `string[] \| undefined` | — |
| localeMonthsShort | `string[] \| undefined` | — |
| localeWeekdays | `string[] \| undefined` | — |
| localeWeekdaysLong | `string[] \| undefined` | — |
| maxDate | `Date \| undefined` | — |
| minDate | `Date \| undefined` | — |
| mode | `CalendarMode \| undefined` | `"single"` |
| modifiers | `Record<string, Matcher \| Matcher[]> \| undefined` | — |
| modifiersClassNames | `Record<string, string> \| undefined` | — |
| nextIcon | `ReactNode` | — |
| numberOfMonths | `number \| undefined` | `1` |
| onSelect | `((date: Date \| DateRange \| undefined) => void) \| undefined` | — |
| prevIcon | `ReactNode` | — |
| selected | `Date \| DateRange \| null \| undefined` | — |
| showOutsideDays | `boolean \| undefined` | `true` |
| weekStartsOn | `0 \| 1 \| 2 \| 3 \| 4 \| 5 \| 6 \| undefined` | `0` |

- `classNames` — Classes for the calendar's parts, keyed by part name.
- `disabled` — Days that can't be selected: `true` for all, a date, a list of dates, a function that returns `true` for a date, `{ before }` and `{ after }` limits, or `{ dayOfWeek }` with 0 for Sunday. Pass an array to combine them.
- `disableOutsideDays` — Whether days from the previous and next months can't be selected.
- `fixedWeeks` — Whether every month shows six weeks, so the calendar's height doesn't change between months.
- `localeMonths` — Full month names, starting from January. Defaults to English.
- `localeMonthsShort` — Short month names, starting from January, for the month picker and the selection summary. Defaults to English.
- `localeWeekdays` — Short weekday names for the column headings, starting from Sunday. Defaults to English.
- `localeWeekdaysLong` — Full weekday names for screen readers, starting from Sunday. Defaults to English.
- `maxDate` — The latest date that can be selected. The calendar can't navigate past its month.
- `minDate` — The earliest date that can be selected. The calendar can't navigate before its month.
- `mode` — Whether the user picks one date (`single`) or a start and end date (`range`).
- `modifiers` — Named groups of days, each matched the same ways as `disabled`. Style them with `modifiersClassNames`.
- `modifiersClassNames` — Classes for the days in each group named in `modifiers`, keyed by the group's name.
- `nextIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `numberOfMonths` — How many months to show side by side.
- `onSelect` — Called with the new date, or the new `{ from, to }` range in `range` mode, when the user picks a day.
- `prevIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `selected` — The selected date, or `{ from, to }` in `range` mode. The calendar is controlled: update it from `onSelect`.
- `showOutsideDays` — Whether to show the days of the previous and next months that fill the first and last weeks.
- `weekStartsOn` — The first day of the week, from 0 for Sunday to 6 for Saturday.

Required props are bold. Full docs: https://ui.xiod.dev/docs
