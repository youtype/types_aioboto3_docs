# Examples

> [Index](../README.md) > [WorkMailMessageFlow](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WorkMailMessageFlow](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow)
    type annotations stubs module [types-aiobotocore-workmailmessageflow](https://pypi.org/project/types-aiobotocore-workmailmessageflow/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[workmailmessageflow]` package installed.

Write your `WorkMailMessageFlow` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("workmailmessageflow") as client:  # (1)
        result = await client.get_raw_message_content()  # (2)
    ```

    1. client: [WorkMailMessageFlowClient](./client.md)
    2. result: [:material-code-braces: GetRawMessageContentResponseTypeDef](./type_defs.md#getrawmessagecontentresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[workmailmessageflow]`
or a standalone `types_aiobotocore_workmailmessageflow` package, you have to explicitly specify
`client: WorkMailMessageFlowClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_workmailmessageflow.client import WorkMailMessageFlowClient
    from types_aiobotocore_workmailmessageflow.type_defs import GetRawMessageContentResponseTypeDef
    from types_aiobotocore_workmailmessageflow.type_defs import GetRawMessageContentRequestRequestTypeDef


    session = Session()

    client: WorkMailMessageFlowClient
    async with session.client("workmailmessageflow") as client:  # (1)
        kwargs: GetRawMessageContentRequestRequestTypeDef = {...}  # (2)
        result: GetRawMessageContentResponseTypeDef = await client.get_raw_message_content(**kwargs)  # (3)
    ```

    1. client: [WorkMailMessageFlowClient](./client.md)
    2. kwargs: [:material-code-braces: GetRawMessageContentRequestRequestTypeDef](./type_defs.md#getrawmessagecontentrequestrequesttypedef) 
    3. result: [:material-code-braces: GetRawMessageContentResponseTypeDef](./type_defs.md#getrawmessagecontentresponsetypedef) 






