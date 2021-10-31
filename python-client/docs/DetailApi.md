# swagger_client.DetailApi

All URIs are relative to *http://localhost:8000/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**detail_delete**](DetailApi.md#detail_delete) | **DELETE** /detail/{short_url}/ | 
[**detail_partial_update**](DetailApi.md#detail_partial_update) | **PATCH** /detail/{short_url}/ | 
[**detail_read**](DetailApi.md#detail_read) | **GET** /detail/{short_url}/ | 
[**detail_update**](DetailApi.md#detail_update) | **PUT** /detail/{short_url}/ | 


# **detail_delete**
> detail_delete(short_url)





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
api_instance = swagger_client.DetailApi(swagger_client.ApiClient(configuration))
short_url = 'short_url_example' # str | 

try:
    api_instance.detail_delete(short_url)
except ApiException as e:
    print("Exception when calling DetailApi->detail_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **short_url** | **str**|  | 

### Return type

void (empty response body)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **detail_partial_update**
> Url detail_partial_update(short_url, data)





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
api_instance = swagger_client.DetailApi(swagger_client.ApiClient(configuration))
short_url = 'short_url_example' # str | 
data = swagger_client.Url() # Url | 

try:
    api_response = api_instance.detail_partial_update(short_url, data)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DetailApi->detail_partial_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **short_url** | **str**|  | 
 **data** | [**Url**](Url.md)|  | 

### Return type

[**Url**](Url.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **detail_read**
> Url detail_read(short_url)





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
api_instance = swagger_client.DetailApi(swagger_client.ApiClient(configuration))
short_url = 'short_url_example' # str | 

try:
    api_response = api_instance.detail_read(short_url)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DetailApi->detail_read: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **short_url** | **str**|  | 

### Return type

[**Url**](Url.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **detail_update**
> Url detail_update(short_url, data)





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
api_instance = swagger_client.DetailApi(swagger_client.ApiClient(configuration))
short_url = 'short_url_example' # str | 
data = swagger_client.Url() # Url | 

try:
    api_response = api_instance.detail_update(short_url, data)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DetailApi->detail_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **short_url** | **str**|  | 
 **data** | [**Url**](Url.md)|  | 

### Return type

[**Url**](Url.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

