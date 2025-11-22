
# Upload


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`hash` | string
`ext` | string
`mime` | string
`size` | string
`url` | string
`provider` | string
`createdBy` | number
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { Upload } from 'testcollab-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "name": myfile.jpg,
  "hash": aa1d5608cc8347ebba775ac11dda00be,
  "ext": .jpg,
  "mime": image/jpeg,
  "size": 201.2,
  "url": https://loremflickr.com/640/360,
  "provider": mock,
  "createdBy": 3,
  "createdAt": 2019-04-30T17:11:24.000Z,
  "updatedAt": 2019-04-30T17:11:24.000Z,
} satisfies Upload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Upload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


