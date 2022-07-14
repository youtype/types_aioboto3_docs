# Examples

> [Index](../README.md) > [DataSync](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DataSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
    type annotations stubs module [types-aiobotocore-datasync](https://pypi.org/project/types-aiobotocore-datasync/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[datasync]` package installed.

Write your `DataSync` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("datasync") as client:  # (1)
        result = await client.create_agent()  # (2)
    ```

    1. client: [DataSyncClient](./client.md)
    2. result: [:material-code-braces: CreateAgentResponseTypeDef](./type_defs.md#createagentresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("datasync") as client:  # (1)
        paginator = client.get_paginator("list_agents")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [DataSyncClient](./client.md)
    2. paginator: [ListAgentsPaginator](./paginators.md#listagentspaginator)
    3. item: [:material-code-braces: ListAgentsResponseTypeDef](./type_defs.md#listagentsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[datasync]`
or a standalone `types_aiobotocore_datasync` package, you have to explicitly specify
`client: DataSyncClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_datasync.client import DataSyncClient
    from types_aiobotocore_datasync.type_defs import CreateAgentResponseTypeDef
    from types_aiobotocore_datasync.type_defs import CreateAgentRequestRequestTypeDef


    session = Session()

    client: DataSyncClient
    async with session.client("datasync") as client:  # (1)
        kwargs: CreateAgentRequestRequestTypeDef = {...}  # (2)
        result: CreateAgentResponseTypeDef = await client.create_agent(**kwargs)  # (3)
    ```

    1. client: [DataSyncClient](./client.md)
    2. kwargs: [:material-code-braces: CreateAgentRequestRequestTypeDef](./type_defs.md#createagentrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateAgentResponseTypeDef](./type_defs.md#createagentresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_datasync.client import DataSyncClient
    from types_aiobotocore_datasync.paginator import ListAgentsPaginator
    from types_aiobotocore_datasync.type_defs import ListAgentsResponseTypeDef


    session = Session()

    client: DataSyncClient
    async with session.client("datasync") as client:  # (1)
        paginator: ListAgentsPaginator = client.get_paginator("list_agents")  # (2)
        async for item in paginator.paginate(...):
            item: ListAgentsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [DataSyncClient](./client.md)
    2. paginator: [ListAgentsPaginator](./paginators.md#listagentspaginator)
    3. item: [:material-code-braces: ListAgentsResponseTypeDef](./type_defs.md#listagentsresponsetypedef) 




