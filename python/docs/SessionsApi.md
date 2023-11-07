# cloudhub_client.SessionsApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_sessions_certificate_get**](SessionsApi.md#api_sessions_certificate_get) | **GET** /api/sessions/certificate | 
[**api_sessions_post**](SessionsApi.md#api_sessions_post) | **POST** /api/sessions | 
[**api_sessions_sign_hash_post**](SessionsApi.md#api_sessions_sign_hash_post) | **POST** /api/sessions/sign-hash | 
[**api_v2_sessions_certificate_get**](SessionsApi.md#api_v2_sessions_certificate_get) | **GET** /api/v2/sessions/certificate | 

# **api_sessions_certificate_get**
> str api_sessions_certificate_get(session=session)



### Example
```python
from __future__ import print_function
import time
import cloudhub_client
from cloudhub_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: ApiKey
configuration = cloudhub_client.Configuration()
configuration.api_key['X-Api-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Api-Key'] = 'Bearer'

# create an instance of the API class
api_instance = cloudhub_client.SessionsApi(cloudhub_client.ApiClient(configuration))
session = 'session_example' # str |  (optional)

try:
    api_response = api_instance.api_sessions_certificate_get(session=session)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling SessionsApi->api_sessions_certificate_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **session** | **str**|  | [optional] 

### Return type

**str**

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_sessions_post**
> SessionModel api_sessions_post(body=body)



### Example
```python
from __future__ import print_function
import time
import cloudhub_client
from cloudhub_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: ApiKey
configuration = cloudhub_client.Configuration()
configuration.api_key['X-Api-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Api-Key'] = 'Bearer'

# create an instance of the API class
api_instance = cloudhub_client.SessionsApi(cloudhub_client.ApiClient(configuration))
body = cloudhub_client.SessionCreateRequest() # SessionCreateRequest |  (optional)

try:
    api_response = api_instance.api_sessions_post(body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling SessionsApi->api_sessions_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**SessionCreateRequest**](SessionCreateRequest.md)|  | [optional] 

### Return type

[**SessionModel**](SessionModel.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_sessions_sign_hash_post**
> str api_sessions_sign_hash_post(body=body)



### Example
```python
from __future__ import print_function
import time
import cloudhub_client
from cloudhub_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: ApiKey
configuration = cloudhub_client.Configuration()
configuration.api_key['X-Api-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Api-Key'] = 'Bearer'

# create an instance of the API class
api_instance = cloudhub_client.SessionsApi(cloudhub_client.ApiClient(configuration))
body = cloudhub_client.SignHashRequest() # SignHashRequest |  (optional)

try:
    api_response = api_instance.api_sessions_sign_hash_post(body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling SessionsApi->api_sessions_sign_hash_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**SignHashRequest**](SignHashRequest.md)|  | [optional] 

### Return type

**str**

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_v2_sessions_certificate_get**
> CertificateModel api_v2_sessions_certificate_get(session=session)



### Example
```python
from __future__ import print_function
import time
import cloudhub_client
from cloudhub_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: ApiKey
configuration = cloudhub_client.Configuration()
configuration.api_key['X-Api-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Api-Key'] = 'Bearer'

# create an instance of the API class
api_instance = cloudhub_client.SessionsApi(cloudhub_client.ApiClient(configuration))
session = 'session_example' # str |  (optional)

try:
    api_response = api_instance.api_v2_sessions_certificate_get(session=session)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling SessionsApi->api_v2_sessions_certificate_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **session** | **str**|  | [optional] 

### Return type

[**CertificateModel**](CertificateModel.md)

### Authorization

[ApiKey](../README.md#ApiKey)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

