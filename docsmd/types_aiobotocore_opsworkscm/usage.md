# Examples

> [Index](../README.md) > [OpsWorksCM](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [OpsWorksCM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
    type annotations stubs module [types-aiobotocore-opsworkscm](https://pypi.org/project/types-aiobotocore-opsworkscm/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[opsworkscm]` package installed.

Write your `OpsWorksCM` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("opsworkscm") as client:  # (1)
        result = await client.associate_node()  # (2)
    ```

    1. client: [OpsWorksCMClient](./client.md)
    2. result: [:material-code-braces: AssociateNodeResponseTypeDef](./type_defs.md#associatenoderesponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("opsworkscm") as client:  # (1)
        paginator = client.get_paginator("describe_backups")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [OpsWorksCMClient](./client.md)
    2. paginator: [DescribeBackupsPaginator](./paginators.md#describebackupspaginator)
    3. item: [:material-code-braces: DescribeBackupsResponseTypeDef](./type_defs.md#describebackupsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("opsworkscm") as client:  # (1)
        waiter = client.get_waiter("node_associated")  # (2)
        await waiter.wait()
    ```

    1. client: [OpsWorksCMClient](./client.md)
    2. waiter: [NodeAssociatedWaiter](./waiters.md#nodeassociatedwaiter)


### Explicit type annotations

With `types-aioboto3-lite[opsworkscm]`
or a standalone `types_aiobotocore_opsworkscm` package, you have to explicitly specify
`client: OpsWorksCMClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_opsworkscm.client import OpsWorksCMClient
    from types_aiobotocore_opsworkscm.type_defs import AssociateNodeResponseTypeDef
    from types_aiobotocore_opsworkscm.type_defs import AssociateNodeRequestRequestTypeDef


    session = Session()

    client: OpsWorksCMClient
    async with session.client("opsworkscm") as client:  # (1)
        kwargs: AssociateNodeRequestRequestTypeDef = {...}  # (2)
        result: AssociateNodeResponseTypeDef = await client.associate_node(**kwargs)  # (3)
    ```

    1. client: [OpsWorksCMClient](./client.md)
    2. kwargs: [:material-code-braces: AssociateNodeRequestRequestTypeDef](./type_defs.md#associatenoderequestrequesttypedef) 
    3. result: [:material-code-braces: AssociateNodeResponseTypeDef](./type_defs.md#associatenoderesponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_opsworkscm.client import OpsWorksCMClient
    from types_aiobotocore_opsworkscm.paginator import DescribeBackupsPaginator
    from types_aiobotocore_opsworkscm.type_defs import DescribeBackupsResponseTypeDef


    session = Session()

    client: OpsWorksCMClient
    async with session.client("opsworkscm") as client:  # (1)
        paginator: DescribeBackupsPaginator = client.get_paginator("describe_backups")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeBackupsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [OpsWorksCMClient](./client.md)
    2. paginator: [DescribeBackupsPaginator](./paginators.md#describebackupspaginator)
    3. item: [:material-code-braces: DescribeBackupsResponseTypeDef](./type_defs.md#describebackupsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_opsworkscm.client import OpsWorksCMClient
    from types_aiobotocore_opsworkscm.waiter import NodeAssociatedWaiter


    session = Session()

    async with session.client("opsworkscm") as client:  # (1)
        waiter = client.get_waiter("node_associated")  # (2)
        await waiter.wait()
    ```

    1. client: [OpsWorksCMClient](./client.md)
    2. waiter: [NodeAssociatedWaiter](./waiters.md#nodeassociatedwaiter)


