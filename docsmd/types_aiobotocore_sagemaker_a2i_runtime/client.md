# AugmentedAIRuntimeClient

> [Index](../README.md) > [AugmentedAIRuntime](./README.md) > AugmentedAIRuntimeClient

!!! note ""

    Auto-generated documentation for [AugmentedAIRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#augmentedairuntime)
    type annotations stubs module [types-aiobotocore-sagemaker-a2i-runtime](https://pypi.org/project/types-aiobotocore-sagemaker-a2i-runtime/).

## AugmentedAIRuntimeClient

Type annotations and code completion for `#!python session.client("sagemaker-a2i-runtime")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)

```python
# AugmentedAIRuntimeClient usage example

from aioboto3.session import Session
from types_aiobotocore_sagemaker_a2i_runtime.client import AugmentedAIRuntimeClient

session = Session()
async with session.client("sagemaker-a2i-runtime") as client:
    client: AugmentedAIRuntimeClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("sagemaker-a2i-runtime").exceptions` structure.

```python
# AugmentedAIRuntimeClient.exceptions usage example

async with session.client("sagemaker-a2i-runtime") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# AugmentedAIRuntimeClient.exceptions type checking example

from types_aiobotocore_sagemaker_a2i_runtime.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("sagemaker-a2i-runtime").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("sagemaker-a2i-runtime").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)

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


### delete\_human\_loop

Deletes the specified human loop for a flow definition.

Type annotations and code completion for `#!python session.client("sagemaker-a2i-runtime").delete_human_loop` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)

```python
# delete_human_loop method definition

await def delete_human_loop(
    self,
    *,
    HumanLoopName: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_human_loop method usage example with argument unpacking

kwargs: DeleteHumanLoopRequestRequestTypeDef = {  # (1)
    "HumanLoopName": ...,
}

parent.delete_human_loop(**kwargs)
```

1. See [:material-code-braces: DeleteHumanLoopRequestRequestTypeDef](./type_defs.md#deletehumanlooprequestrequesttypedef) 

### describe\_human\_loop

Returns information about the specified human loop.

Type annotations and code completion for `#!python session.client("sagemaker-a2i-runtime").describe_human_loop` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)

```python
# describe_human_loop method definition

await def describe_human_loop(
    self,
    *,
    HumanLoopName: str,
) -> DescribeHumanLoopResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeHumanLoopResponseTypeDef](./type_defs.md#describehumanloopresponsetypedef) 


```python
# describe_human_loop method usage example with argument unpacking

kwargs: DescribeHumanLoopRequestRequestTypeDef = {  # (1)
    "HumanLoopName": ...,
}

parent.describe_human_loop(**kwargs)
```

1. See [:material-code-braces: DescribeHumanLoopRequestRequestTypeDef](./type_defs.md#describehumanlooprequestrequesttypedef) 

### list\_human\_loops

Returns information about human loops, given the specified parameters.

Type annotations and code completion for `#!python session.client("sagemaker-a2i-runtime").list_human_loops` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)

```python
# list_human_loops method definition

await def list_human_loops(
    self,
    *,
    FlowDefinitionArn: str,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    SortOrder: SortOrderType = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListHumanLoopsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-braces: ListHumanLoopsResponseTypeDef](./type_defs.md#listhumanloopsresponsetypedef) 


```python
# list_human_loops method usage example with argument unpacking

kwargs: ListHumanLoopsRequestRequestTypeDef = {  # (1)
    "FlowDefinitionArn": ...,
}

parent.list_human_loops(**kwargs)
```

1. See [:material-code-braces: ListHumanLoopsRequestRequestTypeDef](./type_defs.md#listhumanloopsrequestrequesttypedef) 

### start\_human\_loop

Starts a human loop, provided that at least one activation condition is met.

Type annotations and code completion for `#!python session.client("sagemaker-a2i-runtime").start_human_loop` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)

```python
# start_human_loop method definition

await def start_human_loop(
    self,
    *,
    HumanLoopName: str,
    FlowDefinitionArn: str,
    HumanLoopInput: HumanLoopInputTypeDef,  # (1)
    DataAttributes: HumanLoopDataAttributesTypeDef = ...,  # (2)
) -> StartHumanLoopResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: HumanLoopInputTypeDef](./type_defs.md#humanloopinputtypedef) 
2. See [:material-code-braces: HumanLoopDataAttributesTypeDef](./type_defs.md#humanloopdataattributestypedef) 
3. See [:material-code-braces: StartHumanLoopResponseTypeDef](./type_defs.md#starthumanloopresponsetypedef) 


```python
# start_human_loop method usage example with argument unpacking

kwargs: StartHumanLoopRequestRequestTypeDef = {  # (1)
    "HumanLoopName": ...,
    "FlowDefinitionArn": ...,
    "HumanLoopInput": ...,
}

parent.start_human_loop(**kwargs)
```

1. See [:material-code-braces: StartHumanLoopRequestRequestTypeDef](./type_defs.md#starthumanlooprequestrequesttypedef) 

### stop\_human\_loop

Stops the specified human loop.

Type annotations and code completion for `#!python session.client("sagemaker-a2i-runtime").stop_human_loop` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)

```python
# stop_human_loop method definition

await def stop_human_loop(
    self,
    *,
    HumanLoopName: str,
) -> dict[str, Any]:
    ...
```



```python
# stop_human_loop method usage example with argument unpacking

kwargs: StopHumanLoopRequestRequestTypeDef = {  # (1)
    "HumanLoopName": ...,
}

parent.stop_human_loop(**kwargs)
```

1. See [:material-code-braces: StopHumanLoopRequestRequestTypeDef](./type_defs.md#stophumanlooprequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("sagemaker-a2i-runtime").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("sagemaker-a2i-runtime").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)

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

Type annotations and code completion for `#!python session.client("sagemaker-a2i-runtime").get_paginator` method with overloads.

- `client.get_paginator("list_human_loops")` -> [ListHumanLoopsPaginator](./paginators.md#listhumanloopspaginator)


