# Waiters

> [Index](../README.md) > [Schemas](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [Schemas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#schemas)
    type annotations stubs module [types-aiobotocore-schemas](https://pypi.org/project/types-aiobotocore-schemas/).

## CodeBindingExistsWaiter

Type annotations and code completion for `#!python session.client("schemas").get_waiter("code_binding_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas/waiter/CodeBindingExists.html#Schemas.Waiter.CodeBindingExists)

```python
# CodeBindingExistsWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_schemas.waiter import CodeBindingExistsWaiter

session = get_session()
async with session.client("schemas") as client:  # (1)
    waiter: CodeBindingExistsWaiter = client.get_waiter("code_binding_exists")  # (2)
    await waiter.wait()
```

1. client: [SchemasClient](./client.md)
2. waiter: [CodeBindingExistsWaiter](./waiters.md#codebindingexistswaiter)


### wait

Type annotations and code completion for `#!python CodeBindingExistsWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Language: str,
    RegistryName: str,
    SchemaName: str,
    SchemaVersion: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeCodeBindingRequestWaitTypeDef = {  # (1)
    "Language": ...,
    "RegistryName": ...,
    "SchemaName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeCodeBindingRequestWaitTypeDef](./type_defs.md#describecodebindingrequestwaittypedef) 