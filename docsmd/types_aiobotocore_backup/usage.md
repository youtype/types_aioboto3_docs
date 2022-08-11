# Examples

> [Index](../README.md) > [Backup](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Backup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
    type annotations stubs module [types-aiobotocore-backup](https://pypi.org/project/types-aiobotocore-backup/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[backup]` package installed.

Write your `Backup` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("backup") as client:  # (1)
        result = await client.create_backup_plan()  # (2)
    ```

    1. client: [BackupClient](./client.md)
    2. result: [:material-code-braces: CreateBackupPlanOutputTypeDef](./type_defs.md#createbackupplanoutputtypedef) 






### Explicit type annotations

With `types-aioboto3-lite[backup]`
or a standalone `types_aiobotocore_backup` package, you have to explicitly specify
`client: BackupClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_backup.client import BackupClient
    from types_aiobotocore_backup.type_defs import CreateBackupPlanOutputTypeDef
    from types_aiobotocore_backup.type_defs import CreateBackupPlanInputRequestTypeDef


    session = Session()

    client: BackupClient
    async with session.client("backup") as client:  # (1)
        kwargs: CreateBackupPlanInputRequestTypeDef = {...}  # (2)
        result: CreateBackupPlanOutputTypeDef = await client.create_backup_plan(**kwargs)  # (3)
    ```

    1. client: [BackupClient](./client.md)
    2. kwargs: [:material-code-braces: CreateBackupPlanInputRequestTypeDef](./type_defs.md#createbackupplaninputrequesttypedef) 
    3. result: [:material-code-braces: CreateBackupPlanOutputTypeDef](./type_defs.md#createbackupplanoutputtypedef) 






