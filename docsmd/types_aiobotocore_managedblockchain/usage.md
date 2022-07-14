# Examples

> [Index](../README.md) > [ManagedBlockchain](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ManagedBlockchain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
    type annotations stubs module [types-aiobotocore-managedblockchain](https://pypi.org/project/types-aiobotocore-managedblockchain/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[managedblockchain]` package installed.

Write your `ManagedBlockchain` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("managedblockchain") as client:  # (1)
        result = await client.create_member()  # (2)
    ```

    1. client: [ManagedBlockchainClient](./client.md)
    2. result: [:material-code-braces: CreateMemberOutputTypeDef](./type_defs.md#creatememberoutputtypedef) 






### Explicit type annotations

With `types-aioboto3-lite[managedblockchain]`
or a standalone `types_aiobotocore_managedblockchain` package, you have to explicitly specify
`client: ManagedBlockchainClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_managedblockchain.client import ManagedBlockchainClient
    from types_aiobotocore_managedblockchain.type_defs import CreateMemberOutputTypeDef
    from types_aiobotocore_managedblockchain.type_defs import CreateMemberInputRequestTypeDef


    session = Session()

    client: ManagedBlockchainClient
    async with session.client("managedblockchain") as client:  # (1)
        kwargs: CreateMemberInputRequestTypeDef = {...}  # (2)
        result: CreateMemberOutputTypeDef = await client.create_member(**kwargs)  # (3)
    ```

    1. client: [ManagedBlockchainClient](./client.md)
    2. kwargs: [:material-code-braces: CreateMemberInputRequestTypeDef](./type_defs.md#creatememberinputrequesttypedef) 
    3. result: [:material-code-braces: CreateMemberOutputTypeDef](./type_defs.md#creatememberoutputtypedef) 






