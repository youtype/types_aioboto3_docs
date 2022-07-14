# Examples

> [Index](../README.md) > [BackupGateway](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [BackupGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
    type annotations stubs module [types-aiobotocore-backup-gateway](https://pypi.org/project/types-aiobotocore-backup-gateway/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[backup-gateway]` package installed.

Write your `BackupGateway` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("backup-gateway") as client:  # (1)
        result = await client.associate_gateway_to_server()  # (2)
    ```

    1. client: [BackupGatewayClient](./client.md)
    2. result: [:material-code-braces: AssociateGatewayToServerOutputTypeDef](./type_defs.md#associategatewaytoserveroutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("backup-gateway") as client:  # (1)
        paginator = client.get_paginator("list_gateways")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [BackupGatewayClient](./client.md)
    2. paginator: [ListGatewaysPaginator](./paginators.md#listgatewayspaginator)
    3. item: [:material-code-braces: ListGatewaysOutputTypeDef](./type_defs.md#listgatewaysoutputtypedef) 




### Explicit type annotations

With `types-aioboto3-lite[backup-gateway]`
or a standalone `types_aiobotocore_backup_gateway` package, you have to explicitly specify
`client: BackupGatewayClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_backup_gateway.client import BackupGatewayClient
    from types_aiobotocore_backup_gateway.type_defs import AssociateGatewayToServerOutputTypeDef
    from types_aiobotocore_backup_gateway.type_defs import AssociateGatewayToServerInputRequestTypeDef


    session = Session()

    client: BackupGatewayClient
    async with session.client("backup-gateway") as client:  # (1)
        kwargs: AssociateGatewayToServerInputRequestTypeDef = {...}  # (2)
        result: AssociateGatewayToServerOutputTypeDef = await client.associate_gateway_to_server(**kwargs)  # (3)
    ```

    1. client: [BackupGatewayClient](./client.md)
    2. kwargs: [:material-code-braces: AssociateGatewayToServerInputRequestTypeDef](./type_defs.md#associategatewaytoserverinputrequesttypedef) 
    3. result: [:material-code-braces: AssociateGatewayToServerOutputTypeDef](./type_defs.md#associategatewaytoserveroutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_backup_gateway.client import BackupGatewayClient
    from types_aiobotocore_backup_gateway.paginator import ListGatewaysPaginator
    from types_aiobotocore_backup_gateway.type_defs import ListGatewaysOutputTypeDef


    session = Session()

    client: BackupGatewayClient
    async with session.client("backup-gateway") as client:  # (1)
        paginator: ListGatewaysPaginator = client.get_paginator("list_gateways")  # (2)
        async for item in paginator.paginate(...):
            item: ListGatewaysOutputTypeDef
            print(item)  # (3)
    ```

    1. client: [BackupGatewayClient](./client.md)
    2. paginator: [ListGatewaysPaginator](./paginators.md#listgatewayspaginator)
    3. item: [:material-code-braces: ListGatewaysOutputTypeDef](./type_defs.md#listgatewaysoutputtypedef) 




