# Examples

> [Index](../README.md) > [ChimeSDKMediaPipelines](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ChimeSDKMediaPipelines](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
    type annotations stubs module [types-aiobotocore-chime-sdk-media-pipelines](https://pypi.org/project/types-aiobotocore-chime-sdk-media-pipelines/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[chime-sdk-media-pipelines]` package installed.

Write your `ChimeSDKMediaPipelines` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("chime-sdk-media-pipelines") as client:  # (1)
        result = await client.create_media_capture_pipeline()  # (2)
    ```

    1. client: [ChimeSDKMediaPipelinesClient](./client.md)
    2. result: [:material-code-braces: CreateMediaCapturePipelineResponseTypeDef](./type_defs.md#createmediacapturepipelineresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[chime-sdk-media-pipelines]`
or a standalone `types_aiobotocore_chime_sdk_media_pipelines` package, you have to explicitly specify
`client: ChimeSDKMediaPipelinesClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_chime_sdk_media_pipelines.client import ChimeSDKMediaPipelinesClient
    from types_aiobotocore_chime_sdk_media_pipelines.type_defs import CreateMediaCapturePipelineResponseTypeDef
    from types_aiobotocore_chime_sdk_media_pipelines.type_defs import CreateMediaCapturePipelineRequestRequestTypeDef


    session = Session()

    client: ChimeSDKMediaPipelinesClient
    async with session.client("chime-sdk-media-pipelines") as client:  # (1)
        kwargs: CreateMediaCapturePipelineRequestRequestTypeDef = {...}  # (2)
        result: CreateMediaCapturePipelineResponseTypeDef = await client.create_media_capture_pipeline(**kwargs)  # (3)
    ```

    1. client: [ChimeSDKMediaPipelinesClient](./client.md)
    2. kwargs: [:material-code-braces: CreateMediaCapturePipelineRequestRequestTypeDef](./type_defs.md#createmediacapturepipelinerequestrequesttypedef) 
    3. result: [:material-code-braces: CreateMediaCapturePipelineResponseTypeDef](./type_defs.md#createmediacapturepipelineresponsetypedef) 






