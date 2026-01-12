# AnalyzeApi

All URIs are relative to *https://api.the-no-corp.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**analyzeDocumentV1AnalyzePost**](AnalyzeApi.md#analyzedocumentv1analyzepost) | **POST** /v1/analyze | Analyze Document |



## analyzeDocumentV1AnalyzePost

> AnalyzeResponse analyzeDocumentV1AnalyzePost(authorization, file)

Analyze Document

Analyze a document for fraud indicators.  Requires API token authentication via Authorization header: &#x60;&#x60;&#x60; Authorization: Bearer shj_your_api_token_here &#x60;&#x60;&#x60;  Supported file types: - JPEG images (.jpg, .jpeg) - PNG images (.png) - PDF documents (.pdf)

### Example

```ts
import {
  Configuration,
  AnalyzeApi,
} from '@the-no-corp/shinjitsu';
import type { AnalyzeDocumentV1AnalyzePostRequest } from '@the-no-corp/shinjitsu';

async function example() {
  console.log("🚀 Testing @the-no-corp/shinjitsu SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: BearerAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AnalyzeApi(config);

  const body = {
    // string | Bearer token: \'Bearer shj_...\'
    authorization: authorization_example,
    // Blob
    file: BINARY_DATA_HERE,
  } satisfies AnalyzeDocumentV1AnalyzePostRequest;

  try {
    const data = await api.analyzeDocumentV1AnalyzePost(body);
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
| **authorization** | `string` | Bearer token: \&#39;Bearer shj_...\&#39; | [Defaults to `undefined`] |
| **file** | `Blob` |  | [Defaults to `undefined`] |

### Return type

[**AnalyzeResponse**](AnalyzeResponse.md)

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

