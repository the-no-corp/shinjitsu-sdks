# ScanIndicatorSimple

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Service** | **string** | Detection service name | 
**Type** | **string** | Type of detection | 
**Severity** | **string** | Severity level | 
**Score** | **float32** | Detection score (0-1) | 
**Description** | **string** | Human-readable description | 

## Methods

### NewScanIndicatorSimple

`func NewScanIndicatorSimple(service string, type_ string, severity string, score float32, description string, ) *ScanIndicatorSimple`

NewScanIndicatorSimple instantiates a new ScanIndicatorSimple object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScanIndicatorSimpleWithDefaults

`func NewScanIndicatorSimpleWithDefaults() *ScanIndicatorSimple`

NewScanIndicatorSimpleWithDefaults instantiates a new ScanIndicatorSimple object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetService

`func (o *ScanIndicatorSimple) GetService() string`

GetService returns the Service field if non-nil, zero value otherwise.

### GetServiceOk

`func (o *ScanIndicatorSimple) GetServiceOk() (*string, bool)`

GetServiceOk returns a tuple with the Service field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetService

`func (o *ScanIndicatorSimple) SetService(v string)`

SetService sets Service field to given value.


### GetType

`func (o *ScanIndicatorSimple) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ScanIndicatorSimple) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ScanIndicatorSimple) SetType(v string)`

SetType sets Type field to given value.


### GetSeverity

`func (o *ScanIndicatorSimple) GetSeverity() string`

GetSeverity returns the Severity field if non-nil, zero value otherwise.

### GetSeverityOk

`func (o *ScanIndicatorSimple) GetSeverityOk() (*string, bool)`

GetSeverityOk returns a tuple with the Severity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeverity

`func (o *ScanIndicatorSimple) SetSeverity(v string)`

SetSeverity sets Severity field to given value.


### GetScore

`func (o *ScanIndicatorSimple) GetScore() float32`

GetScore returns the Score field if non-nil, zero value otherwise.

### GetScoreOk

`func (o *ScanIndicatorSimple) GetScoreOk() (*float32, bool)`

GetScoreOk returns a tuple with the Score field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScore

`func (o *ScanIndicatorSimple) SetScore(v float32)`

SetScore sets Score field to given value.


### GetDescription

`func (o *ScanIndicatorSimple) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ScanIndicatorSimple) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ScanIndicatorSimple) SetDescription(v string)`

SetDescription sets Description field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


