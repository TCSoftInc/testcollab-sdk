
# AppManagerTestPayload


## Properties

Name | Type
------------ | -------------
`title` | string
`entity` | string
`entityId` | number
`entityTitle` | string
`activityType` | string
`appManager` | string
`company` | number
`_configuration` | string

## Example

```typescript
import type { AppManagerTestPayload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "title": null,
  "entity": null,
  "entityId": null,
  "entityTitle": null,
  "activityType": null,
  "appManager": null,
  "company": null,
  "_configuration": {},
} satisfies AppManagerTestPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AppManagerTestPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


