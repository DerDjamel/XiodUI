# InputPayment

```tsx
import { InputPayment, InputPaymentBrandIcon, InputPaymentCardNumber, InputPaymentCVC, InputPaymentExpiry, InputPaymentGroup, InputPaymentMethodSelector, InputPaymentUpiGroup, InputPaymentUpiId, InputPaymentUpiProviderIcon, InputPaymentZip, PaymentInput, PaymentInputBrandIcon, PaymentInputCardNumber, PaymentInputCVC, PaymentInputExpiry, PaymentInputGroup, PaymentInputMethodSelector, PaymentInputUpiGroup, PaymentInputUpiId, PaymentInputUpiProviderIcon, PaymentInputZip, useInputPayment, usePaymentInput, usePaymentInputContext } from "xiod-ui/input-payment";
```

## InputPayment

| Prop | Type | Default |
| :--- | :--- | :--- |
| autoFocusNext | `boolean \| undefined` | `true` |
| cardCvc | `string \| undefined` | — |
| cardExpiry | `string \| undefined` | — |
| cardNumber | `string \| undefined` | — |
| cardZip | `string \| undefined` | — |
| children | `ReactNode` | — |
| defaultCardCvc | `string \| undefined` | `""` |
| defaultCardExpiry | `string \| undefined` | `""` |
| defaultCardNumber | `string \| undefined` | `""` |
| defaultCardZip | `string \| undefined` | `""` |
| defaultPaymentMethod | `PaymentMethod \| undefined` | `"card"` |
| defaultUpiId | `string \| undefined` | `""` |
| disabled | `boolean \| undefined` | `false` |
| onCardCvcChange | `((val: string) => void) \| undefined` | — |
| onCardExpiryChange | `((val: string) => void) \| undefined` | — |
| onCardNumberChange | `((val: string) => void) \| undefined` | — |
| onCardZipChange | `((val: string) => void) \| undefined` | — |
| onPaymentMethodChange | `((method: PaymentMethod) => void) \| undefined` | — |
| onUpiIdChange | `((val: string) => void) \| undefined` | — |
| onValidationChange | `((isValid: boolean, errors: PaymentInputErrors) => void) \| undefined` | — |
| paymentMethod | `PaymentMethod \| undefined` | — |
| readOnly | `boolean \| undefined` | `false` |
| upiId | `string \| undefined` | — |

- `autoFocusNext` — Whether focus moves to the next field once a field is complete and valid, and back to the previous one on Backspace in an empty field.
- `cardCvc` — The security code. Use with `onCardCvcChange` to control it.
- `cardExpiry` — The expiry date as `MM/YY`. Use with `onCardExpiryChange` to control it.
- `cardNumber` — The card number, spaced in groups as it is shown. Use with `onCardNumberChange` to control it.
- `cardZip` — The postal code. Use with `onCardZipChange` to control it.
- `defaultCardCvc` — The security code at first, when it isn't controlled.
- `defaultCardExpiry` — The expiry date at first, when it isn't controlled.
- `defaultCardNumber` — The card number at first, when it isn't controlled.
- `defaultCardZip` — The postal code at first, when it isn't controlled.
- `defaultPaymentMethod` — The payment method selected at first, when it isn't controlled.
- `defaultUpiId` — The UPI ID at first, when it isn't controlled.
- `onCardCvcChange` — Called with the security code as the user types, cut to the card brand's length.
- `onCardExpiryChange` — Called with the formatted expiry date as the user types.
- `onCardNumberChange` — Called with the formatted card number as the user types.
- `onCardZipChange` — Called with the postal code as the user types.
- `onPaymentMethodChange` — Called with the new method when the user switches between card and UPI.
- `onUpiIdChange` — Called with the UPI ID as the user types.
- `onValidationChange` — Called whenever the details become valid or invalid, with a message for each field that has an error.
- `paymentMethod` — Whether the user is paying by `card` or `upi`. Use with `onPaymentMethodChange` to control it.
- `upiId` — The UPI ID, such as `name@bank`. Use with `onUpiIdChange` to control it.

## InputPaymentBrandIcon

Renders a `<div>` and takes its props. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| icon | `ReactNode` |

