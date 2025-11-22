
# Status


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`systemName` | string
`description` | string
`priority` | number
`isSystemField` | boolean
`isActive` | boolean
`color` | string
`ignoreResult` | boolean
`enableReportBug` | boolean
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { Status } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "name": Passed,
  "systemName": passed,
  "description": Test case was executed successfully,
  "priority": 1,
  "isSystemField": true,
  "isActive": true,
  "color": #4CAF50,
  "ignoreResult": false,
  "enableReportBug": false,
  "createdAt": 2025-05-28T12:00Z,
  "updatedAt": 2025-05-28T12:30Z,
} satisfies Status

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Status
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


