# InputPhone

```tsx
import { InputPhone, InputPhoneCountrySelect, InputPhoneFlag, InputPhoneInput, PhoneInput, PhoneInputCountrySelect, PhoneInputFlag, PhoneInputInput, useInputPhone, usePhoneInput } from "xiod-ui/input-phone";
```

## InputPhone

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| countries | `CountryData[] \| undefined` | `COUNTRIES` |
| defaultCountry | `string \| undefined` | `"US"` |
| defaultValue | `string \| undefined` | `""` |
| disabled | `boolean \| undefined` | — |
| name | `string \| undefined` | — |
| onChange | `((e164: string, country: CountryData, nationalNumber: string) => void) \| undefined` | — |
| readOnly | `boolean \| undefined` | — |
| size | `"sm" \| "default" \| "lg" \| null \| undefined` | `"default"` |
| value | `string \| undefined` | — |
| variant | `"default" \| "ghost" \| "filled" \| null \| undefined` | `"default"` |

- `countries` — The countries the user can choose from. Defaults to the built-in list, exported as `COUNTRIES`.
- `defaultCountry` — The code of the country selected at first, such as `"US"`, when no number sets it.
- `defaultValue` — The number at first, when it isn't controlled, in E.164 format such as `"+15550000000"`. Its dialling code picks the country.
- `name` — Submits the E.164 value (e.g. "+15550000000") with a form under this name.
- `onChange` — Called when the number or country changes, with the full number in E.164 format, the selected country, and the digits typed without the dialling code.
- `value` — The number in E.164 format, such as `"+15550000000"`. Use with `onChange` to control it.

## InputPhoneCountrySelect

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| clearIcon | `ReactNode` |
| searchIcon | `ReactNode` |
| selectedIcon | `ReactNode` |
| triggerIcon | `ReactNode` |

- `clearIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `searchIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `selectedIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `triggerIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.

## InputPhoneFlag

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| code | `string \| undefined` |

- `code` — The code of the country whose flag to show, such as `"GB"`. Defaults to the selected country.

## InputPhoneInput

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| className | `string \| undefined` |
| clearIcon | `ReactNode` |
| defaultValue | `string \| number \| readonly string[] \| undefined` |
| nativeInput | `boolean \| undefined` |
| onValueChange | `((value: string, eventDetails: { reason: "none"; event: Event; cancel: () => void; allowPropagation: () => void; isCanceled: boolean; isPropagationAllowed: boolean; trigger: Element \| undefined; }) => void) \| undefined` |
| size | `number \| "sm" \| "default" \| "lg" \| undefined` |
| style | `CSSProperties \| undefined` |
| unstyled | `boolean \| undefined` |

- `clearIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `defaultValue` — The default value of the input. Use when uncontrolled.
- `nativeInput` — Whether to render a plain `<input>` instead of Base UI's `Input`. A plain input doesn't register with a surrounding `Field`.
- `onValueChange` — Callback fired when the `value` changes. Use when controlled.
- `unstyled` — Whether to drop the border, background and focus ring, leaving only the text field. Use inside your own styled container.

## PhoneInput

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| countries | `CountryData[] \| undefined` |
| defaultCountry | `string \| undefined` |
| defaultValue | `string \| undefined` |
| disabled | `boolean \| undefined` |
| name | `string \| undefined` |
| onChange | `((e164: string, country: CountryData, nationalNumber: string) => void) \| undefined` |
| readOnly | `boolean \| undefined` |
| size | `"sm" \| "default" \| "lg" \| null \| undefined` |
| value | `string \| undefined` |
| variant | `"default" \| "ghost" \| "filled" \| null \| undefined` |

- `countries` — The countries the user can choose from. Defaults to the built-in list, exported as `COUNTRIES`.
- `defaultCountry` — The code of the country selected at first, such as `"US"`, when no number sets it.
- `defaultValue` — The number at first, when it isn't controlled, in E.164 format such as `"+15550000000"`. Its dialling code picks the country.
- `name` — Submits the E.164 value (e.g. "+15550000000") with a form under this name.
- `onChange` — Called when the number or country changes, with the full number in E.164 format, the selected country, and the digits typed without the dialling code.
- `value` — The number in E.164 format, such as `"+15550000000"`. Use with `onChange` to control it.

## PhoneInputCountrySelect

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| clearIcon | `ReactNode` |
| searchIcon | `ReactNode` |
| selectedIcon | `ReactNode` |
| triggerIcon | `ReactNode` |

- `clearIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `searchIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `selectedIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `triggerIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.

## PhoneInputFlag

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| code | `string \| undefined` |

- `code` — The code of the country whose flag to show, such as `"GB"`. Defaults to the selected country.

## PhoneInputInput

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| className | `string \| undefined` |
| clearIcon | `ReactNode` |
| defaultValue | `string \| number \| readonly string[] \| undefined` |
| nativeInput | `boolean \| undefined` |
| onValueChange | `((value: string, eventDetails: { reason: "none"; event: Event; cancel: () => void; allowPropagation: () => void; isCanceled: boolean; isPropagationAllowed: boolean; trigger: Element \| undefined; }) => void) \| undefined` |
| size | `number \| "sm" \| "default" \| "lg" \| undefined` |
| style | `CSSProperties \| undefined` |
| unstyled | `boolean \| undefined` |

- `clearIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `defaultValue` — The default value of the input. Use when uncontrolled.
- `nativeInput` — Whether to render a plain `<input>` instead of Base UI's `Input`. A plain input doesn't register with a surrounding `Field`.
- `onValueChange` — Callback fired when the `value` changes. Use when controlled.
- `unstyled` — Whether to drop the border, background and focus ring, leaving only the text field. Use inside your own styled container.

## useInputPhone

```tsx
useInputPhone()
```

Returns `{ containerRef: RefObject<HTMLDivElement | null>; selectedCountry: CountryData; setSelectedCountry: (country: CountryData) => void; nationalNumber: string; setNationalNumber: (num: string) => void; e164Value: string; disabled?: boolean | undefined; readOnly?: boolean | undefined; countries: CountryData[]; onChange?: ((e164: string, country: CountryData, nationalNumber: string) => void) | undefined }`.

## usePhoneInput

```tsx
usePhoneInput()
```

Returns `{ containerRef: RefObject<HTMLDivElement | null>; selectedCountry: CountryData; setSelectedCountry: (country: CountryData) => void; nationalNumber: string; setNationalNumber: (num: string) => void; e164Value: string; disabled?: boolean | undefined; readOnly?: boolean | undefined; countries: CountryData[]; onChange?: ((e164: string, country: CountryData, nationalNumber: string) => void) | undefined }`.

Required props are bold. Full docs: https://ui.xiod.dev/docs
