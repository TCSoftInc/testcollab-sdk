
# TestPlanComment


## Properties

Name | Type
------------ | -------------
`id` | number
`project` | number
`testPlan` | number
`mentions` | [Array&lt;User&gt;](User.md)
`parentId` | number
`comment` | string
`createdBy` | [UserMinified](.md)
`createdAt` | string

## Example

```typescript
import type { TestPlanComment } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": 1,
  "project": 1,
  "testPlan": 1,
  "mentions": [{"id":1,"name":"Jessica Smith","email":"jess@smith.com","avatar":"https://i.pravatar.cc/300","last_active":"2019-06-10T09:12:33.001Z","rank":"Administrator","username":"shritig","projects":[{"id":1,"user":10,"project":1,"role":1}]},{"id":2,"name":"Ron Stewart","email":"ron@stew.com","avatar":"https://i.pravatar.cc/300","last_active":"2019-06-10T09:12:33.001Z","rank":"User","username":"ron","projects":[{"id":1,"user":20,"project":1,"role":1}]}],
  "parentId": 0,
  "comment": This is a comment,
  "createdBy": null,
  "createdAt": 2019-04-30T17:11:24.000Z,
} satisfies TestPlanComment

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TestPlanComment
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


