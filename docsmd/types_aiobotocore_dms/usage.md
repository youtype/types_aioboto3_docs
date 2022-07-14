# Examples

> [Index](../README.md) > [DatabaseMigrationService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DatabaseMigrationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
    type annotations stubs module [types-aiobotocore-dms](https://pypi.org/project/types-aiobotocore-dms/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[dms]` package installed.

Write your `DatabaseMigrationService` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("dms") as client:  # (1)
        result = await client.apply_pending_maintenance_action()  # (2)
    ```

    1. client: [DatabaseMigrationServiceClient](./client.md)
    2. result: [:material-code-braces: ApplyPendingMaintenanceActionResponseTypeDef](./type_defs.md#applypendingmaintenanceactionresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("dms") as client:  # (1)
        paginator = client.get_paginator("describe_certificates")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [DatabaseMigrationServiceClient](./client.md)
    2. paginator: [DescribeCertificatesPaginator](./paginators.md#describecertificatespaginator)
    3. item: [:material-code-braces: DescribeCertificatesResponseTypeDef](./type_defs.md#describecertificatesresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("dms") as client:  # (1)
        waiter = client.get_waiter("endpoint_deleted")  # (2)
        await waiter.wait()
    ```

    1. client: [DatabaseMigrationServiceClient](./client.md)
    2. waiter: [EndpointDeletedWaiter](./waiters.md#endpointdeletedwaiter)


### Explicit type annotations

With `types-aioboto3-lite[dms]`
or a standalone `types_aiobotocore_dms` package, you have to explicitly specify
`client: DatabaseMigrationServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_dms.client import DatabaseMigrationServiceClient
    from types_aiobotocore_dms.type_defs import ApplyPendingMaintenanceActionResponseTypeDef
    from types_aiobotocore_dms.type_defs import ApplyPendingMaintenanceActionMessageRequestTypeDef


    session = Session()

    client: DatabaseMigrationServiceClient
    async with session.client("dms") as client:  # (1)
        kwargs: ApplyPendingMaintenanceActionMessageRequestTypeDef = {...}  # (2)
        result: ApplyPendingMaintenanceActionResponseTypeDef = await client.apply_pending_maintenance_action(**kwargs)  # (3)
    ```

    1. client: [DatabaseMigrationServiceClient](./client.md)
    2. kwargs: [:material-code-braces: ApplyPendingMaintenanceActionMessageRequestTypeDef](./type_defs.md#applypendingmaintenanceactionmessagerequesttypedef) 
    3. result: [:material-code-braces: ApplyPendingMaintenanceActionResponseTypeDef](./type_defs.md#applypendingmaintenanceactionresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_dms.client import DatabaseMigrationServiceClient
    from types_aiobotocore_dms.paginator import DescribeCertificatesPaginator
    from types_aiobotocore_dms.type_defs import DescribeCertificatesResponseTypeDef


    session = Session()

    client: DatabaseMigrationServiceClient
    async with session.client("dms") as client:  # (1)
        paginator: DescribeCertificatesPaginator = client.get_paginator("describe_certificates")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeCertificatesResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [DatabaseMigrationServiceClient](./client.md)
    2. paginator: [DescribeCertificatesPaginator](./paginators.md#describecertificatespaginator)
    3. item: [:material-code-braces: DescribeCertificatesResponseTypeDef](./type_defs.md#describecertificatesresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_dms.client import DatabaseMigrationServiceClient
    from types_aiobotocore_dms.waiter import EndpointDeletedWaiter


    session = Session()

    async with session.client("dms") as client:  # (1)
        waiter = client.get_waiter("endpoint_deleted")  # (2)
        await waiter.wait()
    ```

    1. client: [DatabaseMigrationServiceClient](./client.md)
    2. waiter: [EndpointDeletedWaiter](./waiters.md#endpointdeletedwaiter)


