# WorkSpacesClient

> [Index](../README.md) > [WorkSpaces](./README.md) > WorkSpacesClient

!!! note ""

    Auto-generated documentation for [WorkSpaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#workspaces)
    type annotations stubs module [types-aiobotocore-workspaces](https://pypi.org/project/types-aiobotocore-workspaces/).

## WorkSpacesClient

Type annotations and code completion for `#!python session.client("workspaces")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# WorkSpacesClient usage example

from aioboto3.session import Session
from types_aiobotocore_workspaces.client import WorkSpacesClient

session = Session()
async with session.client("workspaces") as client:
    client: WorkSpacesClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("workspaces").exceptions` structure.

```python
# WorkSpacesClient.exceptions usage example

async with session.client("workspaces") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ApplicationNotSupportedException,
        client.exceptions.ClientError,
        client.exceptions.ComputeNotCompatibleException,
        client.exceptions.ConflictException,
        client.exceptions.IncompatibleApplicationsException,
        client.exceptions.InternalServerException,
        client.exceptions.InvalidParameterValuesException,
        client.exceptions.InvalidResourceStateException,
        client.exceptions.OperatingSystemNotCompatibleException,
        client.exceptions.OperationInProgressException,
        client.exceptions.OperationNotSupportedException,
        client.exceptions.ResourceAlreadyExistsException,
        client.exceptions.ResourceAssociatedException,
        client.exceptions.ResourceCreationFailedException,
        client.exceptions.ResourceInUseException,
        client.exceptions.ResourceLimitExceededException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ResourceUnavailableException,
        client.exceptions.UnsupportedNetworkConfigurationException,
        client.exceptions.UnsupportedWorkspaceConfigurationException,
        client.exceptions.ValidationException,
        client.exceptions.WorkspacesDefaultRoleNotFoundException,
    ) as e:
        print(e)
```

```python
# WorkSpacesClient.exceptions type checking example

from types_aiobotocore_workspaces.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("workspaces").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("workspaces").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### accept\_account\_link\_invitation

Accepts the account link invitation.

Type annotations and code completion for `#!python session.client("workspaces").accept_account_link_invitation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# accept_account_link_invitation method definition

await def accept_account_link_invitation(
    self,
    *,
    LinkId: str,
    ClientToken: str = ...,
) -> AcceptAccountLinkInvitationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AcceptAccountLinkInvitationResultTypeDef](./type_defs.md#acceptaccountlinkinvitationresulttypedef) 


```python
# accept_account_link_invitation method usage example with argument unpacking

kwargs: AcceptAccountLinkInvitationRequestRequestTypeDef = {  # (1)
    "LinkId": ...,
}

parent.accept_account_link_invitation(**kwargs)
```

1. See [:material-code-braces: AcceptAccountLinkInvitationRequestRequestTypeDef](./type_defs.md#acceptaccountlinkinvitationrequestrequesttypedef) 

### associate\_connection\_alias

Associates the specified connection alias with the specified directory to
enable cross-Region redirection.

Type annotations and code completion for `#!python session.client("workspaces").associate_connection_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# associate_connection_alias method definition

await def associate_connection_alias(
    self,
    *,
    AliasId: str,
    ResourceId: str,
) -> AssociateConnectionAliasResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateConnectionAliasResultTypeDef](./type_defs.md#associateconnectionaliasresulttypedef) 


```python
# associate_connection_alias method usage example with argument unpacking

kwargs: AssociateConnectionAliasRequestRequestTypeDef = {  # (1)
    "AliasId": ...,
    "ResourceId": ...,
}

parent.associate_connection_alias(**kwargs)
```

1. See [:material-code-braces: AssociateConnectionAliasRequestRequestTypeDef](./type_defs.md#associateconnectionaliasrequestrequesttypedef) 

### associate\_ip\_groups

Associates the specified IP access control group with the specified directory.

Type annotations and code completion for `#!python session.client("workspaces").associate_ip_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# associate_ip_groups method definition

await def associate_ip_groups(
    self,
    *,
    DirectoryId: str,
    GroupIds: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# associate_ip_groups method usage example with argument unpacking

kwargs: AssociateIpGroupsRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
    "GroupIds": ...,
}

parent.associate_ip_groups(**kwargs)
```

1. See [:material-code-braces: AssociateIpGroupsRequestRequestTypeDef](./type_defs.md#associateipgroupsrequestrequesttypedef) 

### associate\_workspace\_application

Associates the specified application to the specified WorkSpace.

Type annotations and code completion for `#!python session.client("workspaces").associate_workspace_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# associate_workspace_application method definition

await def associate_workspace_application(
    self,
    *,
    WorkspaceId: str,
    ApplicationId: str,
) -> AssociateWorkspaceApplicationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateWorkspaceApplicationResultTypeDef](./type_defs.md#associateworkspaceapplicationresulttypedef) 


```python
# associate_workspace_application method usage example with argument unpacking

kwargs: AssociateWorkspaceApplicationRequestRequestTypeDef = {  # (1)
    "WorkspaceId": ...,
    "ApplicationId": ...,
}

parent.associate_workspace_application(**kwargs)
```

1. See [:material-code-braces: AssociateWorkspaceApplicationRequestRequestTypeDef](./type_defs.md#associateworkspaceapplicationrequestrequesttypedef) 

### authorize\_ip\_rules

Adds one or more rules to the specified IP access control group.

Type annotations and code completion for `#!python session.client("workspaces").authorize_ip_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# authorize_ip_rules method definition

await def authorize_ip_rules(
    self,
    *,
    GroupId: str,
    UserRules: Sequence[IpRuleItemTypeDef],  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: IpRuleItemTypeDef](./type_defs.md#ipruleitemtypedef) 


```python
# authorize_ip_rules method usage example with argument unpacking

kwargs: AuthorizeIpRulesRequestRequestTypeDef = {  # (1)
    "GroupId": ...,
    "UserRules": ...,
}

parent.authorize_ip_rules(**kwargs)
```

1. See [:material-code-braces: AuthorizeIpRulesRequestRequestTypeDef](./type_defs.md#authorizeiprulesrequestrequesttypedef) 

### copy\_workspace\_image

Copies the specified image from the specified Region to the current Region.

Type annotations and code completion for `#!python session.client("workspaces").copy_workspace_image` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# copy_workspace_image method definition

await def copy_workspace_image(
    self,
    *,
    Name: str,
    SourceImageId: str,
    SourceRegion: str,
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CopyWorkspaceImageResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CopyWorkspaceImageResultTypeDef](./type_defs.md#copyworkspaceimageresulttypedef) 


```python
# copy_workspace_image method usage example with argument unpacking

kwargs: CopyWorkspaceImageRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "SourceImageId": ...,
    "SourceRegion": ...,
}

parent.copy_workspace_image(**kwargs)
```

1. See [:material-code-braces: CopyWorkspaceImageRequestRequestTypeDef](./type_defs.md#copyworkspaceimagerequestrequesttypedef) 

### create\_account\_link\_invitation

Creates the account link invitation.

Type annotations and code completion for `#!python session.client("workspaces").create_account_link_invitation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# create_account_link_invitation method definition

await def create_account_link_invitation(
    self,
    *,
    TargetAccountId: str,
    ClientToken: str = ...,
) -> CreateAccountLinkInvitationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateAccountLinkInvitationResultTypeDef](./type_defs.md#createaccountlinkinvitationresulttypedef) 


```python
# create_account_link_invitation method usage example with argument unpacking

kwargs: CreateAccountLinkInvitationRequestRequestTypeDef = {  # (1)
    "TargetAccountId": ...,
}

parent.create_account_link_invitation(**kwargs)
```

1. See [:material-code-braces: CreateAccountLinkInvitationRequestRequestTypeDef](./type_defs.md#createaccountlinkinvitationrequestrequesttypedef) 

### create\_connect\_client\_add\_in

Creates a client-add-in for Amazon Connect within a directory.

Type annotations and code completion for `#!python session.client("workspaces").create_connect_client_add_in` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# create_connect_client_add_in method definition

await def create_connect_client_add_in(
    self,
    *,
    ResourceId: str,
    Name: str,
    URL: str,
) -> CreateConnectClientAddInResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateConnectClientAddInResultTypeDef](./type_defs.md#createconnectclientaddinresulttypedef) 


```python
# create_connect_client_add_in method usage example with argument unpacking

kwargs: CreateConnectClientAddInRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
    "Name": ...,
    "URL": ...,
}

parent.create_connect_client_add_in(**kwargs)
```

1. See [:material-code-braces: CreateConnectClientAddInRequestRequestTypeDef](./type_defs.md#createconnectclientaddinrequestrequesttypedef) 

### create\_connection\_alias

Creates the specified connection alias for use with cross-Region redirection.

Type annotations and code completion for `#!python session.client("workspaces").create_connection_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# create_connection_alias method definition

await def create_connection_alias(
    self,
    *,
    ConnectionString: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateConnectionAliasResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateConnectionAliasResultTypeDef](./type_defs.md#createconnectionaliasresulttypedef) 


```python
# create_connection_alias method usage example with argument unpacking

kwargs: CreateConnectionAliasRequestRequestTypeDef = {  # (1)
    "ConnectionString": ...,
}

parent.create_connection_alias(**kwargs)
```

1. See [:material-code-braces: CreateConnectionAliasRequestRequestTypeDef](./type_defs.md#createconnectionaliasrequestrequesttypedef) 

### create\_ip\_group

Creates an IP access control group.

Type annotations and code completion for `#!python session.client("workspaces").create_ip_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# create_ip_group method definition

await def create_ip_group(
    self,
    *,
    GroupName: str,
    GroupDesc: str = ...,
    UserRules: Sequence[IpRuleItemTypeDef] = ...,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateIpGroupResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: IpRuleItemTypeDef](./type_defs.md#ipruleitemtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateIpGroupResultTypeDef](./type_defs.md#createipgroupresulttypedef) 


```python
# create_ip_group method usage example with argument unpacking

kwargs: CreateIpGroupRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
}

parent.create_ip_group(**kwargs)
```

1. See [:material-code-braces: CreateIpGroupRequestRequestTypeDef](./type_defs.md#createipgrouprequestrequesttypedef) 

### create\_standby\_workspaces

Creates a standby WorkSpace in a secondary Region.

Type annotations and code completion for `#!python session.client("workspaces").create_standby_workspaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# create_standby_workspaces method definition

await def create_standby_workspaces(
    self,
    *,
    PrimaryRegion: str,
    StandbyWorkspaces: Sequence[StandbyWorkspaceUnionTypeDef],  # (1)
) -> CreateStandbyWorkspacesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StandbyWorkspaceTypeDef](./type_defs.md#standbyworkspacetypedef) [:material-code-braces: StandbyWorkspaceOutputTypeDef](./type_defs.md#standbyworkspaceoutputtypedef) 
2. See [:material-code-braces: CreateStandbyWorkspacesResultTypeDef](./type_defs.md#createstandbyworkspacesresulttypedef) 


```python
# create_standby_workspaces method usage example with argument unpacking

kwargs: CreateStandbyWorkspacesRequestRequestTypeDef = {  # (1)
    "PrimaryRegion": ...,
    "StandbyWorkspaces": ...,
}

parent.create_standby_workspaces(**kwargs)
```

1. See [:material-code-braces: CreateStandbyWorkspacesRequestRequestTypeDef](./type_defs.md#createstandbyworkspacesrequestrequesttypedef) 

### create\_tags

Creates the specified tags for the specified WorkSpaces resource.

Type annotations and code completion for `#!python session.client("workspaces").create_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# create_tags method definition

await def create_tags(
    self,
    *,
    ResourceId: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# create_tags method usage example with argument unpacking

kwargs: CreateTagsRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
    "Tags": ...,
}

parent.create_tags(**kwargs)
```

1. See [:material-code-braces: CreateTagsRequestRequestTypeDef](./type_defs.md#createtagsrequestrequesttypedef) 

### create\_updated\_workspace\_image

Creates a new updated WorkSpace image based on the specified source image.

Type annotations and code completion for `#!python session.client("workspaces").create_updated_workspace_image` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# create_updated_workspace_image method definition

await def create_updated_workspace_image(
    self,
    *,
    Name: str,
    Description: str,
    SourceImageId: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateUpdatedWorkspaceImageResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateUpdatedWorkspaceImageResultTypeDef](./type_defs.md#createupdatedworkspaceimageresulttypedef) 


```python
# create_updated_workspace_image method usage example with argument unpacking

kwargs: CreateUpdatedWorkspaceImageRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Description": ...,
    "SourceImageId": ...,
}

parent.create_updated_workspace_image(**kwargs)
```

1. See [:material-code-braces: CreateUpdatedWorkspaceImageRequestRequestTypeDef](./type_defs.md#createupdatedworkspaceimagerequestrequesttypedef) 

### create\_workspace\_bundle

Creates the specified WorkSpace bundle.

Type annotations and code completion for `#!python session.client("workspaces").create_workspace_bundle` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# create_workspace_bundle method definition

await def create_workspace_bundle(
    self,
    *,
    BundleName: str,
    BundleDescription: str,
    ImageId: str,
    ComputeType: ComputeTypeTypeDef,  # (1)
    UserStorage: UserStorageTypeDef,  # (2)
    RootStorage: RootStorageTypeDef = ...,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateWorkspaceBundleResultTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: ComputeTypeTypeDef](./type_defs.md#computetypetypedef) 
2. See [:material-code-braces: UserStorageTypeDef](./type_defs.md#userstoragetypedef) 
3. See [:material-code-braces: RootStorageTypeDef](./type_defs.md#rootstoragetypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateWorkspaceBundleResultTypeDef](./type_defs.md#createworkspacebundleresulttypedef) 


```python
# create_workspace_bundle method usage example with argument unpacking

kwargs: CreateWorkspaceBundleRequestRequestTypeDef = {  # (1)
    "BundleName": ...,
    "BundleDescription": ...,
    "ImageId": ...,
    "ComputeType": ...,
    "UserStorage": ...,
}

parent.create_workspace_bundle(**kwargs)
```

1. See [:material-code-braces: CreateWorkspaceBundleRequestRequestTypeDef](./type_defs.md#createworkspacebundlerequestrequesttypedef) 

### create\_workspace\_image

Creates a new WorkSpace image from an existing WorkSpace.

Type annotations and code completion for `#!python session.client("workspaces").create_workspace_image` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# create_workspace_image method definition

await def create_workspace_image(
    self,
    *,
    Name: str,
    Description: str,
    WorkspaceId: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateWorkspaceImageResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateWorkspaceImageResultTypeDef](./type_defs.md#createworkspaceimageresulttypedef) 


```python
# create_workspace_image method usage example with argument unpacking

kwargs: CreateWorkspaceImageRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Description": ...,
    "WorkspaceId": ...,
}

parent.create_workspace_image(**kwargs)
```

1. See [:material-code-braces: CreateWorkspaceImageRequestRequestTypeDef](./type_defs.md#createworkspaceimagerequestrequesttypedef) 

### create\_workspaces

Creates one or more WorkSpaces.

Type annotations and code completion for `#!python session.client("workspaces").create_workspaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# create_workspaces method definition

await def create_workspaces(
    self,
    *,
    Workspaces: Sequence[WorkspaceRequestUnionTypeDef],  # (1)
) -> CreateWorkspacesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: WorkspaceRequestTypeDef](./type_defs.md#workspacerequesttypedef) [:material-code-braces: WorkspaceRequestOutputTypeDef](./type_defs.md#workspacerequestoutputtypedef) 
2. See [:material-code-braces: CreateWorkspacesResultTypeDef](./type_defs.md#createworkspacesresulttypedef) 


```python
# create_workspaces method usage example with argument unpacking

kwargs: CreateWorkspacesRequestRequestTypeDef = {  # (1)
    "Workspaces": ...,
}

parent.create_workspaces(**kwargs)
```

1. See [:material-code-braces: CreateWorkspacesRequestRequestTypeDef](./type_defs.md#createworkspacesrequestrequesttypedef) 

### create\_workspaces\_pool

Creates a pool of WorkSpaces.

Type annotations and code completion for `#!python session.client("workspaces").create_workspaces_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# create_workspaces_pool method definition

await def create_workspaces_pool(
    self,
    *,
    PoolName: str,
    Description: str,
    BundleId: str,
    DirectoryId: str,
    Capacity: CapacityTypeDef,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    ApplicationSettings: ApplicationSettingsRequestTypeDef = ...,  # (3)
    TimeoutSettings: TimeoutSettingsTypeDef = ...,  # (4)
) -> CreateWorkspacesPoolResultTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: CapacityTypeDef](./type_defs.md#capacitytypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ApplicationSettingsRequestTypeDef](./type_defs.md#applicationsettingsrequesttypedef) 
4. See [:material-code-braces: TimeoutSettingsTypeDef](./type_defs.md#timeoutsettingstypedef) 
5. See [:material-code-braces: CreateWorkspacesPoolResultTypeDef](./type_defs.md#createworkspacespoolresulttypedef) 


```python
# create_workspaces_pool method usage example with argument unpacking

kwargs: CreateWorkspacesPoolRequestRequestTypeDef = {  # (1)
    "PoolName": ...,
    "Description": ...,
    "BundleId": ...,
    "DirectoryId": ...,
    "Capacity": ...,
}

parent.create_workspaces_pool(**kwargs)
```

1. See [:material-code-braces: CreateWorkspacesPoolRequestRequestTypeDef](./type_defs.md#createworkspacespoolrequestrequesttypedef) 

### delete\_account\_link\_invitation

Deletes the account link invitation.

Type annotations and code completion for `#!python session.client("workspaces").delete_account_link_invitation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# delete_account_link_invitation method definition

await def delete_account_link_invitation(
    self,
    *,
    LinkId: str,
    ClientToken: str = ...,
) -> DeleteAccountLinkInvitationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAccountLinkInvitationResultTypeDef](./type_defs.md#deleteaccountlinkinvitationresulttypedef) 


```python
# delete_account_link_invitation method usage example with argument unpacking

kwargs: DeleteAccountLinkInvitationRequestRequestTypeDef = {  # (1)
    "LinkId": ...,
}

parent.delete_account_link_invitation(**kwargs)
```

1. See [:material-code-braces: DeleteAccountLinkInvitationRequestRequestTypeDef](./type_defs.md#deleteaccountlinkinvitationrequestrequesttypedef) 

### delete\_client\_branding

Deletes customized client branding.

Type annotations and code completion for `#!python session.client("workspaces").delete_client_branding` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# delete_client_branding method definition

await def delete_client_branding(
    self,
    *,
    ResourceId: str,
    Platforms: Sequence[ClientDeviceTypeType],  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ClientDeviceTypeType](./literals.md#clientdevicetypetype) 


```python
# delete_client_branding method usage example with argument unpacking

kwargs: DeleteClientBrandingRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
    "Platforms": ...,
}

parent.delete_client_branding(**kwargs)
```

1. See [:material-code-braces: DeleteClientBrandingRequestRequestTypeDef](./type_defs.md#deleteclientbrandingrequestrequesttypedef) 

### delete\_connect\_client\_add\_in

Deletes a client-add-in for Amazon Connect that is configured within a
directory.

Type annotations and code completion for `#!python session.client("workspaces").delete_connect_client_add_in` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# delete_connect_client_add_in method definition

await def delete_connect_client_add_in(
    self,
    *,
    AddInId: str,
    ResourceId: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_connect_client_add_in method usage example with argument unpacking

kwargs: DeleteConnectClientAddInRequestRequestTypeDef = {  # (1)
    "AddInId": ...,
    "ResourceId": ...,
}

parent.delete_connect_client_add_in(**kwargs)
```

1. See [:material-code-braces: DeleteConnectClientAddInRequestRequestTypeDef](./type_defs.md#deleteconnectclientaddinrequestrequesttypedef) 

### delete\_connection\_alias

Deletes the specified connection alias.

Type annotations and code completion for `#!python session.client("workspaces").delete_connection_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# delete_connection_alias method definition

await def delete_connection_alias(
    self,
    *,
    AliasId: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_connection_alias method usage example with argument unpacking

kwargs: DeleteConnectionAliasRequestRequestTypeDef = {  # (1)
    "AliasId": ...,
}

parent.delete_connection_alias(**kwargs)
```

1. See [:material-code-braces: DeleteConnectionAliasRequestRequestTypeDef](./type_defs.md#deleteconnectionaliasrequestrequesttypedef) 

### delete\_ip\_group

Deletes the specified IP access control group.

Type annotations and code completion for `#!python session.client("workspaces").delete_ip_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# delete_ip_group method definition

await def delete_ip_group(
    self,
    *,
    GroupId: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_ip_group method usage example with argument unpacking

kwargs: DeleteIpGroupRequestRequestTypeDef = {  # (1)
    "GroupId": ...,
}

parent.delete_ip_group(**kwargs)
```

1. See [:material-code-braces: DeleteIpGroupRequestRequestTypeDef](./type_defs.md#deleteipgrouprequestrequesttypedef) 

### delete\_tags

Deletes the specified tags from the specified WorkSpaces resource.

Type annotations and code completion for `#!python session.client("workspaces").delete_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# delete_tags method definition

await def delete_tags(
    self,
    *,
    ResourceId: str,
    TagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# delete_tags method usage example with argument unpacking

kwargs: DeleteTagsRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
    "TagKeys": ...,
}

parent.delete_tags(**kwargs)
```

1. See [:material-code-braces: DeleteTagsRequestRequestTypeDef](./type_defs.md#deletetagsrequestrequesttypedef) 

### delete\_workspace\_bundle

Deletes the specified WorkSpace bundle.

Type annotations and code completion for `#!python session.client("workspaces").delete_workspace_bundle` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# delete_workspace_bundle method definition

await def delete_workspace_bundle(
    self,
    *,
    BundleId: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_workspace_bundle method usage example with argument unpacking

kwargs: DeleteWorkspaceBundleRequestRequestTypeDef = {  # (1)
    "BundleId": ...,
}

parent.delete_workspace_bundle(**kwargs)
```

1. See [:material-code-braces: DeleteWorkspaceBundleRequestRequestTypeDef](./type_defs.md#deleteworkspacebundlerequestrequesttypedef) 

### delete\_workspace\_image

Deletes the specified image from your account.

Type annotations and code completion for `#!python session.client("workspaces").delete_workspace_image` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# delete_workspace_image method definition

await def delete_workspace_image(
    self,
    *,
    ImageId: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_workspace_image method usage example with argument unpacking

kwargs: DeleteWorkspaceImageRequestRequestTypeDef = {  # (1)
    "ImageId": ...,
}

parent.delete_workspace_image(**kwargs)
```

1. See [:material-code-braces: DeleteWorkspaceImageRequestRequestTypeDef](./type_defs.md#deleteworkspaceimagerequestrequesttypedef) 

### deploy\_workspace\_applications

Deploys associated applications to the specified WorkSpace.

Type annotations and code completion for `#!python session.client("workspaces").deploy_workspace_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# deploy_workspace_applications method definition

await def deploy_workspace_applications(
    self,
    *,
    WorkspaceId: str,
    Force: bool = ...,
) -> DeployWorkspaceApplicationsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeployWorkspaceApplicationsResultTypeDef](./type_defs.md#deployworkspaceapplicationsresulttypedef) 


```python
# deploy_workspace_applications method usage example with argument unpacking

kwargs: DeployWorkspaceApplicationsRequestRequestTypeDef = {  # (1)
    "WorkspaceId": ...,
}

parent.deploy_workspace_applications(**kwargs)
```

1. See [:material-code-braces: DeployWorkspaceApplicationsRequestRequestTypeDef](./type_defs.md#deployworkspaceapplicationsrequestrequesttypedef) 

### deregister\_workspace\_directory

Deregisters the specified directory.

Type annotations and code completion for `#!python session.client("workspaces").deregister_workspace_directory` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# deregister_workspace_directory method definition

await def deregister_workspace_directory(
    self,
    *,
    DirectoryId: str,
) -> dict[str, Any]:
    ...
```



```python
# deregister_workspace_directory method usage example with argument unpacking

kwargs: DeregisterWorkspaceDirectoryRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.deregister_workspace_directory(**kwargs)
```

1. See [:material-code-braces: DeregisterWorkspaceDirectoryRequestRequestTypeDef](./type_defs.md#deregisterworkspacedirectoryrequestrequesttypedef) 

### describe\_account

Retrieves a list that describes the configuration of Bring Your Own License
(BYOL) for the specified account.

Type annotations and code completion for `#!python session.client("workspaces").describe_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_account method definition

await def describe_account(
    self,
) -> DescribeAccountResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAccountResultTypeDef](./type_defs.md#describeaccountresulttypedef) 

### describe\_account\_modifications

Retrieves a list that describes modifications to the configuration of Bring
Your Own License (BYOL) for the specified account.

Type annotations and code completion for `#!python session.client("workspaces").describe_account_modifications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_account_modifications method definition

await def describe_account_modifications(
    self,
    *,
    NextToken: str = ...,
) -> DescribeAccountModificationsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAccountModificationsResultTypeDef](./type_defs.md#describeaccountmodificationsresulttypedef) 


```python
# describe_account_modifications method usage example with argument unpacking

kwargs: DescribeAccountModificationsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.describe_account_modifications(**kwargs)
```

1. See [:material-code-braces: DescribeAccountModificationsRequestRequestTypeDef](./type_defs.md#describeaccountmodificationsrequestrequesttypedef) 

### describe\_application\_associations

Describes the associations between the application and the specified associated
resources.

Type annotations and code completion for `#!python session.client("workspaces").describe_application_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_application_associations method definition

await def describe_application_associations(
    self,
    *,
    ApplicationId: str,
    AssociatedResourceTypes: Sequence[ApplicationAssociatedResourceTypeType],  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeApplicationAssociationsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ApplicationAssociatedResourceTypeType](./literals.md#applicationassociatedresourcetypetype) 
2. See [:material-code-braces: DescribeApplicationAssociationsResultTypeDef](./type_defs.md#describeapplicationassociationsresulttypedef) 


```python
# describe_application_associations method usage example with argument unpacking

kwargs: DescribeApplicationAssociationsRequestRequestTypeDef = {  # (1)
    "ApplicationId": ...,
    "AssociatedResourceTypes": ...,
}

parent.describe_application_associations(**kwargs)
```

1. See [:material-code-braces: DescribeApplicationAssociationsRequestRequestTypeDef](./type_defs.md#describeapplicationassociationsrequestrequesttypedef) 

### describe\_applications

Describes the specified applications by filtering based on their compute types,
license availability, operating systems, and owners.

Type annotations and code completion for `#!python session.client("workspaces").describe_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_applications method definition

await def describe_applications(
    self,
    *,
    ApplicationIds: Sequence[str] = ...,
    ComputeTypeNames: Sequence[ComputeType] = ...,  # (1)
    LicenseType: WorkSpaceApplicationLicenseTypeType = ...,  # (2)
    OperatingSystemNames: Sequence[OperatingSystemNameType] = ...,  # (3)
    Owner: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeApplicationsResultTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ComputeType](./literals.md#computetype) 
2. See [:material-code-brackets: WorkSpaceApplicationLicenseTypeType](./literals.md#workspaceapplicationlicensetypetype) 
3. See [:material-code-brackets: OperatingSystemNameType](./literals.md#operatingsystemnametype) 
4. See [:material-code-braces: DescribeApplicationsResultTypeDef](./type_defs.md#describeapplicationsresulttypedef) 


```python
# describe_applications method usage example with argument unpacking

kwargs: DescribeApplicationsRequestRequestTypeDef = {  # (1)
    "ApplicationIds": ...,
}

parent.describe_applications(**kwargs)
```

1. See [:material-code-braces: DescribeApplicationsRequestRequestTypeDef](./type_defs.md#describeapplicationsrequestrequesttypedef) 

### describe\_bundle\_associations

Describes the associations between the applications and the specified bundle.

Type annotations and code completion for `#!python session.client("workspaces").describe_bundle_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_bundle_associations method definition

await def describe_bundle_associations(
    self,
    *,
    BundleId: str,
    AssociatedResourceTypes: Sequence[BundleAssociatedResourceTypeType],  # (1)
) -> DescribeBundleAssociationsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: BundleAssociatedResourceTypeType](./literals.md#bundleassociatedresourcetypetype) 
2. See [:material-code-braces: DescribeBundleAssociationsResultTypeDef](./type_defs.md#describebundleassociationsresulttypedef) 


```python
# describe_bundle_associations method usage example with argument unpacking

kwargs: DescribeBundleAssociationsRequestRequestTypeDef = {  # (1)
    "BundleId": ...,
    "AssociatedResourceTypes": ...,
}

parent.describe_bundle_associations(**kwargs)
```

1. See [:material-code-braces: DescribeBundleAssociationsRequestRequestTypeDef](./type_defs.md#describebundleassociationsrequestrequesttypedef) 

### describe\_client\_branding

Describes the specified client branding.

Type annotations and code completion for `#!python session.client("workspaces").describe_client_branding` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_client_branding method definition

await def describe_client_branding(
    self,
    *,
    ResourceId: str,
) -> DescribeClientBrandingResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeClientBrandingResultTypeDef](./type_defs.md#describeclientbrandingresulttypedef) 


```python
# describe_client_branding method usage example with argument unpacking

kwargs: DescribeClientBrandingRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
}

parent.describe_client_branding(**kwargs)
```

1. See [:material-code-braces: DescribeClientBrandingRequestRequestTypeDef](./type_defs.md#describeclientbrandingrequestrequesttypedef) 

### describe\_client\_properties

Retrieves a list that describes one or more specified Amazon WorkSpaces clients.

Type annotations and code completion for `#!python session.client("workspaces").describe_client_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_client_properties method definition

await def describe_client_properties(
    self,
    *,
    ResourceIds: Sequence[str],
) -> DescribeClientPropertiesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeClientPropertiesResultTypeDef](./type_defs.md#describeclientpropertiesresulttypedef) 


```python
# describe_client_properties method usage example with argument unpacking

kwargs: DescribeClientPropertiesRequestRequestTypeDef = {  # (1)
    "ResourceIds": ...,
}

parent.describe_client_properties(**kwargs)
```

1. See [:material-code-braces: DescribeClientPropertiesRequestRequestTypeDef](./type_defs.md#describeclientpropertiesrequestrequesttypedef) 

### describe\_connect\_client\_add\_ins

Retrieves a list of Amazon Connect client add-ins that have been created.

Type annotations and code completion for `#!python session.client("workspaces").describe_connect_client_add_ins` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_connect_client_add_ins method definition

await def describe_connect_client_add_ins(
    self,
    *,
    ResourceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeConnectClientAddInsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeConnectClientAddInsResultTypeDef](./type_defs.md#describeconnectclientaddinsresulttypedef) 


```python
# describe_connect_client_add_ins method usage example with argument unpacking

kwargs: DescribeConnectClientAddInsRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
}

parent.describe_connect_client_add_ins(**kwargs)
```

1. See [:material-code-braces: DescribeConnectClientAddInsRequestRequestTypeDef](./type_defs.md#describeconnectclientaddinsrequestrequesttypedef) 

### describe\_connection\_alias\_permissions

Describes the permissions that the owner of a connection alias has granted to
another Amazon Web Services account for the specified connection alias.

Type annotations and code completion for `#!python session.client("workspaces").describe_connection_alias_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_connection_alias_permissions method definition

await def describe_connection_alias_permissions(
    self,
    *,
    AliasId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeConnectionAliasPermissionsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeConnectionAliasPermissionsResultTypeDef](./type_defs.md#describeconnectionaliaspermissionsresulttypedef) 


```python
# describe_connection_alias_permissions method usage example with argument unpacking

kwargs: DescribeConnectionAliasPermissionsRequestRequestTypeDef = {  # (1)
    "AliasId": ...,
}

parent.describe_connection_alias_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeConnectionAliasPermissionsRequestRequestTypeDef](./type_defs.md#describeconnectionaliaspermissionsrequestrequesttypedef) 

### describe\_connection\_aliases

Retrieves a list that describes the connection aliases used for cross-Region
redirection.

Type annotations and code completion for `#!python session.client("workspaces").describe_connection_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_connection_aliases method definition

await def describe_connection_aliases(
    self,
    *,
    AliasIds: Sequence[str] = ...,
    ResourceId: str = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeConnectionAliasesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeConnectionAliasesResultTypeDef](./type_defs.md#describeconnectionaliasesresulttypedef) 


```python
# describe_connection_aliases method usage example with argument unpacking

kwargs: DescribeConnectionAliasesRequestRequestTypeDef = {  # (1)
    "AliasIds": ...,
}

parent.describe_connection_aliases(**kwargs)
```

1. See [:material-code-braces: DescribeConnectionAliasesRequestRequestTypeDef](./type_defs.md#describeconnectionaliasesrequestrequesttypedef) 

### describe\_image\_associations

Describes the associations between the applications and the specified image.

Type annotations and code completion for `#!python session.client("workspaces").describe_image_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_image_associations method definition

await def describe_image_associations(
    self,
    *,
    ImageId: str,
    AssociatedResourceTypes: Sequence[ImageAssociatedResourceTypeType],  # (1)
) -> DescribeImageAssociationsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ImageAssociatedResourceTypeType](./literals.md#imageassociatedresourcetypetype) 
2. See [:material-code-braces: DescribeImageAssociationsResultTypeDef](./type_defs.md#describeimageassociationsresulttypedef) 


```python
# describe_image_associations method usage example with argument unpacking

kwargs: DescribeImageAssociationsRequestRequestTypeDef = {  # (1)
    "ImageId": ...,
    "AssociatedResourceTypes": ...,
}

parent.describe_image_associations(**kwargs)
```

1. See [:material-code-braces: DescribeImageAssociationsRequestRequestTypeDef](./type_defs.md#describeimageassociationsrequestrequesttypedef) 

### describe\_ip\_groups

Describes one or more of your IP access control groups.

Type annotations and code completion for `#!python session.client("workspaces").describe_ip_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_ip_groups method definition

await def describe_ip_groups(
    self,
    *,
    GroupIds: Sequence[str] = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeIpGroupsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeIpGroupsResultTypeDef](./type_defs.md#describeipgroupsresulttypedef) 


```python
# describe_ip_groups method usage example with argument unpacking

kwargs: DescribeIpGroupsRequestRequestTypeDef = {  # (1)
    "GroupIds": ...,
}

parent.describe_ip_groups(**kwargs)
```

1. See [:material-code-braces: DescribeIpGroupsRequestRequestTypeDef](./type_defs.md#describeipgroupsrequestrequesttypedef) 

### describe\_tags

Describes the specified tags for the specified WorkSpaces resource.

Type annotations and code completion for `#!python session.client("workspaces").describe_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_tags method definition

await def describe_tags(
    self,
    *,
    ResourceId: str,
) -> DescribeTagsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTagsResultTypeDef](./type_defs.md#describetagsresulttypedef) 


```python
# describe_tags method usage example with argument unpacking

kwargs: DescribeTagsRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
}

parent.describe_tags(**kwargs)
```

1. See [:material-code-braces: DescribeTagsRequestRequestTypeDef](./type_defs.md#describetagsrequestrequesttypedef) 

### describe\_workspace\_associations

Describes the associations betweens applications and the specified WorkSpace.

Type annotations and code completion for `#!python session.client("workspaces").describe_workspace_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_workspace_associations method definition

await def describe_workspace_associations(
    self,
    *,
    WorkspaceId: str,
    AssociatedResourceTypes: Sequence[WorkSpaceAssociatedResourceTypeType],  # (1)
) -> DescribeWorkspaceAssociationsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: WorkSpaceAssociatedResourceTypeType](./literals.md#workspaceassociatedresourcetypetype) 
2. See [:material-code-braces: DescribeWorkspaceAssociationsResultTypeDef](./type_defs.md#describeworkspaceassociationsresulttypedef) 


```python
# describe_workspace_associations method usage example with argument unpacking

kwargs: DescribeWorkspaceAssociationsRequestRequestTypeDef = {  # (1)
    "WorkspaceId": ...,
    "AssociatedResourceTypes": ...,
}

parent.describe_workspace_associations(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceAssociationsRequestRequestTypeDef](./type_defs.md#describeworkspaceassociationsrequestrequesttypedef) 

### describe\_workspace\_bundles

Retrieves a list that describes the available WorkSpace bundles.

Type annotations and code completion for `#!python session.client("workspaces").describe_workspace_bundles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_workspace_bundles method definition

await def describe_workspace_bundles(
    self,
    *,
    BundleIds: Sequence[str] = ...,
    Owner: str = ...,
    NextToken: str = ...,
) -> DescribeWorkspaceBundlesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWorkspaceBundlesResultTypeDef](./type_defs.md#describeworkspacebundlesresulttypedef) 


```python
# describe_workspace_bundles method usage example with argument unpacking

kwargs: DescribeWorkspaceBundlesRequestRequestTypeDef = {  # (1)
    "BundleIds": ...,
}

parent.describe_workspace_bundles(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceBundlesRequestRequestTypeDef](./type_defs.md#describeworkspacebundlesrequestrequesttypedef) 

### describe\_workspace\_directories

Describes the available directories that are registered with Amazon WorkSpaces.

Type annotations and code completion for `#!python session.client("workspaces").describe_workspace_directories` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_workspace_directories method definition

await def describe_workspace_directories(
    self,
    *,
    DirectoryIds: Sequence[str] = ...,
    WorkspaceDirectoryNames: Sequence[str] = ...,
    Limit: int = ...,
    NextToken: str = ...,
    Filters: Sequence[DescribeWorkspaceDirectoriesFilterTypeDef] = ...,  # (1)
) -> DescribeWorkspaceDirectoriesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DescribeWorkspaceDirectoriesFilterTypeDef](./type_defs.md#describeworkspacedirectoriesfiltertypedef) 
2. See [:material-code-braces: DescribeWorkspaceDirectoriesResultTypeDef](./type_defs.md#describeworkspacedirectoriesresulttypedef) 


```python
# describe_workspace_directories method usage example with argument unpacking

kwargs: DescribeWorkspaceDirectoriesRequestRequestTypeDef = {  # (1)
    "DirectoryIds": ...,
}

parent.describe_workspace_directories(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceDirectoriesRequestRequestTypeDef](./type_defs.md#describeworkspacedirectoriesrequestrequesttypedef) 

### describe\_workspace\_image\_permissions

Describes the permissions that the owner of an image has granted to other
Amazon Web Services accounts for an image.

Type annotations and code completion for `#!python session.client("workspaces").describe_workspace_image_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_workspace_image_permissions method definition

await def describe_workspace_image_permissions(
    self,
    *,
    ImageId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeWorkspaceImagePermissionsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWorkspaceImagePermissionsResultTypeDef](./type_defs.md#describeworkspaceimagepermissionsresulttypedef) 


```python
# describe_workspace_image_permissions method usage example with argument unpacking

kwargs: DescribeWorkspaceImagePermissionsRequestRequestTypeDef = {  # (1)
    "ImageId": ...,
}

parent.describe_workspace_image_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceImagePermissionsRequestRequestTypeDef](./type_defs.md#describeworkspaceimagepermissionsrequestrequesttypedef) 

### describe\_workspace\_images

Retrieves a list that describes one or more specified images, if the image
identifiers are provided.

Type annotations and code completion for `#!python session.client("workspaces").describe_workspace_images` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_workspace_images method definition

await def describe_workspace_images(
    self,
    *,
    ImageIds: Sequence[str] = ...,
    ImageType: ImageTypeType = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeWorkspaceImagesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ImageTypeType](./literals.md#imagetypetype) 
2. See [:material-code-braces: DescribeWorkspaceImagesResultTypeDef](./type_defs.md#describeworkspaceimagesresulttypedef) 


```python
# describe_workspace_images method usage example with argument unpacking

kwargs: DescribeWorkspaceImagesRequestRequestTypeDef = {  # (1)
    "ImageIds": ...,
}

parent.describe_workspace_images(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceImagesRequestRequestTypeDef](./type_defs.md#describeworkspaceimagesrequestrequesttypedef) 

### describe\_workspace\_snapshots

Describes the snapshots for the specified WorkSpace.

Type annotations and code completion for `#!python session.client("workspaces").describe_workspace_snapshots` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_workspace_snapshots method definition

await def describe_workspace_snapshots(
    self,
    *,
    WorkspaceId: str,
) -> DescribeWorkspaceSnapshotsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWorkspaceSnapshotsResultTypeDef](./type_defs.md#describeworkspacesnapshotsresulttypedef) 


```python
# describe_workspace_snapshots method usage example with argument unpacking

kwargs: DescribeWorkspaceSnapshotsRequestRequestTypeDef = {  # (1)
    "WorkspaceId": ...,
}

parent.describe_workspace_snapshots(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceSnapshotsRequestRequestTypeDef](./type_defs.md#describeworkspacesnapshotsrequestrequesttypedef) 

### describe\_workspaces

Describes the specified WorkSpaces.

Type annotations and code completion for `#!python session.client("workspaces").describe_workspaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_workspaces method definition

await def describe_workspaces(
    self,
    *,
    WorkspaceIds: Sequence[str] = ...,
    DirectoryId: str = ...,
    UserName: str = ...,
    BundleId: str = ...,
    Limit: int = ...,
    NextToken: str = ...,
    WorkspaceName: str = ...,
) -> DescribeWorkspacesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWorkspacesResultTypeDef](./type_defs.md#describeworkspacesresulttypedef) 


```python
# describe_workspaces method usage example with argument unpacking

kwargs: DescribeWorkspacesRequestRequestTypeDef = {  # (1)
    "WorkspaceIds": ...,
}

parent.describe_workspaces(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspacesRequestRequestTypeDef](./type_defs.md#describeworkspacesrequestrequesttypedef) 

### describe\_workspaces\_connection\_status

Describes the connection status of the specified WorkSpaces.

Type annotations and code completion for `#!python session.client("workspaces").describe_workspaces_connection_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_workspaces_connection_status method definition

await def describe_workspaces_connection_status(
    self,
    *,
    WorkspaceIds: Sequence[str] = ...,
    NextToken: str = ...,
) -> DescribeWorkspacesConnectionStatusResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWorkspacesConnectionStatusResultTypeDef](./type_defs.md#describeworkspacesconnectionstatusresulttypedef) 


```python
# describe_workspaces_connection_status method usage example with argument unpacking

kwargs: DescribeWorkspacesConnectionStatusRequestRequestTypeDef = {  # (1)
    "WorkspaceIds": ...,
}

parent.describe_workspaces_connection_status(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspacesConnectionStatusRequestRequestTypeDef](./type_defs.md#describeworkspacesconnectionstatusrequestrequesttypedef) 

### describe\_workspaces\_pool\_sessions

Retrieves a list that describes the streaming sessions for a specified pool.

Type annotations and code completion for `#!python session.client("workspaces").describe_workspaces_pool_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_workspaces_pool_sessions method definition

await def describe_workspaces_pool_sessions(
    self,
    *,
    PoolId: str,
    UserId: str = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeWorkspacesPoolSessionsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWorkspacesPoolSessionsResultTypeDef](./type_defs.md#describeworkspacespoolsessionsresulttypedef) 


```python
# describe_workspaces_pool_sessions method usage example with argument unpacking

kwargs: DescribeWorkspacesPoolSessionsRequestRequestTypeDef = {  # (1)
    "PoolId": ...,
}

parent.describe_workspaces_pool_sessions(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspacesPoolSessionsRequestRequestTypeDef](./type_defs.md#describeworkspacespoolsessionsrequestrequesttypedef) 

### describe\_workspaces\_pools

Describes the specified WorkSpaces Pools.

Type annotations and code completion for `#!python session.client("workspaces").describe_workspaces_pools` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# describe_workspaces_pools method definition

await def describe_workspaces_pools(
    self,
    *,
    PoolIds: Sequence[str] = ...,
    Filters: Sequence[DescribeWorkspacesPoolsFilterTypeDef] = ...,  # (1)
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeWorkspacesPoolsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DescribeWorkspacesPoolsFilterTypeDef](./type_defs.md#describeworkspacespoolsfiltertypedef) 
2. See [:material-code-braces: DescribeWorkspacesPoolsResultTypeDef](./type_defs.md#describeworkspacespoolsresulttypedef) 


```python
# describe_workspaces_pools method usage example with argument unpacking

kwargs: DescribeWorkspacesPoolsRequestRequestTypeDef = {  # (1)
    "PoolIds": ...,
}

parent.describe_workspaces_pools(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspacesPoolsRequestRequestTypeDef](./type_defs.md#describeworkspacespoolsrequestrequesttypedef) 

### disassociate\_connection\_alias

Disassociates a connection alias from a directory.

Type annotations and code completion for `#!python session.client("workspaces").disassociate_connection_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# disassociate_connection_alias method definition

await def disassociate_connection_alias(
    self,
    *,
    AliasId: str,
) -> dict[str, Any]:
    ...
```



```python
# disassociate_connection_alias method usage example with argument unpacking

kwargs: DisassociateConnectionAliasRequestRequestTypeDef = {  # (1)
    "AliasId": ...,
}

parent.disassociate_connection_alias(**kwargs)
```

1. See [:material-code-braces: DisassociateConnectionAliasRequestRequestTypeDef](./type_defs.md#disassociateconnectionaliasrequestrequesttypedef) 

### disassociate\_ip\_groups

Disassociates the specified IP access control group from the specified
directory.

Type annotations and code completion for `#!python session.client("workspaces").disassociate_ip_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# disassociate_ip_groups method definition

await def disassociate_ip_groups(
    self,
    *,
    DirectoryId: str,
    GroupIds: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# disassociate_ip_groups method usage example with argument unpacking

kwargs: DisassociateIpGroupsRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
    "GroupIds": ...,
}

parent.disassociate_ip_groups(**kwargs)
```

1. See [:material-code-braces: DisassociateIpGroupsRequestRequestTypeDef](./type_defs.md#disassociateipgroupsrequestrequesttypedef) 

### disassociate\_workspace\_application

Disassociates the specified application from a WorkSpace.

Type annotations and code completion for `#!python session.client("workspaces").disassociate_workspace_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# disassociate_workspace_application method definition

await def disassociate_workspace_application(
    self,
    *,
    WorkspaceId: str,
    ApplicationId: str,
) -> DisassociateWorkspaceApplicationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisassociateWorkspaceApplicationResultTypeDef](./type_defs.md#disassociateworkspaceapplicationresulttypedef) 


```python
# disassociate_workspace_application method usage example with argument unpacking

kwargs: DisassociateWorkspaceApplicationRequestRequestTypeDef = {  # (1)
    "WorkspaceId": ...,
    "ApplicationId": ...,
}

parent.disassociate_workspace_application(**kwargs)
```

1. See [:material-code-braces: DisassociateWorkspaceApplicationRequestRequestTypeDef](./type_defs.md#disassociateworkspaceapplicationrequestrequesttypedef) 

### get\_account\_link

Retrieves account link information.

Type annotations and code completion for `#!python session.client("workspaces").get_account_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# get_account_link method definition

await def get_account_link(
    self,
    *,
    LinkId: str = ...,
    LinkedAccountId: str = ...,
) -> GetAccountLinkResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccountLinkResultTypeDef](./type_defs.md#getaccountlinkresulttypedef) 


```python
# get_account_link method usage example with argument unpacking

kwargs: GetAccountLinkRequestRequestTypeDef = {  # (1)
    "LinkId": ...,
}

parent.get_account_link(**kwargs)
```

1. See [:material-code-braces: GetAccountLinkRequestRequestTypeDef](./type_defs.md#getaccountlinkrequestrequesttypedef) 

### import\_client\_branding

Imports client branding.

Type annotations and code completion for `#!python session.client("workspaces").import_client_branding` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# import_client_branding method definition

await def import_client_branding(
    self,
    *,
    ResourceId: str,
    DeviceTypeWindows: DefaultImportClientBrandingAttributesTypeDef = ...,  # (1)
    DeviceTypeOsx: DefaultImportClientBrandingAttributesTypeDef = ...,  # (1)
    DeviceTypeAndroid: DefaultImportClientBrandingAttributesTypeDef = ...,  # (1)
    DeviceTypeIos: IosImportClientBrandingAttributesTypeDef = ...,  # (4)
    DeviceTypeLinux: DefaultImportClientBrandingAttributesTypeDef = ...,  # (1)
    DeviceTypeWeb: DefaultImportClientBrandingAttributesTypeDef = ...,  # (1)
) -> ImportClientBrandingResultTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: DefaultImportClientBrandingAttributesTypeDef](./type_defs.md#defaultimportclientbrandingattributestypedef) 
2. See [:material-code-braces: DefaultImportClientBrandingAttributesTypeDef](./type_defs.md#defaultimportclientbrandingattributestypedef) 
3. See [:material-code-braces: DefaultImportClientBrandingAttributesTypeDef](./type_defs.md#defaultimportclientbrandingattributestypedef) 
4. See [:material-code-braces: IosImportClientBrandingAttributesTypeDef](./type_defs.md#iosimportclientbrandingattributestypedef) 
5. See [:material-code-braces: DefaultImportClientBrandingAttributesTypeDef](./type_defs.md#defaultimportclientbrandingattributestypedef) 
6. See [:material-code-braces: DefaultImportClientBrandingAttributesTypeDef](./type_defs.md#defaultimportclientbrandingattributestypedef) 
7. See [:material-code-braces: ImportClientBrandingResultTypeDef](./type_defs.md#importclientbrandingresulttypedef) 


```python
# import_client_branding method usage example with argument unpacking

kwargs: ImportClientBrandingRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
}

parent.import_client_branding(**kwargs)
```

1. See [:material-code-braces: ImportClientBrandingRequestRequestTypeDef](./type_defs.md#importclientbrandingrequestrequesttypedef) 

### import\_workspace\_image

Imports the specified Windows 10 or 11 Bring Your Own License (BYOL) image into
Amazon WorkSpaces.

Type annotations and code completion for `#!python session.client("workspaces").import_workspace_image` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# import_workspace_image method definition

await def import_workspace_image(
    self,
    *,
    Ec2ImageId: str,
    IngestionProcess: WorkspaceImageIngestionProcessType,  # (1)
    ImageName: str,
    ImageDescription: str,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    Applications: Sequence[ApplicationType] = ...,  # (3)
) -> ImportWorkspaceImageResultTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: WorkspaceImageIngestionProcessType](./literals.md#workspaceimageingestionprocesstype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: ApplicationType](./literals.md#applicationtype) 
4. See [:material-code-braces: ImportWorkspaceImageResultTypeDef](./type_defs.md#importworkspaceimageresulttypedef) 


```python
# import_workspace_image method usage example with argument unpacking

kwargs: ImportWorkspaceImageRequestRequestTypeDef = {  # (1)
    "Ec2ImageId": ...,
    "IngestionProcess": ...,
    "ImageName": ...,
    "ImageDescription": ...,
}

parent.import_workspace_image(**kwargs)
```

1. See [:material-code-braces: ImportWorkspaceImageRequestRequestTypeDef](./type_defs.md#importworkspaceimagerequestrequesttypedef) 

### list\_account\_links

Lists all account links.

Type annotations and code completion for `#!python session.client("workspaces").list_account_links` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# list_account_links method definition

await def list_account_links(
    self,
    *,
    LinkStatusFilter: Sequence[AccountLinkStatusEnumType] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAccountLinksResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AccountLinkStatusEnumType](./literals.md#accountlinkstatusenumtype) 
2. See [:material-code-braces: ListAccountLinksResultTypeDef](./type_defs.md#listaccountlinksresulttypedef) 


```python
# list_account_links method usage example with argument unpacking

kwargs: ListAccountLinksRequestRequestTypeDef = {  # (1)
    "LinkStatusFilter": ...,
}

parent.list_account_links(**kwargs)
```

1. See [:material-code-braces: ListAccountLinksRequestRequestTypeDef](./type_defs.md#listaccountlinksrequestrequesttypedef) 

### list\_available\_management\_cidr\_ranges

Retrieves a list of IP address ranges, specified as IPv4 CIDR blocks, that you
can use for the network management interface when you enable Bring Your Own
License (BYOL).

Type annotations and code completion for `#!python session.client("workspaces").list_available_management_cidr_ranges` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# list_available_management_cidr_ranges method definition

await def list_available_management_cidr_ranges(
    self,
    *,
    ManagementCidrRangeConstraint: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAvailableManagementCidrRangesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAvailableManagementCidrRangesResultTypeDef](./type_defs.md#listavailablemanagementcidrrangesresulttypedef) 


```python
# list_available_management_cidr_ranges method usage example with argument unpacking

kwargs: ListAvailableManagementCidrRangesRequestRequestTypeDef = {  # (1)
    "ManagementCidrRangeConstraint": ...,
}

parent.list_available_management_cidr_ranges(**kwargs)
```

1. See [:material-code-braces: ListAvailableManagementCidrRangesRequestRequestTypeDef](./type_defs.md#listavailablemanagementcidrrangesrequestrequesttypedef) 

### migrate\_workspace

Migrates a WorkSpace from one operating system or bundle type to another, while
retaining the data on the user volume.

Type annotations and code completion for `#!python session.client("workspaces").migrate_workspace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# migrate_workspace method definition

await def migrate_workspace(
    self,
    *,
    SourceWorkspaceId: str,
    BundleId: str,
) -> MigrateWorkspaceResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: MigrateWorkspaceResultTypeDef](./type_defs.md#migrateworkspaceresulttypedef) 


```python
# migrate_workspace method usage example with argument unpacking

kwargs: MigrateWorkspaceRequestRequestTypeDef = {  # (1)
    "SourceWorkspaceId": ...,
    "BundleId": ...,
}

parent.migrate_workspace(**kwargs)
```

1. See [:material-code-braces: MigrateWorkspaceRequestRequestTypeDef](./type_defs.md#migrateworkspacerequestrequesttypedef) 

### modify\_account

Modifies the configuration of Bring Your Own License (BYOL) for the specified
account.

Type annotations and code completion for `#!python session.client("workspaces").modify_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# modify_account method definition

await def modify_account(
    self,
    *,
    DedicatedTenancySupport: DedicatedTenancySupportEnumType = ...,  # (1)
    DedicatedTenancyManagementCidrRange: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: DedicatedTenancySupportEnumType](./literals.md#dedicatedtenancysupportenumtype) 


```python
# modify_account method usage example with argument unpacking

kwargs: ModifyAccountRequestRequestTypeDef = {  # (1)
    "DedicatedTenancySupport": ...,
}

parent.modify_account(**kwargs)
```

1. See [:material-code-braces: ModifyAccountRequestRequestTypeDef](./type_defs.md#modifyaccountrequestrequesttypedef) 

### modify\_certificate\_based\_auth\_properties

Modifies the properties of the certificate-based authentication you want to use
with your WorkSpaces.

Type annotations and code completion for `#!python session.client("workspaces").modify_certificate_based_auth_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# modify_certificate_based_auth_properties method definition

await def modify_certificate_based_auth_properties(
    self,
    *,
    ResourceId: str,
    CertificateBasedAuthProperties: CertificateBasedAuthPropertiesTypeDef = ...,  # (1)
    PropertiesToDelete: Sequence[DeletableCertificateBasedAuthPropertyType] = ...,  # (2)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: CertificateBasedAuthPropertiesTypeDef](./type_defs.md#certificatebasedauthpropertiestypedef) 
2. See [:material-code-brackets: DeletableCertificateBasedAuthPropertyType](./literals.md#deletablecertificatebasedauthpropertytype) 


```python
# modify_certificate_based_auth_properties method usage example with argument unpacking

kwargs: ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
}

parent.modify_certificate_based_auth_properties(**kwargs)
```

1. See [:material-code-braces: ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef](./type_defs.md#modifycertificatebasedauthpropertiesrequestrequesttypedef) 

### modify\_client\_properties

Modifies the properties of the specified Amazon WorkSpaces clients.

Type annotations and code completion for `#!python session.client("workspaces").modify_client_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# modify_client_properties method definition

await def modify_client_properties(
    self,
    *,
    ResourceId: str,
    ClientProperties: ClientPropertiesTypeDef,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: ClientPropertiesTypeDef](./type_defs.md#clientpropertiestypedef) 


```python
# modify_client_properties method usage example with argument unpacking

kwargs: ModifyClientPropertiesRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
    "ClientProperties": ...,
}

parent.modify_client_properties(**kwargs)
```

1. See [:material-code-braces: ModifyClientPropertiesRequestRequestTypeDef](./type_defs.md#modifyclientpropertiesrequestrequesttypedef) 

### modify\_saml\_properties

Modifies multiple properties related to SAML 2.0 authentication, including the
enablement status, user access URL, and relay state parameter name that are
used for configuring federation with an SAML 2.0 identity provider.

Type annotations and code completion for `#!python session.client("workspaces").modify_saml_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# modify_saml_properties method definition

await def modify_saml_properties(
    self,
    *,
    ResourceId: str,
    SamlProperties: SamlPropertiesTypeDef = ...,  # (1)
    PropertiesToDelete: Sequence[DeletableSamlPropertyType] = ...,  # (2)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: SamlPropertiesTypeDef](./type_defs.md#samlpropertiestypedef) 
2. See [:material-code-brackets: DeletableSamlPropertyType](./literals.md#deletablesamlpropertytype) 


```python
# modify_saml_properties method usage example with argument unpacking

kwargs: ModifySamlPropertiesRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
}

parent.modify_saml_properties(**kwargs)
```

1. See [:material-code-braces: ModifySamlPropertiesRequestRequestTypeDef](./type_defs.md#modifysamlpropertiesrequestrequesttypedef) 

### modify\_selfservice\_permissions

Modifies the self-service WorkSpace management capabilities for your users.

Type annotations and code completion for `#!python session.client("workspaces").modify_selfservice_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# modify_selfservice_permissions method definition

await def modify_selfservice_permissions(
    self,
    *,
    ResourceId: str,
    SelfservicePermissions: SelfservicePermissionsTypeDef,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: SelfservicePermissionsTypeDef](./type_defs.md#selfservicepermissionstypedef) 


```python
# modify_selfservice_permissions method usage example with argument unpacking

kwargs: ModifySelfservicePermissionsRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
    "SelfservicePermissions": ...,
}

parent.modify_selfservice_permissions(**kwargs)
```

1. See [:material-code-braces: ModifySelfservicePermissionsRequestRequestTypeDef](./type_defs.md#modifyselfservicepermissionsrequestrequesttypedef) 

### modify\_streaming\_properties

Modifies the specified streaming properties.

Type annotations and code completion for `#!python session.client("workspaces").modify_streaming_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# modify_streaming_properties method definition

await def modify_streaming_properties(
    self,
    *,
    ResourceId: str,
    StreamingProperties: StreamingPropertiesTypeDef = ...,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: StreamingPropertiesTypeDef](./type_defs.md#streamingpropertiestypedef) 


```python
# modify_streaming_properties method usage example with argument unpacking

kwargs: ModifyStreamingPropertiesRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
}

parent.modify_streaming_properties(**kwargs)
```

1. See [:material-code-braces: ModifyStreamingPropertiesRequestRequestTypeDef](./type_defs.md#modifystreamingpropertiesrequestrequesttypedef) 

### modify\_workspace\_access\_properties

Specifies which devices and operating systems users can use to access their
WorkSpaces.

Type annotations and code completion for `#!python session.client("workspaces").modify_workspace_access_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# modify_workspace_access_properties method definition

await def modify_workspace_access_properties(
    self,
    *,
    ResourceId: str,
    WorkspaceAccessProperties: WorkspaceAccessPropertiesTypeDef,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: WorkspaceAccessPropertiesTypeDef](./type_defs.md#workspaceaccesspropertiestypedef) 


```python
# modify_workspace_access_properties method usage example with argument unpacking

kwargs: ModifyWorkspaceAccessPropertiesRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
    "WorkspaceAccessProperties": ...,
}

parent.modify_workspace_access_properties(**kwargs)
```

1. See [:material-code-braces: ModifyWorkspaceAccessPropertiesRequestRequestTypeDef](./type_defs.md#modifyworkspaceaccesspropertiesrequestrequesttypedef) 

### modify\_workspace\_creation\_properties

Modify the default properties used to create WorkSpaces.

Type annotations and code completion for `#!python session.client("workspaces").modify_workspace_creation_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# modify_workspace_creation_properties method definition

await def modify_workspace_creation_properties(
    self,
    *,
    ResourceId: str,
    WorkspaceCreationProperties: WorkspaceCreationPropertiesTypeDef,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: WorkspaceCreationPropertiesTypeDef](./type_defs.md#workspacecreationpropertiestypedef) 


```python
# modify_workspace_creation_properties method usage example with argument unpacking

kwargs: ModifyWorkspaceCreationPropertiesRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
    "WorkspaceCreationProperties": ...,
}

parent.modify_workspace_creation_properties(**kwargs)
```

1. See [:material-code-braces: ModifyWorkspaceCreationPropertiesRequestRequestTypeDef](./type_defs.md#modifyworkspacecreationpropertiesrequestrequesttypedef) 

### modify\_workspace\_properties

Modifies the specified WorkSpace properties.

Type annotations and code completion for `#!python session.client("workspaces").modify_workspace_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# modify_workspace_properties method definition

await def modify_workspace_properties(
    self,
    *,
    WorkspaceId: str,
    WorkspaceProperties: WorkspacePropertiesTypeDef = ...,  # (1)
    DataReplication: DataReplicationType = ...,  # (2)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: WorkspacePropertiesTypeDef](./type_defs.md#workspacepropertiestypedef) 
2. See [:material-code-brackets: DataReplicationType](./literals.md#datareplicationtype) 


```python
# modify_workspace_properties method usage example with argument unpacking

kwargs: ModifyWorkspacePropertiesRequestRequestTypeDef = {  # (1)
    "WorkspaceId": ...,
}

parent.modify_workspace_properties(**kwargs)
```

1. See [:material-code-braces: ModifyWorkspacePropertiesRequestRequestTypeDef](./type_defs.md#modifyworkspacepropertiesrequestrequesttypedef) 

### modify\_workspace\_state

Sets the state of the specified WorkSpace.

Type annotations and code completion for `#!python session.client("workspaces").modify_workspace_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# modify_workspace_state method definition

await def modify_workspace_state(
    self,
    *,
    WorkspaceId: str,
    WorkspaceState: TargetWorkspaceStateType,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: TargetWorkspaceStateType](./literals.md#targetworkspacestatetype) 


```python
# modify_workspace_state method usage example with argument unpacking

kwargs: ModifyWorkspaceStateRequestRequestTypeDef = {  # (1)
    "WorkspaceId": ...,
    "WorkspaceState": ...,
}

parent.modify_workspace_state(**kwargs)
```

1. See [:material-code-braces: ModifyWorkspaceStateRequestRequestTypeDef](./type_defs.md#modifyworkspacestaterequestrequesttypedef) 

### reboot\_workspaces

Reboots the specified WorkSpaces.

Type annotations and code completion for `#!python session.client("workspaces").reboot_workspaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# reboot_workspaces method definition

await def reboot_workspaces(
    self,
    *,
    RebootWorkspaceRequests: Sequence[RebootRequestTypeDef],  # (1)
) -> RebootWorkspacesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RebootRequestTypeDef](./type_defs.md#rebootrequesttypedef) 
2. See [:material-code-braces: RebootWorkspacesResultTypeDef](./type_defs.md#rebootworkspacesresulttypedef) 


```python
# reboot_workspaces method usage example with argument unpacking

kwargs: RebootWorkspacesRequestRequestTypeDef = {  # (1)
    "RebootWorkspaceRequests": ...,
}

parent.reboot_workspaces(**kwargs)
```

1. See [:material-code-braces: RebootWorkspacesRequestRequestTypeDef](./type_defs.md#rebootworkspacesrequestrequesttypedef) 

### rebuild\_workspaces

Rebuilds the specified WorkSpace.

Type annotations and code completion for `#!python session.client("workspaces").rebuild_workspaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# rebuild_workspaces method definition

await def rebuild_workspaces(
    self,
    *,
    RebuildWorkspaceRequests: Sequence[RebuildRequestTypeDef],  # (1)
) -> RebuildWorkspacesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RebuildRequestTypeDef](./type_defs.md#rebuildrequesttypedef) 
2. See [:material-code-braces: RebuildWorkspacesResultTypeDef](./type_defs.md#rebuildworkspacesresulttypedef) 


```python
# rebuild_workspaces method usage example with argument unpacking

kwargs: RebuildWorkspacesRequestRequestTypeDef = {  # (1)
    "RebuildWorkspaceRequests": ...,
}

parent.rebuild_workspaces(**kwargs)
```

1. See [:material-code-braces: RebuildWorkspacesRequestRequestTypeDef](./type_defs.md#rebuildworkspacesrequestrequesttypedef) 

### register\_workspace\_directory

Registers the specified directory.

Type annotations and code completion for `#!python session.client("workspaces").register_workspace_directory` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# register_workspace_directory method definition

await def register_workspace_directory(
    self,
    *,
    DirectoryId: str = ...,
    SubnetIds: Sequence[str] = ...,
    EnableWorkDocs: bool = ...,
    EnableSelfService: bool = ...,
    Tenancy: TenancyType = ...,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    WorkspaceDirectoryName: str = ...,
    WorkspaceDirectoryDescription: str = ...,
    UserIdentityType: UserIdentityTypeType = ...,  # (3)
    IdcInstanceArn: str = ...,
    MicrosoftEntraConfig: MicrosoftEntraConfigTypeDef = ...,  # (4)
    WorkspaceType: WorkspaceTypeType = ...,  # (5)
    ActiveDirectoryConfig: ActiveDirectoryConfigTypeDef = ...,  # (6)
) -> RegisterWorkspaceDirectoryResultTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: TenancyType](./literals.md#tenancytype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: UserIdentityTypeType](./literals.md#useridentitytypetype) 
4. See [:material-code-braces: MicrosoftEntraConfigTypeDef](./type_defs.md#microsoftentraconfigtypedef) 
5. See [:material-code-brackets: WorkspaceTypeType](./literals.md#workspacetypetype) 
6. See [:material-code-braces: ActiveDirectoryConfigTypeDef](./type_defs.md#activedirectoryconfigtypedef) 
7. See [:material-code-braces: RegisterWorkspaceDirectoryResultTypeDef](./type_defs.md#registerworkspacedirectoryresulttypedef) 


```python
# register_workspace_directory method usage example with argument unpacking

kwargs: RegisterWorkspaceDirectoryRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.register_workspace_directory(**kwargs)
```

1. See [:material-code-braces: RegisterWorkspaceDirectoryRequestRequestTypeDef](./type_defs.md#registerworkspacedirectoryrequestrequesttypedef) 

### reject\_account\_link\_invitation

Rejects the account link invitation.

Type annotations and code completion for `#!python session.client("workspaces").reject_account_link_invitation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# reject_account_link_invitation method definition

await def reject_account_link_invitation(
    self,
    *,
    LinkId: str,
    ClientToken: str = ...,
) -> RejectAccountLinkInvitationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RejectAccountLinkInvitationResultTypeDef](./type_defs.md#rejectaccountlinkinvitationresulttypedef) 


```python
# reject_account_link_invitation method usage example with argument unpacking

kwargs: RejectAccountLinkInvitationRequestRequestTypeDef = {  # (1)
    "LinkId": ...,
}

parent.reject_account_link_invitation(**kwargs)
```

1. See [:material-code-braces: RejectAccountLinkInvitationRequestRequestTypeDef](./type_defs.md#rejectaccountlinkinvitationrequestrequesttypedef) 

### restore\_workspace

Restores the specified WorkSpace to its last known healthy state.

Type annotations and code completion for `#!python session.client("workspaces").restore_workspace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# restore_workspace method definition

await def restore_workspace(
    self,
    *,
    WorkspaceId: str,
) -> dict[str, Any]:
    ...
```



```python
# restore_workspace method usage example with argument unpacking

kwargs: RestoreWorkspaceRequestRequestTypeDef = {  # (1)
    "WorkspaceId": ...,
}

parent.restore_workspace(**kwargs)
```

1. See [:material-code-braces: RestoreWorkspaceRequestRequestTypeDef](./type_defs.md#restoreworkspacerequestrequesttypedef) 

### revoke\_ip\_rules

Removes one or more rules from the specified IP access control group.

Type annotations and code completion for `#!python session.client("workspaces").revoke_ip_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# revoke_ip_rules method definition

await def revoke_ip_rules(
    self,
    *,
    GroupId: str,
    UserRules: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# revoke_ip_rules method usage example with argument unpacking

kwargs: RevokeIpRulesRequestRequestTypeDef = {  # (1)
    "GroupId": ...,
    "UserRules": ...,
}

parent.revoke_ip_rules(**kwargs)
```

1. See [:material-code-braces: RevokeIpRulesRequestRequestTypeDef](./type_defs.md#revokeiprulesrequestrequesttypedef) 

### start\_workspaces

Starts the specified WorkSpaces.

Type annotations and code completion for `#!python session.client("workspaces").start_workspaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# start_workspaces method definition

await def start_workspaces(
    self,
    *,
    StartWorkspaceRequests: Sequence[StartRequestTypeDef],  # (1)
) -> StartWorkspacesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StartRequestTypeDef](./type_defs.md#startrequesttypedef) 
2. See [:material-code-braces: StartWorkspacesResultTypeDef](./type_defs.md#startworkspacesresulttypedef) 


```python
# start_workspaces method usage example with argument unpacking

kwargs: StartWorkspacesRequestRequestTypeDef = {  # (1)
    "StartWorkspaceRequests": ...,
}

parent.start_workspaces(**kwargs)
```

1. See [:material-code-braces: StartWorkspacesRequestRequestTypeDef](./type_defs.md#startworkspacesrequestrequesttypedef) 

### start\_workspaces\_pool

Starts the specified pool.

Type annotations and code completion for `#!python session.client("workspaces").start_workspaces_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# start_workspaces_pool method definition

await def start_workspaces_pool(
    self,
    *,
    PoolId: str,
) -> dict[str, Any]:
    ...
```



```python
# start_workspaces_pool method usage example with argument unpacking

kwargs: StartWorkspacesPoolRequestRequestTypeDef = {  # (1)
    "PoolId": ...,
}

parent.start_workspaces_pool(**kwargs)
```

1. See [:material-code-braces: StartWorkspacesPoolRequestRequestTypeDef](./type_defs.md#startworkspacespoolrequestrequesttypedef) 

### stop\_workspaces

Stops the specified WorkSpaces.

Type annotations and code completion for `#!python session.client("workspaces").stop_workspaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# stop_workspaces method definition

await def stop_workspaces(
    self,
    *,
    StopWorkspaceRequests: Sequence[StopRequestTypeDef],  # (1)
) -> StopWorkspacesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StopRequestTypeDef](./type_defs.md#stoprequesttypedef) 
2. See [:material-code-braces: StopWorkspacesResultTypeDef](./type_defs.md#stopworkspacesresulttypedef) 


```python
# stop_workspaces method usage example with argument unpacking

kwargs: StopWorkspacesRequestRequestTypeDef = {  # (1)
    "StopWorkspaceRequests": ...,
}

parent.stop_workspaces(**kwargs)
```

1. See [:material-code-braces: StopWorkspacesRequestRequestTypeDef](./type_defs.md#stopworkspacesrequestrequesttypedef) 

### stop\_workspaces\_pool

Stops the specified pool.

Type annotations and code completion for `#!python session.client("workspaces").stop_workspaces_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# stop_workspaces_pool method definition

await def stop_workspaces_pool(
    self,
    *,
    PoolId: str,
) -> dict[str, Any]:
    ...
```



```python
# stop_workspaces_pool method usage example with argument unpacking

kwargs: StopWorkspacesPoolRequestRequestTypeDef = {  # (1)
    "PoolId": ...,
}

parent.stop_workspaces_pool(**kwargs)
```

1. See [:material-code-braces: StopWorkspacesPoolRequestRequestTypeDef](./type_defs.md#stopworkspacespoolrequestrequesttypedef) 

### terminate\_workspaces

Terminates the specified WorkSpaces.

Type annotations and code completion for `#!python session.client("workspaces").terminate_workspaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# terminate_workspaces method definition

await def terminate_workspaces(
    self,
    *,
    TerminateWorkspaceRequests: Sequence[TerminateRequestTypeDef],  # (1)
) -> TerminateWorkspacesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TerminateRequestTypeDef](./type_defs.md#terminaterequesttypedef) 
2. See [:material-code-braces: TerminateWorkspacesResultTypeDef](./type_defs.md#terminateworkspacesresulttypedef) 


```python
# terminate_workspaces method usage example with argument unpacking

kwargs: TerminateWorkspacesRequestRequestTypeDef = {  # (1)
    "TerminateWorkspaceRequests": ...,
}

parent.terminate_workspaces(**kwargs)
```

1. See [:material-code-braces: TerminateWorkspacesRequestRequestTypeDef](./type_defs.md#terminateworkspacesrequestrequesttypedef) 

### terminate\_workspaces\_pool

Terminates the specified pool.

Type annotations and code completion for `#!python session.client("workspaces").terminate_workspaces_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# terminate_workspaces_pool method definition

await def terminate_workspaces_pool(
    self,
    *,
    PoolId: str,
) -> dict[str, Any]:
    ...
```



```python
# terminate_workspaces_pool method usage example with argument unpacking

kwargs: TerminateWorkspacesPoolRequestRequestTypeDef = {  # (1)
    "PoolId": ...,
}

parent.terminate_workspaces_pool(**kwargs)
```

1. See [:material-code-braces: TerminateWorkspacesPoolRequestRequestTypeDef](./type_defs.md#terminateworkspacespoolrequestrequesttypedef) 

### terminate\_workspaces\_pool\_session

Terminates the pool session.

Type annotations and code completion for `#!python session.client("workspaces").terminate_workspaces_pool_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# terminate_workspaces_pool_session method definition

await def terminate_workspaces_pool_session(
    self,
    *,
    SessionId: str,
) -> dict[str, Any]:
    ...
```



```python
# terminate_workspaces_pool_session method usage example with argument unpacking

kwargs: TerminateWorkspacesPoolSessionRequestRequestTypeDef = {  # (1)
    "SessionId": ...,
}

parent.terminate_workspaces_pool_session(**kwargs)
```

1. See [:material-code-braces: TerminateWorkspacesPoolSessionRequestRequestTypeDef](./type_defs.md#terminateworkspacespoolsessionrequestrequesttypedef) 

### update\_connect\_client\_add\_in

Updates a Amazon Connect client add-in.

Type annotations and code completion for `#!python session.client("workspaces").update_connect_client_add_in` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# update_connect_client_add_in method definition

await def update_connect_client_add_in(
    self,
    *,
    AddInId: str,
    ResourceId: str,
    Name: str = ...,
    URL: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# update_connect_client_add_in method usage example with argument unpacking

kwargs: UpdateConnectClientAddInRequestRequestTypeDef = {  # (1)
    "AddInId": ...,
    "ResourceId": ...,
}

parent.update_connect_client_add_in(**kwargs)
```

1. See [:material-code-braces: UpdateConnectClientAddInRequestRequestTypeDef](./type_defs.md#updateconnectclientaddinrequestrequesttypedef) 

### update\_connection\_alias\_permission

Shares or unshares a connection alias with one account by specifying whether
that account has permission to associate the connection alias with a directory.

Type annotations and code completion for `#!python session.client("workspaces").update_connection_alias_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# update_connection_alias_permission method definition

await def update_connection_alias_permission(
    self,
    *,
    AliasId: str,
    ConnectionAliasPermission: ConnectionAliasPermissionTypeDef,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: ConnectionAliasPermissionTypeDef](./type_defs.md#connectionaliaspermissiontypedef) 


```python
# update_connection_alias_permission method usage example with argument unpacking

kwargs: UpdateConnectionAliasPermissionRequestRequestTypeDef = {  # (1)
    "AliasId": ...,
    "ConnectionAliasPermission": ...,
}

parent.update_connection_alias_permission(**kwargs)
```

1. See [:material-code-braces: UpdateConnectionAliasPermissionRequestRequestTypeDef](./type_defs.md#updateconnectionaliaspermissionrequestrequesttypedef) 

### update\_rules\_of\_ip\_group

Replaces the current rules of the specified IP access control group with the
specified rules.

Type annotations and code completion for `#!python session.client("workspaces").update_rules_of_ip_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# update_rules_of_ip_group method definition

await def update_rules_of_ip_group(
    self,
    *,
    GroupId: str,
    UserRules: Sequence[IpRuleItemTypeDef],  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: IpRuleItemTypeDef](./type_defs.md#ipruleitemtypedef) 


```python
# update_rules_of_ip_group method usage example with argument unpacking

kwargs: UpdateRulesOfIpGroupRequestRequestTypeDef = {  # (1)
    "GroupId": ...,
    "UserRules": ...,
}

parent.update_rules_of_ip_group(**kwargs)
```

1. See [:material-code-braces: UpdateRulesOfIpGroupRequestRequestTypeDef](./type_defs.md#updaterulesofipgrouprequestrequesttypedef) 

### update\_workspace\_bundle

Updates a WorkSpace bundle with a new image.

Type annotations and code completion for `#!python session.client("workspaces").update_workspace_bundle` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# update_workspace_bundle method definition

await def update_workspace_bundle(
    self,
    *,
    BundleId: str = ...,
    ImageId: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# update_workspace_bundle method usage example with argument unpacking

kwargs: UpdateWorkspaceBundleRequestRequestTypeDef = {  # (1)
    "BundleId": ...,
}

parent.update_workspace_bundle(**kwargs)
```

1. See [:material-code-braces: UpdateWorkspaceBundleRequestRequestTypeDef](./type_defs.md#updateworkspacebundlerequestrequesttypedef) 

### update\_workspace\_image\_permission

Shares or unshares an image with one account in the same Amazon Web Services
Region by specifying whether that account has permission to copy the image.

Type annotations and code completion for `#!python session.client("workspaces").update_workspace_image_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# update_workspace_image_permission method definition

await def update_workspace_image_permission(
    self,
    *,
    ImageId: str,
    AllowCopyImage: bool,
    SharedAccountId: str,
) -> dict[str, Any]:
    ...
```



```python
# update_workspace_image_permission method usage example with argument unpacking

kwargs: UpdateWorkspaceImagePermissionRequestRequestTypeDef = {  # (1)
    "ImageId": ...,
    "AllowCopyImage": ...,
    "SharedAccountId": ...,
}

parent.update_workspace_image_permission(**kwargs)
```

1. See [:material-code-braces: UpdateWorkspaceImagePermissionRequestRequestTypeDef](./type_defs.md#updateworkspaceimagepermissionrequestrequesttypedef) 

### update\_workspaces\_pool

Updates the specified pool.

Type annotations and code completion for `#!python session.client("workspaces").update_workspaces_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# update_workspaces_pool method definition

await def update_workspaces_pool(
    self,
    *,
    PoolId: str,
    Description: str = ...,
    BundleId: str = ...,
    DirectoryId: str = ...,
    Capacity: CapacityTypeDef = ...,  # (1)
    ApplicationSettings: ApplicationSettingsRequestTypeDef = ...,  # (2)
    TimeoutSettings: TimeoutSettingsTypeDef = ...,  # (3)
) -> UpdateWorkspacesPoolResultTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: CapacityTypeDef](./type_defs.md#capacitytypedef) 
2. See [:material-code-braces: ApplicationSettingsRequestTypeDef](./type_defs.md#applicationsettingsrequesttypedef) 
3. See [:material-code-braces: TimeoutSettingsTypeDef](./type_defs.md#timeoutsettingstypedef) 
4. See [:material-code-braces: UpdateWorkspacesPoolResultTypeDef](./type_defs.md#updateworkspacespoolresulttypedef) 


```python
# update_workspaces_pool method usage example with argument unpacking

kwargs: UpdateWorkspacesPoolRequestRequestTypeDef = {  # (1)
    "PoolId": ...,
}

parent.update_workspaces_pool(**kwargs)
```

1. See [:material-code-braces: UpdateWorkspacesPoolRequestRequestTypeDef](./type_defs.md#updateworkspacespoolrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("workspaces").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("workspaces").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("workspaces").get_paginator` method with overloads.

- `client.get_paginator("describe_account_modifications")` -> [DescribeAccountModificationsPaginator](./paginators.md#describeaccountmodificationspaginator)
- `client.get_paginator("describe_ip_groups")` -> [DescribeIpGroupsPaginator](./paginators.md#describeipgroupspaginator)
- `client.get_paginator("describe_workspace_bundles")` -> [DescribeWorkspaceBundlesPaginator](./paginators.md#describeworkspacebundlespaginator)
- `client.get_paginator("describe_workspace_directories")` -> [DescribeWorkspaceDirectoriesPaginator](./paginators.md#describeworkspacedirectoriespaginator)
- `client.get_paginator("describe_workspace_images")` -> [DescribeWorkspaceImagesPaginator](./paginators.md#describeworkspaceimagespaginator)
- `client.get_paginator("describe_workspaces_connection_status")` -> [DescribeWorkspacesConnectionStatusPaginator](./paginators.md#describeworkspacesconnectionstatuspaginator)
- `client.get_paginator("describe_workspaces")` -> [DescribeWorkspacesPaginator](./paginators.md#describeworkspacespaginator)
- `client.get_paginator("list_account_links")` -> [ListAccountLinksPaginator](./paginators.md#listaccountlinkspaginator)
- `client.get_paginator("list_available_management_cidr_ranges")` -> [ListAvailableManagementCidrRangesPaginator](./paginators.md#listavailablemanagementcidrrangespaginator)


