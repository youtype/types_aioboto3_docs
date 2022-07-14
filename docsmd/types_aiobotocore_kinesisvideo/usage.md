# Examples

> [Index](../README.md) > [KinesisVideo](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [KinesisVideo](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
    type annotations stubs module [types-aiobotocore-kinesisvideo](https://pypi.org/project/types-aiobotocore-kinesisvideo/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[kinesisvideo]` package installed.

Write your `KinesisVideo` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("kinesisvideo") as client:  # (1)
        result = await client.create_signaling_channel()  # (2)
    ```

    1. client: [KinesisVideoClient](./client.md)
    2. result: [:material-code-braces: CreateSignalingChannelOutputTypeDef](./type_defs.md#createsignalingchanneloutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("kinesisvideo") as client:  # (1)
        paginator = client.get_paginator("list_signaling_channels")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [KinesisVideoClient](./client.md)
    2. paginator: [ListSignalingChannelsPaginator](./paginators.md#listsignalingchannelspaginator)
    3. item: [:material-code-braces: ListSignalingChannelsOutputTypeDef](./type_defs.md#listsignalingchannelsoutputtypedef) 




### Explicit type annotations

With `types-aioboto3-lite[kinesisvideo]`
or a standalone `types_aiobotocore_kinesisvideo` package, you have to explicitly specify
`client: KinesisVideoClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_kinesisvideo.client import KinesisVideoClient
    from types_aiobotocore_kinesisvideo.type_defs import CreateSignalingChannelOutputTypeDef
    from types_aiobotocore_kinesisvideo.type_defs import CreateSignalingChannelInputRequestTypeDef


    session = Session()

    client: KinesisVideoClient
    async with session.client("kinesisvideo") as client:  # (1)
        kwargs: CreateSignalingChannelInputRequestTypeDef = {...}  # (2)
        result: CreateSignalingChannelOutputTypeDef = await client.create_signaling_channel(**kwargs)  # (3)
    ```

    1. client: [KinesisVideoClient](./client.md)
    2. kwargs: [:material-code-braces: CreateSignalingChannelInputRequestTypeDef](./type_defs.md#createsignalingchannelinputrequesttypedef) 
    3. result: [:material-code-braces: CreateSignalingChannelOutputTypeDef](./type_defs.md#createsignalingchanneloutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_kinesisvideo.client import KinesisVideoClient
    from types_aiobotocore_kinesisvideo.paginator import ListSignalingChannelsPaginator
    from types_aiobotocore_kinesisvideo.type_defs import ListSignalingChannelsOutputTypeDef


    session = Session()

    client: KinesisVideoClient
    async with session.client("kinesisvideo") as client:  # (1)
        paginator: ListSignalingChannelsPaginator = client.get_paginator("list_signaling_channels")  # (2)
        async for item in paginator.paginate(...):
            item: ListSignalingChannelsOutputTypeDef
            print(item)  # (3)
    ```

    1. client: [KinesisVideoClient](./client.md)
    2. paginator: [ListSignalingChannelsPaginator](./paginators.md#listsignalingchannelspaginator)
    3. item: [:material-code-braces: ListSignalingChannelsOutputTypeDef](./type_defs.md#listsignalingchannelsoutputtypedef) 




