# Examples

> [Index](../README.md) > [Neptune](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Neptune](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
    type annotations stubs module [types-aiobotocore-neptune](https://pypi.org/project/types-aiobotocore-neptune/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[neptune]` package installed.

Write your `Neptune` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("neptune") as client:  # (1)
        result = await client.add_role_to_db_cluster()  # (2)
    ```

    1. client: [NeptuneClient](./client.md)
    2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("neptune") as client:  # (1)
        paginator = client.get_paginator("describe_db_cluster_endpoints")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [NeptuneClient](./client.md)
    2. paginator: [DescribeDBClusterEndpointsPaginator](./paginators.md#describedbclusterendpointspaginator)
    3. item: [:material-code-braces: DBClusterEndpointMessageTypeDef](./type_defs.md#dbclusterendpointmessagetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("neptune") as client:  # (1)
        waiter = client.get_waiter("db_instance_available")  # (2)
        await waiter.wait()
    ```

    1. client: [NeptuneClient](./client.md)
    2. waiter: [DBInstanceAvailableWaiter](./waiters.md#dbinstanceavailablewaiter)


### Explicit type annotations

With `types-aioboto3-lite[neptune]`
or a standalone `types_aiobotocore_neptune` package, you have to explicitly specify
`client: NeptuneClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_neptune.client import NeptuneClient
    from types_aiobotocore_neptune.type_defs import EmptyResponseMetadataTypeDef
    from types_aiobotocore_neptune.type_defs import AddRoleToDBClusterMessageRequestTypeDef


    session = Session()

    client: NeptuneClient
    async with session.client("neptune") as client:  # (1)
        kwargs: AddRoleToDBClusterMessageRequestTypeDef = {...}  # (2)
        result: EmptyResponseMetadataTypeDef = await client.add_role_to_db_cluster(**kwargs)  # (3)
    ```

    1. client: [NeptuneClient](./client.md)
    2. kwargs: [:material-code-braces: AddRoleToDBClusterMessageRequestTypeDef](./type_defs.md#addroletodbclustermessagerequesttypedef) 
    3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_neptune.client import NeptuneClient
    from types_aiobotocore_neptune.paginator import DescribeDBClusterEndpointsPaginator
    from types_aiobotocore_neptune.type_defs import DBClusterEndpointMessageTypeDef


    session = Session()

    client: NeptuneClient
    async with session.client("neptune") as client:  # (1)
        paginator: DescribeDBClusterEndpointsPaginator = client.get_paginator("describe_db_cluster_endpoints")  # (2)
        async for item in paginator.paginate(...):
            item: DBClusterEndpointMessageTypeDef
            print(item)  # (3)
    ```

    1. client: [NeptuneClient](./client.md)
    2. paginator: [DescribeDBClusterEndpointsPaginator](./paginators.md#describedbclusterendpointspaginator)
    3. item: [:material-code-braces: DBClusterEndpointMessageTypeDef](./type_defs.md#dbclusterendpointmessagetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_neptune.client import NeptuneClient
    from types_aiobotocore_neptune.waiter import DBInstanceAvailableWaiter


    session = Session()

    async with session.client("neptune") as client:  # (1)
        waiter = client.get_waiter("db_instance_available")  # (2)
        await waiter.wait()
    ```

    1. client: [NeptuneClient](./client.md)
    2. waiter: [DBInstanceAvailableWaiter](./waiters.md#dbinstanceavailablewaiter)


