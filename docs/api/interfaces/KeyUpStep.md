[@puppeteer/replay](../README.md) / KeyUpStep

# Interface: KeyUpStep

## Hierarchy

- [`StepWithTarget`](Schema.StepWithTarget.md)

  ↳ **`KeyUpStep`**

## Table of contents

### Properties

- [assertedEvents](KeyUpStep.md#assertedevents)
- [key](KeyUpStep.md#key)
- [target](KeyUpStep.md#target)
- [timeout](KeyUpStep.md#timeout)
- [type](KeyUpStep.md#type)

## Properties

### assertedEvents

• `Optional` **assertedEvents**: [`NavigationEvent`](Schema.NavigationEvent.md)[]

#### Inherited from

[StepWithTarget](Schema.StepWithTarget.md).[assertedEvents](Schema.StepWithTarget.md#assertedevents)

#### Defined in

[Schema.ts:33](https://github.com/puppeteer/replay/blob/main/src/Schema.ts#L33)

---

### key

• **key**: [`Key`](../modules/Schema.md#key)

#### Defined in

[Schema.ts:131](https://github.com/puppeteer/replay/blob/main/src/Schema.ts#L131)

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

• **type**: `"keyUp"`

#### Overrides

[StepWithTarget](Schema.StepWithTarget.md).[type](Schema.StepWithTarget.md#type)

#### Defined in

[Schema.ts:130](https://github.com/puppeteer/replay/blob/main/src/Schema.ts#L130)
