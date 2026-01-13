
# ScanResult

Response from POST /v1/scan - clean public API.

## Properties

Name | Type
------------ | -------------
`scanId` | string
`verdict` | string
`riskScore` | number
`indicators` | [Array&lt;ScanIndicatorSimple&gt;](ScanIndicatorSimple.md)
`summary` | string
`processingTimeMs` | number
`fileName` | string
`fileType` | string

## Example

```typescript
import type { ScanResult } from '@the-no-corp/shinjitsu'

// TODO: Update the object below with actual values
const example = {
  "scanId": null,
  "verdict": null,
  "riskScore": null,
  "indicators": null,
  "summary": null,
  "processingTimeMs": null,
  "fileName": null,
  "fileType": null,
} satisfies ScanResult

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ScanResult
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


