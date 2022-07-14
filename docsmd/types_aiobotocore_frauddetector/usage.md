# Examples

> [Index](../README.md) > [FraudDetector](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [FraudDetector](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
    type annotations stubs module [types-aiobotocore-frauddetector](https://pypi.org/project/types-aiobotocore-frauddetector/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[frauddetector]` package installed.

Write your `FraudDetector` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("frauddetector") as client:  # (1)
        result = await client.batch_create_variable()  # (2)
    ```

    1. client: [FraudDetectorClient](./client.md)
    2. result: [:material-code-braces: BatchCreateVariableResultTypeDef](./type_defs.md#batchcreatevariableresulttypedef) 






### Explicit type annotations

With `types-aioboto3-lite[frauddetector]`
or a standalone `types_aiobotocore_frauddetector` package, you have to explicitly specify
`client: FraudDetectorClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_frauddetector.client import FraudDetectorClient
    from types_aiobotocore_frauddetector.type_defs import BatchCreateVariableResultTypeDef
    from types_aiobotocore_frauddetector.type_defs import BatchCreateVariableRequestRequestTypeDef


    session = Session()

    client: FraudDetectorClient
    async with session.client("frauddetector") as client:  # (1)
        kwargs: BatchCreateVariableRequestRequestTypeDef = {...}  # (2)
        result: BatchCreateVariableResultTypeDef = await client.batch_create_variable(**kwargs)  # (3)
    ```

    1. client: [FraudDetectorClient](./client.md)
    2. kwargs: [:material-code-braces: BatchCreateVariableRequestRequestTypeDef](./type_defs.md#batchcreatevariablerequestrequesttypedef) 
    3. result: [:material-code-braces: BatchCreateVariableResultTypeDef](./type_defs.md#batchcreatevariableresulttypedef) 






