# Examples

> [Index](../README.md) > [TranscribeService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [TranscribeService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
    type annotations stubs module [types-aiobotocore-transcribe](https://pypi.org/project/types-aiobotocore-transcribe/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[transcribe]` package installed.

Write your `TranscribeService` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("transcribe") as client:  # (1)
        result = await client.create_call_analytics_category()  # (2)
    ```

    1. client: [TranscribeServiceClient](./client.md)
    2. result: [:material-code-braces: CreateCallAnalyticsCategoryResponseTypeDef](./type_defs.md#createcallanalyticscategoryresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[transcribe]`
or a standalone `types_aiobotocore_transcribe` package, you have to explicitly specify
`client: TranscribeServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_transcribe.client import TranscribeServiceClient
    from types_aiobotocore_transcribe.type_defs import CreateCallAnalyticsCategoryResponseTypeDef
    from types_aiobotocore_transcribe.type_defs import CreateCallAnalyticsCategoryRequestRequestTypeDef


    session = Session()

    client: TranscribeServiceClient
    async with session.client("transcribe") as client:  # (1)
        kwargs: CreateCallAnalyticsCategoryRequestRequestTypeDef = {...}  # (2)
        result: CreateCallAnalyticsCategoryResponseTypeDef = await client.create_call_analytics_category(**kwargs)  # (3)
    ```

    1. client: [TranscribeServiceClient](./client.md)
    2. kwargs: [:material-code-braces: CreateCallAnalyticsCategoryRequestRequestTypeDef](./type_defs.md#createcallanalyticscategoryrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateCallAnalyticsCategoryResponseTypeDef](./type_defs.md#createcallanalyticscategoryresponsetypedef) 






