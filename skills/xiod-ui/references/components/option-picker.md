# OptionPicker

```tsx
import { OptionPicker } from "xiod-ui/option-picker";
```

## OptionPicker

| Prop | Type |
| :--- | :--- |
| defaultValue | `string \| undefined` |
| icon | `ReactNode` |
| onChange | `((value: string) => void) \| undefined` |
| **options** | `Option[]` |
| popupClassName | `string \| undefined` |
| triggerClassName | `string \| undefined` |
| value | `string \| undefined` |

- `defaultValue` — The `id` of the option selected at first, when it isn't controlled. Defaults to the first option.
- `icon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `onChange` — Called with the option's `id` when the user picks one.
- `options` — The options to choose from. Up to five are shown; any more are left out.
- `popupClassName` — Classes for the popup that lists the options.
- `triggerClassName` — Classes for the button that shows the selected option.
- `value` — The `id` of the selected option. Use with `onChange` to control it.

Required props are bold. Full docs: https://ui.xiod.dev/docs
