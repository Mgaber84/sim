[**simstudio-ts-sdk**](../README.md)

***

[simstudio-ts-sdk](../globals.md) / SimStudioClient

# Class: SimStudioClient

Defined in: packages/ts-sdk/src/index.ts:109

## Constructors

### Constructor

> **new SimStudioClient**(`config`): `SimStudioClient`

Defined in: packages/ts-sdk/src/index.ts:114

#### Parameters

##### config

[`SimStudioConfig`](../interfaces/SimStudioConfig.md)

#### Returns

`SimStudioClient`

## Methods

### executeWithRetry()

> **executeWithRetry**(`workflowId`, `input?`, `options?`, `retryOptions?`): `Promise`\<[`WorkflowExecutionResult`](../interfaces/WorkflowExecutionResult.md) \| [`AsyncExecutionResult`](../interfaces/AsyncExecutionResult.md)\>

Defined in: packages/ts-sdk/src/index.ts:375

Execute workflow with automatic retry on rate limit

#### Parameters

##### workflowId

`string`

The ID of the workflow to execute

##### input?

`any`

Input data to pass to the workflow

##### options?

[`ExecutionOptions`](../interfaces/ExecutionOptions.md) = `{}`

Execution options (timeout, stream, async, etc.)

##### retryOptions?

[`RetryOptions`](../interfaces/RetryOptions.md) = `{}`

Retry configuration (maxRetries, delays, etc.)

#### Returns

`Promise`\<[`WorkflowExecutionResult`](../interfaces/WorkflowExecutionResult.md) \| [`AsyncExecutionResult`](../interfaces/AsyncExecutionResult.md)\>

***

### executeWorkflow()

> **executeWorkflow**(`workflowId`, `input?`, `options?`): `Promise`\<[`WorkflowExecutionResult`](../interfaces/WorkflowExecutionResult.md) \| [`AsyncExecutionResult`](../interfaces/AsyncExecutionResult.md)\>

Defined in: packages/ts-sdk/src/index.ts:174

Execute a workflow with optional input data

#### Parameters

##### workflowId

`string`

The ID of the workflow to execute

##### input?

`any`

Input data to pass to the workflow (object, primitive, or array)

##### options?

[`ExecutionOptions`](../interfaces/ExecutionOptions.md) = `{}`

Execution options (timeout, stream, async, etc.)

#### Returns

`Promise`\<[`WorkflowExecutionResult`](../interfaces/WorkflowExecutionResult.md) \| [`AsyncExecutionResult`](../interfaces/AsyncExecutionResult.md)\>

***

### executeWorkflowSync()

> **executeWorkflowSync**(`workflowId`, `input?`, `options?`): `Promise`\<[`WorkflowExecutionResult`](../interfaces/WorkflowExecutionResult.md)\>

Defined in: packages/ts-sdk/src/index.ts:296

Execute a workflow synchronously (ensures non-async mode)

#### Parameters

##### workflowId

`string`

The ID of the workflow to execute

##### input?

`any`

Input data to pass to the workflow

##### options?

[`ExecutionOptions`](../interfaces/ExecutionOptions.md) = `{}`

Execution options (timeout, stream, etc.)

#### Returns

`Promise`\<[`WorkflowExecutionResult`](../interfaces/WorkflowExecutionResult.md)\>

***

### getJobStatus()

> **getJobStatus**(`taskId`): `Promise`\<`any`\>

Defined in: packages/ts-sdk/src/index.ts:335

Get the status of an async job

#### Parameters

##### taskId

`string`

The task ID returned from async execution

#### Returns

`Promise`\<`any`\>

***

### getRateLimitInfo()

> **getRateLimitInfo**(): [`RateLimitInfo`](../interfaces/RateLimitInfo.md) \| `null`

Defined in: packages/ts-sdk/src/index.ts:424

Get current rate limit information

#### Returns

[`RateLimitInfo`](../interfaces/RateLimitInfo.md) \| `null`

***

### getUsageLimits()

> **getUsageLimits**(): `Promise`\<[`UsageLimits`](../interfaces/UsageLimits.md)\>

Defined in: packages/ts-sdk/src/index.ts:451

Get current usage limits and quota information

#### Returns

`Promise`\<[`UsageLimits`](../interfaces/UsageLimits.md)\>

***

### getWorkflowStatus()

> **getWorkflowStatus**(`workflowId`): `Promise`\<[`WorkflowStatus`](../interfaces/WorkflowStatus.md)\>

Defined in: packages/ts-sdk/src/index.ts:259

Get the status of a workflow (deployment status, etc.)

#### Parameters

##### workflowId

`string`

#### Returns

`Promise`\<[`WorkflowStatus`](../interfaces/WorkflowStatus.md)\>

***

### setApiKey()

> **setApiKey**(`apiKey`): `void`

Defined in: packages/ts-sdk/src/index.ts:320

Set a new API key

#### Parameters

##### apiKey

`string`

#### Returns

`void`

***

### setBaseUrl()

> **setBaseUrl**(`baseUrl`): `void`

Defined in: packages/ts-sdk/src/index.ts:327

Set a new base URL

#### Parameters

##### baseUrl

`string`

#### Returns

`void`

***

### validateWorkflow()

> **validateWorkflow**(`workflowId`): `Promise`\<`boolean`\>

Defined in: packages/ts-sdk/src/index.ts:308

Validate that a workflow is ready for execution

#### Parameters

##### workflowId

`string`

#### Returns

`Promise`\<`boolean`\>
