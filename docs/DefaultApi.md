# inokufu_encoder_client.DefaultApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**encode_encode_post**](DefaultApi.md#encode_encode_post) | **POST** /encode | Encode


# **encode_encode_post**
> List[ResponseModel] encode_encode_post(query_model)

Encode

Encode a list of maximum 25 queries and return the corresponding vectors

### Example

```python
import time
import os
import inokufu_encoder_client
from inokufu_encoder_client.models.query_model import QueryModel
from inokufu_encoder_client.models.response_model import ResponseModel
from inokufu_encoder_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = inokufu_encoder_client.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with inokufu_encoder_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = inokufu_encoder_client.DefaultApi(api_client)
    query_model = [inokufu_encoder_client.QueryModel()] # List[QueryModel] | 

    try:
        # Encode
        api_response = api_instance.encode_encode_post(query_model)
        print("The response of DefaultApi->encode_encode_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->encode_encode_post: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query_model** | [**List[QueryModel]**](QueryModel.md)|  | 

### Return type

[**List[ResponseModel]**](ResponseModel.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

