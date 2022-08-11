# Examples

> [Index](../README.md) > [RDS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [RDS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
    type annotations stubs module [types-aiobotocore-rds](https://pypi.org/project/types-aiobotocore-rds/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[rds]` package installed.

Write your `RDS` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("rds") as client:  # (1)
        result = await client.add_role_to_db_cluster()  # (2)
    ```

    1. client: [RDSClient](./client.md)
    2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("rds") as client:  # (1)
        paginator = client.get_paginator("describe_certificates")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [RDSClient](./client.md)
    2. paginator: [DescribeCertificatesPaginator](./paginators.md#describecertificatespaginator)
    3. item: [:material-code-braces: CertificateMessageTypeDef](./type_defs.md#certificatemessagetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("rds") as client:  # (1)
        waiter = client.get_waiter("db_cluster_snapshot_available")  # (2)
        await waiter.wait()
    ```

    1. client: [RDSClient](./client.md)
    2. waiter: [DBClusterSnapshotAvailableWaiter](./waiters.md#dbclustersnapshotavailablewaiter)


### Explicit type annotations

With `types-aioboto3-lite[rds]`
or a standalone `types_aiobotocore_rds` package, you have to explicitly specify
`client: RDSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_rds.client import RDSClient
    from types_aiobotocore_rds.type_defs import EmptyResponseMetadataTypeDef
    from types_aiobotocore_rds.type_defs import AddRoleToDBClusterMessageRequestTypeDef


    session = Session()

    client: RDSClient
    async with session.client("rds") as client:  # (1)
        kwargs: AddRoleToDBClusterMessageRequestTypeDef = {...}  # (2)
        result: EmptyResponseMetadataTypeDef = await client.add_role_to_db_cluster(**kwargs)  # (3)
    ```

    1. client: [RDSClient](./client.md)
    2. kwargs: [:material-code-braces: AddRoleToDBClusterMessageRequestTypeDef](./type_defs.md#addroletodbclustermessagerequesttypedef) 
    3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_rds.client import RDSClient
    from types_aiobotocore_rds.paginator import DescribeCertificatesPaginator
    from types_aiobotocore_rds.type_defs import CertificateMessageTypeDef


    session = Session()

    client: RDSClient
    async with session.client("rds") as client:  # (1)
        paginator: DescribeCertificatesPaginator = client.get_paginator("describe_certificates")  # (2)
        async for item in paginator.paginate(...):
            item: CertificateMessageTypeDef
            print(item)  # (3)
    ```

    1. client: [RDSClient](./client.md)
    2. paginator: [DescribeCertificatesPaginator](./paginators.md#describecertificatespaginator)
    3. item: [:material-code-braces: CertificateMessageTypeDef](./type_defs.md#certificatemessagetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_rds.client import RDSClient
    from types_aiobotocore_rds.waiter import DBClusterSnapshotAvailableWaiter


    session = Session()

    async with session.client("rds") as client:  # (1)
        waiter = client.get_waiter("db_cluster_snapshot_available")  # (2)
        await waiter.wait()
    ```

    1. client: [RDSClient](./client.md)
    2. waiter: [DBClusterSnapshotAvailableWaiter](./waiters.md#dbclustersnapshotavailablewaiter)


