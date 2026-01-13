# ScanResult

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ScanId** | **string** | Unique scan identifier | 
**Verdict** | **string** | Overall fraud assessment: clean, suspicious, fraudulent, not_applicable | 
**RiskScore** | **float32** | Risk score (0&#x3D;clean, 1&#x3D;fraud) | 
**Indicators** | [**[]ScanIndicatorSimple**](ScanIndicatorSimple.md) | Fraud indicators found | 
**Summary** | **string** | Human-readable summary | 
**ProcessingTimeMs** | **int32** | Processing time in milliseconds | 
**FileName** | **string** | Original file name | 
**FileType** | **string** | MIME type of uploaded file | 

## Methods

### NewScanResult

`func NewScanResult(scanId string, verdict string, riskScore float32, indicators []ScanIndicatorSimple, summary string, processingTimeMs int32, fileName string, fileType string, ) *ScanResult`

NewScanResult instantiates a new ScanResult object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScanResultWithDefaults

`func NewScanResultWithDefaults() *ScanResult`

NewScanResultWithDefaults instantiates a new ScanResult object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetScanId

`func (o *ScanResult) GetScanId() string`

GetScanId returns the ScanId field if non-nil, zero value otherwise.

### GetScanIdOk

`func (o *ScanResult) GetScanIdOk() (*string, bool)`

GetScanIdOk returns a tuple with the ScanId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScanId

`func (o *ScanResult) SetScanId(v string)`

SetScanId sets ScanId field to given value.


### GetVerdict

`func (o *ScanResult) GetVerdict() string`

GetVerdict returns the Verdict field if non-nil, zero value otherwise.

### GetVerdictOk

`func (o *ScanResult) GetVerdictOk() (*string, bool)`

GetVerdictOk returns a tuple with the Verdict field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVerdict

`func (o *ScanResult) SetVerdict(v string)`

SetVerdict sets Verdict field to given value.


### GetRiskScore

`func (o *ScanResult) GetRiskScore() float32`

GetRiskScore returns the RiskScore field if non-nil, zero value otherwise.

### GetRiskScoreOk

`func (o *ScanResult) GetRiskScoreOk() (*float32, bool)`

GetRiskScoreOk returns a tuple with the RiskScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRiskScore

`func (o *ScanResult) SetRiskScore(v float32)`

SetRiskScore sets RiskScore field to given value.


### GetIndicators

`func (o *ScanResult) GetIndicators() []ScanIndicatorSimple`

GetIndicators returns the Indicators field if non-nil, zero value otherwise.

### GetIndicatorsOk

`func (o *ScanResult) GetIndicatorsOk() (*[]ScanIndicatorSimple, bool)`

GetIndicatorsOk returns a tuple with the Indicators field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIndicators

`func (o *ScanResult) SetIndicators(v []ScanIndicatorSimple)`

SetIndicators sets Indicators field to given value.


### GetSummary

`func (o *ScanResult) GetSummary() string`

GetSummary returns the Summary field if non-nil, zero value otherwise.

### GetSummaryOk

`func (o *ScanResult) GetSummaryOk() (*string, bool)`

GetSummaryOk returns a tuple with the Summary field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSummary

`func (o *ScanResult) SetSummary(v string)`

SetSummary sets Summary field to given value.


### GetProcessingTimeMs

`func (o *ScanResult) GetProcessingTimeMs() int32`

GetProcessingTimeMs returns the ProcessingTimeMs field if non-nil, zero value otherwise.

### GetProcessingTimeMsOk

`func (o *ScanResult) GetProcessingTimeMsOk() (*int32, bool)`

GetProcessingTimeMsOk returns a tuple with the ProcessingTimeMs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProcessingTimeMs

`func (o *ScanResult) SetProcessingTimeMs(v int32)`

SetProcessingTimeMs sets ProcessingTimeMs field to given value.


### GetFileName

`func (o *ScanResult) GetFileName() string`

GetFileName returns the FileName field if non-nil, zero value otherwise.

### GetFileNameOk

`func (o *ScanResult) GetFileNameOk() (*string, bool)`

GetFileNameOk returns a tuple with the FileName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileName

`func (o *ScanResult) SetFileName(v string)`

SetFileName sets FileName field to given value.


### GetFileType

`func (o *ScanResult) GetFileType() string`

GetFileType returns the FileType field if non-nil, zero value otherwise.

### GetFileTypeOk

`func (o *ScanResult) GetFileTypeOk() (*string, bool)`

GetFileTypeOk returns a tuple with the FileType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileType

`func (o *ScanResult) SetFileType(v string)`

SetFileType sets FileType field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


