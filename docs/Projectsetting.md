
# Projectsetting

For setting_type review, review_groups_enabled is \"1\" to enable saved reviewer groups or \"0\" to disable them (the default). It is configurable only while review is enabled. default_reviewer_group stores an active reviewer group ID from this project as a string; an empty value clears it. It is configurable when review is enabled. With mandatory review, the UI pre-fills this group on add/edit/bulk edit when there is no explicit selection or existing assignment. Individual default settings retain their existing meaning.

## Properties

Name | Type
------------ | -------------
`name` | string
`value` | string
`label` | string
`project` | [ProjectMini](ProjectMini.md)

## Example

```typescript
import type { Projectsetting } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": dateFormat,
  "value": m-d-yy,
  "label": Date format,
  "project": null,
} satisfies Projectsetting

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Projectsetting
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


