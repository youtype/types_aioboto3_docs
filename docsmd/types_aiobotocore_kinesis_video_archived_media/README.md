# KinesisVideoArchivedMedia module

> [Index](../README.md) > KinesisVideoArchivedMedia


!!! note ""

    Auto-generated documentation for [KinesisVideoArchivedMedia](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#kinesisvideoarchivedmedia)
    type annotations stubs module [types-aiobotocore-kinesis-video-archived-media](https://pypi.org/project/types-aiobotocore-kinesis-video-archived-media/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `KinesisVideoArchivedMedia` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `KinesisVideoArchivedMedia` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[kinesis-video-archived-media]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[kinesis-video-archived-media]'

# standalone installation
python -m pip install types-aiobotocore-kinesis-video-archived-media
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-kinesis-video-archived-media
```

## Usage

Code samples can be found in [Examples](./usage.md).

## KinesisVideoArchivedMediaClient

Type annotations and code completion for  `#!python session.client("kinesis-video-archived-media")` as [KinesisVideoArchivedMediaClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client)

```python
# KinesisVideoArchivedMediaClient usage example

from aioboto3.session import Session

from types_aiobotocore_kinesis_video_archived_media.client import KinesisVideoArchivedMediaClient


session = Session()
async with session.client("kinesis-video-archived-media") as client:
    client: KinesisVideoArchivedMediaClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("kinesis-video-archived-media").get_paginator("...")`.

```python
# GetImagesPaginator usage example

from types_aiobotocore_kinesis_video_archived_media.paginator import GetImagesPaginator

def get_get_images_paginator() -> GetImagesPaginator:
    return client.get_paginator("get_images"))
```

- [GetImagesPaginator](./paginators.md#getimagespaginator)
- [ListFragmentsPaginator](./paginators.md#listfragmentspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ClipFragmentSelectorTypeType usage example

from types_aiobotocore_kinesis_video_archived_media.literals import ClipFragmentSelectorTypeType

def get_value() -> ClipFragmentSelectorTypeType:
    return "PRODUCER_TIMESTAMP"
```

- [ClipFragmentSelectorTypeType](./literals.md#clipfragmentselectortypetype)
- [ContainerFormatType](./literals.md#containerformattype)
- [DASHDisplayFragmentNumberType](./literals.md#dashdisplayfragmentnumbertype)
- [DASHDisplayFragmentTimestampType](./literals.md#dashdisplayfragmenttimestamptype)
- [DASHFragmentSelectorTypeType](./literals.md#dashfragmentselectortypetype)
- [DASHPlaybackModeType](./literals.md#dashplaybackmodetype)
- [FormatConfigKeyType](./literals.md#formatconfigkeytype)
- [FormatType](./literals.md#formattype)
- [FragmentSelectorTypeType](./literals.md#fragmentselectortypetype)
- [GetImagesPaginatorName](./literals.md#getimagespaginatorname)
- [HLSDiscontinuityModeType](./literals.md#hlsdiscontinuitymodetype)
- [HLSDisplayFragmentTimestampType](./literals.md#hlsdisplayfragmenttimestamptype)
- [HLSFragmentSelectorTypeType](./literals.md#hlsfragmentselectortypetype)
- [HLSPlaybackModeType](./literals.md#hlsplaybackmodetype)
- [ImageErrorType](./literals.md#imageerrortype)
- [ImageSelectorTypeType](./literals.md#imageselectortypetype)
- [ListFragmentsPaginatorName](./literals.md#listfragmentspaginatorname)
- [KinesisVideoArchivedMediaServiceName](./literals.md#kinesisvideoarchivedmediaservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [FragmentTypeDef](./type_defs.md#fragmenttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ImageTypeDef](./type_defs.md#imagetypedef)
- [GetMediaForFragmentListInputRequestTypeDef](./type_defs.md#getmediaforfragmentlistinputrequesttypedef)
- [ClipTimestampRangeTypeDef](./type_defs.md#cliptimestamprangetypedef)
- [DASHTimestampRangeTypeDef](./type_defs.md#dashtimestamprangetypedef)
- [GetImagesInputRequestTypeDef](./type_defs.md#getimagesinputrequesttypedef)
- [HLSTimestampRangeTypeDef](./type_defs.md#hlstimestamprangetypedef)
- [TimestampRangeTypeDef](./type_defs.md#timestamprangetypedef)
- [GetClipOutputTypeDef](./type_defs.md#getclipoutputtypedef)
- [GetDASHStreamingSessionURLOutputTypeDef](./type_defs.md#getdashstreamingsessionurloutputtypedef)
- [GetHLSStreamingSessionURLOutputTypeDef](./type_defs.md#gethlsstreamingsessionurloutputtypedef)
- [GetMediaForFragmentListOutputTypeDef](./type_defs.md#getmediaforfragmentlistoutputtypedef)
- [ListFragmentsOutputTypeDef](./type_defs.md#listfragmentsoutputtypedef)
- [GetImagesInputPaginateTypeDef](./type_defs.md#getimagesinputpaginatetypedef)
- [GetImagesOutputTypeDef](./type_defs.md#getimagesoutputtypedef)
- [ClipFragmentSelectorTypeDef](./type_defs.md#clipfragmentselectortypedef)
- [DASHFragmentSelectorTypeDef](./type_defs.md#dashfragmentselectortypedef)
- [HLSFragmentSelectorTypeDef](./type_defs.md#hlsfragmentselectortypedef)
- [FragmentSelectorTypeDef](./type_defs.md#fragmentselectortypedef)
- [GetClipInputRequestTypeDef](./type_defs.md#getclipinputrequesttypedef)
- [GetDASHStreamingSessionURLInputRequestTypeDef](./type_defs.md#getdashstreamingsessionurlinputrequesttypedef)
- [GetHLSStreamingSessionURLInputRequestTypeDef](./type_defs.md#gethlsstreamingsessionurlinputrequesttypedef)
- [ListFragmentsInputPaginateTypeDef](./type_defs.md#listfragmentsinputpaginatetypedef)
- [ListFragmentsInputRequestTypeDef](./type_defs.md#listfragmentsinputrequesttypedef)