- `icon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.

## InputPaymentCardNumber

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| className | `string \| undefined` | — |
| defaultValue | `string \| number \| readonly string[] \| undefined` | — |
| onChange | `ChangeEventHandler<HTMLInputElement, Element> \| undefined` | — |
| onKeyDown | `KeyboardEventHandler<HTMLInputElement> \| undefined` | — |
| onValueChange | `((value: string, eventDetails: { reason: "none"; event: Event; cancel: () => void; allowPropagation: () => void; isCanceled: boolean; isPropagationAllowed: boolean; trigger: Element \| undefined; }) => void) \| undefined` | — |
| size | `number \| "sm" \| "default" \| "lg" \| undefined` | `"default"` |
| style | `CSSProperties \| undefined` | — |
| value | `string \| number \| readonly string[] \| undefined` | — |

- `defaultValue` — The default value of the input. Use when uncontrolled.
- `onChange` — Called with the input's change event, after the field has formatted and stored the new value.
- `onKeyDown` — Called with the input's keydown event.
- `onValueChange` — Callback fired when the `value` changes. Use when controlled.
- `value` — The value of the input. Use when controlled.

## InputPaymentCVC

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| className | `string \| undefined` | — |
| defaultValue | `string \| number \| readonly string[] \| undefined` | — |
| onChange | `ChangeEventHandler<HTMLInputElement, Element> \| undefined` | — |
| onKeyDown | `KeyboardEventHandler<HTMLInputElement> \| undefined` | — |
| onValueChange | `((value: string, eventDetails: { reason: "none"; event: Event; cancel: () => void; allowPropagation: () => void; isCanceled: boolean; isPropagationAllowed: boolean; trigger: Element \| undefined; }) => void) \| undefined` | — |
| size | `number \| "sm" \| "default" \| "lg" \| undefined` | `"default"` |
| style | `CSSProperties \| undefined` | — |
| value | `string \| number \| readonly string[] \| undefined` | — |

- `defaultValue` — The default value of the input. Use when uncontrolled.
- `onChange` — Called with the input's change event, after the field has formatted and stored the new value.
- `onKeyDown` — Called with the input's keydown event.
- `onValueChange` — Callback fired when the `value` changes. Use when controlled.
- `value` — The value of the input. Use when controlled.

## InputPaymentExpiry

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| className | `string \| undefined` | — |
| defaultValue | `string \| number \| readonly string[] \| undefined` | — |
| onChange | `ChangeEventHandler<HTMLInputElement, Element> \| undefined` | — |
| onKeyDown | `KeyboardEventHandler<HTMLInputElement> \| undefined` | — |
| onValueChange | `((value: string, eventDetails: { reason: "none"; event: Event; cancel: () => void; allowPropagation: () => void; isCanceled: boolean; isPropagationAllowed: boolean; trigger: Element \| undefined; }) => void) \| undefined` | — |
| size | `number \| "sm" \| "default" \| "lg" \| undefined` | `"default"` |
| style | `CSSProperties \| undefined` | — |
| value | `string \| number \| readonly string[] \| undefined` | — |

- `defaultValue` — The default value of the input. Use when uncontrolled.
- `onChange` — Called with the input's change event, after the field has formatted and stored the new value.
- `onKeyDown` — Called with the input's keydown event.
- `onValueChange` — Callback fired when the `value` changes. Use when controlled.
- `value` — The value of the input. Use when controlled.

## InputPaymentGroup

Renders a `<div>` and takes its props. Pass `render` to render a different element.

## InputPaymentMethodSelector

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| cardIcon | `ReactNode` |
| className | `string \| ((state: TabsRootState) => string \| undefined) \| undefined` |
| defaultValue | `any` |
| onValueChange | `((value: any, eventDetails: TabsRootChangeEventDetails) => void) \| undefined` |
| orientation | `Orientation \| undefined` |
| style | `CSSProperties \| ((state: TabsRootState) => CSSProperties \| undefined) \| undefined` |
| upiIcon | `ReactNode` |
| value | `any` |

- `cardIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `className` — CSS class applied to the element, or a function that returns a class based on the component's state.
- `defaultValue` — The default value. Use when the component is not controlled. When the value is `null`, no Tab will be active.
- `onValueChange` — Callback invoked when new value is being set.
  The event `reason` is `'none'` for user-initiated changes, such as a click or keyboard navigation; `'initial'` for the first automatic selection or fallback in uncontrolled roots when `defaultValue` is omitted or `undefined`, including when the implicit initial value is disabled or missing; `'disabled'` for automatic fallback when the selected tab becomes disabled in uncontrolled roots; or `'missing'` for automatic fallback when the selected tab is removed, or when an explicit `defaultValue` never matches a mounted tab in uncontrolled roots.
  For automatic changes, the selected value can be `null` when no enabled Tab is available as a fallback.
  Automatic changes cannot be canceled; calling `eventDetails.cancel()` for `'initial'`, `'disabled'`, or `'missing'` has no effect.
