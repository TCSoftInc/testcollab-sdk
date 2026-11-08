
# Changelog


## Properties

Name | Type
------------ | -------------
`available` | boolean
`entries` | [Array&lt;ChangelogEntry&gt;](ChangelogEntry.md)
`readEntries` | Array&lt;string&gt;

## Example

```typescript
import type { Changelog } from '@testcollab/sdk'

// TODO: Update the object below with actual values
const example = {
  "available": true,
  "entries": null,
  "readEntries": ["2026-11-06-risk-based-testing-on-elite"],
} satisfies Changelog

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Changelog
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


