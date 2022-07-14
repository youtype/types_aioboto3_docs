# Examples

> [Index](../README.md) > [SMS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
    type annotations stubs module [types-aiobotocore-sms](https://pypi.org/project/types-aiobotocore-sms/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[sms]` package installed.

Write your `SMS` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("sms") as client:  # (1)
        result = await client.create_app()  # (2)
    ```

    1. client: [SMSClient](./client.md)
    2. result: [:material-code-braces: CreateAppResponseTypeDef](./type_defs.md#createappresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("sms") as client:  # (1)
        paginator = client.get_paginator("get_connectors")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [SMSClient](./client.md)
    2. paginator: [GetConnectorsPaginator](./paginators.md#getconnectorspaginator)
    3. item: [:material-code-braces: GetConnectorsResponseTypeDef](./type_defs.md#getconnectorsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[sms]`
or a standalone `types_aiobotocore_sms` package, you have to explicitly specify
`client: SMSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_sms.client import SMSClient
    from types_aiobotocore_sms.type_defs import CreateAppResponseTypeDef
    from types_aiobotocore_sms.type_defs import CreateAppRequestRequestTypeDef


    session = Session()

    client: SMSClient
    async with session.client("sms") as client:  # (1)
        kwargs: CreateAppRequestRequestTypeDef = {...}  # (2)
        result: CreateAppResponseTypeDef = await client.create_app(**kwargs)  # (3)
    ```

    1. client: [SMSClient](./client.md)
    2. kwargs: [:material-code-braces: CreateAppRequestRequestTypeDef](./type_defs.md#createapprequestrequesttypedef) 
    3. result: [:material-code-braces: CreateAppResponseTypeDef](./type_defs.md#createappresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_sms.client import SMSClient
    from types_aiobotocore_sms.paginator import GetConnectorsPaginator
    from types_aiobotocore_sms.type_defs import GetConnectorsResponseTypeDef


    session = Session()

    client: SMSClient
    async with session.client("sms") as client:  # (1)
        paginator: GetConnectorsPaginator = client.get_paginator("get_connectors")  # (2)
        async for item in paginator.paginate(...):
            item: GetConnectorsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [SMSClient](./client.md)
    2. paginator: [GetConnectorsPaginator](./paginators.md#getconnectorspaginator)
    3. item: [:material-code-braces: GetConnectorsResponseTypeDef](./type_defs.md#getconnectorsresponsetypedef) 




