# Examples

> [Index](../README.md) > [CloudTrail](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudTrail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
    type annotations stubs module [types-aiobotocore-cloudtrail](https://pypi.org/project/types-aiobotocore-cloudtrail/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[cloudtrail]` package installed.

Write your `CloudTrail` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cloudtrail") as client:  # (1)
        result = await client.cancel_query()  # (2)
    ```

    1. client: [CloudTrailClient](./client.md)
    2. result: [:material-code-braces: CancelQueryResponseTypeDef](./type_defs.md#cancelqueryresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cloudtrail") as client:  # (1)
        paginator = client.get_paginator("list_public_keys")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [CloudTrailClient](./client.md)
    2. paginator: [ListPublicKeysPaginator](./paginators.md#listpublickeyspaginator)
    3. item: [:material-code-braces: ListPublicKeysResponseTypeDef](./type_defs.md#listpublickeysresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[cloudtrail]`
or a standalone `types_aiobotocore_cloudtrail` package, you have to explicitly specify
`client: CloudTrailClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudtrail.client import CloudTrailClient
    from types_aiobotocore_cloudtrail.type_defs import CancelQueryResponseTypeDef
    from types_aiobotocore_cloudtrail.type_defs import CancelQueryRequestRequestTypeDef


    session = Session()

    client: CloudTrailClient
    async with session.client("cloudtrail") as client:  # (1)
        kwargs: CancelQueryRequestRequestTypeDef = {...}  # (2)
        result: CancelQueryResponseTypeDef = await client.cancel_query(**kwargs)  # (3)
    ```

    1. client: [CloudTrailClient](./client.md)
    2. kwargs: [:material-code-braces: CancelQueryRequestRequestTypeDef](./type_defs.md#cancelqueryrequestrequesttypedef) 
    3. result: [:material-code-braces: CancelQueryResponseTypeDef](./type_defs.md#cancelqueryresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudtrail.client import CloudTrailClient
    from types_aiobotocore_cloudtrail.paginator import ListPublicKeysPaginator
    from types_aiobotocore_cloudtrail.type_defs import ListPublicKeysResponseTypeDef


    session = Session()

    client: CloudTrailClient
    async with session.client("cloudtrail") as client:  # (1)
        paginator: ListPublicKeysPaginator = client.get_paginator("list_public_keys")  # (2)
        async for item in paginator.paginate(...):
            item: ListPublicKeysResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [CloudTrailClient](./client.md)
    2. paginator: [ListPublicKeysPaginator](./paginators.md#listpublickeyspaginator)
    3. item: [:material-code-braces: ListPublicKeysResponseTypeDef](./type_defs.md#listpublickeysresponsetypedef) 




