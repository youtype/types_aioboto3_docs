# Waiters

> [Index](../README.md) > [Lambda](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [Lambda](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#lambda)
    type annotations stubs module [types-aiobotocore-lambda](https://pypi.org/project/types-aiobotocore-lambda/).

## FunctionActiveV2Waiter

Type annotations and code completion for `#!python session.client("lambda").get_waiter("function_active_v2")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda/waiter/FunctionActiveV2.html#Lambda.Waiter.FunctionActiveV2)

```python
# FunctionActiveV2Waiter usage example

from aioboto3.session import Session

from types_aiobotocore_lambda.waiter import FunctionActiveV2Waiter

session = get_session()
async with session.client("lambda") as client:  # (1)
    waiter: FunctionActiveV2Waiter = client.get_waiter("function_active_v2")  # (2)
    await waiter.wait()
```

1. client: [LambdaClient](./client.md)
2. waiter: [FunctionActiveV2Waiter](./waiters.md#functionactivev2waiter)


### wait

Type annotations and code completion for `#!python FunctionActiveV2Waiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    FunctionName: str,
    Qualifier: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetFunctionRequestWaitTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetFunctionRequestWaitTypeDef](./type_defs.md#getfunctionrequestwaittypedef) 
## FunctionActiveWaiter

Type annotations and code completion for `#!python session.client("lambda").get_waiter("function_active")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda/waiter/FunctionActive.html#Lambda.Waiter.FunctionActive)

```python
# FunctionActiveWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_lambda.waiter import FunctionActiveWaiter

session = get_session()
async with session.client("lambda") as client:  # (1)
    waiter: FunctionActiveWaiter = client.get_waiter("function_active")  # (2)
    await waiter.wait()
```

1. client: [LambdaClient](./client.md)
2. waiter: [FunctionActiveWaiter](./waiters.md#functionactivewaiter)


### wait

Type annotations and code completion for `#!python FunctionActiveWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    FunctionName: str,
    Qualifier: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetFunctionConfigurationRequestWaitTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetFunctionConfigurationRequestWaitTypeDef](./type_defs.md#getfunctionconfigurationrequestwaittypedef) 
## FunctionExistsWaiter

Type annotations and code completion for `#!python session.client("lambda").get_waiter("function_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda/waiter/FunctionExists.html#Lambda.Waiter.FunctionExists)

```python
# FunctionExistsWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_lambda.waiter import FunctionExistsWaiter

session = get_session()
async with session.client("lambda") as client:  # (1)
    waiter: FunctionExistsWaiter = client.get_waiter("function_exists")  # (2)
    await waiter.wait()
```

1. client: [LambdaClient](./client.md)
2. waiter: [FunctionExistsWaiter](./waiters.md#functionexistswaiter)


### wait

Type annotations and code completion for `#!python FunctionExistsWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    FunctionName: str,
    Qualifier: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetFunctionRequestWaitTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetFunctionRequestWaitTypeDef](./type_defs.md#getfunctionrequestwaittypedef) 
## FunctionUpdatedV2Waiter

Type annotations and code completion for `#!python session.client("lambda").get_waiter("function_updated_v2")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda/waiter/FunctionUpdatedV2.html#Lambda.Waiter.FunctionUpdatedV2)

```python
# FunctionUpdatedV2Waiter usage example

from aioboto3.session import Session

from types_aiobotocore_lambda.waiter import FunctionUpdatedV2Waiter

session = get_session()
async with session.client("lambda") as client:  # (1)
    waiter: FunctionUpdatedV2Waiter = client.get_waiter("function_updated_v2")  # (2)
    await waiter.wait()
```

1. client: [LambdaClient](./client.md)
2. waiter: [FunctionUpdatedV2Waiter](./waiters.md#functionupdatedv2waiter)


### wait

Type annotations and code completion for `#!python FunctionUpdatedV2Waiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    FunctionName: str,
    Qualifier: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetFunctionRequestWaitTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetFunctionRequestWaitTypeDef](./type_defs.md#getfunctionrequestwaittypedef) 
## FunctionUpdatedWaiter

Type annotations and code completion for `#!python session.client("lambda").get_waiter("function_updated")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda/waiter/FunctionUpdated.html#Lambda.Waiter.FunctionUpdated)

```python
# FunctionUpdatedWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_lambda.waiter import FunctionUpdatedWaiter

session = get_session()
async with session.client("lambda") as client:  # (1)
    waiter: FunctionUpdatedWaiter = client.get_waiter("function_updated")  # (2)
    await waiter.wait()
```

1. client: [LambdaClient](./client.md)
2. waiter: [FunctionUpdatedWaiter](./waiters.md#functionupdatedwaiter)


### wait

Type annotations and code completion for `#!python FunctionUpdatedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    FunctionName: str,
    Qualifier: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetFunctionConfigurationRequestWaitTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetFunctionConfigurationRequestWaitTypeDef](./type_defs.md#getfunctionconfigurationrequestwaittypedef) 
## PublishedVersionActiveWaiter

Type annotations and code completion for `#!python session.client("lambda").get_waiter("published_version_active")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda/waiter/PublishedVersionActive.html#Lambda.Waiter.PublishedVersionActive)

```python
# PublishedVersionActiveWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_lambda.waiter import PublishedVersionActiveWaiter

session = get_session()
async with session.client("lambda") as client:  # (1)
    waiter: PublishedVersionActiveWaiter = client.get_waiter("published_version_active")  # (2)
    await waiter.wait()
```

1. client: [LambdaClient](./client.md)
2. waiter: [PublishedVersionActiveWaiter](./waiters.md#publishedversionactivewaiter)


### wait

Type annotations and code completion for `#!python PublishedVersionActiveWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    FunctionName: str,
    Qualifier: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetFunctionConfigurationRequestWaitTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetFunctionConfigurationRequestWaitTypeDef](./type_defs.md#getfunctionconfigurationrequestwaittypedef) 