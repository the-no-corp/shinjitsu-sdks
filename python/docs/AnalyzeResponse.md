# AnalyzeResponse

Response from document analysis.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**scan_id** | **str** |  | 
**risk_score** | **float** |  | 
**verdict** | **str** |  | 
**indicators** | [**List[SrcControllersV1DemoFraudIndicator]**](SrcControllersV1DemoFraudIndicator.md) |  | 
**summary** | **str** |  | 
**processing_time_ms** | **int** |  | 
**file_name** | **str** |  | 
**file_type** | **str** |  | 

## Example

```python
from shinjitsu.models.analyze_response import AnalyzeResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyzeResponse from a JSON string
analyze_response_instance = AnalyzeResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyzeResponse.to_json())

# convert the object into a dict
analyze_response_dict = analyze_response_instance.to_dict()
# create an instance of AnalyzeResponse from a dict
analyze_response_from_dict = AnalyzeResponse.from_dict(analyze_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


