# KinesisVideoClient

> [Index](../README.md) > [KinesisVideo](./README.md) > KinesisVideoClient

!!! note ""

    Auto-generated documentation for [KinesisVideo](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#kinesisvideo)
    type annotations stubs module [types-aiobotocore-kinesisvideo](https://pypi.org/project/types-aiobotocore-kinesisvideo/).

## KinesisVideoClient

Type annotations and code completion for `#!python session.client("kinesisvideo")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# KinesisVideoClient usage example

from aioboto3.session import Session
from types_aiobotocore_kinesisvideo.client import KinesisVideoClient

session = Session()
async with session.client("kinesisvideo") as client:
    client: KinesisVideoClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("kinesisvideo").exceptions` structure.

```python
# KinesisVideoClient.exceptions usage example

async with session.client("kinesisvideo") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.AccountChannelLimitExceededException,
        client.exceptions.AccountStreamLimitExceededException,
        client.exceptions.ClientError,
        client.exceptions.ClientLimitExceededException,
        client.exceptions.DeviceStreamLimitExceededException,
        client.exceptions.InvalidArgumentException,
        client.exceptions.InvalidDeviceException,
        client.exceptions.InvalidResourceFormatException,
        client.exceptions.NoDataRetentionException,
        client.exceptions.NotAuthorizedException,
        client.exceptions.ResourceInUseException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.StreamEdgeConfigurationNotFoundException,
        client.exceptions.TagsPerResourceExceededLimitException,
        client.exceptions.VersionMismatchException,
    ) as e:
        print(e)
```

```python
# KinesisVideoClient.exceptions type checking example

from types_aiobotocore_kinesisvideo.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("kinesisvideo").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("kinesisvideo").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### create\_signaling\_channel

Creates a signaling channel.

Type annotations and code completion for `#!python session.client("kinesisvideo").create_signaling_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# create_signaling_channel method definition

await def create_signaling_channel(
    self,
    *,
    ChannelName: str,
    ChannelType: ChannelTypeType = ...,  # (1)
    SingleMasterConfiguration: SingleMasterConfigurationTypeDef = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateSignalingChannelOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
2. See [:material-code-braces: SingleMasterConfigurationTypeDef](./type_defs.md#singlemasterconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateSignalingChannelOutputTypeDef](./type_defs.md#createsignalingchanneloutputtypedef) 


```python
# create_signaling_channel method usage example with argument unpacking

kwargs: CreateSignalingChannelInputRequestTypeDef = {  # (1)
    "ChannelName": ...,
}

parent.create_signaling_channel(**kwargs)
```

1. See [:material-code-braces: CreateSignalingChannelInputRequestTypeDef](./type_defs.md#createsignalingchannelinputrequesttypedef) 

### create\_stream

Creates a new Kinesis video stream.

Type annotations and code completion for `#!python session.client("kinesisvideo").create_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# create_stream method definition

await def create_stream(
    self,
    *,
    StreamName: str,
    DeviceName: str = ...,
    MediaType: str = ...,
    KmsKeyId: str = ...,
    DataRetentionInHours: int = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateStreamOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateStreamOutputTypeDef](./type_defs.md#createstreamoutputtypedef) 


```python
# create_stream method usage example with argument unpacking

kwargs: CreateStreamInputRequestTypeDef = {  # (1)
    "StreamName": ...,
}

parent.create_stream(**kwargs)
```

1. See [:material-code-braces: CreateStreamInputRequestTypeDef](./type_defs.md#createstreaminputrequesttypedef) 

### delete\_edge\_configuration

An asynchronous API that deletes a stream's existing edge configuration, as
well as the corresponding media from the Edge Agent.

Type annotations and code completion for `#!python session.client("kinesisvideo").delete_edge_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# delete_edge_configuration method definition

await def delete_edge_configuration(
    self,
    *,
    StreamName: str = ...,
    StreamARN: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_edge_configuration method usage example with argument unpacking

kwargs: DeleteEdgeConfigurationInputRequestTypeDef = {  # (1)
    "StreamName": ...,
}

parent.delete_edge_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteEdgeConfigurationInputRequestTypeDef](./type_defs.md#deleteedgeconfigurationinputrequesttypedef) 

### delete\_signaling\_channel

Deletes a specified signaling channel.

Type annotations and code completion for `#!python session.client("kinesisvideo").delete_signaling_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# delete_signaling_channel method definition

await def delete_signaling_channel(
    self,
    *,
    ChannelARN: str,
    CurrentVersion: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_signaling_channel method usage example with argument unpacking

kwargs: DeleteSignalingChannelInputRequestTypeDef = {  # (1)
    "ChannelARN": ...,
}

parent.delete_signaling_channel(**kwargs)
```

1. See [:material-code-braces: DeleteSignalingChannelInputRequestTypeDef](./type_defs.md#deletesignalingchannelinputrequesttypedef) 

### delete\_stream

Deletes a Kinesis video stream and the data contained in the stream.

Type annotations and code completion for `#!python session.client("kinesisvideo").delete_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# delete_stream method definition

await def delete_stream(
    self,
    *,
    StreamARN: str,
    CurrentVersion: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_stream method usage example with argument unpacking

kwargs: DeleteStreamInputRequestTypeDef = {  # (1)
    "StreamARN": ...,
}

parent.delete_stream(**kwargs)
```

1. See [:material-code-braces: DeleteStreamInputRequestTypeDef](./type_defs.md#deletestreaminputrequesttypedef) 

### describe\_edge\_configuration

Describes a stream's edge configuration that was set using the
<code>StartEdgeConfigurationUpdate</code> API and the latest status of the edge
agent's recorder and uploader jobs.

Type annotations and code completion for `#!python session.client("kinesisvideo").describe_edge_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# describe_edge_configuration method definition

await def describe_edge_configuration(
    self,
    *,
    StreamName: str = ...,
    StreamARN: str = ...,
) -> DescribeEdgeConfigurationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEdgeConfigurationOutputTypeDef](./type_defs.md#describeedgeconfigurationoutputtypedef) 


```python
# describe_edge_configuration method usage example with argument unpacking

kwargs: DescribeEdgeConfigurationInputRequestTypeDef = {  # (1)
    "StreamName": ...,
}

parent.describe_edge_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeEdgeConfigurationInputRequestTypeDef](./type_defs.md#describeedgeconfigurationinputrequesttypedef) 

### describe\_image\_generation\_configuration

Gets the <code>ImageGenerationConfiguration</code> for a given Kinesis video
stream.

Type annotations and code completion for `#!python session.client("kinesisvideo").describe_image_generation_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# describe_image_generation_configuration method definition

await def describe_image_generation_configuration(
    self,
    *,
    StreamName: str = ...,
    StreamARN: str = ...,
) -> DescribeImageGenerationConfigurationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeImageGenerationConfigurationOutputTypeDef](./type_defs.md#describeimagegenerationconfigurationoutputtypedef) 


```python
# describe_image_generation_configuration method usage example with argument unpacking

kwargs: DescribeImageGenerationConfigurationInputRequestTypeDef = {  # (1)
    "StreamName": ...,
}

parent.describe_image_generation_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeImageGenerationConfigurationInputRequestTypeDef](./type_defs.md#describeimagegenerationconfigurationinputrequesttypedef) 

### describe\_mapped\_resource\_configuration

Returns the most current information about the stream.

Type annotations and code completion for `#!python session.client("kinesisvideo").describe_mapped_resource_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# describe_mapped_resource_configuration method definition

await def describe_mapped_resource_configuration(
    self,
    *,
    StreamName: str = ...,
    StreamARN: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeMappedResourceConfigurationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMappedResourceConfigurationOutputTypeDef](./type_defs.md#describemappedresourceconfigurationoutputtypedef) 


```python
# describe_mapped_resource_configuration method usage example with argument unpacking

kwargs: DescribeMappedResourceConfigurationInputRequestTypeDef = {  # (1)
    "StreamName": ...,
}

parent.describe_mapped_resource_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeMappedResourceConfigurationInputRequestTypeDef](./type_defs.md#describemappedresourceconfigurationinputrequesttypedef) 

### describe\_media\_storage\_configuration

Returns the most current information about the channel.

Type annotations and code completion for `#!python session.client("kinesisvideo").describe_media_storage_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# describe_media_storage_configuration method definition

await def describe_media_storage_configuration(
    self,
    *,
    ChannelName: str = ...,
    ChannelARN: str = ...,
) -> DescribeMediaStorageConfigurationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMediaStorageConfigurationOutputTypeDef](./type_defs.md#describemediastorageconfigurationoutputtypedef) 


```python
# describe_media_storage_configuration method usage example with argument unpacking

kwargs: DescribeMediaStorageConfigurationInputRequestTypeDef = {  # (1)
    "ChannelName": ...,
}

parent.describe_media_storage_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeMediaStorageConfigurationInputRequestTypeDef](./type_defs.md#describemediastorageconfigurationinputrequesttypedef) 

### describe\_notification\_configuration

Gets the <code>NotificationConfiguration</code> for a given Kinesis video
stream.

Type annotations and code completion for `#!python session.client("kinesisvideo").describe_notification_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# describe_notification_configuration method definition

await def describe_notification_configuration(
    self,
    *,
    StreamName: str = ...,
    StreamARN: str = ...,
) -> DescribeNotificationConfigurationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeNotificationConfigurationOutputTypeDef](./type_defs.md#describenotificationconfigurationoutputtypedef) 


```python
# describe_notification_configuration method usage example with argument unpacking

kwargs: DescribeNotificationConfigurationInputRequestTypeDef = {  # (1)
    "StreamName": ...,
}

parent.describe_notification_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeNotificationConfigurationInputRequestTypeDef](./type_defs.md#describenotificationconfigurationinputrequesttypedef) 

### describe\_signaling\_channel

Returns the most current information about the signaling channel.

Type annotations and code completion for `#!python session.client("kinesisvideo").describe_signaling_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# describe_signaling_channel method definition

await def describe_signaling_channel(
    self,
    *,
    ChannelName: str = ...,
    ChannelARN: str = ...,
) -> DescribeSignalingChannelOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSignalingChannelOutputTypeDef](./type_defs.md#describesignalingchanneloutputtypedef) 


```python
# describe_signaling_channel method usage example with argument unpacking

kwargs: DescribeSignalingChannelInputRequestTypeDef = {  # (1)
    "ChannelName": ...,
}

parent.describe_signaling_channel(**kwargs)
```

1. See [:material-code-braces: DescribeSignalingChannelInputRequestTypeDef](./type_defs.md#describesignalingchannelinputrequesttypedef) 

### describe\_stream

Returns the most current information about the specified stream.

Type annotations and code completion for `#!python session.client("kinesisvideo").describe_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# describe_stream method definition

await def describe_stream(
    self,
    *,
    StreamName: str = ...,
    StreamARN: str = ...,
) -> DescribeStreamOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeStreamOutputTypeDef](./type_defs.md#describestreamoutputtypedef) 


```python
# describe_stream method usage example with argument unpacking

kwargs: DescribeStreamInputRequestTypeDef = {  # (1)
    "StreamName": ...,
}

parent.describe_stream(**kwargs)
```

1. See [:material-code-braces: DescribeStreamInputRequestTypeDef](./type_defs.md#describestreaminputrequesttypedef) 

### get\_data\_endpoint

Gets an endpoint for a specified stream for either reading or writing.

Type annotations and code completion for `#!python session.client("kinesisvideo").get_data_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# get_data_endpoint method definition

await def get_data_endpoint(
    self,
    *,
    APIName: APINameType,  # (1)
    StreamName: str = ...,
    StreamARN: str = ...,
) -> GetDataEndpointOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: APINameType](./literals.md#apinametype) 
2. See [:material-code-braces: GetDataEndpointOutputTypeDef](./type_defs.md#getdataendpointoutputtypedef) 


```python
# get_data_endpoint method usage example with argument unpacking

kwargs: GetDataEndpointInputRequestTypeDef = {  # (1)
    "APIName": ...,
}

parent.get_data_endpoint(**kwargs)
```

1. See [:material-code-braces: GetDataEndpointInputRequestTypeDef](./type_defs.md#getdataendpointinputrequesttypedef) 

### get\_signaling\_channel\_endpoint

Provides an endpoint for the specified signaling channel to send and receive
messages.

Type annotations and code completion for `#!python session.client("kinesisvideo").get_signaling_channel_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# get_signaling_channel_endpoint method definition

await def get_signaling_channel_endpoint(
    self,
    *,
    ChannelARN: str,
    SingleMasterChannelEndpointConfiguration: SingleMasterChannelEndpointConfigurationTypeDef = ...,  # (1)
) -> GetSignalingChannelEndpointOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SingleMasterChannelEndpointConfigurationTypeDef](./type_defs.md#singlemasterchannelendpointconfigurationtypedef) 
2. See [:material-code-braces: GetSignalingChannelEndpointOutputTypeDef](./type_defs.md#getsignalingchannelendpointoutputtypedef) 


```python
# get_signaling_channel_endpoint method usage example with argument unpacking

kwargs: GetSignalingChannelEndpointInputRequestTypeDef = {  # (1)
    "ChannelARN": ...,
}

parent.get_signaling_channel_endpoint(**kwargs)
```

1. See [:material-code-braces: GetSignalingChannelEndpointInputRequestTypeDef](./type_defs.md#getsignalingchannelendpointinputrequesttypedef) 

### list\_edge\_agent\_configurations

Returns an array of edge configurations associated with the specified Edge
Agent.

Type annotations and code completion for `#!python session.client("kinesisvideo").list_edge_agent_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# list_edge_agent_configurations method definition

await def list_edge_agent_configurations(
    self,
    *,
    HubDeviceArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListEdgeAgentConfigurationsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEdgeAgentConfigurationsOutputTypeDef](./type_defs.md#listedgeagentconfigurationsoutputtypedef) 


```python
# list_edge_agent_configurations method usage example with argument unpacking

kwargs: ListEdgeAgentConfigurationsInputRequestTypeDef = {  # (1)
    "HubDeviceArn": ...,
}

parent.list_edge_agent_configurations(**kwargs)
```

1. See [:material-code-braces: ListEdgeAgentConfigurationsInputRequestTypeDef](./type_defs.md#listedgeagentconfigurationsinputrequesttypedef) 

### list\_signaling\_channels

Returns an array of <code>ChannelInfo</code> objects.

Type annotations and code completion for `#!python session.client("kinesisvideo").list_signaling_channels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# list_signaling_channels method definition

await def list_signaling_channels(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    ChannelNameCondition: ChannelNameConditionTypeDef = ...,  # (1)
) -> ListSignalingChannelsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ChannelNameConditionTypeDef](./type_defs.md#channelnameconditiontypedef) 
2. See [:material-code-braces: ListSignalingChannelsOutputTypeDef](./type_defs.md#listsignalingchannelsoutputtypedef) 


```python
# list_signaling_channels method usage example with argument unpacking

kwargs: ListSignalingChannelsInputRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_signaling_channels(**kwargs)
```

1. See [:material-code-braces: ListSignalingChannelsInputRequestTypeDef](./type_defs.md#listsignalingchannelsinputrequesttypedef) 

### list\_streams

Returns an array of <code>StreamInfo</code> objects.

Type annotations and code completion for `#!python session.client("kinesisvideo").list_streams` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# list_streams method definition

await def list_streams(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    StreamNameCondition: StreamNameConditionTypeDef = ...,  # (1)
) -> ListStreamsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StreamNameConditionTypeDef](./type_defs.md#streamnameconditiontypedef) 
2. See [:material-code-braces: ListStreamsOutputTypeDef](./type_defs.md#liststreamsoutputtypedef) 


```python
# list_streams method usage example with argument unpacking

kwargs: ListStreamsInputRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_streams(**kwargs)
```

1. See [:material-code-braces: ListStreamsInputRequestTypeDef](./type_defs.md#liststreamsinputrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of tags associated with the specified signaling channel.

Type annotations and code completion for `#!python session.client("kinesisvideo").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
    NextToken: str = ...,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef) 

### list\_tags\_for\_stream

Returns a list of tags associated with the specified stream.

Type annotations and code completion for `#!python session.client("kinesisvideo").list_tags_for_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# list_tags_for_stream method definition

await def list_tags_for_stream(
    self,
    *,
    NextToken: str = ...,
    StreamARN: str = ...,
    StreamName: str = ...,
) -> ListTagsForStreamOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForStreamOutputTypeDef](./type_defs.md#listtagsforstreamoutputtypedef) 


```python
# list_tags_for_stream method usage example with argument unpacking

kwargs: ListTagsForStreamInputRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_tags_for_stream(**kwargs)
```

1. See [:material-code-braces: ListTagsForStreamInputRequestTypeDef](./type_defs.md#listtagsforstreaminputrequesttypedef) 

### start\_edge\_configuration\_update

An asynchronous API that updates a stream's existing edge configuration.

Type annotations and code completion for `#!python session.client("kinesisvideo").start_edge_configuration_update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# start_edge_configuration_update method definition

await def start_edge_configuration_update(
    self,
    *,
    EdgeConfig: EdgeConfigTypeDef,  # (1)
    StreamName: str = ...,
    StreamARN: str = ...,
) -> StartEdgeConfigurationUpdateOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EdgeConfigTypeDef](./type_defs.md#edgeconfigtypedef) 
2. See [:material-code-braces: StartEdgeConfigurationUpdateOutputTypeDef](./type_defs.md#startedgeconfigurationupdateoutputtypedef) 


```python
# start_edge_configuration_update method usage example with argument unpacking

kwargs: StartEdgeConfigurationUpdateInputRequestTypeDef = {  # (1)
    "EdgeConfig": ...,
}

parent.start_edge_configuration_update(**kwargs)
```

1. See [:material-code-braces: StartEdgeConfigurationUpdateInputRequestTypeDef](./type_defs.md#startedgeconfigurationupdateinputrequesttypedef) 

### tag\_resource

Adds one or more tags to a signaling channel.

Type annotations and code completion for `#!python session.client("kinesisvideo").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef) 

### tag\_stream

Adds one or more tags to a stream.

Type annotations and code completion for `#!python session.client("kinesisvideo").tag_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# tag_stream method definition

await def tag_stream(
    self,
    *,
    Tags: Mapping[str, str],
    StreamARN: str = ...,
    StreamName: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# tag_stream method usage example with argument unpacking

kwargs: TagStreamInputRequestTypeDef = {  # (1)
    "Tags": ...,
}

parent.tag_stream(**kwargs)
```

1. See [:material-code-braces: TagStreamInputRequestTypeDef](./type_defs.md#tagstreaminputrequesttypedef) 

### untag\_resource

Removes one or more tags from a signaling channel.

Type annotations and code completion for `#!python session.client("kinesisvideo").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeyList: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceInputRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeyList": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef) 

### untag\_stream

Removes one or more tags from a stream.

Type annotations and code completion for `#!python session.client("kinesisvideo").untag_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# untag_stream method definition

await def untag_stream(
    self,
    *,
    TagKeyList: Sequence[str],
    StreamARN: str = ...,
    StreamName: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# untag_stream method usage example with argument unpacking

kwargs: UntagStreamInputRequestTypeDef = {  # (1)
    "TagKeyList": ...,
}

parent.untag_stream(**kwargs)
```

1. See [:material-code-braces: UntagStreamInputRequestTypeDef](./type_defs.md#untagstreaminputrequesttypedef) 

### update\_data\_retention

Increases or decreases the stream's data retention period by the value that you
specify.

Type annotations and code completion for `#!python session.client("kinesisvideo").update_data_retention` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# update_data_retention method definition

await def update_data_retention(
    self,
    *,
    CurrentVersion: str,
    Operation: UpdateDataRetentionOperationType,  # (1)
    DataRetentionChangeInHours: int,
    StreamName: str = ...,
    StreamARN: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: UpdateDataRetentionOperationType](./literals.md#updatedataretentionoperationtype) 


```python
# update_data_retention method usage example with argument unpacking

kwargs: UpdateDataRetentionInputRequestTypeDef = {  # (1)
    "CurrentVersion": ...,
    "Operation": ...,
    "DataRetentionChangeInHours": ...,
}

parent.update_data_retention(**kwargs)
```

1. See [:material-code-braces: UpdateDataRetentionInputRequestTypeDef](./type_defs.md#updatedataretentioninputrequesttypedef) 

### update\_image\_generation\_configuration

Updates the <code>StreamInfo</code> and
<code>ImageProcessingConfiguration</code> fields.

Type annotations and code completion for `#!python session.client("kinesisvideo").update_image_generation_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# update_image_generation_configuration method definition

await def update_image_generation_configuration(
    self,
    *,
    StreamName: str = ...,
    StreamARN: str = ...,
    ImageGenerationConfiguration: ImageGenerationConfigurationTypeDef = ...,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: ImageGenerationConfigurationTypeDef](./type_defs.md#imagegenerationconfigurationtypedef) 


```python
# update_image_generation_configuration method usage example with argument unpacking

kwargs: UpdateImageGenerationConfigurationInputRequestTypeDef = {  # (1)
    "StreamName": ...,
}

parent.update_image_generation_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateImageGenerationConfigurationInputRequestTypeDef](./type_defs.md#updateimagegenerationconfigurationinputrequesttypedef) 

### update\_media\_storage\_configuration

Associates a <code>SignalingChannel</code> to a stream to store the media.

Type annotations and code completion for `#!python session.client("kinesisvideo").update_media_storage_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# update_media_storage_configuration method definition

await def update_media_storage_configuration(
    self,
    *,
    ChannelARN: str,
    MediaStorageConfiguration: MediaStorageConfigurationTypeDef,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: MediaStorageConfigurationTypeDef](./type_defs.md#mediastorageconfigurationtypedef) 


```python
# update_media_storage_configuration method usage example with argument unpacking

kwargs: UpdateMediaStorageConfigurationInputRequestTypeDef = {  # (1)
    "ChannelARN": ...,
    "MediaStorageConfiguration": ...,
}

parent.update_media_storage_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateMediaStorageConfigurationInputRequestTypeDef](./type_defs.md#updatemediastorageconfigurationinputrequesttypedef) 

### update\_notification\_configuration

Updates the notification information for a stream.

Type annotations and code completion for `#!python session.client("kinesisvideo").update_notification_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# update_notification_configuration method definition

await def update_notification_configuration(
    self,
    *,
    StreamName: str = ...,
    StreamARN: str = ...,
    NotificationConfiguration: NotificationConfigurationTypeDef = ...,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 


```python
# update_notification_configuration method usage example with argument unpacking

kwargs: UpdateNotificationConfigurationInputRequestTypeDef = {  # (1)
    "StreamName": ...,
}

parent.update_notification_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateNotificationConfigurationInputRequestTypeDef](./type_defs.md#updatenotificationconfigurationinputrequesttypedef) 

### update\_signaling\_channel

Updates the existing signaling channel.

Type annotations and code completion for `#!python session.client("kinesisvideo").update_signaling_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# update_signaling_channel method definition

await def update_signaling_channel(
    self,
    *,
    ChannelARN: str,
    CurrentVersion: str,
    SingleMasterConfiguration: SingleMasterConfigurationTypeDef = ...,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: SingleMasterConfigurationTypeDef](./type_defs.md#singlemasterconfigurationtypedef) 


```python
# update_signaling_channel method usage example with argument unpacking

kwargs: UpdateSignalingChannelInputRequestTypeDef = {  # (1)
    "ChannelARN": ...,
    "CurrentVersion": ...,
}

parent.update_signaling_channel(**kwargs)
```

1. See [:material-code-braces: UpdateSignalingChannelInputRequestTypeDef](./type_defs.md#updatesignalingchannelinputrequesttypedef) 

### update\_stream

Updates stream metadata, such as the device name and media type.

Type annotations and code completion for `#!python session.client("kinesisvideo").update_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# update_stream method definition

await def update_stream(
    self,
    *,
    CurrentVersion: str,
    StreamName: str = ...,
    StreamARN: str = ...,
    DeviceName: str = ...,
    MediaType: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# update_stream method usage example with argument unpacking

kwargs: UpdateStreamInputRequestTypeDef = {  # (1)
    "CurrentVersion": ...,
}

parent.update_stream(**kwargs)
```

1. See [:material-code-braces: UpdateStreamInputRequestTypeDef](./type_defs.md#updatestreaminputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("kinesisvideo").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("kinesisvideo").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("kinesisvideo").get_paginator` method with overloads.

- `client.get_paginator("describe_mapped_resource_configuration")` -> [DescribeMappedResourceConfigurationPaginator](./paginators.md#describemappedresourceconfigurationpaginator)
- `client.get_paginator("list_edge_agent_configurations")` -> [ListEdgeAgentConfigurationsPaginator](./paginators.md#listedgeagentconfigurationspaginator)
- `client.get_paginator("list_signaling_channels")` -> [ListSignalingChannelsPaginator](./paginators.md#listsignalingchannelspaginator)
- `client.get_paginator("list_streams")` -> [ListStreamsPaginator](./paginators.md#liststreamspaginator)


