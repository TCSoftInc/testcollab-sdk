
# SendVerificationPayload


## Properties

Name | Type
------------ | -------------
`email` | string
`entry` | string
`utmCampaign` | string
`turnstileToken` | string

## Example

```typescript
import type { SendVerificationPayload } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "email": dnyanesh@gigapromoters.com,
  "entry": ai-test-case-generation,
  "utmCampaign": spring-ppc,
  "turnstileToken": 0.zrSnRHO7h0HwSjSCU8oyzbjEtD8p.d62306d4ee00c77dda697f959ebbd7bd97,
} satisfies SendVerificationPayload

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SendVerificationPayload
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


