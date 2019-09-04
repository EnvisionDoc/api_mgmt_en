# Deleting APIs

Users can delete the APIs that no longer need to be published on EnOS. Deleting an API does not affect the backend services of the API agent.

## Task Description

This article describes how to delete an API through API Management.

## Prerequisites

- You own an EnOS account and the permissions to define APIs. See [Policies, Roles and Permissions](/docs/iam/en/latest/access_policy).
- You have understood the concepts related to [API Management](api_management_concepts).
- You have complete the task [Creating APIs](creating_api).

## Procedure

1. Select **API Management > My API**, and click the API group where the API to be deleted is located.

2. In the API list, make sure that the API to be deleted is **Offline**.

3. Click **Delete**.

## Result

The API consumers can no longer use this API to invoke the backend services. There are no impact on backend services.
