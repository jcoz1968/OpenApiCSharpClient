# IO.Swagger.Api.ProductApi

All URIs are relative to *https://virtserver.swaggerhub.com/hplussport8/catalog/1.0.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ProductGet**](ProductApi.md#productget) | **GET** /product | 
[**ProductPost**](ProductApi.md#productpost) | **POST** /product | 
[**ProductProductIdGet**](ProductApi.md#productproductidget) | **GET** /product/{productId} | 

<a name="productget"></a>
# **ProductGet**
> List<Product> ProductGet (int? pageNumber = null, int? pageSize = null)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ProductGetExample
    {
        public void main()
        {
            var apiInstance = new ProductApi();
            var pageNumber = 56;  // int? | Page number to return (optional) 
            var pageSize = 56;  // int? | Number of items to return (optional) 

            try
            {
                List&lt;Product&gt; result = apiInstance.ProductGet(pageNumber, pageSize);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ProductApi.ProductGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pageNumber** | **int?**| Page number to return | [optional] 
 **pageSize** | **int?**| Number of items to return | [optional] 

### Return type

[**List<Product>**](Product.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="productpost"></a>
# **ProductPost**
> void ProductPost (Product body = null)



Add a product to the catalog

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ProductPostExample
    {
        public void main()
        {
            // Configure OAuth2 access token for authorization: password
            Configuration.Default.AccessToken = "YOUR_ACCESS_TOKEN";

            var apiInstance = new ProductApi();
            var body = new Product(); // Product |  (optional) 

            try
            {
                apiInstance.ProductPost(body);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ProductApi.ProductPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Product**](Product.md)|  | [optional] 

### Return type

void (empty response body)

### Authorization

[password](../README.md#password)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="productproductidget"></a>
# **ProductProductIdGet**
> Product ProductProductIdGet (int? productId, int? customerSecurityHeader = null)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ProductProductIdGetExample
    {
        public void main()
        {
            var apiInstance = new ProductApi();
            var productId = 56;  // int? | 
            var customerSecurityHeader = 56;  // int? |  (optional) 

            try
            {
                Product result = apiInstance.ProductProductIdGet(productId, customerSecurityHeader);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ProductApi.ProductProductIdGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productId** | **int?**|  | 
 **customerSecurityHeader** | **int?**|  | [optional] 

### Return type

[**Product**](Product.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
