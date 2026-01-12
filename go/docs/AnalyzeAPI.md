# \AnalyzeAPI

All URIs are relative to *https://api.the-no-corp.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AnalyzeDocumentV1AnalyzePost**](AnalyzeAPI.md#AnalyzeDocumentV1AnalyzePost) | **Post** /v1/analyze | Analyze Document



## AnalyzeDocumentV1AnalyzePost

> AnalyzeResponse AnalyzeDocumentV1AnalyzePost(ctx).Authorization(authorization).File(file).Execute()

Analyze Document



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	authorization := "authorization_example" // string | Bearer token: 'Bearer shj_...'
	file := os.NewFile(1234, "some_file") // *os.File | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AnalyzeAPI.AnalyzeDocumentV1AnalyzePost(context.Background()).Authorization(authorization).File(file).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AnalyzeAPI.AnalyzeDocumentV1AnalyzePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AnalyzeDocumentV1AnalyzePost`: AnalyzeResponse
	fmt.Fprintf(os.Stdout, "Response from `AnalyzeAPI.AnalyzeDocumentV1AnalyzePost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAnalyzeDocumentV1AnalyzePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string** | Bearer token: &#39;Bearer shj_...&#39; | 
 **file** | ***os.File** |  | 

### Return type

[**AnalyzeResponse**](AnalyzeResponse.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

