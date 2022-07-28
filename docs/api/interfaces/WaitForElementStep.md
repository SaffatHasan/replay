[@puppeteer/replay](../README.md) / WaitForElementStep

# Interface: WaitForElementStep

`waitForElement` allows waiting for the presence (or absence) of the number
of elements identified by the selector.

For example, the following step would wait for less than three elements
to be on the page that match the selector `.my-class`.

```
{
  "type": "waitForElement",
  "selectors": [".my-class"],
  "operator": "<=",
  "count": 2,
}
```

## Hierarchy

- [`StepWithSelectors`](Schema.StepWithSelectors.md)

  ↳ **`WaitForElementStep`**

## Table of contents

### Properties

- [assertedEvents](WaitForElementStep.md#assertedevents)
- [count](WaitForElementStep.md#count)
- [frame](WaitForElementStep.md#frame)
- [operator](WaitForElementStep.md#operator)
- [selectors](WaitForElementStep.md#selectors)
- [target](WaitForElementStep.md#target)
- [timeout](WaitForElementStep.md#timeout)
- [type](WaitForElementStep.md#type)

## Properties

### assertedEvents

• `Optional` **assertedEvents**: [`NavigationEvent`](Schema.NavigationEvent.md)[]

#### Inherited from

[StepWithSelectors](Schema.StepWithSelectors.md).[assertedEvents](Schema.StepWithSelectors.md#assertedevents)

#### Defined in

[Schema.ts:33](https://github.com/puppeteer/replay/blob/main/src/Schema.ts#L33)

---

### count

• `Optional` **count**: `number`

Defaults to 1

#### Defined in

[Schema.ts:218](https://github.com/puppeteer/replay/blob/main/src/Schema.ts#L218)

---

### frame

• `Optional` **frame**: [`FrameSelector`](../modules/Schema.md#frameselector)

Defaults to main frame

#### Inherited from

[StepWithSelectors](Schema.StepWithSelectors.md).[frame](Schema.StepWithSelectors.md#frame)

#### Defined in

[Schema.ts:47](https://github.com/puppeteer/replay/blob/main/src/Schema.ts#L47)

---

### operator

• `Optional` **operator**: `">="` \| `"=="` \| `"<="`

Defaults to '=='

#### Defined in

[Schema.ts:214](https://github.com/puppeteer/replay/blob/main/src/Schema.ts#L214)

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

• **type**: `"waitForElement"`

#### Overrides

[StepWithSelectors](Schema.StepWithSelectors.md).[type](Schema.StepWithSelectors.md#type)

#### Defined in

[Schema.ts:210](https://github.com/puppeteer/replay/blob/main/src/Schema.ts#L210)
