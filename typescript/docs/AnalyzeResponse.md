
# AnalyzeResponse

Response from document analysis.

## Properties

Name | Type
------------ | -------------
`scanId` | string
`riskScore` | number
`verdict` | string
`indicators` | [Array&lt;SrcControllersV1AnalyzeFraudIndicator&gt;](SrcControllersV1AnalyzeFraudIndicator.md)
`summary` | string
`processingTimeMs` | number
`fileName` | string
`fileType` | string

## Example

```typescript
import type { AnalyzeResponse } from '@the-no-corp/shinjitsu'

// TODO: Update the object below with actual values
const example = {
  "scanId": null,
  "riskScore": null,
  "verdict": null,
  "indicators": null,
  "summary": null,
  "processingTimeMs": null,
  "fileName": null,
  "fileType": null,
} satisfies AnalyzeResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AnalyzeResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


