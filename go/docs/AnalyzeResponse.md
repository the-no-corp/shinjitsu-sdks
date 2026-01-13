# AnalyzeResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ScanId** | **string** |  | 
**RiskScore** | **float32** |  | 
**Verdict** | **string** |  | 
**Indicators** | [**[]SrcControllersV1AnalyzeFraudIndicator**](SrcControllersV1AnalyzeFraudIndicator.md) |  | 
**Summary** | **string** |  | 
**ProcessingTimeMs** | **int32** |  | 
**FileName** | **string** |  | 
**FileType** | **string** |  | 

## Methods

### NewAnalyzeResponse

`func NewAnalyzeResponse(scanId string, riskScore float32, verdict string, indicators []SrcControllersV1AnalyzeFraudIndicator, summary string, processingTimeMs int32, fileName string, fileType string, ) *AnalyzeResponse`

NewAnalyzeResponse instantiates a new AnalyzeResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAnalyzeResponseWithDefaults

`func NewAnalyzeResponseWithDefaults() *AnalyzeResponse`

NewAnalyzeResponseWithDefaults instantiates a new AnalyzeResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetScanId

`func (o *AnalyzeResponse) GetScanId() string`

GetScanId returns the ScanId field if non-nil, zero value otherwise.

### GetScanIdOk

`func (o *AnalyzeResponse) GetScanIdOk() (*string, bool)`

GetScanIdOk returns a tuple with the ScanId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanId

`func (o *AnalyzeResponse) SetScanId(v string)`

SetScanId sets ScanId field to given value.


### GetRiskScore

`func (o *AnalyzeResponse) GetRiskScore() float32`

GetRiskScore returns the RiskScore field if non-nil, zero value otherwise.

### GetRiskScoreOk

`func (o *AnalyzeResponse) GetRiskScoreOk() (*float32, bool)`

GetRiskScoreOk returns a tuple with the RiskScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRiskScore

`func (o *AnalyzeResponse) SetRiskScore(v float32)`

SetRiskScore sets RiskScore field to given value.


### GetVerdict

`func (o *AnalyzeResponse) GetVerdict() string`

GetVerdict returns the Verdict field if non-nil, zero value otherwise.

### GetVerdictOk

`func (o *AnalyzeResponse) GetVerdictOk() (*string, bool)`

GetVerdictOk returns a tuple with the Verdict field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVerdict

`func (o *AnalyzeResponse) SetVerdict(v string)`

SetVerdict sets Verdict field to given value.


### GetIndicators

`func (o *AnalyzeResponse) GetIndicators() []SrcControllersV1AnalyzeFraudIndicator`

GetIndicators returns the Indicators field if non-nil, zero value otherwise.

### GetIndicatorsOk

`func (o *AnalyzeResponse) GetIndicatorsOk() (*[]SrcControllersV1AnalyzeFraudIndicator, bool)`

GetIndicatorsOk returns a tuple with the Indicators field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIndicators

`func (o *AnalyzeResponse) SetIndicators(v []SrcControllersV1AnalyzeFraudIndicator)`

SetIndicators sets Indicators field to given value.


### GetSummary

`func (o *AnalyzeResponse) GetSummary() string`

GetSummary returns the Summary field if non-nil, zero value otherwise.

### GetSummaryOk

`func (o *AnalyzeResponse) GetSummaryOk() (*string, bool)`

GetSummaryOk returns a tuple with the Summary field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSummary

`func (o *AnalyzeResponse) SetSummary(v string)`

SetSummary sets Summary field to given value.


### GetProcessingTimeMs

`func (o *AnalyzeResponse) GetProcessingTimeMs() int32`

GetProcessingTimeMs returns the ProcessingTimeMs field if non-nil, zero value otherwise.

### GetProcessingTimeMsOk

`func (o *AnalyzeResponse) GetProcessingTimeMsOk() (*int32, bool)`

GetProcessingTimeMsOk returns a tuple with the ProcessingTimeMs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProcessingTimeMs

`func (o *AnalyzeResponse) SetProcessingTimeMs(v int32)`

SetProcessingTimeMs sets ProcessingTimeMs field to given value.


### GetFileName

`func (o *AnalyzeResponse) GetFileName() string`

GetFileName returns the FileName field if non-nil, zero value otherwise.

### GetFileNameOk

`func (o *AnalyzeResponse) GetFileNameOk() (*string, bool)`

GetFileNameOk returns a tuple with the FileName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileName

`func (o *AnalyzeResponse) SetFileName(v string)`

SetFileName sets FileName field to given value.


### GetFileType

`func (o *AnalyzeResponse) GetFileType() string`

GetFileType returns the FileType field if non-nil, zero value otherwise.

### GetFileTypeOk

`func (o *AnalyzeResponse) GetFileTypeOk() (*string, bool)`

GetFileTypeOk returns a tuple with the FileType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileType

`func (o *AnalyzeResponse) SetFileType(v string)`

SetFileType sets FileType field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


