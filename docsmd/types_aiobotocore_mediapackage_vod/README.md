# MediaPackageVod module

> [Index](../README.md) > MediaPackageVod


!!! note ""

    Auto-generated documentation for [MediaPackageVod](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
    type annotations stubs module [types-aiobotocore-mediapackage-vod](https://pypi.org/project/types-aiobotocore-mediapackage-vod/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `MediaPackageVod` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[mediapackage-vod]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[mediapackage-vod]'


# standalone installation
python -m pip install types-aiobotocore-mediapackage-vod
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-mediapackage-vod
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MediaPackageVodClient

Type annotations and code completion for  `#!python session.client("mediapackage-vod")` as [MediaPackageVodClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_mediapackage_vod.client import MediaPackageVodClient


session = Session()
async with session.client("mediapackage-vod") as client:
    client: MediaPackageVodClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("mediapackage-vod").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_mediapackage_vod.paginator import ListAssetsPaginator

def get_list_assets_paginator() -> ListAssetsPaginator:
    return client.get_paginator("list_assets"))
```

- [ListAssetsPaginator](./paginators.md#listassetspaginator)
- [ListPackagingConfigurationsPaginator](./paginators.md#listpackagingconfigurationspaginator)
- [ListPackagingGroupsPaginator](./paginators.md#listpackaginggroupspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_mediapackage_vod.literals import AdMarkersType

def get_value() -> AdMarkersType:
    return "NONE"
```

- [AdMarkersType](./literals.md#admarkerstype)
- [EncryptionMethodType](./literals.md#encryptionmethodtype)
- [ListAssetsPaginatorName](./literals.md#listassetspaginatorname)
- [ListPackagingConfigurationsPaginatorName](./literals.md#listpackagingconfigurationspaginatorname)
- [ListPackagingGroupsPaginatorName](./literals.md#listpackaginggroupspaginatorname)
- [ManifestLayoutType](./literals.md#manifestlayouttype)
- [PeriodTriggersElementType](./literals.md#periodtriggerselementtype)
- [ProfileType](./literals.md#profiletype)
- [SegmentTemplateFormatType](./literals.md#segmenttemplateformattype)
- [StreamOrderType](./literals.md#streamordertype)
- [MediaPackageVodServiceName](./literals.md#mediapackagevodservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_mediapackage_vod.type_defs import AssetShallowTypeDef

def get_value() -> AssetShallowTypeDef:
    return {
        "Arn": ...,
    }
```

- [AssetShallowTypeDef](./type_defs.md#assetshallowtypedef)
- [AuthorizationTypeDef](./type_defs.md#authorizationtypedef)
- [SpekeKeyProviderTypeDef](./type_defs.md#spekekeyprovidertypedef)
- [EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateAssetRequestRequestTypeDef](./type_defs.md#createassetrequestrequesttypedef)
- [EgressEndpointTypeDef](./type_defs.md#egressendpointtypedef)
- [StreamSelectionTypeDef](./type_defs.md#streamselectiontypedef)
- [DeleteAssetRequestRequestTypeDef](./type_defs.md#deleteassetrequestrequesttypedef)
- [DeletePackagingConfigurationRequestRequestTypeDef](./type_defs.md#deletepackagingconfigurationrequestrequesttypedef)
- [DeletePackagingGroupRequestRequestTypeDef](./type_defs.md#deletepackaginggrouprequestrequesttypedef)
- [DescribeAssetRequestRequestTypeDef](./type_defs.md#describeassetrequestrequesttypedef)
- [DescribePackagingConfigurationRequestRequestTypeDef](./type_defs.md#describepackagingconfigurationrequestrequesttypedef)
- [DescribePackagingGroupRequestRequestTypeDef](./type_defs.md#describepackaginggrouprequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAssetsRequestRequestTypeDef](./type_defs.md#listassetsrequestrequesttypedef)
- [ListPackagingConfigurationsRequestRequestTypeDef](./type_defs.md#listpackagingconfigurationsrequestrequesttypedef)
- [ListPackagingGroupsRequestRequestTypeDef](./type_defs.md#listpackaginggroupsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdatePackagingGroupRequestRequestTypeDef](./type_defs.md#updatepackaginggrouprequestrequesttypedef)
- [CmafEncryptionTypeDef](./type_defs.md#cmafencryptiontypedef)
- [DashEncryptionTypeDef](./type_defs.md#dashencryptiontypedef)
- [HlsEncryptionTypeDef](./type_defs.md#hlsencryptiontypedef)
- [MssEncryptionTypeDef](./type_defs.md#mssencryptiontypedef)
- [ConfigureLogsRequestRequestTypeDef](./type_defs.md#configurelogsrequestrequesttypedef)
- [CreatePackagingGroupRequestRequestTypeDef](./type_defs.md#createpackaginggrouprequestrequesttypedef)
- [PackagingGroupTypeDef](./type_defs.md#packaginggrouptypedef)
- [ConfigureLogsResponseTypeDef](./type_defs.md#configurelogsresponsetypedef)
- [CreatePackagingGroupResponseTypeDef](./type_defs.md#createpackaginggroupresponsetypedef)
- [DescribePackagingGroupResponseTypeDef](./type_defs.md#describepackaginggroupresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListAssetsResponseTypeDef](./type_defs.md#listassetsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdatePackagingGroupResponseTypeDef](./type_defs.md#updatepackaginggroupresponsetypedef)
- [CreateAssetResponseTypeDef](./type_defs.md#createassetresponsetypedef)
- [DescribeAssetResponseTypeDef](./type_defs.md#describeassetresponsetypedef)
- [DashManifestTypeDef](./type_defs.md#dashmanifesttypedef)
- [HlsManifestTypeDef](./type_defs.md#hlsmanifesttypedef)
- [MssManifestTypeDef](./type_defs.md#mssmanifesttypedef)
- [ListAssetsRequestListAssetsPaginateTypeDef](./type_defs.md#listassetsrequestlistassetspaginatetypedef)
- [ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef](./type_defs.md#listpackagingconfigurationsrequestlistpackagingconfigurationspaginatetypedef)
- [ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef](./type_defs.md#listpackaginggroupsrequestlistpackaginggroupspaginatetypedef)
- [ListPackagingGroupsResponseTypeDef](./type_defs.md#listpackaginggroupsresponsetypedef)
- [DashPackageTypeDef](./type_defs.md#dashpackagetypedef)
- [CmafPackageTypeDef](./type_defs.md#cmafpackagetypedef)
- [HlsPackageTypeDef](./type_defs.md#hlspackagetypedef)
- [MssPackageTypeDef](./type_defs.md#msspackagetypedef)
- [CreatePackagingConfigurationRequestRequestTypeDef](./type_defs.md#createpackagingconfigurationrequestrequesttypedef)
- [CreatePackagingConfigurationResponseTypeDef](./type_defs.md#createpackagingconfigurationresponsetypedef)
- [DescribePackagingConfigurationResponseTypeDef](./type_defs.md#describepackagingconfigurationresponsetypedef)
- [PackagingConfigurationTypeDef](./type_defs.md#packagingconfigurationtypedef)
- [ListPackagingConfigurationsResponseTypeDef](./type_defs.md#listpackagingconfigurationsresponsetypedef)

