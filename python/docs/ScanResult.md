# ScanResult

Response from POST /v1/scan - clean public API.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**scan_id** | **str** | Unique scan identifier | 
**verdict** | **str** | Overall fraud assessment: clean, suspicious, fraudulent, not_applicable | 
**risk_score** | **float** | Risk score (0&#x3D;clean, 1&#x3D;fraud) | 
**indicators** | [**List[ScanIndicatorSimple]**](ScanIndicatorSimple.md) | Fraud indicators found | 
**summary** | **str** | Human-readable summary | 
**processing_time_ms** | **int** | Processing time in milliseconds | 
**file_name** | **str** | Original file name | 
**file_type** | **str** | MIME type of uploaded file | 

## Example

```python
from shinjitsu.models.scan_result import ScanResult

# TODO update the JSON string below
json = "{}"
# create an instance of ScanResult from a JSON string
scan_result_instance = ScanResult.from_json(json)
# print the JSON string representation of the object
print(ScanResult.to_json())

# convert the object into a dict
scan_result_dict = scan_result_instance.to_dict()
# create an instance of ScanResult from a dict
scan_result_from_dict = ScanResult.from_dict(scan_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


