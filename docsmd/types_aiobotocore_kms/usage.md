# Examples

> [Index](../README.md) > [KMS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [KMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
    type annotations stubs module [types-aiobotocore-kms](https://pypi.org/project/types-aiobotocore-kms/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[kms]` package installed.

Write your `KMS` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("kms") as client:  # (1)
        result = await client.cancel_key_deletion()  # (2)
    ```

    1. client: [KMSClient](./client.md)
    2. result: [:material-code-braces: CancelKeyDeletionResponseTypeDef](./type_defs.md#cancelkeydeletionresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("kms") as client:  # (1)
        paginator = client.get_paginator("list_aliases")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [KMSClient](./client.md)
    2. paginator: [ListAliasesPaginator](./paginators.md#listaliasespaginator)
    3. item: [:material-code-braces: ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[kms]`
or a standalone `types_aiobotocore_kms` package, you have to explicitly specify
`client: KMSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_kms.client import KMSClient
    from types_aiobotocore_kms.type_defs import CancelKeyDeletionResponseTypeDef
    from types_aiobotocore_kms.type_defs import CancelKeyDeletionRequestRequestTypeDef


    session = Session()

    client: KMSClient
    async with session.client("kms") as client:  # (1)
        kwargs: CancelKeyDeletionRequestRequestTypeDef = {...}  # (2)
        result: CancelKeyDeletionResponseTypeDef = await client.cancel_key_deletion(**kwargs)  # (3)
    ```

    1. client: [KMSClient](./client.md)
    2. kwargs: [:material-code-braces: CancelKeyDeletionRequestRequestTypeDef](./type_defs.md#cancelkeydeletionrequestrequesttypedef) 
    3. result: [:material-code-braces: CancelKeyDeletionResponseTypeDef](./type_defs.md#cancelkeydeletionresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_kms.client import KMSClient
    from types_aiobotocore_kms.paginator import ListAliasesPaginator
    from types_aiobotocore_kms.type_defs import ListAliasesResponseTypeDef


    session = Session()

    client: KMSClient
    async with session.client("kms") as client:  # (1)
        paginator: ListAliasesPaginator = client.get_paginator("list_aliases")  # (2)
        async for item in paginator.paginate(...):
            item: ListAliasesResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [KMSClient](./client.md)
    2. paginator: [ListAliasesPaginator](./paginators.md#listaliasespaginator)
    3. item: [:material-code-braces: ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef) 




