# IO.Swagger.Api.OrderApi

All URIs are relative to *https://virtserver.swaggerhub.com/hplussport8/catalog/1.0.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**OrderPost**](OrderApi.md#orderpost) | **POST** /order | 

<a name="orderpost"></a>
# **OrderPost**
> Order OrderPost (Order body = null)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class OrderPostExample
    {
        public void main()
        {
            // Configure OAuth2 access token for authorization: password
            Configuration.Default.AccessToken = "YOUR_ACCESS_TOKEN";

            var apiInstance = new OrderApi();
            var body = new Order(); // Order |  (optional) 

            try
            {
                Order result = apiInstance.OrderPost(body);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling OrderApi.OrderPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Order**](Order.md)|  | [optional] 

### Return type

[**Order**](Order.md)

### Authorization

[password](../README.md#password)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