- `orientation` — The component orientation (layout flow direction).
- `style` — Style applied to the element, or a function that returns a style object based on the component's state.
- `upiIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `value` — The value of the currently active `Tab`. Use when the component is controlled. When the value is `null`, no Tab will be active.

## InputPaymentUpiGroup

Renders a `<div>` and takes its props. Pass `render` to render a different element.

## InputPaymentUpiId

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| className | `string \| undefined` | — |
| defaultValue | `string \| number \| readonly string[] \| undefined` | — |
| onChange | `ChangeEventHandler<HTMLInputElement, Element> \| undefined` | — |
| onKeyDown | `KeyboardEventHandler<HTMLInputElement> \| undefined` | — |
| onValueChange | `((value: string, eventDetails: { reason: "none"; event: Event; cancel: () => void; allowPropagation: () => void; isCanceled: boolean; isPropagationAllowed: boolean; trigger: Element \| undefined; }) => void) \| undefined` | — |
| size | `number \| "sm" \| "default" \| "lg" \| undefined` | `"default"` |
| style | `CSSProperties \| undefined` | — |
| value | `string \| number \| readonly string[] \| undefined` | — |

- `defaultValue` — The default value of the input. Use when uncontrolled.
- `onChange` — Called with the input's change event, after the field has formatted and stored the new value.
- `onKeyDown` — Called with the input's keydown event.
- `onValueChange` — Callback fired when the `value` changes. Use when controlled.
- `value` — The value of the input. Use when controlled.

## InputPaymentUpiProviderIcon

Renders a `<div>` and takes its props. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| icon | `ReactNode` |

- `icon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.

## InputPaymentZip

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type | Default |
| :--- | :--- | :--- |
| className | `string \| undefined` | — |
| defaultValue | `string \| number \| readonly string[] \| undefined` | — |
| onChange | `ChangeEventHandler<HTMLInputElement, Element> \| undefined` | — |
| onKeyDown | `KeyboardEventHandler<HTMLInputElement> \| undefined` | — |
| onValueChange | `((value: string, eventDetails: { reason: "none"; event: Event; cancel: () => void; allowPropagation: () => void; isCanceled: boolean; isPropagationAllowed: boolean; trigger: Element \| undefined; }) => void) \| undefined` | — |
| size | `number \| "sm" \| "default" \| "lg" \| undefined` | `"default"` |
| style | `CSSProperties \| undefined` | — |
| value | `string \| number \| readonly string[] \| undefined` | — |

- `defaultValue` — The default value of the input. Use when uncontrolled.
- `onChange` — Called with the input's change event, after the field has formatted and stored the new value.
- `onKeyDown` — Called with the input's keydown event.
- `onValueChange` — Callback fired when the `value` changes. Use when controlled.
- `value` — The value of the input. Use when controlled.

## PaymentInput

| Prop | Type |
| :--- | :--- |
| autoFocusNext | `boolean \| undefined` |
| cardCvc | `string \| undefined` |
| cardExpiry | `string \| undefined` |
| cardNumber | `string \| undefined` |
| cardZip | `string \| undefined` |
| children | `ReactNode` |
| defaultCardCvc | `string \| undefined` |
| defaultCardExpiry | `string \| undefined` |
| defaultCardNumber | `string \| undefined` |
| defaultCardZip | `string \| undefined` |
| defaultPaymentMethod | `PaymentMethod \| undefined` |
| defaultUpiId | `string \| undefined` |
| disabled | `boolean \| undefined` |
| onCardCvcChange | `((val: string) => void) \| undefined` |
| onCardExpiryChange | `((val: string) => void) \| undefined` |
| onCardNumberChange | `((val: string) => void) \| undefined` |
| onCardZipChange | `((val: string) => void) \| undefined` |
| onPaymentMethodChange | `((method: PaymentMethod) => void) \| undefined` |
| onUpiIdChange | `((val: string) => void) \| undefined` |
| onValidationChange | `((isValid: boolean, errors: PaymentInputErrors) => void) \| undefined` |
| paymentMethod | `PaymentMethod \| undefined` |
| readOnly | `boolean \| undefined` |
| upiId | `string \| undefined` |

