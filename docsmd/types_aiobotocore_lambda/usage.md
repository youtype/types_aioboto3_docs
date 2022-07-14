# Examples

> [Index](../README.md) > [Lambda](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Lambda](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
    type annotations stubs module [types-aiobotocore-lambda](https://pypi.org/project/types-aiobotocore-lambda/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[lambda]` package installed.

Write your `Lambda` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("lambda") as client:  # (1)
        result = await client.add_layer_version_permission()  # (2)
    ```

    1. client: [LambdaClient](./client.md)
    2. result: [:material-code-braces: AddLayerVersionPermissionResponseTypeDef](./type_defs.md#addlayerversionpermissionresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("lambda") as client:  # (1)
        paginator = client.get_paginator("list_aliases")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [LambdaClient](./client.md)
    2. paginator: [ListAliasesPaginator](./paginators.md#listaliasespaginator)
    3. item: [:material-code-braces: ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("lambda") as client:  # (1)
        waiter = client.get_waiter("function_active")  # (2)
        await waiter.wait()
    ```

    1. client: [LambdaClient](./client.md)
    2. waiter: [FunctionActiveWaiter](./waiters.md#functionactivewaiter)


### Explicit type annotations

With `types-aioboto3-lite[lambda]`
or a standalone `types_aiobotocore_lambda` package, you have to explicitly specify
`client: LambdaClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_lambda.client import LambdaClient
    from types_aiobotocore_lambda.type_defs import AddLayerVersionPermissionResponseTypeDef
    from types_aiobotocore_lambda.type_defs import AddLayerVersionPermissionRequestRequestTypeDef


    session = Session()

    client: LambdaClient
    async with session.client("lambda") as client:  # (1)
        kwargs: AddLayerVersionPermissionRequestRequestTypeDef = {...}  # (2)
        result: AddLayerVersionPermissionResponseTypeDef = await client.add_layer_version_permission(**kwargs)  # (3)
    ```

    1. client: [LambdaClient](./client.md)
    2. kwargs: [:material-code-braces: AddLayerVersionPermissionRequestRequestTypeDef](./type_defs.md#addlayerversionpermissionrequestrequesttypedef) 
    3. result: [:material-code-braces: AddLayerVersionPermissionResponseTypeDef](./type_defs.md#addlayerversionpermissionresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_lambda.client import LambdaClient
    from types_aiobotocore_lambda.paginator import ListAliasesPaginator
    from types_aiobotocore_lambda.type_defs import ListAliasesResponseTypeDef


    session = Session()

    client: LambdaClient
    async with session.client("lambda") as client:  # (1)
        paginator: ListAliasesPaginator = client.get_paginator("list_aliases")  # (2)
        async for item in paginator.paginate(...):
            item: ListAliasesResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [LambdaClient](./client.md)
    2. paginator: [ListAliasesPaginator](./paginators.md#listaliasespaginator)
    3. item: [:material-code-braces: ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_lambda.client import LambdaClient
    from types_aiobotocore_lambda.waiter import FunctionActiveWaiter


    session = Session()

    async with session.client("lambda") as client:  # (1)
        waiter = client.get_waiter("function_active")  # (2)
        await waiter.wait()
    ```

    1. client: [LambdaClient](./client.md)
    2. waiter: [FunctionActiveWaiter](./waiters.md#functionactivewaiter)


