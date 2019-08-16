# Creating APIs

To publish an API through EnOS and make them available to authorized consumers, you should define the API.

## About This Task

This article describes how to create an API in the API Management page.

## Before You Start

- You own an EnOS account and the permissions required to define APIs. See [Policies, Roles and Permissions](/docs/iam/zh_CN/latest/access_policy).
- You have understood the [concepts] related to [API management](api_management_concepts).

## Creating API groups

1. Select **API Management > My APIs**;

2. Click **Create an API Group**, and complete the following fields:
   
   - Name: Uppercase and lowercase English letters, numbers, and hyphen (-) are supported and its length is limited within 32 characters;
   - Path
   - Description: limited within 140 characters.

3. Click **Save** to complete the creation;

   
## Creating an API

1. Click the API group you created and then click **Add API**.
   
2. In **API Basic Information** page, complete the following fields and click **Next**:
   - API name
   - API type: private and third-party APIs supported.
   - API description

3. In the **Backend Service** page, complete the following fields and click **Next**:
   - Backend Service Address: HTTP address and port that actually provide the API service
   - HTTP Method: GET, POST, PUT and DELETE supported on EnOS currently
   - Backend Request Path: the path where the resource provide the API service is located
   - Parameter Processing Mode: processing mode of API gateway for incoming parameters, where passthrough and mapping are supported
      - Mapping: when the API gateway receives the API request from an API consumer, it converts the request into a format required by the backend through a mapping relationship.
      - Passthrough: After receiving the API request, the API gateway forwards it directly to the backend service rather than processing it.
   - Backend Timeout Time: After the API request arrives at the API gateway, the API gateway invokes the response time of the API backend service, which is the length of time for which the API gateway requests the backend service until the API gateway receives the result returned by the backend. The timeout time is calculated in ms. If the response time exceeds this value, the API gateway will stop requesting the backend service and return an appropriate error message to the user.
   - Backend Parameters: the parameters that are required to invoke backend services. Including the following fields:
      - Name
      - Location: the location of the parameter in the request, which may be Head, Query or Path
      - Data Type: the type of field, for which String, Int, Long, Float, Double, Boolean, Binary, Date, DateTime and Password are supported.
      - Required
      - Default Value
      - Description
   - Constant parameters: these parameters are not visible to API consumers, however the API gateway will add these parameters to the specified location in the request when transferring the request, and then pass it to the backend service to meet the backend business needs. Including the following fields:
      - Name
      - Location: the location of the constant parameter in the request, which may be Head or Query
      - Mapping
      - Default Value
      - Description
      - Operation

4. In the **Front-end Request** page, complete the following fields and click **Next**:
   - Version: used to identify different versions of the API. Different versions of the same API can be mounted under the same API group. 
   - Request Path: the path used by the API consumer to invoke the API. If mapping is selected as the incoming parameter request mode, the request path may be set by the API developer as needed; if passthrough is selected as the incoming parameter request mode, the request path needs to be consistent with the backend request path.

5. In the **Response** page, complete the following fields and click **Next**:
   - Content Type
   - Successful result samples
   - Failed result samples: optional
   - Response parameter definition
   - Error code definition

6. In the **Advanced Configuration** page, the user can add additional configurations for the API to be released in EnOS. The EnOS currently supports the following functions:
   - Traffic control
   - Request size limitations
   - IP limitations
   - Mock testing

   Click **OK**

## Result

In the page of API group details, you can see the API that has been created successfully, and its status is shown as **Offline** with the attribute of **Visibility** shown as **Private**.

## Next Steps

[Deploying APIs](deploying_api)
