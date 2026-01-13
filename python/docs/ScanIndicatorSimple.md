# ScanIndicatorSimple

A fraud indicator in simplified format for public API.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**service** | **str** | Detection service name | 
**type** | **str** | Type of detection | 
**severity** | **str** | Severity level | 
**score** | **float** | Detection score (0-1) | 
**description** | **str** | Human-readable description | 

## Example

```python
from shinjitsu.models.scan_indicator_simple import ScanIndicatorSimple

# TODO update the JSON string below
json = "{}"
# create an instance of ScanIndicatorSimple from a JSON string
scan_indicator_simple_instance = ScanIndicatorSimple.from_json(json)
# print the JSON string representation of the object
print(ScanIndicatorSimple.to_json())

# convert the object into a dict
scan_indicator_simple_dict = scan_indicator_simple_instance.to_dict()
# create an instance of ScanIndicatorSimple from a dict
scan_indicator_simple_from_dict = ScanIndicatorSimple.from_dict(scan_indicator_simple_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


