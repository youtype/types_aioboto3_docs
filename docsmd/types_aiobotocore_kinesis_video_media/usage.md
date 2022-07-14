# Examples

> [Index](../README.md) > [KinesisVideoMedia](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [KinesisVideoMedia](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia)
    type annotations stubs module [types-aiobotocore-kinesis-video-media](https://pypi.org/project/types-aiobotocore-kinesis-video-media/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[kinesis-video-media]` package installed.

Write your `KinesisVideoMedia` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("kinesis-video-media") as client:  # (1)
        result = await client.get_media()  # (2)
    ```

    1. client: [KinesisVideoMediaClient](./client.md)
    2. result: [:material-code-braces: GetMediaOutputTypeDef](./type_defs.md#getmediaoutputtypedef) 






### Explicit type annotations

With `types-aioboto3-lite[kinesis-video-media]`
or a standalone `types_aiobotocore_kinesis_video_media` package, you have to explicitly specify
`client: KinesisVideoMediaClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_kinesis_video_media.client import KinesisVideoMediaClient
    from types_aiobotocore_kinesis_video_media.type_defs import GetMediaOutputTypeDef
    from types_aiobotocore_kinesis_video_media.type_defs import GetMediaInputRequestTypeDef


    session = Session()

    client: KinesisVideoMediaClient
    async with session.client("kinesis-video-media") as client:  # (1)
        kwargs: GetMediaInputRequestTypeDef = {...}  # (2)
        result: GetMediaOutputTypeDef = await client.get_media(**kwargs)  # (3)
    ```

    1. client: [KinesisVideoMediaClient](./client.md)
    2. kwargs: [:material-code-braces: GetMediaInputRequestTypeDef](./type_defs.md#getmediainputrequesttypedef) 
    3. result: [:material-code-braces: GetMediaOutputTypeDef](./type_defs.md#getmediaoutputtypedef) 






