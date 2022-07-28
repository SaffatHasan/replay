[@puppeteer/replay](../README.md) / StepWithFrame

# Interface: StepWithFrame

## Hierarchy

- [`StepWithTarget`](Schema.StepWithTarget.md)

  ↳ **`StepWithFrame`**

## Table of contents

### Properties

- [assertedEvents](StepWithFrame.md#assertedevents)
- [frame](StepWithFrame.md#frame)
- [target](StepWithFrame.md#target)
- [timeout](StepWithFrame.md#timeout)
- [type](StepWithFrame.md#type)

## Properties

### assertedEvents

• `Optional` **assertedEvents**: [`NavigationEvent`](Schema.NavigationEvent.md)[]

#### Inherited from

[StepWithTarget](Schema.StepWithTarget.md).[assertedEvents](Schema.StepWithTarget.md#assertedevents)

#### Defined in

[Schema.ts:33](https://github.com/puppeteer/replay/blob/main/src/Schema.ts#L33)

---

### frame

• `Optional` **frame**: [`FrameSelector`](../modules/Schema.md#frameselector)

Defaults to main frame

#### Defined in

[Schema.ts:47](https://github.com/puppeteer/replay/blob/main/src/Schema.ts#L47)

---

### target

• `Optional` **target**: `string`

Defaults to main

#### Inherited from

[StepWithTarget](Schema.StepWithTarget.md).[target](Schema.StepWithTarget.md#target)

#### Defined in

[Schema.ts:40](https://github.com/puppeteer/replay/blob/main/src/Schema.ts#L40)

---

### timeout

• `Optional` **timeout**: `number`

#### Inherited from

[StepWithTarget](Schema.StepWithTarget.md).[timeout](Schema.StepWithTarget.md#timeout)

#### Defined in

[Schema.ts:32](https://github.com/puppeteer/replay/blob/main/src/Schema.ts#L32)

---

### type

• **type**: `string`

#### Inherited from

[StepWithTarget](Schema.StepWithTarget.md).[type](Schema.StepWithTarget.md#type)

#### Defined in

[Schema.ts:31](https://github.com/puppeteer/replay/blob/main/src/Schema.ts#L31)
