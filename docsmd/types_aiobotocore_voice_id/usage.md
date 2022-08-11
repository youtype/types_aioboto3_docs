# Examples

> [Index](../README.md) > [VoiceID](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [VoiceID](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
    type annotations stubs module [types-aiobotocore-voice-id](https://pypi.org/project/types-aiobotocore-voice-id/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[voice-id]` package installed.

Write your `VoiceID` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("voice-id") as client:  # (1)
        result = await client.create_domain()  # (2)
    ```

    1. client: [VoiceIDClient](./client.md)
    2. result: [:material-code-braces: CreateDomainResponseTypeDef](./type_defs.md#createdomainresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[voice-id]`
or a standalone `types_aiobotocore_voice_id` package, you have to explicitly specify
`client: VoiceIDClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_voice_id.client import VoiceIDClient
    from types_aiobotocore_voice_id.type_defs import CreateDomainResponseTypeDef
    from types_aiobotocore_voice_id.type_defs import CreateDomainRequestRequestTypeDef


    session = Session()

    client: VoiceIDClient
    async with session.client("voice-id") as client:  # (1)
        kwargs: CreateDomainRequestRequestTypeDef = {...}  # (2)
        result: CreateDomainResponseTypeDef = await client.create_domain(**kwargs)  # (3)
    ```

    1. client: [VoiceIDClient](./client.md)
    2. kwargs: [:material-code-braces: CreateDomainRequestRequestTypeDef](./type_defs.md#createdomainrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateDomainResponseTypeDef](./type_defs.md#createdomainresponsetypedef) 






