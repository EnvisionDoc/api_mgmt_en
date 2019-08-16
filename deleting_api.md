# Deleting APIs

Users may delete the APIs that do not need to be exposed on EnOS. Deleting an API does not affect the backend services of the API agent.

## About This Task

This article describes how to delete an API through API Management.

## Before You Start

- You own an EnOS account and the permissions required to define APIs. See [Policies, Roles and Permissions](/docs/iam/zh_CN/latest/access_policy).
- You have understood the [concepts] related to API managemnt (api_management_concepts).
- You have complete the task [Creating APIs] (creating_api).

## Procedure

1. Select **API Management > My APIs**, and then click the API group where the API to be deleted is located;

2. In the API list, check and make sure that the API to be deleted is **Offline**;

3. Click **Delete API**.

## Result

The corresponding API is deleted and the API consumers can not invoke the backend services. There are no impact on backend services.
