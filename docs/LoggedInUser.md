
# LoggedInUser


## Properties

Name | Type
------------ | -------------
`jwt` | string
`mfacode` | string
`user` | [LoggedInUserUser](LoggedInUserUser.md)

## Example

```typescript
import type { LoggedInUser } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "jwt": eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6MSwiaWF0IjoxNTU1Njc3MzY2LCJleHAiOjE1NTgyNjkzNjZ9.oi6-rdVD8Lg5AsHMJ8Qtb85eocOfLkgrZmzb9J8B8Yo,
  "mfacode": null,
  "user": null,
} satisfies LoggedInUser

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as LoggedInUser
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


