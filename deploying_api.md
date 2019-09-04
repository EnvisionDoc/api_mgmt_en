# Deploying APIs

The private APIs can be usable within the OU only after being published on EnOS; while the third-party APIs can be invoked by a third party only after being published and setting as pubilc on EnOS.

## Task Description

This article describes how to deploy APIs.

## Prerequisites
- You own an EnOS account and the permissions to define APIs. See [Policies, Roles and Permissions](/docs/iam/en/latest/access_policy).
- You have complete the task [Creating APIs](creating_api).

## Procedure

1. Select **API Management > My API**, and click the API group where the API to be deployed is located.

2. In the **API List**:
   - For the private API to be published, switch its status from **Make Online** to **Make Offline**.
   - For the third-party API to be published, switch its status from **Make Online** to **Make Offline**. You can test the API that is going to be public. For more information about testing, see [Testing APIs](testing_api).

3. For the published and tested third-party API, switch its status of **Visibility** from **Private** to **Public** to complete its deployment.

## Result

The private APIs with a status of **Make Offline** can be used in the OU.

The third-party APIs with **Public** as **Visibility** can be found by selecting **API Management > Public API**.

## Next Step

For those APIs that no longer need to used, you can select [Deleting APIs](deleting_api) to delete them.

