
# VideoPlayback


## Properties

Name | Type
------------ | -------------
`url` | string
`expiresAt` | Date
`contentType` | string

## Example

```typescript
import type { VideoPlayback } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "url": null,
  "expiresAt": null,
  "contentType": video/webm,
} satisfies VideoPlayback

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as VideoPlayback
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


