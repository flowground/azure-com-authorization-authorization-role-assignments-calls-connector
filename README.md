# ![LOGO](logo.png) AuthorizationManagementClient **flow**ground Connector

## Description

A generated **flow**ground connector for the AuthorizationManagementClient API (version 2018-09-01-preview).

Generated from: https://api.apis.guru/v2/specs/azure.com/authorization-authorization-RoleAssignmentsCalls/2018-09-01-preview/swagger.json<br/>
Generated at: 2019-05-07T17:37:17+03:00

## API Description

Role based access control provides you a way to apply granular level policy administration down to individual resources or resource groups. These operations enable you to manage role assignments. A role assignment grants access to Azure Active Directory users.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Gets all role assignments for the subscription.

*Tags:* `RoleAssignments`

#### Input Parameters
* `$filter` - _optional_ - The filter to apply on the operation. Use $filter=atScope() to return all role assignments at or above the scope. Use $filter=principalId eq {id} to return all role assignments at, above or below the scope for the specified principal.
* `api-version` - _required_ - The API version to use for this operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Gets role assignments for a resource group.

*Tags:* `RoleAssignments`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `$filter` - _optional_ - The filter to apply on the operation. Use $filter=atScope() to return all role assignments at or above the scope. Use $filter=principalId eq {id} to return all role assignments at, above or below the scope for the specified principal.
* `api-version` - _required_ - The API version to use for this operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Gets role assignments for a resource.

*Tags:* `RoleAssignments`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `resourceProviderNamespace` - _required_ - The namespace of the resource provider.
* `parentResourcePath` - _required_ - The parent resource identity.
* `resourceType` - _required_ - The resource type of the resource.
* `resourceName` - _required_ - The name of the resource to get role assignments for.
* `$filter` - _optional_ - The filter to apply on the operation. Use $filter=atScope() to return all role assignments at or above the scope. Use $filter=principalId eq {id} to return all role assignments at, above or below the scope for the specified principal.
* `api-version` - _required_ - The API version to use for this operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Deletes a role assignment.

*Tags:* `RoleAssignments`

#### Input Parameters
* `roleId` - _required_ - The ID of the role assignment to delete.
* `api-version` - _required_ - The API version to use for this operation.

### Gets a role assignment by ID.

*Tags:* `RoleAssignments`

#### Input Parameters
* `roleId` - _required_ - The ID of the role assignment to get.
* `api-version` - _required_ - The API version to use for this operation.

### Creates a role assignment by ID.

*Tags:* `RoleAssignments`

#### Input Parameters
* `roleId` - _required_ - The ID of the role assignment to create.
* `api-version` - _required_ - The API version to use for this operation.

### Gets role assignments for a scope.

*Tags:* `RoleAssignments`

#### Input Parameters
* `scope` - _required_ - The scope of the role assignments.
* `$filter` - _optional_ - The filter to apply on the operation. Use $filter=atScope() to return all role assignments at or above the scope. Use $filter=principalId eq {id} to return all role assignments at, above or below the scope for the specified principal.
* `api-version` - _required_ - The API version to use for this operation.

### Deletes a role assignment.

*Tags:* `RoleAssignments`

#### Input Parameters
* `scope` - _required_ - The scope of the role assignment to delete.
* `roleAssignmentName` - _required_ - The name of the role assignment to delete.
* `api-version` - _required_ - The API version to use for this operation.

### Get the specified role assignment.

*Tags:* `RoleAssignments`

#### Input Parameters
* `scope` - _required_ - The scope of the role assignment.
* `roleAssignmentName` - _required_ - The name of the role assignment to get.
* `api-version` - _required_ - The API version to use for this operation.

### Creates a role assignment.

*Tags:* `RoleAssignments`

#### Input Parameters
* `scope` - _required_ - The scope of the role assignment to create. The scope can be any REST resource instance. For example, use '/subscriptions/{subscription-id}/' for a subscription, '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}' for a resource group, and '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}/providers/{resource-provider}/{resource-type}/{resource-name}' for a resource.
* `roleAssignmentName` - _required_ - The name of the role assignment to create. It can be any valid GUID.
* `api-version` - _required_ - The API version to use for this operation.

## License

**flow**ground :- Telekom iPaaS / azure-com-authorization-authorization-role-assignments-calls-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
