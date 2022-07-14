# Examples

> [Index](../README.md) > [KinesisAnalytics](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [KinesisAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
    type annotations stubs module [types-aiobotocore-kinesisanalytics](https://pypi.org/project/types-aiobotocore-kinesisanalytics/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[kinesisanalytics]` package installed.

Write your `KinesisAnalytics` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("kinesisanalytics") as client:  # (1)
        result = await client.create_application()  # (2)
    ```

    1. client: [KinesisAnalyticsClient](./client.md)
    2. result: [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[kinesisanalytics]`
or a standalone `types_aiobotocore_kinesisanalytics` package, you have to explicitly specify
`client: KinesisAnalyticsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_kinesisanalytics.client import KinesisAnalyticsClient
    from types_aiobotocore_kinesisanalytics.type_defs import CreateApplicationResponseTypeDef
    from types_aiobotocore_kinesisanalytics.type_defs import CreateApplicationRequestRequestTypeDef


    session = Session()

    client: KinesisAnalyticsClient
    async with session.client("kinesisanalytics") as client:  # (1)
        kwargs: CreateApplicationRequestRequestTypeDef = {...}  # (2)
        result: CreateApplicationResponseTypeDef = await client.create_application(**kwargs)  # (3)
    ```

    1. client: [KinesisAnalyticsClient](./client.md)
    2. kwargs: [:material-code-braces: CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef) 






