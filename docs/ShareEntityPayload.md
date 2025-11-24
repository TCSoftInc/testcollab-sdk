
# ShareEntityPayload


## Properties

Name | Type
------------ | -------------
`company` | number
`project` | number
`entity` | string
`entityId` | number
`expiresIn` | string

## Example

```typescript
import type { ShareEntityPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "company": null,
  "project": null,
  "entity": testplan,
  "entityId": null,
  "expiresIn": null,
} satisfies ShareEntityPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ShareEntityPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


