# Deploying APIs

The private APIs that have been created can be usable within the OU only after being released on EnOS, while the third-party APIs that have been created can be invoked by a third party only after being released and exposed on EnOS.

## Task description

This article describes how to deploy APIs.

## Prerequisites
- You own an EnOS account and the permissions required to define APIs. See [Policies, Roles and Permissions](/docs/iam/zh_CN/latest/access_policy).
- You have understood the [concepts] related to API management (api_management_concepts).
- You have complete the task [Creating APIs] (creating_api).

## Steps

1. Select **API Management > My APIs**, and then click the API group where the API to be deployed is located to enter the page of API group details;

2. In the API list:
   - Select the private API to be released, and switch its status from **Offline** to **Released**;
   - For the third-party API to be released, switch its status from **Offline** to **Released**, and you can test the API to be exposed. For more information about testing, see [Testing APIs] (testing_api)

3. For the third-party API released and tested, switch its status of **Exposed or not** from **Private** to **Exposed** to complete its deployment.

## Results

The private APIs with a status of **Released** can be used in the OU.

The third-party APIs with a status of **Exposed** can be found by selecting **API Management > Exposed APIs**. Click **Export Documents**, and you can check the API documents in .txt format.

## Subsequent operations

The user can select [Deleting APIs](deleting_api) to delete any APIs that do not need to be used any more.

