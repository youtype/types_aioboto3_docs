# MediaPackageClient

> [Index](../README.md) > [MediaPackage](./README.md) > MediaPackageClient

!!! note ""

    Auto-generated documentation for [MediaPackage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#mediapackage)
    type annotations stubs module [types-aiobotocore-mediapackage](https://pypi.org/project/types-aiobotocore-mediapackage/).

## MediaPackageClient

Type annotations and code completion for `#!python session.client("mediapackage")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# MediaPackageClient usage example

from aioboto3.session import Session
from types_aiobotocore_mediapackage.client import MediaPackageClient

session = Session()
async with session.client("mediapackage") as client:
    client: MediaPackageClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("mediapackage").exceptions` structure.

```python
# MediaPackageClient.exceptions usage example

async with session.client("mediapackage") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.ForbiddenException,
        client.exceptions.InternalServerErrorException,
        client.exceptions.NotFoundException,
        client.exceptions.ServiceUnavailableException,
        client.exceptions.TooManyRequestsException,
        client.exceptions.UnprocessableEntityException,
    ) as e:
        print(e)
```

```python
# MediaPackageClient.exceptions type checking example

from types_aiobotocore_mediapackage.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("mediapackage").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("mediapackage").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

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


### configure\_logs

Changes the Channel's properities to configure log subscription.

Type annotations and code completion for `#!python session.client("mediapackage").configure_logs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# configure_logs method definition

await def configure_logs(
    self,
    *,
    Id: str,
    EgressAccessLogs: EgressAccessLogsTypeDef = ...,  # (1)
    IngressAccessLogs: IngressAccessLogsTypeDef = ...,  # (2)
) -> ConfigureLogsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef) 
2. See [:material-code-braces: IngressAccessLogsTypeDef](./type_defs.md#ingressaccesslogstypedef) 
3. See [:material-code-braces: ConfigureLogsResponseTypeDef](./type_defs.md#configurelogsresponsetypedef) 


```python
# configure_logs method usage example with argument unpacking

kwargs: ConfigureLogsRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.configure_logs(**kwargs)
```

1. See [:material-code-braces: ConfigureLogsRequestRequestTypeDef](./type_defs.md#configurelogsrequestrequesttypedef) 

### create\_channel

Creates a new Channel.

Type annotations and code completion for `#!python session.client("mediapackage").create_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# create_channel method definition

await def create_channel(
    self,
    *,
    Id: str,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateChannelResponseTypeDef](./type_defs.md#createchannelresponsetypedef) 


```python
# create_channel method usage example with argument unpacking

kwargs: CreateChannelRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.create_channel(**kwargs)
```

1. See [:material-code-braces: CreateChannelRequestRequestTypeDef](./type_defs.md#createchannelrequestrequesttypedef) 

### create\_harvest\_job

Creates a new HarvestJob record.

Type annotations and code completion for `#!python session.client("mediapackage").create_harvest_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# create_harvest_job method definition

await def create_harvest_job(
    self,
    *,
    EndTime: str,
    Id: str,
    OriginEndpointId: str,
    S3Destination: S3DestinationTypeDef,  # (1)
    StartTime: str,
) -> CreateHarvestJobResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
2. See [:material-code-braces: CreateHarvestJobResponseTypeDef](./type_defs.md#createharvestjobresponsetypedef) 


```python
# create_harvest_job method usage example with argument unpacking

kwargs: CreateHarvestJobRequestRequestTypeDef = {  # (1)
    "EndTime": ...,
    "Id": ...,
    "OriginEndpointId": ...,
    "S3Destination": ...,
    "StartTime": ...,
}

parent.create_harvest_job(**kwargs)
```

1. See [:material-code-braces: CreateHarvestJobRequestRequestTypeDef](./type_defs.md#createharvestjobrequestrequesttypedef) 

### create\_origin\_endpoint

Creates a new OriginEndpoint record.

Type annotations and code completion for `#!python session.client("mediapackage").create_origin_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# create_origin_endpoint method definition

await def create_origin_endpoint(
    self,
    *,
    ChannelId: str,
    Id: str,
    Authorization: AuthorizationTypeDef = ...,  # (1)
    CmafPackage: CmafPackageCreateOrUpdateParametersTypeDef = ...,  # (2)
    DashPackage: DashPackageTypeDef = ...,  # (3)
    Description: str = ...,
    HlsPackage: HlsPackageTypeDef = ...,  # (4)
    ManifestName: str = ...,
    MssPackage: MssPackageTypeDef = ...,  # (5)
    Origination: OriginationType = ...,  # (6)
    StartoverWindowSeconds: int = ...,
    Tags: Mapping[str, str] = ...,
    TimeDelaySeconds: int = ...,
    Whitelist: Sequence[str] = ...,
) -> CreateOriginEndpointResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: AuthorizationTypeDef](./type_defs.md#authorizationtypedef) 
2. See [:material-code-braces: CmafPackageCreateOrUpdateParametersTypeDef](./type_defs.md#cmafpackagecreateorupdateparameterstypedef) 
3. See [:material-code-braces: DashPackageTypeDef](./type_defs.md#dashpackagetypedef) 
4. See [:material-code-braces: HlsPackageTypeDef](./type_defs.md#hlspackagetypedef) 
5. See [:material-code-braces: MssPackageTypeDef](./type_defs.md#msspackagetypedef) 
6. See [:material-code-brackets: OriginationType](./literals.md#originationtype) 
7. See [:material-code-braces: CreateOriginEndpointResponseTypeDef](./type_defs.md#createoriginendpointresponsetypedef) 


```python
# create_origin_endpoint method usage example with argument unpacking

kwargs: CreateOriginEndpointRequestRequestTypeDef = {  # (1)
    "ChannelId": ...,
    "Id": ...,
}

parent.create_origin_endpoint(**kwargs)
```

1. See [:material-code-braces: CreateOriginEndpointRequestRequestTypeDef](./type_defs.md#createoriginendpointrequestrequesttypedef) 

### delete\_channel

Deletes an existing Channel.

Type annotations and code completion for `#!python session.client("mediapackage").delete_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# delete_channel method definition

await def delete_channel(
    self,
    *,
    Id: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_channel method usage example with argument unpacking

kwargs: DeleteChannelRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_channel(**kwargs)
```

1. See [:material-code-braces: DeleteChannelRequestRequestTypeDef](./type_defs.md#deletechannelrequestrequesttypedef) 

### delete\_origin\_endpoint

Deletes an existing OriginEndpoint.

Type annotations and code completion for `#!python session.client("mediapackage").delete_origin_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# delete_origin_endpoint method definition

await def delete_origin_endpoint(
    self,
    *,
    Id: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_origin_endpoint method usage example with argument unpacking

kwargs: DeleteOriginEndpointRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_origin_endpoint(**kwargs)
```

1. See [:material-code-braces: DeleteOriginEndpointRequestRequestTypeDef](./type_defs.md#deleteoriginendpointrequestrequesttypedef) 

### describe\_channel

Gets details about a Channel.

Type annotations and code completion for `#!python session.client("mediapackage").describe_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# describe_channel method definition

await def describe_channel(
    self,
    *,
    Id: str,
) -> DescribeChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeChannelResponseTypeDef](./type_defs.md#describechannelresponsetypedef) 


```python
# describe_channel method usage example with argument unpacking

kwargs: DescribeChannelRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.describe_channel(**kwargs)
```

1. See [:material-code-braces: DescribeChannelRequestRequestTypeDef](./type_defs.md#describechannelrequestrequesttypedef) 

### describe\_harvest\_job

Gets details about an existing HarvestJob.

Type annotations and code completion for `#!python session.client("mediapackage").describe_harvest_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# describe_harvest_job method definition

await def describe_harvest_job(
    self,
    *,
    Id: str,
) -> DescribeHarvestJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeHarvestJobResponseTypeDef](./type_defs.md#describeharvestjobresponsetypedef) 


```python
# describe_harvest_job method usage example with argument unpacking

kwargs: DescribeHarvestJobRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.describe_harvest_job(**kwargs)
```

1. See [:material-code-braces: DescribeHarvestJobRequestRequestTypeDef](./type_defs.md#describeharvestjobrequestrequesttypedef) 

### describe\_origin\_endpoint

Gets details about an existing OriginEndpoint.

Type annotations and code completion for `#!python session.client("mediapackage").describe_origin_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# describe_origin_endpoint method definition

await def describe_origin_endpoint(
    self,
    *,
    Id: str,
) -> DescribeOriginEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeOriginEndpointResponseTypeDef](./type_defs.md#describeoriginendpointresponsetypedef) 


```python
# describe_origin_endpoint method usage example with argument unpacking

kwargs: DescribeOriginEndpointRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.describe_origin_endpoint(**kwargs)
```

1. See [:material-code-braces: DescribeOriginEndpointRequestRequestTypeDef](./type_defs.md#describeoriginendpointrequestrequesttypedef) 

### list\_channels

Returns a collection of Channels.

Type annotations and code completion for `#!python session.client("mediapackage").list_channels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# list_channels method definition

await def list_channels(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListChannelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


```python
# list_channels method usage example with argument unpacking

kwargs: ListChannelsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_channels(**kwargs)
```

1. See [:material-code-braces: ListChannelsRequestRequestTypeDef](./type_defs.md#listchannelsrequestrequesttypedef) 

### list\_harvest\_jobs

Returns a collection of HarvestJob records.

Type annotations and code completion for `#!python session.client("mediapackage").list_harvest_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# list_harvest_jobs method definition

await def list_harvest_jobs(
    self,
    *,
    IncludeChannelId: str = ...,
    IncludeStatus: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListHarvestJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListHarvestJobsResponseTypeDef](./type_defs.md#listharvestjobsresponsetypedef) 


```python
# list_harvest_jobs method usage example with argument unpacking

kwargs: ListHarvestJobsRequestRequestTypeDef = {  # (1)
    "IncludeChannelId": ...,
}

parent.list_harvest_jobs(**kwargs)
```

1. See [:material-code-braces: ListHarvestJobsRequestRequestTypeDef](./type_defs.md#listharvestjobsrequestrequesttypedef) 

### list\_origin\_endpoints

Returns a collection of OriginEndpoint records.

Type annotations and code completion for `#!python session.client("mediapackage").list_origin_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# list_origin_endpoints method definition

await def list_origin_endpoints(
    self,
    *,
    ChannelId: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListOriginEndpointsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOriginEndpointsResponseTypeDef](./type_defs.md#listoriginendpointsresponsetypedef) 


```python
# list_origin_endpoints method usage example with argument unpacking

kwargs: ListOriginEndpointsRequestRequestTypeDef = {  # (1)
    "ChannelId": ...,
}

parent.list_origin_endpoints(**kwargs)
```

1. See [:material-code-braces: ListOriginEndpointsRequestRequestTypeDef](./type_defs.md#listoriginendpointsrequestrequesttypedef) 

### list\_tags\_for\_resource



Type annotations and code completion for `#!python session.client("mediapackage").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### rotate\_channel\_credentials

Changes the Channel's first IngestEndpoint's username and password.

Type annotations and code completion for `#!python session.client("mediapackage").rotate_channel_credentials` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# rotate_channel_credentials method definition

await def rotate_channel_credentials(
    self,
    *,
    Id: str,
) -> RotateChannelCredentialsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RotateChannelCredentialsResponseTypeDef](./type_defs.md#rotatechannelcredentialsresponsetypedef) 


```python
# rotate_channel_credentials method usage example with argument unpacking

kwargs: RotateChannelCredentialsRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.rotate_channel_credentials(**kwargs)
```

1. See [:material-code-braces: RotateChannelCredentialsRequestRequestTypeDef](./type_defs.md#rotatechannelcredentialsrequestrequesttypedef) 

### rotate\_ingest\_endpoint\_credentials

Rotate the IngestEndpoint's username and password, as specified by the
IngestEndpoint's id.

Type annotations and code completion for `#!python session.client("mediapackage").rotate_ingest_endpoint_credentials` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# rotate_ingest_endpoint_credentials method definition

await def rotate_ingest_endpoint_credentials(
    self,
    *,
    Id: str,
    IngestEndpointId: str,
) -> RotateIngestEndpointCredentialsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RotateIngestEndpointCredentialsResponseTypeDef](./type_defs.md#rotateingestendpointcredentialsresponsetypedef) 


```python
# rotate_ingest_endpoint_credentials method usage example with argument unpacking

kwargs: RotateIngestEndpointCredentialsRequestRequestTypeDef = {  # (1)
    "Id": ...,
    "IngestEndpointId": ...,
}

parent.rotate_ingest_endpoint_credentials(**kwargs)
```

1. See [:material-code-braces: RotateIngestEndpointCredentialsRequestRequestTypeDef](./type_defs.md#rotateingestendpointcredentialsrequestrequesttypedef) 

### tag\_resource



Type annotations and code completion for `#!python session.client("mediapackage").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource



Type annotations and code completion for `#!python session.client("mediapackage").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_channel

Updates an existing Channel.

Type annotations and code completion for `#!python session.client("mediapackage").update_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# update_channel method definition

await def update_channel(
    self,
    *,
    Id: str,
    Description: str = ...,
) -> UpdateChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateChannelResponseTypeDef](./type_defs.md#updatechannelresponsetypedef) 


```python
# update_channel method usage example with argument unpacking

kwargs: UpdateChannelRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.update_channel(**kwargs)
```

1. See [:material-code-braces: UpdateChannelRequestRequestTypeDef](./type_defs.md#updatechannelrequestrequesttypedef) 

### update\_origin\_endpoint

Updates an existing OriginEndpoint.

Type annotations and code completion for `#!python session.client("mediapackage").update_origin_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# update_origin_endpoint method definition

await def update_origin_endpoint(
    self,
    *,
    Id: str,
    Authorization: AuthorizationTypeDef = ...,  # (1)
    CmafPackage: CmafPackageCreateOrUpdateParametersTypeDef = ...,  # (2)
    DashPackage: DashPackageTypeDef = ...,  # (3)
    Description: str = ...,
    HlsPackage: HlsPackageTypeDef = ...,  # (4)
    ManifestName: str = ...,
    MssPackage: MssPackageTypeDef = ...,  # (5)
    Origination: OriginationType = ...,  # (6)
    StartoverWindowSeconds: int = ...,
    TimeDelaySeconds: int = ...,
    Whitelist: Sequence[str] = ...,
) -> UpdateOriginEndpointResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: AuthorizationTypeDef](./type_defs.md#authorizationtypedef) 
2. See [:material-code-braces: CmafPackageCreateOrUpdateParametersTypeDef](./type_defs.md#cmafpackagecreateorupdateparameterstypedef) 
3. See [:material-code-braces: DashPackageTypeDef](./type_defs.md#dashpackagetypedef) 
4. See [:material-code-braces: HlsPackageTypeDef](./type_defs.md#hlspackagetypedef) 
5. See [:material-code-braces: MssPackageTypeDef](./type_defs.md#msspackagetypedef) 
6. See [:material-code-brackets: OriginationType](./literals.md#originationtype) 
7. See [:material-code-braces: UpdateOriginEndpointResponseTypeDef](./type_defs.md#updateoriginendpointresponsetypedef) 


```python
# update_origin_endpoint method usage example with argument unpacking

kwargs: UpdateOriginEndpointRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.update_origin_endpoint(**kwargs)
```

1. See [:material-code-braces: UpdateOriginEndpointRequestRequestTypeDef](./type_defs.md#updateoriginendpointrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("mediapackage").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("mediapackage").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

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

Type annotations and code completion for `#!python session.client("mediapackage").get_paginator` method with overloads.

- `client.get_paginator("list_channels")` -> [ListChannelsPaginator](./paginators.md#listchannelspaginator)
- `client.get_paginator("list_harvest_jobs")` -> [ListHarvestJobsPaginator](./paginators.md#listharvestjobspaginator)
- `client.get_paginator("list_origin_endpoints")` -> [ListOriginEndpointsPaginator](./paginators.md#listoriginendpointspaginator)


