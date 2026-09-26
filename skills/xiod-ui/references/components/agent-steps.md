# AgentSteps

```tsx
import { AgentStep, AgentStepIcon, AgentStepIndicator, AgentStepLabel, AgentSteps } from "xiod-ui/agent-steps";
```

## AgentStep

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| status | `"completed" \| "waiting" \| "running" \| "failed" \| undefined` | `"running"` |

## AgentStepIcon

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| icon | `AgentStepIconValue` | — |
| showSpinner | `boolean \| undefined` | `false` |

## AgentStepIndicator

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| disableShimmer | `boolean \| undefined` | `false` |
| icon | `AgentStepIconValue` | — |
| interval | `number \| undefined` | `4000` |
| label | `ReactNode` | — |
| showIcon | `boolean \| undefined` | `true` |
| showSpinner | `boolean \| undefined` | `false` |
| size | `"sm" \| "lg" \| "md" \| null \| undefined` | `"md"` |
| status | `"completed" \| "waiting" \| "running" \| "failed" \| undefined` | `"running"` |
| steps | `string[] \| AgentStepItem[] \| undefined` | — |

- `disableShimmer` — Whether to turn off the shimmer that sweeps across the text. Used when there are no `children`.
- `icon` — The step's icon: a built-in name such as `thinking` or `searching`, or an icon component. Used when there are no `children`.
- `interval` — How long each of the `steps` is shown, in milliseconds.
- `label` — The text of the step shown. Used when there are no `children`.
- `showIcon` — Whether to show the icon. Used when there are no `children`.
- `showSpinner` — Whether to show a spinning dashed ring around the icon while the step is `running`. Used when there are no `children`.
- `status` — The step's status. `completed`, `failed` and `waiting` show their own icon and text style; the shimmer and spinner only run while `running`. Used when there are no `children`.
- `steps` — Steps to show one after another, every `interval` milliseconds, looping. Take the place of `label` and `icon`. Used when there are no `children`.

## AgentStepLabel

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| shimmer | `boolean \| undefined` | `true` |

- `shimmer` — Whether the label shows a shimmer sweep while its step is running.

## AgentSteps

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| disableShimmer | `boolean \| undefined` | `false` |
| icon | `AgentStepIconValue` | — |
| interval | `number \| undefined` | `4000` |
| label | `ReactNode` | — |
| showIcon | `boolean \| undefined` | `true` |
| showSpinner | `boolean \| undefined` | `false` |
| size | `"sm" \| "lg" \| "md" \| null \| undefined` | `"md"` |
| status | `"completed" \| "waiting" \| "running" \| "failed" \| undefined` | `"running"` |
| steps | `string[] \| AgentStepItem[] \| undefined` | — |

- `disableShimmer` — Whether to turn off the shimmer that sweeps across the text. Used when there are no `children`.
- `icon` — The step's icon: a built-in name such as `thinking` or `searching`, or an icon component. Used when there are no `children`.
- `interval` — How long each of the `steps` is shown, in milliseconds.
- `label` — The text of the step shown. Used when there are no `children`.
- `showIcon` — Whether to show the icon. Used when there are no `children`.
- `showSpinner` — Whether to show a spinning dashed ring around the icon while the step is `running`. Used when there are no `children`.
- `status` — The step's status. `completed`, `failed` and `waiting` show their own icon and text style; the shimmer and spinner only run while `running`. Used when there are no `children`.
- `steps` — Steps to show one after another, every `interval` milliseconds, looping. Take the place of `label` and `icon`. Used when there are no `children`.

Required props are bold. Full docs: https://ui.xiod.dev/docs
