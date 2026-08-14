
# Build


## Properties

Name | Type
------------ | -------------
`id` | number
`version` | string
`environment` | string
`releaseDate` | string
`notes` | string
`releaseNotesUrl` | string
`source` | string
`vcsProvider` | string
`ciProvider` | string
`commitSha` | string
`branch` | string
`tag` | string
`repoUrl` | string
`commitUrl` | string
`buildNumber` | string
`buildUrl` | string
`externalRef` | string
`metadata` | { [key: string]: any; }
`release` | [ReleaseMinified](.md)
`releaseManual` | boolean
`project` | number
`createdBy` | [UserMinified](.md)
`createdAt` | string
`updatedAt` | string

## Example

```typescript
import type { Build } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "version": v2.14.1,
  "environment": Production,
  "releaseDate": 2026-06-27,
  "notes": SEPA batch fixes, FX rounding patch, bulk upload limits,
  "releaseNotesUrl": https://wiki.example.com/releases/v2.14.1,
  "source": manual,
  "vcsProvider": azure_devops,
  "ciProvider": azure_devops,
  "commitSha": 9fceb02d,
  "branch": release/2.14,
  "tag": v2.14.1,
  "repoUrl": https://dev.azure.com/acme/payments/_git/payments-backend,
  "commitUrl": https://dev.azure.com/acme/payments/_git/payments-backend/commit/9fceb02d,
  "buildNumber": Release-142,
  "buildUrl": https://dev.azure.com/acme/payments/_release?releaseId=142,
  "externalRef": azure:release:142,
  "metadata": null,
  "release": null,
  "releaseManual": false,
  "project": 1,
  "createdBy": null,
  "createdAt": 2026-06-27T15:04:00.000Z,
  "updatedAt": 2026-06-27T15:04:00.000Z,
} satisfies Build

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Build
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


