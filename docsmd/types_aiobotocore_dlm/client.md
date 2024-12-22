# DLMClient

> [Index](../README.md) > [DLM](./README.md) > DLMClient

!!! note ""

    Auto-generated documentation for [DLM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#dlm)
    type annotations stubs module [types-aiobotocore-dlm](https://pypi.org/project/types-aiobotocore-dlm/).

## DLMClient

Type annotations and code completion for `#!python session.client("dlm")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client)

```python
# DLMClient usage example

from aioboto3.session import Session
from types_aiobotocore_dlm.client import DLMClient

session = Session()
async with session.client("dlm") as client:
    client: DLMClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("dlm").exceptions` structure.

```python
# DLMClient.exceptions usage example

async with session.client("dlm") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.InternalServerException,
        client.exceptions.InvalidRequestException,
        client.exceptions.LimitExceededException,
        client.exceptions.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python
# DLMClient.exceptions type checking example

from types_aiobotocore_dlm.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("dlm").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("dlm").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client)

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


### create\_lifecycle\_policy

Creates an Amazon Data Lifecycle Manager lifecycle policy.

Type annotations and code completion for `#!python session.client("dlm").create_lifecycle_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client)

```python
# create_lifecycle_policy method definition

await def create_lifecycle_policy(
    self,
    *,
    ExecutionRoleArn: str,
    Description: str,
    State: SettablePolicyStateValuesType,  # (1)
    PolicyDetails: PolicyDetailsTypeDef = ...,  # (2)
    Tags: Mapping[str, str] = ...,
    DefaultPolicy: DefaultPolicyTypeValuesType = ...,  # (3)
    CreateInterval: int = ...,
    RetainInterval: int = ...,
    CopyTags: bool = ...,
    ExtendDeletion: bool = ...,
    CrossRegionCopyTargets: Sequence[CrossRegionCopyTargetTypeDef] = ...,  # (4)
    Exclusions: ExclusionsTypeDef = ...,  # (5)
) -> CreateLifecyclePolicyResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: SettablePolicyStateValuesType](./literals.md#settablepolicystatevaluestype) 
2. See [:material-code-braces: PolicyDetailsTypeDef](./type_defs.md#policydetailstypedef) 
3. See [:material-code-brackets: DefaultPolicyTypeValuesType](./literals.md#defaultpolicytypevaluestype) 
4. See [:material-code-braces: CrossRegionCopyTargetTypeDef](./type_defs.md#crossregioncopytargettypedef) 
5. See [:material-code-braces: ExclusionsTypeDef](./type_defs.md#exclusionstypedef) 
6. See [:material-code-braces: CreateLifecyclePolicyResponseTypeDef](./type_defs.md#createlifecyclepolicyresponsetypedef) 


```python
# create_lifecycle_policy method usage example with argument unpacking

kwargs: CreateLifecyclePolicyRequestRequestTypeDef = {  # (1)
    "ExecutionRoleArn": ...,
    "Description": ...,
    "State": ...,
}

parent.create_lifecycle_policy(**kwargs)
```

1. See [:material-code-braces: CreateLifecyclePolicyRequestRequestTypeDef](./type_defs.md#createlifecyclepolicyrequestrequesttypedef) 

### delete\_lifecycle\_policy

Deletes the specified lifecycle policy and halts the automated operations that
the policy specified.

Type annotations and code completion for `#!python session.client("dlm").delete_lifecycle_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client)

```python
# delete_lifecycle_policy method definition

await def delete_lifecycle_policy(
    self,
    *,
    PolicyId: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_lifecycle_policy method usage example with argument unpacking

kwargs: DeleteLifecyclePolicyRequestRequestTypeDef = {  # (1)
    "PolicyId": ...,
}

parent.delete_lifecycle_policy(**kwargs)
```

1. See [:material-code-braces: DeleteLifecyclePolicyRequestRequestTypeDef](./type_defs.md#deletelifecyclepolicyrequestrequesttypedef) 

### get\_lifecycle\_policies

Gets summary information about all or the specified data lifecycle policies.

Type annotations and code completion for `#!python session.client("dlm").get_lifecycle_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client)

```python
# get_lifecycle_policies method definition

await def get_lifecycle_policies(
    self,
    *,
    PolicyIds: Sequence[str] = ...,
    State: GettablePolicyStateValuesType = ...,  # (1)
    ResourceTypes: Sequence[ResourceTypeValuesType] = ...,  # (2)
    TargetTags: Sequence[str] = ...,
    TagsToAdd: Sequence[str] = ...,
    DefaultPolicyType: DefaultPoliciesTypeValuesType = ...,  # (3)
) -> GetLifecyclePoliciesResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: GettablePolicyStateValuesType](./literals.md#gettablepolicystatevaluestype) 
2. See [:material-code-brackets: ResourceTypeValuesType](./literals.md#resourcetypevaluestype) 
3. See [:material-code-brackets: DefaultPoliciesTypeValuesType](./literals.md#defaultpoliciestypevaluestype) 
4. See [:material-code-braces: GetLifecyclePoliciesResponseTypeDef](./type_defs.md#getlifecyclepoliciesresponsetypedef) 


```python
# get_lifecycle_policies method usage example with argument unpacking

kwargs: GetLifecyclePoliciesRequestRequestTypeDef = {  # (1)
    "PolicyIds": ...,
}

parent.get_lifecycle_policies(**kwargs)
```

1. See [:material-code-braces: GetLifecyclePoliciesRequestRequestTypeDef](./type_defs.md#getlifecyclepoliciesrequestrequesttypedef) 

### get\_lifecycle\_policy

Gets detailed information about the specified lifecycle policy.

Type annotations and code completion for `#!python session.client("dlm").get_lifecycle_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client)

```python
# get_lifecycle_policy method definition

await def get_lifecycle_policy(
    self,
    *,
    PolicyId: str,
) -> GetLifecyclePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLifecyclePolicyResponseTypeDef](./type_defs.md#getlifecyclepolicyresponsetypedef) 


```python
# get_lifecycle_policy method usage example with argument unpacking

kwargs: GetLifecyclePolicyRequestRequestTypeDef = {  # (1)
    "PolicyId": ...,
}

parent.get_lifecycle_policy(**kwargs)
```

1. See [:material-code-braces: GetLifecyclePolicyRequestRequestTypeDef](./type_defs.md#getlifecyclepolicyrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags for the specified resource.

Type annotations and code completion for `#!python session.client("dlm").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client)

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

### tag\_resource

Adds the specified tags to the specified resource.

Type annotations and code completion for `#!python session.client("dlm").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes the specified tags from the specified resource.

Type annotations and code completion for `#!python session.client("dlm").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client)

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

### update\_lifecycle\_policy

Updates the specified lifecycle policy.

Type annotations and code completion for `#!python session.client("dlm").update_lifecycle_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client)

```python
# update_lifecycle_policy method definition

await def update_lifecycle_policy(
    self,
    *,
    PolicyId: str,
    ExecutionRoleArn: str = ...,
    State: SettablePolicyStateValuesType = ...,  # (1)
    Description: str = ...,
    PolicyDetails: PolicyDetailsTypeDef = ...,  # (2)
    CreateInterval: int = ...,
    RetainInterval: int = ...,
    CopyTags: bool = ...,
    ExtendDeletion: bool = ...,
    CrossRegionCopyTargets: Sequence[CrossRegionCopyTargetTypeDef] = ...,  # (3)
    Exclusions: ExclusionsTypeDef = ...,  # (4)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: SettablePolicyStateValuesType](./literals.md#settablepolicystatevaluestype) 
2. See [:material-code-braces: PolicyDetailsTypeDef](./type_defs.md#policydetailstypedef) 
3. See [:material-code-braces: CrossRegionCopyTargetTypeDef](./type_defs.md#crossregioncopytargettypedef) 
4. See [:material-code-braces: ExclusionsTypeDef](./type_defs.md#exclusionstypedef) 


```python
# update_lifecycle_policy method usage example with argument unpacking

kwargs: UpdateLifecyclePolicyRequestRequestTypeDef = {  # (1)
    "PolicyId": ...,
}

parent.update_lifecycle_policy(**kwargs)
```

1. See [:material-code-braces: UpdateLifecyclePolicyRequestRequestTypeDef](./type_defs.md#updatelifecyclepolicyrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("dlm").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("dlm").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client)

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





