# Examples

> [Index](../README.md) > [PersonalizeEvents](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PersonalizeEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
    type annotations stubs module [types-aiobotocore-personalize-events](https://pypi.org/project/types-aiobotocore-personalize-events/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[personalize-events]` package installed.

Write your `PersonalizeEvents` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("personalize-events") as client:  # (1)
        result = await client.put_events()  # (2)
    ```

    1. client: [PersonalizeEventsClient](./client.md)
    2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 






### Explicit type annotations

With `types-aioboto3-lite[personalize-events]`
or a standalone `types_aiobotocore_personalize_events` package, you have to explicitly specify
`client: PersonalizeEventsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_personalize_events.client import PersonalizeEventsClient
    from types_aiobotocore_personalize_events.type_defs import EmptyResponseMetadataTypeDef
    from types_aiobotocore_personalize_events.type_defs import PutEventsRequestRequestTypeDef


    session = Session()

    client: PersonalizeEventsClient
    async with session.client("personalize-events") as client:  # (1)
        kwargs: PutEventsRequestRequestTypeDef = {...}  # (2)
        result: EmptyResponseMetadataTypeDef = await client.put_events(**kwargs)  # (3)
    ```

    1. client: [PersonalizeEventsClient](./client.md)
    2. kwargs: [:material-code-braces: PutEventsRequestRequestTypeDef](./type_defs.md#puteventsrequestrequesttypedef) 
    3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 






