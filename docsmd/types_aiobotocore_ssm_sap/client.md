# SsmSapClient

> [Index](../README.md) > [SsmSap](./README.md) > SsmSapClient

!!! note ""

    Auto-generated documentation for [SsmSap](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#ssmsap)
    type annotations stubs module [types-aiobotocore-ssm-sap](https://pypi.org/project/types-aiobotocore-ssm-sap/).

## SsmSapClient

Type annotations and code completion for `#!python session.client("ssm-sap")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# SsmSapClient usage example

from aioboto3.session import Session
from types_aiobotocore_ssm_sap.client import SsmSapClient

session = Session()
async with session.client("ssm-sap") as client:
    client: SsmSapClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("ssm-sap").exceptions` structure.

```python
# SsmSapClient.exceptions usage example

async with session.client("ssm-sap") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.UnauthorizedException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# SsmSapClient.exceptions type checking example

from types_aiobotocore_ssm_sap.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("ssm-sap").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("ssm-sap").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

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


### delete\_resource\_permission

Removes permissions associated with the target database.

Type annotations and code completion for `#!python session.client("ssm-sap").delete_resource_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# delete_resource_permission method definition

await def delete_resource_permission(
    self,
    *,
    ResourceArn: str,
    ActionType: PermissionActionTypeType = ...,  # (1)
    SourceResourceArn: str = ...,
) -> DeleteResourcePermissionOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PermissionActionTypeType](./literals.md#permissionactiontypetype) 
2. See [:material-code-braces: DeleteResourcePermissionOutputTypeDef](./type_defs.md#deleteresourcepermissionoutputtypedef) 


```python
# delete_resource_permission method usage example with argument unpacking

kwargs: DeleteResourcePermissionInputRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.delete_resource_permission(**kwargs)
```

1. See [:material-code-braces: DeleteResourcePermissionInputRequestTypeDef](./type_defs.md#deleteresourcepermissioninputrequesttypedef) 

### deregister\_application

Deregister an SAP application with AWS Systems Manager for SAP.

Type annotations and code completion for `#!python session.client("ssm-sap").deregister_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# deregister_application method definition

await def deregister_application(
    self,
    *,
    ApplicationId: str,
) -> dict[str, Any]:
    ...
```



```python
# deregister_application method usage example with argument unpacking

kwargs: DeregisterApplicationInputRequestTypeDef = {  # (1)
    "ApplicationId": ...,
}

parent.deregister_application(**kwargs)
```

1. See [:material-code-braces: DeregisterApplicationInputRequestTypeDef](./type_defs.md#deregisterapplicationinputrequesttypedef) 

### get\_application

Gets an application registered with AWS Systems Manager for SAP.

Type annotations and code completion for `#!python session.client("ssm-sap").get_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# get_application method definition

await def get_application(
    self,
    *,
    ApplicationId: str = ...,
    ApplicationArn: str = ...,
    AppRegistryArn: str = ...,
) -> GetApplicationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetApplicationOutputTypeDef](./type_defs.md#getapplicationoutputtypedef) 


```python
# get_application method usage example with argument unpacking

kwargs: GetApplicationInputRequestTypeDef = {  # (1)
    "ApplicationId": ...,
}

parent.get_application(**kwargs)
```

1. See [:material-code-braces: GetApplicationInputRequestTypeDef](./type_defs.md#getapplicationinputrequesttypedef) 

### get\_component

Gets the component of an application registered with AWS Systems Manager for
SAP.

Type annotations and code completion for `#!python session.client("ssm-sap").get_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# get_component method definition

await def get_component(
    self,
    *,
    ApplicationId: str,
    ComponentId: str,
) -> GetComponentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetComponentOutputTypeDef](./type_defs.md#getcomponentoutputtypedef) 


```python
# get_component method usage example with argument unpacking

kwargs: GetComponentInputRequestTypeDef = {  # (1)
    "ApplicationId": ...,
    "ComponentId": ...,
}

parent.get_component(**kwargs)
```

1. See [:material-code-braces: GetComponentInputRequestTypeDef](./type_defs.md#getcomponentinputrequesttypedef) 

### get\_database

Gets the SAP HANA database of an application registered with AWS Systems
Manager for SAP.

Type annotations and code completion for `#!python session.client("ssm-sap").get_database` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# get_database method definition

await def get_database(
    self,
    *,
    ApplicationId: str = ...,
    ComponentId: str = ...,
    DatabaseId: str = ...,
    DatabaseArn: str = ...,
) -> GetDatabaseOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDatabaseOutputTypeDef](./type_defs.md#getdatabaseoutputtypedef) 


```python
# get_database method usage example with argument unpacking

kwargs: GetDatabaseInputRequestTypeDef = {  # (1)
    "ApplicationId": ...,
}

parent.get_database(**kwargs)
```

1. See [:material-code-braces: GetDatabaseInputRequestTypeDef](./type_defs.md#getdatabaseinputrequesttypedef) 

### get\_operation

Gets the details of an operation by specifying the operation ID.

Type annotations and code completion for `#!python session.client("ssm-sap").get_operation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# get_operation method definition

await def get_operation(
    self,
    *,
    OperationId: str,
) -> GetOperationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOperationOutputTypeDef](./type_defs.md#getoperationoutputtypedef) 


```python
# get_operation method usage example with argument unpacking

kwargs: GetOperationInputRequestTypeDef = {  # (1)
    "OperationId": ...,
}

parent.get_operation(**kwargs)
```

1. See [:material-code-braces: GetOperationInputRequestTypeDef](./type_defs.md#getoperationinputrequesttypedef) 

### get\_resource\_permission

Gets permissions associated with the target database.

Type annotations and code completion for `#!python session.client("ssm-sap").get_resource_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# get_resource_permission method definition

await def get_resource_permission(
    self,
    *,
    ResourceArn: str,
    ActionType: PermissionActionTypeType = ...,  # (1)
) -> GetResourcePermissionOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PermissionActionTypeType](./literals.md#permissionactiontypetype) 
2. See [:material-code-braces: GetResourcePermissionOutputTypeDef](./type_defs.md#getresourcepermissionoutputtypedef) 


```python
# get_resource_permission method usage example with argument unpacking

kwargs: GetResourcePermissionInputRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_resource_permission(**kwargs)
```

1. See [:material-code-braces: GetResourcePermissionInputRequestTypeDef](./type_defs.md#getresourcepermissioninputrequesttypedef) 

### list\_applications

Lists all the applications registered with AWS Systems Manager for SAP.

Type annotations and code completion for `#!python session.client("ssm-sap").list_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# list_applications method definition

await def list_applications(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListApplicationsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListApplicationsOutputTypeDef](./type_defs.md#listapplicationsoutputtypedef) 


```python
# list_applications method usage example with argument unpacking

kwargs: ListApplicationsInputRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_applications(**kwargs)
```

1. See [:material-code-braces: ListApplicationsInputRequestTypeDef](./type_defs.md#listapplicationsinputrequesttypedef) 

### list\_components

Lists all the components registered with AWS Systems Manager for SAP.

Type annotations and code completion for `#!python session.client("ssm-sap").list_components` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# list_components method definition

await def list_components(
    self,
    *,
    ApplicationId: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListComponentsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListComponentsOutputTypeDef](./type_defs.md#listcomponentsoutputtypedef) 


```python
# list_components method usage example with argument unpacking

kwargs: ListComponentsInputRequestTypeDef = {  # (1)
    "ApplicationId": ...,
}

parent.list_components(**kwargs)
```

1. See [:material-code-braces: ListComponentsInputRequestTypeDef](./type_defs.md#listcomponentsinputrequesttypedef) 

### list\_databases

Lists the SAP HANA databases of an application registered with AWS Systems
Manager for SAP.

Type annotations and code completion for `#!python session.client("ssm-sap").list_databases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# list_databases method definition

await def list_databases(
    self,
    *,
    ApplicationId: str = ...,
    ComponentId: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDatabasesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDatabasesOutputTypeDef](./type_defs.md#listdatabasesoutputtypedef) 


```python
# list_databases method usage example with argument unpacking

kwargs: ListDatabasesInputRequestTypeDef = {  # (1)
    "ApplicationId": ...,
}

parent.list_databases(**kwargs)
```

1. See [:material-code-braces: ListDatabasesInputRequestTypeDef](./type_defs.md#listdatabasesinputrequesttypedef) 

### list\_operation\_events

Returns a list of operations events.

Type annotations and code completion for `#!python session.client("ssm-sap").list_operation_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# list_operation_events method definition

await def list_operation_events(
    self,
    *,
    OperationId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListOperationEventsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListOperationEventsOutputTypeDef](./type_defs.md#listoperationeventsoutputtypedef) 


```python
# list_operation_events method usage example with argument unpacking

kwargs: ListOperationEventsInputRequestTypeDef = {  # (1)
    "OperationId": ...,
}

parent.list_operation_events(**kwargs)
```

1. See [:material-code-braces: ListOperationEventsInputRequestTypeDef](./type_defs.md#listoperationeventsinputrequesttypedef) 

### list\_operations

Lists the operations performed by AWS Systems Manager for SAP.

Type annotations and code completion for `#!python session.client("ssm-sap").list_operations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# list_operations method definition

await def list_operations(
    self,
    *,
    ApplicationId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListOperationsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListOperationsOutputTypeDef](./type_defs.md#listoperationsoutputtypedef) 


```python
# list_operations method usage example with argument unpacking

kwargs: ListOperationsInputRequestTypeDef = {  # (1)
    "ApplicationId": ...,
}

parent.list_operations(**kwargs)
```

1. See [:material-code-braces: ListOperationsInputRequestTypeDef](./type_defs.md#listoperationsinputrequesttypedef) 

### list\_tags\_for\_resource

Lists all tags on an SAP HANA application and/or database registered with AWS
Systems Manager for SAP.

Type annotations and code completion for `#!python session.client("ssm-sap").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### put\_resource\_permission

Adds permissions to the target database.

Type annotations and code completion for `#!python session.client("ssm-sap").put_resource_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# put_resource_permission method definition

await def put_resource_permission(
    self,
    *,
    ActionType: PermissionActionTypeType,  # (1)
    SourceResourceArn: str,
    ResourceArn: str,
) -> PutResourcePermissionOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PermissionActionTypeType](./literals.md#permissionactiontypetype) 
2. See [:material-code-braces: PutResourcePermissionOutputTypeDef](./type_defs.md#putresourcepermissionoutputtypedef) 


```python
# put_resource_permission method usage example with argument unpacking

kwargs: PutResourcePermissionInputRequestTypeDef = {  # (1)
    "ActionType": ...,
    "SourceResourceArn": ...,
    "ResourceArn": ...,
}

parent.put_resource_permission(**kwargs)
```

1. See [:material-code-braces: PutResourcePermissionInputRequestTypeDef](./type_defs.md#putresourcepermissioninputrequesttypedef) 

### register\_application

Register an SAP application with AWS Systems Manager for SAP.

Type annotations and code completion for `#!python session.client("ssm-sap").register_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# register_application method definition

await def register_application(
    self,
    *,
    ApplicationId: str,
    ApplicationType: ApplicationTypeType,  # (1)
    Instances: Sequence[str],
    SapInstanceNumber: str = ...,
    Sid: str = ...,
    Tags: Mapping[str, str] = ...,
    Credentials: Sequence[ApplicationCredentialTypeDef] = ...,  # (2)
    DatabaseArn: str = ...,
) -> RegisterApplicationOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ApplicationTypeType](./literals.md#applicationtypetype) 
2. See [:material-code-braces: ApplicationCredentialTypeDef](./type_defs.md#applicationcredentialtypedef) 
3. See [:material-code-braces: RegisterApplicationOutputTypeDef](./type_defs.md#registerapplicationoutputtypedef) 


```python
# register_application method usage example with argument unpacking

kwargs: RegisterApplicationInputRequestTypeDef = {  # (1)
    "ApplicationId": ...,
    "ApplicationType": ...,
    "Instances": ...,
}

parent.register_application(**kwargs)
```

1. See [:material-code-braces: RegisterApplicationInputRequestTypeDef](./type_defs.md#registerapplicationinputrequesttypedef) 

### start\_application

Request is an operation which starts an application.

Type annotations and code completion for `#!python session.client("ssm-sap").start_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# start_application method definition

await def start_application(
    self,
    *,
    ApplicationId: str,
) -> StartApplicationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartApplicationOutputTypeDef](./type_defs.md#startapplicationoutputtypedef) 


```python
# start_application method usage example with argument unpacking

kwargs: StartApplicationInputRequestTypeDef = {  # (1)
    "ApplicationId": ...,
}

parent.start_application(**kwargs)
```

1. See [:material-code-braces: StartApplicationInputRequestTypeDef](./type_defs.md#startapplicationinputrequesttypedef) 

### start\_application\_refresh

Refreshes a registered application.

Type annotations and code completion for `#!python session.client("ssm-sap").start_application_refresh` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# start_application_refresh method definition

await def start_application_refresh(
    self,
    *,
    ApplicationId: str,
) -> StartApplicationRefreshOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartApplicationRefreshOutputTypeDef](./type_defs.md#startapplicationrefreshoutputtypedef) 


```python
# start_application_refresh method usage example with argument unpacking

kwargs: StartApplicationRefreshInputRequestTypeDef = {  # (1)
    "ApplicationId": ...,
}

parent.start_application_refresh(**kwargs)
```

1. See [:material-code-braces: StartApplicationRefreshInputRequestTypeDef](./type_defs.md#startapplicationrefreshinputrequesttypedef) 

### stop\_application

Request is an operation to stop an application.

Type annotations and code completion for `#!python session.client("ssm-sap").stop_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# stop_application method definition

await def stop_application(
    self,
    *,
    ApplicationId: str,
    StopConnectedEntity: ConnectedEntityTypeType = ...,  # (1)
    IncludeEc2InstanceShutdown: bool = ...,
) -> StopApplicationOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ConnectedEntityTypeType](./literals.md#connectedentitytypetype) 
2. See [:material-code-braces: StopApplicationOutputTypeDef](./type_defs.md#stopapplicationoutputtypedef) 


```python
# stop_application method usage example with argument unpacking

kwargs: StopApplicationInputRequestTypeDef = {  # (1)
    "ApplicationId": ...,
}

parent.stop_application(**kwargs)
```

1. See [:material-code-braces: StopApplicationInputRequestTypeDef](./type_defs.md#stopapplicationinputrequesttypedef) 

### tag\_resource

Creates tag for a resource by specifying the ARN.

Type annotations and code completion for `#!python session.client("ssm-sap").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Delete the tags for a resource.

Type annotations and code completion for `#!python session.client("ssm-sap").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_application\_settings

Updates the settings of an application registered with AWS Systems Manager for
SAP.

Type annotations and code completion for `#!python session.client("ssm-sap").update_application_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# update_application_settings method definition

await def update_application_settings(
    self,
    *,
    ApplicationId: str,
    CredentialsToAddOrUpdate: Sequence[ApplicationCredentialTypeDef] = ...,  # (1)
    CredentialsToRemove: Sequence[ApplicationCredentialTypeDef] = ...,  # (1)
    Backint: BackintConfigTypeDef = ...,  # (3)
    DatabaseArn: str = ...,
) -> UpdateApplicationSettingsOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ApplicationCredentialTypeDef](./type_defs.md#applicationcredentialtypedef) 
2. See [:material-code-braces: ApplicationCredentialTypeDef](./type_defs.md#applicationcredentialtypedef) 
3. See [:material-code-braces: BackintConfigTypeDef](./type_defs.md#backintconfigtypedef) 
4. See [:material-code-braces: UpdateApplicationSettingsOutputTypeDef](./type_defs.md#updateapplicationsettingsoutputtypedef) 


```python
# update_application_settings method usage example with argument unpacking

kwargs: UpdateApplicationSettingsInputRequestTypeDef = {  # (1)
    "ApplicationId": ...,
}

parent.update_application_settings(**kwargs)
```

1. See [:material-code-braces: UpdateApplicationSettingsInputRequestTypeDef](./type_defs.md#updateapplicationsettingsinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("ssm-sap").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("ssm-sap").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap.Client)

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

Type annotations and code completion for `#!python session.client("ssm-sap").get_paginator` method with overloads.

- `client.get_paginator("list_applications")` -> [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
- `client.get_paginator("list_components")` -> [ListComponentsPaginator](./paginators.md#listcomponentspaginator)
- `client.get_paginator("list_databases")` -> [ListDatabasesPaginator](./paginators.md#listdatabasespaginator)
- `client.get_paginator("list_operation_events")` -> [ListOperationEventsPaginator](./paginators.md#listoperationeventspaginator)
- `client.get_paginator("list_operations")` -> [ListOperationsPaginator](./paginators.md#listoperationspaginator)


