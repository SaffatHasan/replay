[@puppeteer/replay](../README.md) / ChangeStep

# Interface: ChangeStep

## Hierarchy

- [`StepWithSelectors`](Schema.StepWithSelectors.md)

  ↳ **`ChangeStep`**

## Table of contents

### Properties

- [assertedEvents](ChangeStep.md#assertedevents)
- [frame](ChangeStep.md#frame)
- [selectors](ChangeStep.md#selectors)
- [target](ChangeStep.md#target)
- [timeout](ChangeStep.md#timeout)
- [type](ChangeStep.md#type)
- [value](ChangeStep.md#value)

## Properties

### assertedEvents

• `Optional` **assertedEvents**: [`NavigationEvent`](Schema.NavigationEvent.md)[]

#### Inherited from

[StepWithSelectors](Schema.StepWithSelectors.md).[assertedEvents](Schema.StepWithSelectors.md#assertedevents)

#### Defined in

[Schema.ts:33](https://github.com/puppeteer/replay/blob/main/src/Schema.ts#L33)

---

### frame

• `Optional` **frame**: [`FrameSelector`](../modules/Schema.md#frameselector)

Defaults to main frame

#### Inherited from

[StepWithSelectors](Schema.StepWithSelectors.md).[frame](Schema.StepWithSelectors.md#frame)

#### Defined in

[Schema.ts:47](https://github.com/puppeteer/replay/blob/main/src/Schema.ts#L47)

---

### selectors

• **selectors**: [`Selector`](../modules/Schema.md#selector)[]

A list of alternative selectors that lead to selection of a single element to perform the step on.
Currently, we support CSS selectors and ARIA selectors (start with 'aria/'). Each selector
could be a string or an array of strings. If it's a string, it means that the selector points directly to the target
element. If it's an array, the last element is the selector for the target element and the preceeding selectors
point to the ancestor elements. If the parent element is a shadow root host, the subsequent
selector is evaluated only against the shadow DOM of the host (i.e., `parent.shadowRoot.querySelector`). If the parent
element is not a shadow root host, the subsequent selector is evaluated in the regular DOM (i.e., `parent.querySelector`).

During the execution, it's recommended that the implementation tries out all of the alternative selectors to improve
reliability of the replay as some selectors might get outdated over time.

#### Inherited from

[StepWithSelectors](Schema.StepWithSelectors.md).[selectors](Schema.StepWithSelectors.md#selectors)

#### Defined in

[Schema.ts:63](https://github.com/puppeteer/replay/blob/main/src/Schema.ts#L63)

---

### target

• `Optional` **target**: `string`

Defaults to main

#### Inherited from

[StepWithSelectors](Schema.StepWithSelectors.md).[target](Schema.StepWithSelectors.md#target)

#### Defined in

[Schema.ts:40](https://github.com/puppeteer/replay/blob/main/src/Schema.ts#L40)

---

### timeout

• `Optional` **timeout**: `number`

#### Inherited from

[StepWithSelectors](Schema.StepWithSelectors.md).[timeout](Schema.StepWithSelectors.md#timeout)

#### Defined in

[Schema.ts:32](https://github.com/puppeteer/replay/blob/main/src/Schema.ts#L32)

---

### type

• **type**: `"change"`

#### Overrides

[StepWithSelectors](Schema.StepWithSelectors.md).[type](Schema.StepWithSelectors.md#type)

#### Defined in

[Schema.ts:113](https://github.com/puppeteer/replay/blob/main/src/Schema.ts#L113)

---

### value

• **value**: `string`

#### Defined in

[Schema.ts:114](https://github.com/puppeteer/replay/blob/main/src/Schema.ts#L114)
