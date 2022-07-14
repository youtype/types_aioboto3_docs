# Examples

> [Index](../README.md) > [MQ](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MQ](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
    type annotations stubs module [types-aiobotocore-mq](https://pypi.org/project/types-aiobotocore-mq/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[mq]` package installed.

Write your `MQ` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("mq") as client:  # (1)
        result = await client.create_broker()  # (2)
    ```

    1. client: [MQClient](./client.md)
    2. result: [:material-code-braces: CreateBrokerResponseTypeDef](./type_defs.md#createbrokerresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("mq") as client:  # (1)
        paginator = client.get_paginator("list_brokers")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [MQClient](./client.md)
    2. paginator: [ListBrokersPaginator](./paginators.md#listbrokerspaginator)
    3. item: [:material-code-braces: ListBrokersResponseTypeDef](./type_defs.md#listbrokersresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[mq]`
or a standalone `types_aiobotocore_mq` package, you have to explicitly specify
`client: MQClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_mq.client import MQClient
    from types_aiobotocore_mq.type_defs import CreateBrokerResponseTypeDef
    from types_aiobotocore_mq.type_defs import CreateBrokerRequestRequestTypeDef


    session = Session()

    client: MQClient
    async with session.client("mq") as client:  # (1)
        kwargs: CreateBrokerRequestRequestTypeDef = {...}  # (2)
        result: CreateBrokerResponseTypeDef = await client.create_broker(**kwargs)  # (3)
    ```

    1. client: [MQClient](./client.md)
    2. kwargs: [:material-code-braces: CreateBrokerRequestRequestTypeDef](./type_defs.md#createbrokerrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateBrokerResponseTypeDef](./type_defs.md#createbrokerresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_mq.client import MQClient
    from types_aiobotocore_mq.paginator import ListBrokersPaginator
    from types_aiobotocore_mq.type_defs import ListBrokersResponseTypeDef


    session = Session()

    client: MQClient
    async with session.client("mq") as client:  # (1)
        paginator: ListBrokersPaginator = client.get_paginator("list_brokers")  # (2)
        async for item in paginator.paginate(...):
            item: ListBrokersResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [MQClient](./client.md)
    2. paginator: [ListBrokersPaginator](./paginators.md#listbrokerspaginator)
    3. item: [:material-code-braces: ListBrokersResponseTypeDef](./type_defs.md#listbrokersresponsetypedef) 




