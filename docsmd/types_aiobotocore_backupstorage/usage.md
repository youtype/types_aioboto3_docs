# Examples

> [Index](../README.md) > [BackupStorage](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [BackupStorage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
    type annotations stubs module [types-aiobotocore-backupstorage](https://pypi.org/project/types-aiobotocore-backupstorage/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[backupstorage]` package installed.

Write your `BackupStorage` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("backupstorage") as client:  # (1)
        result = await client.delete_object()  # (2)
    ```

    1. client: [BackupStorageClient](./client.md)
    2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 






### Explicit type annotations

With `types-aioboto3-lite[backupstorage]`
or a standalone `types_aiobotocore_backupstorage` package, you have to explicitly specify
`client: BackupStorageClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_backupstorage.client import BackupStorageClient
    from types_aiobotocore_backupstorage.type_defs import EmptyResponseMetadataTypeDef
    from types_aiobotocore_backupstorage.type_defs import DeleteObjectInputRequestTypeDef


    session = Session()

    client: BackupStorageClient
    async with session.client("backupstorage") as client:  # (1)
        kwargs: DeleteObjectInputRequestTypeDef = {...}  # (2)
        result: EmptyResponseMetadataTypeDef = await client.delete_object(**kwargs)  # (3)
    ```

    1. client: [BackupStorageClient](./client.md)
    2. kwargs: [:material-code-braces: DeleteObjectInputRequestTypeDef](./type_defs.md#deleteobjectinputrequesttypedef) 
    3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 






