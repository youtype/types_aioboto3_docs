# RecycleBinClient

> [Index](../README.md) > [RecycleBin](./README.md) > RecycleBinClient

!!! note ""

    Auto-generated documentation for [RecycleBin](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#recyclebin)
    type annotations stubs module [types-aiobotocore-rbin](https://pypi.org/project/types-aiobotocore-rbin/).

## RecycleBinClient

Type annotations and code completion for `#!python session.client("rbin")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client)

```python
# RecycleBinClient usage example

from aioboto3.session import Session
from types_aiobotocore_rbin.client import RecycleBinClient

session = Session()
async with session.client("rbin") as client:
    client: RecycleBinClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("rbin").exceptions` structure.

```python
# RecycleBinClient.exceptions usage example

async with session.client("rbin") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# RecycleBinClient.exceptions type checking example

from types_aiobotocore_rbin.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("rbin").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("rbin").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client)

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


### create\_rule

Creates a Recycle Bin retention rule.

Type annotations and code completion for `#!python session.client("rbin").create_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client)

```python
# create_rule method definition

await def create_rule(
    self,
    *,
    RetentionPeriod: RetentionPeriodTypeDef,  # (1)
    ResourceType: ResourceTypeType,  # (2)
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    ResourceTags: Sequence[ResourceTagTypeDef] = ...,  # (4)
    LockConfiguration: LockConfigurationTypeDef = ...,  # (5)
    ExcludeResourceTags: Sequence[ResourceTagTypeDef] = ...,  # (4)
) -> CreateRuleResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
5. See [:material-code-braces: LockConfigurationTypeDef](./type_defs.md#lockconfigurationtypedef) 
6. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
7. See [:material-code-braces: CreateRuleResponseTypeDef](./type_defs.md#createruleresponsetypedef) 


```python
# create_rule method usage example with argument unpacking

kwargs: CreateRuleRequestRequestTypeDef = {  # (1)
    "RetentionPeriod": ...,
    "ResourceType": ...,
}

parent.create_rule(**kwargs)
```

1. See [:material-code-braces: CreateRuleRequestRequestTypeDef](./type_defs.md#createrulerequestrequesttypedef) 

### delete\_rule

Deletes a Recycle Bin retention rule.

Type annotations and code completion for `#!python session.client("rbin").delete_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client)

```python
# delete_rule method definition

await def delete_rule(
    self,
    *,
    Identifier: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_rule method usage example with argument unpacking

kwargs: DeleteRuleRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.delete_rule(**kwargs)
```

1. See [:material-code-braces: DeleteRuleRequestRequestTypeDef](./type_defs.md#deleterulerequestrequesttypedef) 

### get\_rule

Gets information about a Recycle Bin retention rule.

Type annotations and code completion for `#!python session.client("rbin").get_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client)

```python
# get_rule method definition

await def get_rule(
    self,
    *,
    Identifier: str,
) -> GetRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRuleResponseTypeDef](./type_defs.md#getruleresponsetypedef) 


```python
# get_rule method usage example with argument unpacking

kwargs: GetRuleRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.get_rule(**kwargs)
```

1. See [:material-code-braces: GetRuleRequestRequestTypeDef](./type_defs.md#getrulerequestrequesttypedef) 

### list\_rules

Lists the Recycle Bin retention rules in the Region.

Type annotations and code completion for `#!python session.client("rbin").list_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client)

```python
# list_rules method definition

await def list_rules(
    self,
    *,
    ResourceType: ResourceTypeType,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
    ResourceTags: Sequence[ResourceTagTypeDef] = ...,  # (2)
    LockState: LockStateType = ...,  # (3)
    ExcludeResourceTags: Sequence[ResourceTagTypeDef] = ...,  # (2)
) -> ListRulesResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
3. See [:material-code-brackets: LockStateType](./literals.md#lockstatetype) 
4. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
5. See [:material-code-braces: ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef) 


```python
# list_rules method usage example with argument unpacking

kwargs: ListRulesRequestRequestTypeDef = {  # (1)
    "ResourceType": ...,
}

parent.list_rules(**kwargs)
```

1. See [:material-code-braces: ListRulesRequestRequestTypeDef](./type_defs.md#listrulesrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags assigned to a retention rule.

Type annotations and code completion for `#!python session.client("rbin").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### lock\_rule

Locks a Region-level retention rule.

Type annotations and code completion for `#!python session.client("rbin").lock_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client)

```python
# lock_rule method definition

await def lock_rule(
    self,
    *,
    Identifier: str,
    LockConfiguration: LockConfigurationTypeDef,  # (1)
) -> LockRuleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LockConfigurationTypeDef](./type_defs.md#lockconfigurationtypedef) 
2. See [:material-code-braces: LockRuleResponseTypeDef](./type_defs.md#lockruleresponsetypedef) 


```python
# lock_rule method usage example with argument unpacking

kwargs: LockRuleRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
    "LockConfiguration": ...,
}

parent.lock_rule(**kwargs)
```

1. See [:material-code-braces: LockRuleRequestRequestTypeDef](./type_defs.md#lockrulerequestrequesttypedef) 

### tag\_resource

Assigns tags to the specified retention rule.

Type annotations and code completion for `#!python session.client("rbin").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### unlock\_rule

Unlocks a retention rule.

Type annotations and code completion for `#!python session.client("rbin").unlock_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client)

```python
# unlock_rule method definition

await def unlock_rule(
    self,
    *,
    Identifier: str,
) -> UnlockRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UnlockRuleResponseTypeDef](./type_defs.md#unlockruleresponsetypedef) 


```python
# unlock_rule method usage example with argument unpacking

kwargs: UnlockRuleRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.unlock_rule(**kwargs)
```

1. See [:material-code-braces: UnlockRuleRequestRequestTypeDef](./type_defs.md#unlockrulerequestrequesttypedef) 

### untag\_resource

Unassigns a tag from a retention rule.

Type annotations and code completion for `#!python session.client("rbin").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_rule

Updates an existing Recycle Bin retention rule.

Type annotations and code completion for `#!python session.client("rbin").update_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client)

```python
# update_rule method definition

await def update_rule(
    self,
    *,
    Identifier: str,
    RetentionPeriod: RetentionPeriodTypeDef = ...,  # (1)
    Description: str = ...,
    ResourceType: ResourceTypeType = ...,  # (2)
    ResourceTags: Sequence[ResourceTagTypeDef] = ...,  # (3)
    ExcludeResourceTags: Sequence[ResourceTagTypeDef] = ...,  # (3)
) -> UpdateRuleResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
4. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
5. See [:material-code-braces: UpdateRuleResponseTypeDef](./type_defs.md#updateruleresponsetypedef) 


```python
# update_rule method usage example with argument unpacking

kwargs: UpdateRuleRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.update_rule(**kwargs)
```

1. See [:material-code-braces: UpdateRuleRequestRequestTypeDef](./type_defs.md#updaterulerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("rbin").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("rbin").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client)

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

Type annotations and code completion for `#!python session.client("rbin").get_paginator` method with overloads.

- `client.get_paginator("list_rules")` -> [ListRulesPaginator](./paginators.md#listrulespaginator)