- `autoFocusNext` — Whether focus moves to the next field once a field is complete and valid, and back to the previous one on Backspace in an empty field.
- `cardCvc` — The security code. Use with `onCardCvcChange` to control it.
- `cardExpiry` — The expiry date as `MM/YY`. Use with `onCardExpiryChange` to control it.
- `cardNumber` — The card number, spaced in groups as it is shown. Use with `onCardNumberChange` to control it.
- `cardZip` — The postal code. Use with `onCardZipChange` to control it.
- `defaultCardCvc` — The security code at first, when it isn't controlled.
- `defaultCardExpiry` — The expiry date at first, when it isn't controlled.
- `defaultCardNumber` — The card number at first, when it isn't controlled.
- `defaultCardZip` — The postal code at first, when it isn't controlled.
- `defaultPaymentMethod` — The payment method selected at first, when it isn't controlled.
- `defaultUpiId` — The UPI ID at first, when it isn't controlled.
- `onCardCvcChange` — Called with the security code as the user types, cut to the card brand's length.
- `onCardExpiryChange` — Called with the formatted expiry date as the user types.
- `onCardNumberChange` — Called with the formatted card number as the user types.
- `onCardZipChange` — Called with the postal code as the user types.
- `onPaymentMethodChange` — Called with the new method when the user switches between card and UPI.
- `onUpiIdChange` — Called with the UPI ID as the user types.
- `onValidationChange` — Called whenever the details become valid or invalid, with a message for each field that has an error.
- `paymentMethod` — Whether the user is paying by `card` or `upi`. Use with `onPaymentMethodChange` to control it.
- `upiId` — The UPI ID, such as `name@bank`. Use with `onUpiIdChange` to control it.

## PaymentInputBrandIcon

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| icon | `ReactNode` |

