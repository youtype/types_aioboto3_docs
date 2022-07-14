# Examples

> [Index](../README.md) > [mgn](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [mgn](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
    type annotations stubs module [types-aiobotocore-mgn](https://pypi.org/project/types-aiobotocore-mgn/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[mgn]` package installed.

Write your `mgn` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("mgn") as client:  # (1)
        result = await client.change_server_life_cycle_state()  # (2)
    ```

    1. client: [mgnClient](./client.md)
    2. result: [:material-code-braces: SourceServerResponseMetadataTypeDef](./type_defs.md#sourceserverresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("mgn") as client:  # (1)
        paginator = client.get_paginator("describe_job_log_items")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [mgnClient](./client.md)
    2. paginator: [DescribeJobLogItemsPaginator](./paginators.md#describejoblogitemspaginator)
    3. item: [:material-code-braces: DescribeJobLogItemsResponseTypeDef](./type_defs.md#describejoblogitemsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[mgn]`
or a standalone `types_aiobotocore_mgn` package, you have to explicitly specify
`client: mgnClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_mgn.client import mgnClient
    from types_aiobotocore_mgn.type_defs import SourceServerResponseMetadataTypeDef
    from types_aiobotocore_mgn.type_defs import ChangeServerLifeCycleStateRequestRequestTypeDef


    session = Session()

    client: mgnClient
    async with session.client("mgn") as client:  # (1)
        kwargs: ChangeServerLifeCycleStateRequestRequestTypeDef = {...}  # (2)
        result: SourceServerResponseMetadataTypeDef = await client.change_server_life_cycle_state(**kwargs)  # (3)
    ```

    1. client: [mgnClient](./client.md)
    2. kwargs: [:material-code-braces: ChangeServerLifeCycleStateRequestRequestTypeDef](./type_defs.md#changeserverlifecyclestaterequestrequesttypedef) 
    3. result: [:material-code-braces: SourceServerResponseMetadataTypeDef](./type_defs.md#sourceserverresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_mgn.client import mgnClient
    from types_aiobotocore_mgn.paginator import DescribeJobLogItemsPaginator
    from types_aiobotocore_mgn.type_defs import DescribeJobLogItemsResponseTypeDef


    session = Session()

    client: mgnClient
    async with session.client("mgn") as client:  # (1)
        paginator: DescribeJobLogItemsPaginator = client.get_paginator("describe_job_log_items")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeJobLogItemsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [mgnClient](./client.md)
    2. paginator: [DescribeJobLogItemsPaginator](./paginators.md#describejoblogitemspaginator)
    3. item: [:material-code-braces: DescribeJobLogItemsResponseTypeDef](./type_defs.md#describejoblogitemsresponsetypedef) 




