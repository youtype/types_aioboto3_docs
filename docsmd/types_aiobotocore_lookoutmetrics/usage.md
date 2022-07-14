# Examples

> [Index](../README.md) > [LookoutMetrics](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LookoutMetrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
    type annotations stubs module [types-aiobotocore-lookoutmetrics](https://pypi.org/project/types-aiobotocore-lookoutmetrics/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[lookoutmetrics]` package installed.

Write your `LookoutMetrics` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("lookoutmetrics") as client:  # (1)
        result = await client.create_alert()  # (2)
    ```

    1. client: [LookoutMetricsClient](./client.md)
    2. result: [:material-code-braces: CreateAlertResponseTypeDef](./type_defs.md#createalertresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[lookoutmetrics]`
or a standalone `types_aiobotocore_lookoutmetrics` package, you have to explicitly specify
`client: LookoutMetricsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_lookoutmetrics.client import LookoutMetricsClient
    from types_aiobotocore_lookoutmetrics.type_defs import CreateAlertResponseTypeDef
    from types_aiobotocore_lookoutmetrics.type_defs import CreateAlertRequestRequestTypeDef


    session = Session()

    client: LookoutMetricsClient
    async with session.client("lookoutmetrics") as client:  # (1)
        kwargs: CreateAlertRequestRequestTypeDef = {...}  # (2)
        result: CreateAlertResponseTypeDef = await client.create_alert(**kwargs)  # (3)
    ```

    1. client: [LookoutMetricsClient](./client.md)
    2. kwargs: [:material-code-braces: CreateAlertRequestRequestTypeDef](./type_defs.md#createalertrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateAlertResponseTypeDef](./type_defs.md#createalertresponsetypedef) 






