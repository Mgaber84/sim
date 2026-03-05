[**simstudio-ts-sdk**](../README.md)

***

[simstudio-ts-sdk](../globals.md) / UsageLimits

# Interface: UsageLimits

Defined in: packages/ts-sdk/src/index.ts:59

## Properties

### rateLimit

> **rateLimit**: `object`

Defined in: packages/ts-sdk/src/index.ts:61

#### async

> **async**: `object`

##### async.isLimited

> **isLimited**: `boolean`

##### async.limit

> **limit**: `number`

##### async.remaining

> **remaining**: `number`

##### async.resetAt

> **resetAt**: `string`

#### authType

> **authType**: `string`

#### sync

> **sync**: `object`

##### sync.isLimited

> **isLimited**: `boolean`

##### sync.limit

> **limit**: `number`

##### sync.remaining

> **remaining**: `number`

##### sync.resetAt

> **resetAt**: `string`

***

### success

> **success**: `boolean`

Defined in: packages/ts-sdk/src/index.ts:60

***

### usage

> **usage**: `object`

Defined in: packages/ts-sdk/src/index.ts:76

#### currentPeriodCost

> **currentPeriodCost**: `number`

#### limit

> **limit**: `number`

#### plan

> **plan**: `string`