- `icon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.

## PaymentInputCardNumber

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| className | `string \| undefined` |
| defaultValue | `string \| number \| readonly string[] \| undefined` |
| onChange | `ChangeEventHandler<HTMLInputElement, Element> \| undefined` |
| onKeyDown | `KeyboardEventHandler<HTMLInputElement> \| undefined` |
| onValueChange | `((value: string, eventDetails: { reason: "none"; event: Event; cancel: () => void; allowPropagation: () => void; isCanceled: boolean; isPropagationAllowed: boolean; trigger: Element \| undefined; }) => void) \| undefined` |
| size | `number \| "sm" \| "default" \| "lg" \| undefined` |
| style | `CSSProperties \| undefined` |
| value | `string \| number \| readonly string[] \| undefined` |

- `defaultValue` — The default value of the input. Use when uncontrolled.
- `onChange` — Called with the input's change event, after the field has formatted and stored the new value.
- `onKeyDown` — Called with the input's keydown event.
- `onValueChange` — Callback fired when the `value` changes. Use when controlled.
- `value` — The value of the input. Use when controlled.

## PaymentInputCVC

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| className | `string \| undefined` |
| defaultValue | `string \| number \| readonly string[] \| undefined` |
| onChange | `ChangeEventHandler<HTMLInputElement, Element> \| undefined` |
| onKeyDown | `KeyboardEventHandler<HTMLInputElement> \| undefined` |
| onValueChange | `((value: string, eventDetails: { reason: "none"; event: Event; cancel: () => void; allowPropagation: () => void; isCanceled: boolean; isPropagationAllowed: boolean; trigger: Element \| undefined; }) => void) \| undefined` |
| size | `number \| "sm" \| "default" \| "lg" \| undefined` |
| style | `CSSProperties \| undefined` |
| value | `string \| number \| readonly string[] \| undefined` |

- `defaultValue` — The default value of the input. Use when uncontrolled.
- `onChange` — Called with the input's change event, after the field has formatted and stored the new value.
- `onKeyDown` — Called with the input's keydown event.
- `onValueChange` — Callback fired when the `value` changes. Use when controlled.
- `value` — The value of the input. Use when controlled.

## PaymentInputExpiry

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| className | `string \| undefined` |
| defaultValue | `string \| number \| readonly string[] \| undefined` |
| onChange | `ChangeEventHandler<HTMLInputElement, Element> \| undefined` |
| onKeyDown | `KeyboardEventHandler<HTMLInputElement> \| undefined` |
| onValueChange | `((value: string, eventDetails: { reason: "none"; event: Event; cancel: () => void; allowPropagation: () => void; isCanceled: boolean; isPropagationAllowed: boolean; trigger: Element \| undefined; }) => void) \| undefined` |
| size | `number \| "sm" \| "default" \| "lg" \| undefined` |
| style | `CSSProperties \| undefined` |
| value | `string \| number \| readonly string[] \| undefined` |

- `defaultValue` — The default value of the input. Use when uncontrolled.
- `onChange` — Called with the input's change event, after the field has formatted and stored the new value.
- `onKeyDown` — Called with the input's keydown event.
- `onValueChange` — Callback fired when the `value` changes. Use when controlled.
- `value` — The value of the input. Use when controlled.

## PaymentInputGroup

Takes the DOM props of the element it renders. Pass `render` to render a different element.

## PaymentInputMethodSelector

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| cardIcon | `ReactNode` |
| className | `string \| ((state: TabsRootState) => string \| undefined) \| undefined` |
| defaultValue | `any` |
| onValueChange | `((value: any, eventDetails: TabsRootChangeEventDetails) => void) \| undefined` |
| orientation | `Orientation \| undefined` |
| style | `CSSProperties \| ((state: TabsRootState) => CSSProperties \| undefined) \| undefined` |
| upiIcon | `ReactNode` |
| value | `any` |

- `cardIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `className` — CSS class applied to the element, or a function that returns a class based on the component's state.
- `defaultValue` — The default value. Use when the component is not controlled. When the value is `null`, no Tab will be active.
- `onValueChange` — Callback invoked when new value is being set.
  The event `reason` is `'none'` for user-initiated changes, such as a click or keyboard navigation; `'initial'` for the first automatic selection or fallback in uncontrolled roots when `defaultValue` is omitted or `undefined`, including when the implicit initial value is disabled or missing; `'disabled'` for automatic fallback when the selected tab becomes disabled in uncontrolled roots; or `'missing'` for automatic fallback when the selected tab is removed, or when an explicit `defaultValue` never matches a mounted tab in uncontrolled roots.
  For automatic changes, the selected value can be `null` when no enabled Tab is available as a fallback.
  Automatic changes cannot be canceled; calling `eventDetails.cancel()` for `'initial'`, `'disabled'`, or `'missing'` has no effect.
