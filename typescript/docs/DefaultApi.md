# DefaultApi

All URIs are relative to *https://api.the-no-corp.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**scanPublicV1ScanPost**](DefaultApi.md#scanpublicv1scanpost) | **POST** /v1/scan | Scan Public |



## scanPublicV1ScanPost

> ScanResult scanPublicV1ScanPost(file)

Scan Public

Scan a document for fraud indicators.  Analyzes the uploaded document (PDF or image) and returns a fraud verdict with supporting indicators. Supports JPEG, PNG images and PDF documents.  **Authentication**: Supports two methods: - Clerk JWT: &#x60;Authorization: Bearer &lt;clerk_jwt&gt;&#x60; - API Token: &#x60;Authorization: Bearer shj_...&#x60;  **Data retention**: Uploaded files are automatically deleted after 24 hours.  Returns: - **scan_id**: Unique identifier for this scan - **verdict**: Overall assessment (clean, suspicious, fraudulent, not_applicable) - **risk_score**: Risk score from 0.0 (clean) to 1.0 (fraud) - **indicators**: List of fraud indicators found - **summary**: Human-readable summary  Returns 403 with SCAN_LIMIT_EXCEEDED if user has reached their limit.

### Example

```ts
import {
  Configuration,
  DefaultApi,
} from '@the-no-corp/shinjitsu';
import type { ScanPublicV1ScanPostRequest } from '@the-no-corp/shinjitsu';

async function example() {
  console.log("🚀 Testing @the-no-corp/shinjitsu SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: BearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DefaultApi(config);

  const body = {
    // Blob | Document to analyze (PDF, JPEG, PNG)
    file: BINARY_DATA_HERE,
  } satisfies ScanPublicV1ScanPostRequest;

  try {
    const data = await api.scanPublicV1ScanPost(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **file** | `Blob` | Document to analyze (PDF, JPEG, PNG) | [Defaults to `undefined`] |

### Return type

[**ScanResult**](ScanResult.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

