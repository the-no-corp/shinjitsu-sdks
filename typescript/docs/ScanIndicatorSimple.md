
# ScanIndicatorSimple

A fraud indicator in simplified format for public API.

## Properties

Name | Type
------------ | -------------
`service` | string
`type` | string
`severity` | string
`score` | number
`description` | string

## Example

```typescript
import type { ScanIndicatorSimple } from '@the-no-corp/shinjitsu'

// TODO: Update the object below with actual values
const example = {
  "service": null,
  "type": null,
  "severity": null,
  "score": null,
  "description": null,
} satisfies ScanIndicatorSimple

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ScanIndicatorSimple
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


