# Examples

> [Index](../README.md) > [MWAA](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MWAA](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
    type annotations stubs module [types-aiobotocore-mwaa](https://pypi.org/project/types-aiobotocore-mwaa/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[mwaa]` package installed.

Write your `MWAA` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("mwaa") as client:  # (1)
        result = await client.create_cli_token()  # (2)
    ```

    1. client: [MWAAClient](./client.md)
    2. result: [:material-code-braces: CreateCliTokenResponseTypeDef](./type_defs.md#createclitokenresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("mwaa") as client:  # (1)
        paginator = client.get_paginator("list_environments")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [MWAAClient](./client.md)
    2. paginator: [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
    3. item: [:material-code-braces: ListEnvironmentsOutputTypeDef](./type_defs.md#listenvironmentsoutputtypedef) 




### Explicit type annotations

With `types-aioboto3-lite[mwaa]`
or a standalone `types_aiobotocore_mwaa` package, you have to explicitly specify
`client: MWAAClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_mwaa.client import MWAAClient
    from types_aiobotocore_mwaa.type_defs import CreateCliTokenResponseTypeDef
    from types_aiobotocore_mwaa.type_defs import CreateCliTokenRequestRequestTypeDef


    session = Session()

    client: MWAAClient
    async with session.client("mwaa") as client:  # (1)
        kwargs: CreateCliTokenRequestRequestTypeDef = {...}  # (2)
        result: CreateCliTokenResponseTypeDef = await client.create_cli_token(**kwargs)  # (3)
    ```

    1. client: [MWAAClient](./client.md)
    2. kwargs: [:material-code-braces: CreateCliTokenRequestRequestTypeDef](./type_defs.md#createclitokenrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateCliTokenResponseTypeDef](./type_defs.md#createclitokenresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_mwaa.client import MWAAClient
    from types_aiobotocore_mwaa.paginator import ListEnvironmentsPaginator
    from types_aiobotocore_mwaa.type_defs import ListEnvironmentsOutputTypeDef


    session = Session()

    client: MWAAClient
    async with session.client("mwaa") as client:  # (1)
        paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")  # (2)
        async for item in paginator.paginate(...):
            item: ListEnvironmentsOutputTypeDef
            print(item)  # (3)
    ```

    1. client: [MWAAClient](./client.md)
    2. paginator: [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
    3. item: [:material-code-braces: ListEnvironmentsOutputTypeDef](./type_defs.md#listenvironmentsoutputtypedef) 




