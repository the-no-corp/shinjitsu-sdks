# \DefaultAPI

All URIs are relative to *https://api.the-no-corp.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ScanPublicV1ScanPost**](DefaultAPI.md#ScanPublicV1ScanPost) | **Post** /v1/scan | Scan Public



## ScanPublicV1ScanPost

> ScanResult ScanPublicV1ScanPost(ctx).File(file).Execute()

Scan Public



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
	file := os.NewFile(1234, "some_file") // *os.File | Document to analyze (PDF, JPEG, PNG)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DefaultAPI.ScanPublicV1ScanPost(context.Background()).File(file).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DefaultAPI.ScanPublicV1ScanPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ScanPublicV1ScanPost`: ScanResult
	fmt.Fprintf(os.Stdout, "Response from `DefaultAPI.ScanPublicV1ScanPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiScanPublicV1ScanPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **file** | ***os.File** | Document to analyze (PDF, JPEG, PNG) | 

### Return type

[**ScanResult**](ScanResult.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

