# ResourceGroupsClient

> [Index](../README.md) > [ResourceGroups](./README.md) > ResourceGroupsClient

!!! note ""

    Auto-generated documentation for [ResourceGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#resourcegroups)
    type annotations stubs module [types-aiobotocore-resource-groups](https://pypi.org/project/types-aiobotocore-resource-groups/).

## ResourceGroupsClient

Type annotations and code completion for `#!python session.client("resource-groups")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# ResourceGroupsClient usage example

from aioboto3.session import Session
from types_aiobotocore_resource_groups.client import ResourceGroupsClient

session = Session()
async with session.client("resource-groups") as client:
    client: ResourceGroupsClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("resource-groups").exceptions` structure.

```python
# ResourceGroupsClient.exceptions usage example

async with session.client("resource-groups") as client:
    try:
        do_something(client)
    except (
            client.exceptions.BadRequestException,
        client.exceptions.ClientError,
        client.exceptions.ForbiddenException,
        client.exceptions.InternalServerErrorException,
        client.exceptions.MethodNotAllowedException,
        client.exceptions.NotFoundException,
        client.exceptions.TooManyRequestsException,
        client.exceptions.UnauthorizedException,
    ) as e:
        print(e)
```

```python
# ResourceGroupsClient.exceptions type checking example

from types_aiobotocore_resource_groups.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("resource-groups").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("resource-groups").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

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


### cancel\_tag\_sync\_task

Cancels the specified tag-sync task.

Type annotations and code completion for `#!python session.client("resource-groups").cancel_tag_sync_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# cancel_tag_sync_task method definition

await def cancel_tag_sync_task(
    self,
    *,
    TaskArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# cancel_tag_sync_task method usage example with argument unpacking

kwargs: CancelTagSyncTaskInputRequestTypeDef = {  # (1)
    "TaskArn": ...,
}

parent.cancel_tag_sync_task(**kwargs)
```

1. See [:material-code-braces: CancelTagSyncTaskInputRequestTypeDef](./type_defs.md#canceltagsynctaskinputrequesttypedef) 

### create\_group

Creates a resource group with the specified name and description.

Type annotations and code completion for `#!python session.client("resource-groups").create_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# create_group method definition

await def create_group(
    self,
    *,
    Name: str,
    Description: str = ...,
    ResourceQuery: ResourceQueryTypeDef = ...,  # (1)
    Tags: Mapping[str, str] = ...,
    Configuration: Sequence[GroupConfigurationItemUnionTypeDef] = ...,  # (2)
    Criticality: int = ...,
    Owner: str = ...,
    DisplayName: str = ...,
) -> CreateGroupOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourceQueryTypeDef](./type_defs.md#resourcequerytypedef) 
2. See [:material-code-braces: GroupConfigurationItemTypeDef](./type_defs.md#groupconfigurationitemtypedef) [:material-code-braces: GroupConfigurationItemOutputTypeDef](./type_defs.md#groupconfigurationitemoutputtypedef) 
3. See [:material-code-braces: CreateGroupOutputTypeDef](./type_defs.md#creategroupoutputtypedef) 


```python
# create_group method usage example with argument unpacking

kwargs: CreateGroupInputRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_group(**kwargs)
```

1. See [:material-code-braces: CreateGroupInputRequestTypeDef](./type_defs.md#creategroupinputrequesttypedef) 

### delete\_group

Deletes the specified resource group.

Type annotations and code completion for `#!python session.client("resource-groups").delete_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# delete_group method definition

await def delete_group(
    self,
    *,
    GroupName: str = ...,
    Group: str = ...,
) -> DeleteGroupOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteGroupOutputTypeDef](./type_defs.md#deletegroupoutputtypedef) 


```python
# delete_group method usage example with argument unpacking

kwargs: DeleteGroupInputRequestTypeDef = {  # (1)
    "GroupName": ...,
}

parent.delete_group(**kwargs)
```

1. See [:material-code-braces: DeleteGroupInputRequestTypeDef](./type_defs.md#deletegroupinputrequesttypedef) 

### get\_account\_settings

Retrieves the current status of optional features in Resource Groups.

Type annotations and code completion for `#!python session.client("resource-groups").get_account_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# get_account_settings method definition

await def get_account_settings(
    self,
) -> GetAccountSettingsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccountSettingsOutputTypeDef](./type_defs.md#getaccountsettingsoutputtypedef) 

### get\_group

Returns information about a specified resource group.

Type annotations and code completion for `#!python session.client("resource-groups").get_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# get_group method definition

await def get_group(
    self,
    *,
    GroupName: str = ...,
    Group: str = ...,
) -> GetGroupOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGroupOutputTypeDef](./type_defs.md#getgroupoutputtypedef) 


```python
# get_group method usage example with argument unpacking

kwargs: GetGroupInputRequestTypeDef = {  # (1)
    "GroupName": ...,
}

parent.get_group(**kwargs)
```

1. See [:material-code-braces: GetGroupInputRequestTypeDef](./type_defs.md#getgroupinputrequesttypedef) 

### get\_group\_configuration

Retrieves the service configuration associated with the specified resource
group.

Type annotations and code completion for `#!python session.client("resource-groups").get_group_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# get_group_configuration method definition

await def get_group_configuration(
    self,
    *,
    Group: str = ...,
) -> GetGroupConfigurationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGroupConfigurationOutputTypeDef](./type_defs.md#getgroupconfigurationoutputtypedef) 


```python
# get_group_configuration method usage example with argument unpacking

kwargs: GetGroupConfigurationInputRequestTypeDef = {  # (1)
    "Group": ...,
}

parent.get_group_configuration(**kwargs)
```

1. See [:material-code-braces: GetGroupConfigurationInputRequestTypeDef](./type_defs.md#getgroupconfigurationinputrequesttypedef) 

### get\_group\_query

Retrieves the resource query associated with the specified resource group.

Type annotations and code completion for `#!python session.client("resource-groups").get_group_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# get_group_query method definition

await def get_group_query(
    self,
    *,
    GroupName: str = ...,
    Group: str = ...,
) -> GetGroupQueryOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGroupQueryOutputTypeDef](./type_defs.md#getgroupqueryoutputtypedef) 


```python
# get_group_query method usage example with argument unpacking

kwargs: GetGroupQueryInputRequestTypeDef = {  # (1)
    "GroupName": ...,
}

parent.get_group_query(**kwargs)
```

1. See [:material-code-braces: GetGroupQueryInputRequestTypeDef](./type_defs.md#getgroupqueryinputrequesttypedef) 

### get\_tag\_sync\_task

Returns information about a specified tag-sync task.

Type annotations and code completion for `#!python session.client("resource-groups").get_tag_sync_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# get_tag_sync_task method definition

await def get_tag_sync_task(
    self,
    *,
    TaskArn: str,
) -> GetTagSyncTaskOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTagSyncTaskOutputTypeDef](./type_defs.md#gettagsynctaskoutputtypedef) 


```python
# get_tag_sync_task method usage example with argument unpacking

kwargs: GetTagSyncTaskInputRequestTypeDef = {  # (1)
    "TaskArn": ...,
}

parent.get_tag_sync_task(**kwargs)
```

1. See [:material-code-braces: GetTagSyncTaskInputRequestTypeDef](./type_defs.md#gettagsynctaskinputrequesttypedef) 

### get\_tags

Returns a list of tags that are associated with a resource group, specified by
an Amazon resource name (ARN).

Type annotations and code completion for `#!python session.client("resource-groups").get_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# get_tags method definition

await def get_tags(
    self,
    *,
    Arn: str,
) -> GetTagsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTagsOutputTypeDef](./type_defs.md#gettagsoutputtypedef) 


```python
# get_tags method usage example with argument unpacking

kwargs: GetTagsInputRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.get_tags(**kwargs)
```

1. See [:material-code-braces: GetTagsInputRequestTypeDef](./type_defs.md#gettagsinputrequesttypedef) 

### group\_resources

Adds the specified resources to the specified group.

Type annotations and code completion for `#!python session.client("resource-groups").group_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# group_resources method definition

await def group_resources(
    self,
    *,
    Group: str,
    ResourceArns: Sequence[str],
) -> GroupResourcesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GroupResourcesOutputTypeDef](./type_defs.md#groupresourcesoutputtypedef) 


```python
# group_resources method usage example with argument unpacking

kwargs: GroupResourcesInputRequestTypeDef = {  # (1)
    "Group": ...,
    "ResourceArns": ...,
}

parent.group_resources(**kwargs)
```

1. See [:material-code-braces: GroupResourcesInputRequestTypeDef](./type_defs.md#groupresourcesinputrequesttypedef) 

### list\_group\_resources

Returns a list of Amazon resource names (ARNs) of the resources that are
members of a specified resource group.

Type annotations and code completion for `#!python session.client("resource-groups").list_group_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# list_group_resources method definition

await def list_group_resources(
    self,
    *,
    GroupName: str = ...,
    Group: str = ...,
    Filters: Sequence[ResourceFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListGroupResourcesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ResourceFilterTypeDef](./type_defs.md#resourcefiltertypedef) 
2. See [:material-code-braces: ListGroupResourcesOutputTypeDef](./type_defs.md#listgroupresourcesoutputtypedef) 


```python
# list_group_resources method usage example with argument unpacking

kwargs: ListGroupResourcesInputRequestTypeDef = {  # (1)
    "GroupName": ...,
}

parent.list_group_resources(**kwargs)
```

1. See [:material-code-braces: ListGroupResourcesInputRequestTypeDef](./type_defs.md#listgroupresourcesinputrequesttypedef) 

### list\_grouping\_statuses

Returns the status of the last grouping or ungrouping action for each resource
in the specified application group.

Type annotations and code completion for `#!python session.client("resource-groups").list_grouping_statuses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# list_grouping_statuses method definition

await def list_grouping_statuses(
    self,
    *,
    Group: str,
    MaxResults: int = ...,
    Filters: Sequence[ListGroupingStatusesFilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
) -> ListGroupingStatusesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListGroupingStatusesFilterTypeDef](./type_defs.md#listgroupingstatusesfiltertypedef) 
2. See [:material-code-braces: ListGroupingStatusesOutputTypeDef](./type_defs.md#listgroupingstatusesoutputtypedef) 


```python
# list_grouping_statuses method usage example with argument unpacking

kwargs: ListGroupingStatusesInputRequestTypeDef = {  # (1)
    "Group": ...,
}

parent.list_grouping_statuses(**kwargs)
```

1. See [:material-code-braces: ListGroupingStatusesInputRequestTypeDef](./type_defs.md#listgroupingstatusesinputrequesttypedef) 

### list\_groups

Returns a list of existing Resource Groups in your account.

Type annotations and code completion for `#!python session.client("resource-groups").list_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# list_groups method definition

await def list_groups(
    self,
    *,
    Filters: Sequence[GroupFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListGroupsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: GroupFilterTypeDef](./type_defs.md#groupfiltertypedef) 
2. See [:material-code-braces: ListGroupsOutputTypeDef](./type_defs.md#listgroupsoutputtypedef) 


```python
# list_groups method usage example with argument unpacking

kwargs: ListGroupsInputRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.list_groups(**kwargs)
```

1. See [:material-code-braces: ListGroupsInputRequestTypeDef](./type_defs.md#listgroupsinputrequesttypedef) 

### list\_tag\_sync\_tasks

Returns a list of tag-sync tasks.

Type annotations and code completion for `#!python session.client("resource-groups").list_tag_sync_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# list_tag_sync_tasks method definition

await def list_tag_sync_tasks(
    self,
    *,
    Filters: Sequence[ListTagSyncTasksFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTagSyncTasksOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListTagSyncTasksFilterTypeDef](./type_defs.md#listtagsynctasksfiltertypedef) 
2. See [:material-code-braces: ListTagSyncTasksOutputTypeDef](./type_defs.md#listtagsynctasksoutputtypedef) 


```python
# list_tag_sync_tasks method usage example with argument unpacking

kwargs: ListTagSyncTasksInputRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.list_tag_sync_tasks(**kwargs)
```

1. See [:material-code-braces: ListTagSyncTasksInputRequestTypeDef](./type_defs.md#listtagsynctasksinputrequesttypedef) 

### put\_group\_configuration

Attaches a service configuration to the specified group.

Type annotations and code completion for `#!python session.client("resource-groups").put_group_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# put_group_configuration method definition

await def put_group_configuration(
    self,
    *,
    Group: str = ...,
    Configuration: Sequence[GroupConfigurationItemTypeDef] = ...,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: GroupConfigurationItemTypeDef](./type_defs.md#groupconfigurationitemtypedef) 


```python
# put_group_configuration method usage example with argument unpacking

kwargs: PutGroupConfigurationInputRequestTypeDef = {  # (1)
    "Group": ...,
}

parent.put_group_configuration(**kwargs)
```

1. See [:material-code-braces: PutGroupConfigurationInputRequestTypeDef](./type_defs.md#putgroupconfigurationinputrequesttypedef) 

### search\_resources

Returns a list of Amazon Web Services resource identifiers that matches the
specified query.

Type annotations and code completion for `#!python session.client("resource-groups").search_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# search_resources method definition

await def search_resources(
    self,
    *,
    ResourceQuery: ResourceQueryTypeDef,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> SearchResourcesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ResourceQueryTypeDef](./type_defs.md#resourcequerytypedef) 
2. See [:material-code-braces: SearchResourcesOutputTypeDef](./type_defs.md#searchresourcesoutputtypedef) 


```python
# search_resources method usage example with argument unpacking

kwargs: SearchResourcesInputRequestTypeDef = {  # (1)
    "ResourceQuery": ...,
}

parent.search_resources(**kwargs)
```

1. See [:material-code-braces: SearchResourcesInputRequestTypeDef](./type_defs.md#searchresourcesinputrequesttypedef) 

### start\_tag\_sync\_task

Creates a new tag-sync task to onboard and sync resources tagged with a
specific tag key-value pair to an application.

Type annotations and code completion for `#!python session.client("resource-groups").start_tag_sync_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# start_tag_sync_task method definition

await def start_tag_sync_task(
    self,
    *,
    Group: str,
    TagKey: str,
    TagValue: str,
    RoleArn: str,
) -> StartTagSyncTaskOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartTagSyncTaskOutputTypeDef](./type_defs.md#starttagsynctaskoutputtypedef) 


```python
# start_tag_sync_task method usage example with argument unpacking

kwargs: StartTagSyncTaskInputRequestTypeDef = {  # (1)
    "Group": ...,
    "TagKey": ...,
    "TagValue": ...,
    "RoleArn": ...,
}

parent.start_tag_sync_task(**kwargs)
```

1. See [:material-code-braces: StartTagSyncTaskInputRequestTypeDef](./type_defs.md#starttagsynctaskinputrequesttypedef) 

### tag

Adds tags to a resource group with the specified Amazon resource name (ARN).

Type annotations and code completion for `#!python session.client("resource-groups").tag` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# tag method definition

await def tag(
    self,
    *,
    Arn: str,
    Tags: Mapping[str, str],
) -> TagOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TagOutputTypeDef](./type_defs.md#tagoutputtypedef) 


```python
# tag method usage example with argument unpacking

kwargs: TagInputRequestTypeDef = {  # (1)
    "Arn": ...,
    "Tags": ...,
}

parent.tag(**kwargs)
```

1. See [:material-code-braces: TagInputRequestTypeDef](./type_defs.md#taginputrequesttypedef) 

### ungroup\_resources

Removes the specified resources from the specified group.

Type annotations and code completion for `#!python session.client("resource-groups").ungroup_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# ungroup_resources method definition

await def ungroup_resources(
    self,
    *,
    Group: str,
    ResourceArns: Sequence[str],
) -> UngroupResourcesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UngroupResourcesOutputTypeDef](./type_defs.md#ungroupresourcesoutputtypedef) 


```python
# ungroup_resources method usage example with argument unpacking

kwargs: UngroupResourcesInputRequestTypeDef = {  # (1)
    "Group": ...,
    "ResourceArns": ...,
}

parent.ungroup_resources(**kwargs)
```

1. See [:material-code-braces: UngroupResourcesInputRequestTypeDef](./type_defs.md#ungroupresourcesinputrequesttypedef) 

### untag

Deletes tags from a specified resource group.

Type annotations and code completion for `#!python session.client("resource-groups").untag` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# untag method definition

await def untag(
    self,
    *,
    Arn: str,
    Keys: Sequence[str],
) -> UntagOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UntagOutputTypeDef](./type_defs.md#untagoutputtypedef) 


```python
# untag method usage example with argument unpacking

kwargs: UntagInputRequestTypeDef = {  # (1)
    "Arn": ...,
    "Keys": ...,
}

parent.untag(**kwargs)
```

1. See [:material-code-braces: UntagInputRequestTypeDef](./type_defs.md#untaginputrequesttypedef) 

### update\_account\_settings

Turns on or turns off optional features in Resource Groups.

Type annotations and code completion for `#!python session.client("resource-groups").update_account_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# update_account_settings method definition

await def update_account_settings(
    self,
    *,
    GroupLifecycleEventsDesiredStatus: GroupLifecycleEventsDesiredStatusType = ...,  # (1)
) -> UpdateAccountSettingsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: GroupLifecycleEventsDesiredStatusType](./literals.md#grouplifecycleeventsdesiredstatustype) 
2. See [:material-code-braces: UpdateAccountSettingsOutputTypeDef](./type_defs.md#updateaccountsettingsoutputtypedef) 


```python
# update_account_settings method usage example with argument unpacking

kwargs: UpdateAccountSettingsInputRequestTypeDef = {  # (1)
    "GroupLifecycleEventsDesiredStatus": ...,
}

parent.update_account_settings(**kwargs)
```

1. See [:material-code-braces: UpdateAccountSettingsInputRequestTypeDef](./type_defs.md#updateaccountsettingsinputrequesttypedef) 

### update\_group

Updates the description for an existing group.

Type annotations and code completion for `#!python session.client("resource-groups").update_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# update_group method definition

await def update_group(
    self,
    *,
    GroupName: str = ...,
    Group: str = ...,
    Description: str = ...,
    Criticality: int = ...,
    Owner: str = ...,
    DisplayName: str = ...,
) -> UpdateGroupOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateGroupOutputTypeDef](./type_defs.md#updategroupoutputtypedef) 


```python
# update_group method usage example with argument unpacking

kwargs: UpdateGroupInputRequestTypeDef = {  # (1)
    "GroupName": ...,
}

parent.update_group(**kwargs)
```

1. See [:material-code-braces: UpdateGroupInputRequestTypeDef](./type_defs.md#updategroupinputrequesttypedef) 

### update\_group\_query

Updates the resource query of a group.

Type annotations and code completion for `#!python session.client("resource-groups").update_group_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# update_group_query method definition

await def update_group_query(
    self,
    *,
    ResourceQuery: ResourceQueryTypeDef,  # (1)
    GroupName: str = ...,
    Group: str = ...,
) -> UpdateGroupQueryOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ResourceQueryTypeDef](./type_defs.md#resourcequerytypedef) 
2. See [:material-code-braces: UpdateGroupQueryOutputTypeDef](./type_defs.md#updategroupqueryoutputtypedef) 


```python
# update_group_query method usage example with argument unpacking

kwargs: UpdateGroupQueryInputRequestTypeDef = {  # (1)
    "ResourceQuery": ...,
}

parent.update_group_query(**kwargs)
```

1. See [:material-code-braces: UpdateGroupQueryInputRequestTypeDef](./type_defs.md#updategroupqueryinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("resource-groups").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("resource-groups").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client)

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

Type annotations and code completion for `#!python session.client("resource-groups").get_paginator` method with overloads.

- `client.get_paginator("list_group_resources")` -> [ListGroupResourcesPaginator](./paginators.md#listgroupresourcespaginator)
- `client.get_paginator("list_grouping_statuses")` -> [ListGroupingStatusesPaginator](./paginators.md#listgroupingstatusespaginator)
- `client.get_paginator("list_groups")` -> [ListGroupsPaginator](./paginators.md#listgroupspaginator)
- `client.get_paginator("list_tag_sync_tasks")` -> [ListTagSyncTasksPaginator](./paginators.md#listtagsynctaskspaginator)
- `client.get_paginator("search_resources")` -> [SearchResourcesPaginator](./paginators.md#searchresourcespaginator)


