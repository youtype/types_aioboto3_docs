# Examples

> [Index](../README.md) > [QLDB](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [QLDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
    type annotations stubs module [types-aiobotocore-qldb](https://pypi.org/project/types-aiobotocore-qldb/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[qldb]` package installed.

Write your `QLDB` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("qldb") as client:  # (1)
        result = await client.cancel_journal_kinesis_stream()  # (2)
    ```

    1. client: [QLDBClient](./client.md)
    2. result: [:material-code-braces: CancelJournalKinesisStreamResponseTypeDef](./type_defs.md#canceljournalkinesisstreamresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[qldb]`
or a standalone `types_aiobotocore_qldb` package, you have to explicitly specify
`client: QLDBClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_qldb.client import QLDBClient
    from types_aiobotocore_qldb.type_defs import CancelJournalKinesisStreamResponseTypeDef
    from types_aiobotocore_qldb.type_defs import CancelJournalKinesisStreamRequestRequestTypeDef


    session = Session()

    client: QLDBClient
    async with session.client("qldb") as client:  # (1)
        kwargs: CancelJournalKinesisStreamRequestRequestTypeDef = {...}  # (2)
        result: CancelJournalKinesisStreamResponseTypeDef = await client.cancel_journal_kinesis_stream(**kwargs)  # (3)
    ```

    1. client: [QLDBClient](./client.md)
    2. kwargs: [:material-code-braces: CancelJournalKinesisStreamRequestRequestTypeDef](./type_defs.md#canceljournalkinesisstreamrequestrequesttypedef) 
    3. result: [:material-code-braces: CancelJournalKinesisStreamResponseTypeDef](./type_defs.md#canceljournalkinesisstreamresponsetypedef) 