- `orientation` — The component orientation (layout flow direction).
- `style` — Style applied to the element, or a function that returns a style object based on the component's state.
- `upiIcon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.
- `value` — The value of the currently active `Tab`. Use when the component is controlled. When the value is `null`, no Tab will be active.

## PaymentInputUpiGroup

Takes the DOM props of the element it renders. Pass `render` to render a different element.

## PaymentInputUpiId

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| className | `string \| undefined` |
| defaultValue | `string \| number \| readonly string[] \| undefined` |
| onChange | `ChangeEventHandler<HTMLInputElement, Element> \| undefined` |
| onKeyDown | `KeyboardEventHandler<HTMLInputElement> \| undefined` |
| onValueChange | `((value: string, eventDetails: { reason: "none"; event: Event; cancel: () => void; allowPropagation: () => void; isCanceled: boolean; isPropagationAllowed: boolean; trigger: Element \| undefined; }) => void) \| undefined` |
| size | `number \| "sm" \| "default" \| "lg" \| undefined` |
| style | `CSSProperties \| undefined` |
| value | `string \| number \| readonly string[] \| undefined` |

- `defaultValue` — The default value of the input. Use when uncontrolled.
- `onChange` — Called with the input's change event, after the field has formatted and stored the new value.
- `onKeyDown` — Called with the input's keydown event.
- `onValueChange` — Callback fired when the `value` changes. Use when controlled.
- `value` — The value of the input. Use when controlled.

## PaymentInputUpiProviderIcon

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| icon | `ReactNode` |

- `icon` — Replaces this icon. Accepts any node; `null` renders no icon. Takes precedence over `IconProvider`.

## PaymentInputZip

Takes the DOM props of the element it renders. Pass `render` to render a different element.

| Prop | Type |
| :--- | :--- |
| className | `string \| undefined` |
| defaultValue | `string \| number \| readonly string[] \| undefined` |
| onChange | `ChangeEventHandler<HTMLInputElement, Element> \| undefined` |
| onKeyDown | `KeyboardEventHandler<HTMLInputElement> \| undefined` |
| onValueChange | `((value: string, eventDetails: { reason: "none"; event: Event; cancel: () => void; allowPropagation: () => void; isCanceled: boolean; isPropagationAllowed: boolean; trigger: Element \| undefined; }) => void) \| undefined` |
| size | `number \| "sm" \| "default" \| "lg" \| undefined` |
| style | `CSSProperties \| undefined` |
| value | `string \| number \| readonly string[] \| undefined` |

- `defaultValue` — The default value of the input. Use when uncontrolled.
- `onChange` — Called with the input's change event, after the field has formatted and stored the new value.
- `onKeyDown` — Called with the input's keydown event.
- `onValueChange` — Callback fired when the `value` changes. Use when controlled.
- `value` — The value of the input. Use when controlled.

## useInputPayment

```tsx
useInputPayment()
```

Returns `{ paymentMethod: PaymentMethod; setPaymentMethod: (method: PaymentMethod) => void; cardNumber: string; cardExpiry: string; cardCvc: string; cardZip: string; upiId: string; brand: CardBrand; cardType: CardTypeConfig; upiProvider: UpiProvider; disabled?: boolean | undefined; readOnly?: boolean | undefined; isInGroup: boolean; autoFocusNext: boolean; isLuhnValid: boolean; errors: PaymentInputErrors; isValid: boolean; cardNumberRef: RefObject<HTMLInputElement | null>; expiryRef: RefObject<HTMLInputElement | null>; cvcRef: RefObject<HTMLInputElement | null>; zipRef: RefObject<HTMLInputElement | null>; upiRef: RefObject<HTMLInputElement | null>; setCardNumber: (val: string) => void; setCardExpiry: (val: string) => void; setCardCvc: (val: string) => void; setCardZip: (val: string) => void; setUpiId: (val: string) => void }`.

## usePaymentInput

```tsx
usePaymentInput()
```

Returns `{ paymentMethod: PaymentMethod; setPaymentMethod: (method: PaymentMethod) => void; cardNumber: string; cardExpiry: string; cardCvc: string; cardZip: string; upiId: string; brand: CardBrand; cardType: CardTypeConfig; upiProvider: UpiProvider; disabled?: boolean | undefined; readOnly?: boolean | undefined; isInGroup: boolean; autoFocusNext: boolean; isLuhnValid: boolean; errors: PaymentInputErrors; isValid: boolean; cardNumberRef: RefObject<HTMLInputElement | null>; expiryRef: RefObject<HTMLInputElement | null>; cvcRef: RefObject<HTMLInputElement | null>; zipRef: RefObject<HTMLInputElement | null>; upiRef: RefObject<HTMLInputElement | null>; setCardNumber: (val: string) => void; setCardExpiry: (val: string) => void; setCardCvc: (val: string) => void; setCardZip: (val: string) => void; setUpiId: (val: string) => void }`.

## usePaymentInputContext

```tsx
usePaymentInputContext()
```

Returns `{ paymentMethod: PaymentMethod; setPaymentMethod: (method: PaymentMethod) => void; cardNumber: string; cardExpiry: string; cardCvc: string; cardZip: string; upiId: string; brand: CardBrand; cardType: CardTypeConfig; upiProvider: UpiProvider; disabled?: boolean | undefined; readOnly?: boolean | undefined; isInGroup: boolean; autoFocusNext: boolean; isLuhnValid: boolean; errors: PaymentInputErrors; isValid: boolean; cardNumberRef: RefObject<HTMLInputElement | null>; expiryRef: RefObject<HTMLInputElement | null>; cvcRef: RefObject<HTMLInputElement | null>; zipRef: RefObject<HTMLInputElement | null>; upiRef: RefObject<HTMLInputElement | null>; setCardNumber: (val: string) => void; setCardExpiry: (val: string) => void; setCardCvc: (val: string) => void; setCardZip: (val: string) => void; setUpiId: (val: string) => void }`.

Required props are bold. Full docs: https://ui.xiod.dev/docs
