# SrcControllersV1DemoFraudIndicator

A single fraud detection indicator.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**service** | **str** |  | 
**type** | **str** |  | 
**severity** | **str** |  | 
**score** | **float** |  | 
**description** | **str** |  | 

## Example

```python
from shinjitsu.models.src_controllers_v1_demo_fraud_indicator import SrcControllersV1DemoFraudIndicator

# TODO update the JSON string below
json = "{}"
# create an instance of SrcControllersV1DemoFraudIndicator from a JSON string
src_controllers_v1_demo_fraud_indicator_instance = SrcControllersV1DemoFraudIndicator.from_json(json)
# print the JSON string representation of the object
print(SrcControllersV1DemoFraudIndicator.to_json())

# convert the object into a dict
src_controllers_v1_demo_fraud_indicator_dict = src_controllers_v1_demo_fraud_indicator_instance.to_dict()
# create an instance of SrcControllersV1DemoFraudIndicator from a dict
src_controllers_v1_demo_fraud_indicator_from_dict = SrcControllersV1DemoFraudIndicator.from_dict(src_controllers_v1_demo_fraud_indicator_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


