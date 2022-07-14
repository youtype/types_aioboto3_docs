# Examples

> [Index](../README.md) > [RDSDataService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [RDSDataService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
    type annotations stubs module [types-aiobotocore-rds-data](https://pypi.org/project/types-aiobotocore-rds-data/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[rds-data]` package installed.

Write your `RDSDataService` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("rds-data") as client:  # (1)
        result = await client.batch_execute_statement()  # (2)
    ```

    1. client: [RDSDataServiceClient](./client.md)
    2. result: [:material-code-braces: BatchExecuteStatementResponseTypeDef](./type_defs.md#batchexecutestatementresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[rds-data]`
or a standalone `types_aiobotocore_rds_data` package, you have to explicitly specify
`client: RDSDataServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_rds_data.client import RDSDataServiceClient
    from types_aiobotocore_rds_data.type_defs import BatchExecuteStatementResponseTypeDef
    from types_aiobotocore_rds_data.type_defs import BatchExecuteStatementRequestRequestTypeDef


    session = Session()

    client: RDSDataServiceClient
    async with session.client("rds-data") as client:  # (1)
        kwargs: BatchExecuteStatementRequestRequestTypeDef = {...}  # (2)
        result: BatchExecuteStatementResponseTypeDef = await client.batch_execute_statement(**kwargs)  # (3)
    ```

    1. client: [RDSDataServiceClient](./client.md)
    2. kwargs: [:material-code-braces: BatchExecuteStatementRequestRequestTypeDef](./type_defs.md#batchexecutestatementrequestrequesttypedef) 
    3. result: [:material-code-braces: BatchExecuteStatementResponseTypeDef](./type_defs.md#batchexecutestatementresponsetypedef) 






