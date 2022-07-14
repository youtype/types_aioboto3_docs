# Examples

> [Index](../README.md) > [SESV2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SESV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
    type annotations stubs module [types-aiobotocore-sesv2](https://pypi.org/project/types-aiobotocore-sesv2/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[sesv2]` package installed.

Write your `SESV2` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("sesv2") as client:  # (1)
        result = await client.create_deliverability_test_report()  # (2)
    ```

    1. client: [SESV2Client](./client.md)
    2. result: [:material-code-braces: CreateDeliverabilityTestReportResponseTypeDef](./type_defs.md#createdeliverabilitytestreportresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[sesv2]`
or a standalone `types_aiobotocore_sesv2` package, you have to explicitly specify
`client: SESV2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_sesv2.client import SESV2Client
    from types_aiobotocore_sesv2.type_defs import CreateDeliverabilityTestReportResponseTypeDef
    from types_aiobotocore_sesv2.type_defs import CreateDeliverabilityTestReportRequestRequestTypeDef


    session = Session()

    client: SESV2Client
    async with session.client("sesv2") as client:  # (1)
        kwargs: CreateDeliverabilityTestReportRequestRequestTypeDef = {...}  # (2)
        result: CreateDeliverabilityTestReportResponseTypeDef = await client.create_deliverability_test_report(**kwargs)  # (3)
    ```

    1. client: [SESV2Client](./client.md)
    2. kwargs: [:material-code-braces: CreateDeliverabilityTestReportRequestRequestTypeDef](./type_defs.md#createdeliverabilitytestreportrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateDeliverabilityTestReportResponseTypeDef](./type_defs.md#createdeliverabilitytestreportresponsetypedef) 






