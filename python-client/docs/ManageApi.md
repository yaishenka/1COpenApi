# swagger_client.ManageApi

All URIs are relative to *http://localhost:8000/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**manage_create**](ManageApi.md#manage_create) | **POST** /manage | 
[**manage_list**](ManageApi.md#manage_list) | **GET** /manage | 


# **manage_create**
> Url manage_create(data)





### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure HTTP basic authorization: Basic
configuration = swagger_client.Configuration()
configuration.username = 'YOUR_USERNAME'
configuration.password = 'YOUR_PASSWORD'

# create an instance of the API class
api_instance = swagger_client.ManageApi(swagger_client.ApiClient(configuration))
data = swagger_client.Url() # Url | 

try:
    api_response = api_instance.manage_create(data)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling ManageApi->manage_create: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Url**](Url.md)|  | 

### Return type

[**Url**](Url.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **manage_list**
> list[Url] manage_list()





### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure HTTP basic authorization: Basic
configuration = swagger_client.Configuration()
configuration.username = 'YOUR_USERNAME'
configuration.password = 'YOUR_PASSWORD'

# create an instance of the API class
api_instance = swagger_client.ManageApi(swagger_client.ApiClient(configuration))

try:
    api_response = api_instance.manage_list()
    pprint(api_response)
except ApiException as e:
    print("Exception when calling ManageApi->manage_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[Url]**](Url.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

