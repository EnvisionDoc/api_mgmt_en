# API Management
EnOS API Management (APIM) releases all the APIs that meets the standards supported by EnOS to API consumers via agents. You can use API Management to configure specific policies, and control and process API parameters. The API Management covers full lifecycle management such as API design, testing, management and release, and manages security, traffic control, logging, billing, monitoring, and reporting of managed APIs.

The API Management decouples the production and consumption of APIs through agents. Changes to the backend APIs do not affect the frontend application's continued access to the APIs through agents, and there is no need for frontend applications to modify the code or configurations.



## Related roles
API Management serves mainly for the following roles:

- API developers

  Write API documents, and design, develop, test and release APIs. 

- API consumers

  Enterprises or individuals that use APIs to build applications often as application developers.


## Main functions
- Defining APIs

  _API developers_ create or import the APIs that meet OpenAPI 3.0 and test them.

- Deploying APIs

  _API developers_ create or import API agents, test API agents, create agent policies and deploy API developed by themselves through API agents.

- API document query

  _API consumers_ query, select and request to use released and exposed APIs.

## Related services

Other EnOS services related to EnOS APIM include:

- Application registration

  API consumers register applications to get the services needed for service account so as to access any necessary APIs. For details about application registration, see [Application Registration](/docs/app-development/en/latest/app_dev_overview)

- IAM

  Provide identity management, authentication, authorization, auditing and other services for APIM. For details about IAM, see [IAM](/docs/iam/en/latest/iam_overview)



