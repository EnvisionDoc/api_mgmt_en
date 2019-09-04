# API Management
EnOS API Management (APIM) publishes all the APIs that meet the standards supported by EnOS to API consumers. You can use API Management to configure specific policies, and control and process API parameters. The API Management covers full lifecycle management such as API design, testing, management and publishing, and manages security, traffic control, logging, billing, monitoring, and report of managed APIs.

The API Management decouples the production and consumption of APIs. When the backend API changes, the frontend application can continue to access the API without modifying application code or configurations.



## Related Roles
API Management serves mainly for the following roles:

- API developers

  Who write API documents, design, develop, test and publish APIs. 

- API consumers

  Who are enterprise or individual developers that build applications with APIs.


## Main Functions
  
- [Creating APIs](creating_api): create the APIs that meet OpenAPI 3.0.

- [Deploying APIs](deploying_api): deploy the APIs for internal or external use.

- [Backing up APIs](exporting_api): export the existed APIs, and transfer them to another EnOS environment.

- [Testing APIs](testing_api): test the APIs before publishing.

- [Monitoring API](monitoring_api): view the invoking number and status of APIs.

## Related Services

Other EnOS services related to EnOS APIM include:

- Application registration

  API consumers register applications to get the services needed for service account so as to access any necessary APIs. For details about application registration, see [Application Registration](/docs/app-development/en/latest/app_dev_overview).

- IAM

  Provide identity management, authentication, authorization, auditing and other services for APIM. For details about IAM, see [IAM](/docs/iam/en/latest/iam_overview).



