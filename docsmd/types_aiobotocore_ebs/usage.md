# Examples

> [Index](../README.md) > [EBS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EBS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
    type annotations stubs module [types-aiobotocore-ebs](https://pypi.org/project/types-aiobotocore-ebs/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[ebs]` package installed.

Write your `EBS` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("ebs") as client:  # (1)
        result = await client.complete_snapshot()  # (2)
    ```

    1. client: [EBSClient](./client.md)
    2. result: [:material-code-braces: CompleteSnapshotResponseTypeDef](./type_defs.md#completesnapshotresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[ebs]`
or a standalone `types_aiobotocore_ebs` package, you have to explicitly specify
`client: EBSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_ebs.client import EBSClient
    from types_aiobotocore_ebs.type_defs import CompleteSnapshotResponseTypeDef
    from types_aiobotocore_ebs.type_defs import CompleteSnapshotRequestRequestTypeDef


    session = Session()

    client: EBSClient
    async with session.client("ebs") as client:  # (1)
        kwargs: CompleteSnapshotRequestRequestTypeDef = {...}  # (2)
        result: CompleteSnapshotResponseTypeDef = await client.complete_snapshot(**kwargs)  # (3)
    ```

    1. client: [EBSClient](./client.md)
    2. kwargs: [:material-code-braces: CompleteSnapshotRequestRequestTypeDef](./type_defs.md#completesnapshotrequestrequesttypedef) 
    3. result: [:material-code-braces: CompleteSnapshotResponseTypeDef](./type_defs.md#completesnapshotresponsetypedef) 






