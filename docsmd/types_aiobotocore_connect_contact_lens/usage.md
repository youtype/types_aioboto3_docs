# Examples

> [Index](../README.md) > [ConnectContactLens](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ConnectContactLens](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens)
    type annotations stubs module [types-aiobotocore-connect-contact-lens](https://pypi.org/project/types-aiobotocore-connect-contact-lens/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[connect-contact-lens]` package installed.

Write your `ConnectContactLens` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("connect-contact-lens") as client:  # (1)
        result = await client.list_realtime_contact_analysis_segments()  # (2)
    ```

    1. client: [ConnectContactLensClient](./client.md)
    2. result: [:material-code-braces: ListRealtimeContactAnalysisSegmentsResponseTypeDef](./type_defs.md#listrealtimecontactanalysissegmentsresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[connect-contact-lens]`
or a standalone `types_aiobotocore_connect_contact_lens` package, you have to explicitly specify
`client: ConnectContactLensClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_connect_contact_lens.client import ConnectContactLensClient
    from types_aiobotocore_connect_contact_lens.type_defs import ListRealtimeContactAnalysisSegmentsResponseTypeDef
    from types_aiobotocore_connect_contact_lens.type_defs import ListRealtimeContactAnalysisSegmentsRequestRequestTypeDef


    session = Session()

    client: ConnectContactLensClient
    async with session.client("connect-contact-lens") as client:  # (1)
        kwargs: ListRealtimeContactAnalysisSegmentsRequestRequestTypeDef = {...}  # (2)
        result: ListRealtimeContactAnalysisSegmentsResponseTypeDef = await client.list_realtime_contact_analysis_segments(**kwargs)  # (3)
    ```

    1. client: [ConnectContactLensClient](./client.md)
    2. kwargs: [:material-code-braces: ListRealtimeContactAnalysisSegmentsRequestRequestTypeDef](./type_defs.md#listrealtimecontactanalysissegmentsrequestrequesttypedef) 
    3. result: [:material-code-braces: ListRealtimeContactAnalysisSegmentsResponseTypeDef](./type_defs.md#listrealtimecontactanalysissegmentsresponsetypedef) 






