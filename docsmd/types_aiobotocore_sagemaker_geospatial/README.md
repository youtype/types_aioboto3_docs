# SageMakergeospatialcapabilities module

> [Index](../README.md) > SageMakergeospatialcapabilities


!!! note ""

    Auto-generated documentation for [SageMakergeospatialcapabilities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#sagemakergeospatialcapabilities)
    type annotations stubs module [types-aiobotocore-sagemaker-geospatial](https://pypi.org/project/types-aiobotocore-sagemaker-geospatial/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `SageMakergeospatialcapabilities` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `SageMakergeospatialcapabilities` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[sagemaker-geospatial]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[sagemaker-geospatial]'

# standalone installation
python -m pip install types-aiobotocore-sagemaker-geospatial
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-sagemaker-geospatial
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SageMakergeospatialcapabilitiesClient

Type annotations and code completion for  `#!python session.client("sagemaker-geospatial")` as [SageMakergeospatialcapabilitiesClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client)

```python
# SageMakergeospatialcapabilitiesClient usage example

from aioboto3.session import Session

from types_aiobotocore_sagemaker_geospatial.client import SageMakergeospatialcapabilitiesClient


session = Session()
async with session.client("sagemaker-geospatial") as client:
    client: SageMakergeospatialcapabilitiesClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("sagemaker-geospatial").get_paginator("...")`.

```python
# ListEarthObservationJobsPaginator usage example

from types_aiobotocore_sagemaker_geospatial.paginator import ListEarthObservationJobsPaginator

def get_list_earth_observation_jobs_paginator() -> ListEarthObservationJobsPaginator:
    return client.get_paginator("list_earth_observation_jobs"))
```

- [ListEarthObservationJobsPaginator](./paginators.md#listearthobservationjobspaginator)
- [ListRasterDataCollectionsPaginator](./paginators.md#listrasterdatacollectionspaginator)
- [ListVectorEnrichmentJobsPaginator](./paginators.md#listvectorenrichmentjobspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AlgorithmNameCloudRemovalType usage example

from types_aiobotocore_sagemaker_geospatial.literals import AlgorithmNameCloudRemovalType

def get_value() -> AlgorithmNameCloudRemovalType:
    return "INTERPOLATION"
```

- [AlgorithmNameCloudRemovalType](./literals.md#algorithmnamecloudremovaltype)
- [AlgorithmNameGeoMosaicType](./literals.md#algorithmnamegeomosaictype)
- [AlgorithmNameResamplingType](./literals.md#algorithmnameresamplingtype)
- [ComparisonOperatorType](./literals.md#comparisonoperatortype)
- [DataCollectionTypeType](./literals.md#datacollectiontypetype)
- [EarthObservationJobErrorTypeType](./literals.md#earthobservationjoberrortypetype)
- [EarthObservationJobExportStatusType](./literals.md#earthobservationjobexportstatustype)
- [EarthObservationJobStatusType](./literals.md#earthobservationjobstatustype)
- [ExportErrorTypeType](./literals.md#exporterrortypetype)
- [GroupByType](./literals.md#groupbytype)
- [ListEarthObservationJobsPaginatorName](./literals.md#listearthobservationjobspaginatorname)
- [ListRasterDataCollectionsPaginatorName](./literals.md#listrasterdatacollectionspaginatorname)
- [ListVectorEnrichmentJobsPaginatorName](./literals.md#listvectorenrichmentjobspaginatorname)
- [LogicalOperatorType](./literals.md#logicaloperatortype)
- [OutputTypeType](./literals.md#outputtypetype)
- [PredefinedResolutionType](./literals.md#predefinedresolutiontype)
- [SortOrderType](./literals.md#sortordertype)
- [TargetOptionsType](./literals.md#targetoptionstype)
- [TemporalStatisticsType](./literals.md#temporalstatisticstype)
- [UnitType](./literals.md#unittype)
- [VectorEnrichmentJobDocumentTypeType](./literals.md#vectorenrichmentjobdocumenttypetype)
- [VectorEnrichmentJobErrorTypeType](./literals.md#vectorenrichmentjoberrortypetype)
- [VectorEnrichmentJobExportErrorTypeType](./literals.md#vectorenrichmentjobexporterrortypetype)
- [VectorEnrichmentJobExportStatusType](./literals.md#vectorenrichmentjobexportstatustype)
- [VectorEnrichmentJobStatusType](./literals.md#vectorenrichmentjobstatustype)
- [VectorEnrichmentJobTypeType](./literals.md#vectorenrichmentjobtypetype)
- [ZonalStatisticsType](./literals.md#zonalstatisticstype)
- [SageMakergeospatialcapabilitiesServiceName](./literals.md#sagemakergeospatialcapabilitiesservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [MultiPolygonGeometryInputOutputTypeDef](./type_defs.md#multipolygongeometryinputoutputtypedef)
- [PolygonGeometryInputOutputTypeDef](./type_defs.md#polygongeometryinputoutputtypedef)
- [AssetValueTypeDef](./type_defs.md#assetvaluetypedef)
- [CloudRemovalConfigInputOutputTypeDef](./type_defs.md#cloudremovalconfiginputoutputtypedef)
- [CloudRemovalConfigInputTypeDef](./type_defs.md#cloudremovalconfiginputtypedef)
- [OperationTypeDef](./type_defs.md#operationtypedef)
- [DeleteEarthObservationJobInputRequestTypeDef](./type_defs.md#deleteearthobservationjobinputrequesttypedef)
- [DeleteVectorEnrichmentJobInputRequestTypeDef](./type_defs.md#deletevectorenrichmentjobinputrequesttypedef)
- [EarthObservationJobErrorDetailsTypeDef](./type_defs.md#earthobservationjoberrordetailstypedef)
- [EoCloudCoverInputTypeDef](./type_defs.md#eocloudcoverinputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ExportErrorDetailsOutputTypeDef](./type_defs.md#exporterrordetailsoutputtypedef)
- [ExportS3DataInputTypeDef](./type_defs.md#exports3datainputtypedef)
- [VectorEnrichmentJobS3DataTypeDef](./type_defs.md#vectorenrichmentjobs3datatypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [GeoMosaicConfigInputOutputTypeDef](./type_defs.md#geomosaicconfiginputoutputtypedef)
- [GeoMosaicConfigInputTypeDef](./type_defs.md#geomosaicconfiginputtypedef)
- [GeometryTypeDef](./type_defs.md#geometrytypedef)
- [GetEarthObservationJobInputRequestTypeDef](./type_defs.md#getearthobservationjobinputrequesttypedef)
- [OutputBandTypeDef](./type_defs.md#outputbandtypedef)
- [GetRasterDataCollectionInputRequestTypeDef](./type_defs.md#getrasterdatacollectioninputrequesttypedef)
- [GetTileInputRequestTypeDef](./type_defs.md#gettileinputrequesttypedef)
- [GetVectorEnrichmentJobInputRequestTypeDef](./type_defs.md#getvectorenrichmentjobinputrequesttypedef)
- [VectorEnrichmentJobErrorDetailsTypeDef](./type_defs.md#vectorenrichmentjoberrordetailstypedef)
- [VectorEnrichmentJobExportErrorDetailsTypeDef](./type_defs.md#vectorenrichmentjobexporterrordetailstypedef)
- [PropertiesTypeDef](./type_defs.md#propertiestypedef)
- [TemporalStatisticsConfigInputOutputTypeDef](./type_defs.md#temporalstatisticsconfiginputoutputtypedef)
- [ZonalStatisticsConfigInputOutputTypeDef](./type_defs.md#zonalstatisticsconfiginputoutputtypedef)
- [LandsatCloudCoverLandInputTypeDef](./type_defs.md#landsatcloudcoverlandinputtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListEarthObservationJobInputRequestTypeDef](./type_defs.md#listearthobservationjobinputrequesttypedef)
- [ListEarthObservationJobOutputConfigTypeDef](./type_defs.md#listearthobservationjoboutputconfigtypedef)
- [ListRasterDataCollectionsInputRequestTypeDef](./type_defs.md#listrasterdatacollectionsinputrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListVectorEnrichmentJobInputRequestTypeDef](./type_defs.md#listvectorenrichmentjobinputrequesttypedef)
- [ListVectorEnrichmentJobOutputConfigTypeDef](./type_defs.md#listvectorenrichmentjoboutputconfigtypedef)
- [MapMatchingConfigTypeDef](./type_defs.md#mapmatchingconfigtypedef)
- [MultiPolygonGeometryInputTypeDef](./type_defs.md#multipolygongeometryinputtypedef)
- [UserDefinedTypeDef](./type_defs.md#userdefinedtypedef)
- [PlatformInputTypeDef](./type_defs.md#platforminputtypedef)
- [PolygonGeometryInputTypeDef](./type_defs.md#polygongeometryinputtypedef)
- [ViewOffNadirInputTypeDef](./type_defs.md#viewoffnadirinputtypedef)
- [ViewSunAzimuthInputTypeDef](./type_defs.md#viewsunazimuthinputtypedef)
- [ViewSunElevationInputTypeDef](./type_defs.md#viewsunelevationinputtypedef)
- [TimeRangeFilterOutputTypeDef](./type_defs.md#timerangefilteroutputtypedef)
- [ReverseGeocodingConfigTypeDef](./type_defs.md#reversegeocodingconfigtypedef)
- [StopEarthObservationJobInputRequestTypeDef](./type_defs.md#stopearthobservationjobinputrequesttypedef)
- [StopVectorEnrichmentJobInputRequestTypeDef](./type_defs.md#stopvectorenrichmentjobinputrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [TemporalStatisticsConfigInputTypeDef](./type_defs.md#temporalstatisticsconfiginputtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [ZonalStatisticsConfigInputTypeDef](./type_defs.md#zonalstatisticsconfiginputtypedef)
- [AreaOfInterestGeometryOutputTypeDef](./type_defs.md#areaofinterestgeometryoutputtypedef)
- [CloudRemovalConfigInputUnionTypeDef](./type_defs.md#cloudremovalconfiginputuniontypedef)
- [CustomIndicesInputOutputTypeDef](./type_defs.md#customindicesinputoutputtypedef)
- [CustomIndicesInputTypeDef](./type_defs.md#customindicesinputtypedef)
- [GetTileOutputTypeDef](./type_defs.md#gettileoutputtypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ExportErrorDetailsTypeDef](./type_defs.md#exporterrordetailstypedef)
- [OutputConfigInputTypeDef](./type_defs.md#outputconfiginputtypedef)
- [ExportVectorEnrichmentJobOutputConfigTypeDef](./type_defs.md#exportvectorenrichmentjoboutputconfigtypedef)
- [VectorEnrichmentJobDataSourceConfigInputTypeDef](./type_defs.md#vectorenrichmentjobdatasourceconfiginputtypedef)
- [GetRasterDataCollectionOutputTypeDef](./type_defs.md#getrasterdatacollectionoutputtypedef)
- [RasterDataCollectionMetadataTypeDef](./type_defs.md#rasterdatacollectionmetadatatypedef)
- [GeoMosaicConfigInputUnionTypeDef](./type_defs.md#geomosaicconfiginputuniontypedef)
- [ItemSourceTypeDef](./type_defs.md#itemsourcetypedef)
- [ListEarthObservationJobInputPaginateTypeDef](./type_defs.md#listearthobservationjobinputpaginatetypedef)
- [ListRasterDataCollectionsInputPaginateTypeDef](./type_defs.md#listrasterdatacollectionsinputpaginatetypedef)
- [ListVectorEnrichmentJobInputPaginateTypeDef](./type_defs.md#listvectorenrichmentjobinputpaginatetypedef)
- [ListEarthObservationJobOutputTypeDef](./type_defs.md#listearthobservationjoboutputtypedef)
- [ListVectorEnrichmentJobOutputTypeDef](./type_defs.md#listvectorenrichmentjoboutputtypedef)
- [MultiPolygonGeometryInputUnionTypeDef](./type_defs.md#multipolygongeometryinputuniontypedef)
- [OutputResolutionResamplingInputTypeDef](./type_defs.md#outputresolutionresamplinginputtypedef)
- [OutputResolutionStackInputTypeDef](./type_defs.md#outputresolutionstackinputtypedef)
- [PolygonGeometryInputUnionTypeDef](./type_defs.md#polygongeometryinputuniontypedef)
- [PropertyTypeDef](./type_defs.md#propertytypedef)
- [VectorEnrichmentJobConfigTypeDef](./type_defs.md#vectorenrichmentjobconfigtypedef)
- [TemporalStatisticsConfigInputUnionTypeDef](./type_defs.md#temporalstatisticsconfiginputuniontypedef)
- [TimeRangeFilterInputTypeDef](./type_defs.md#timerangefilterinputtypedef)
- [ZonalStatisticsConfigInputUnionTypeDef](./type_defs.md#zonalstatisticsconfiginputuniontypedef)
- [AreaOfInterestOutputTypeDef](./type_defs.md#areaofinterestoutputtypedef)
- [BandMathConfigInputOutputTypeDef](./type_defs.md#bandmathconfiginputoutputtypedef)
- [CustomIndicesInputUnionTypeDef](./type_defs.md#customindicesinputuniontypedef)
- [ExportEarthObservationJobInputRequestTypeDef](./type_defs.md#exportearthobservationjobinputrequesttypedef)
- [ExportEarthObservationJobOutputTypeDef](./type_defs.md#exportearthobservationjoboutputtypedef)
- [ExportVectorEnrichmentJobInputRequestTypeDef](./type_defs.md#exportvectorenrichmentjobinputrequesttypedef)
- [ExportVectorEnrichmentJobOutputTypeDef](./type_defs.md#exportvectorenrichmentjoboutputtypedef)
- [VectorEnrichmentJobInputConfigTypeDef](./type_defs.md#vectorenrichmentjobinputconfigtypedef)
- [ListRasterDataCollectionsOutputTypeDef](./type_defs.md#listrasterdatacollectionsoutputtypedef)
- [SearchRasterDataCollectionOutputTypeDef](./type_defs.md#searchrasterdatacollectionoutputtypedef)
- [ResamplingConfigInputOutputTypeDef](./type_defs.md#resamplingconfiginputoutputtypedef)
- [ResamplingConfigInputTypeDef](./type_defs.md#resamplingconfiginputtypedef)
- [StackConfigInputOutputTypeDef](./type_defs.md#stackconfiginputoutputtypedef)
- [StackConfigInputTypeDef](./type_defs.md#stackconfiginputtypedef)
- [AreaOfInterestGeometryTypeDef](./type_defs.md#areaofinterestgeometrytypedef)
- [PropertyFilterTypeDef](./type_defs.md#propertyfiltertypedef)
- [BandMathConfigInputTypeDef](./type_defs.md#bandmathconfiginputtypedef)
- [GetVectorEnrichmentJobOutputTypeDef](./type_defs.md#getvectorenrichmentjoboutputtypedef)
- [StartVectorEnrichmentJobInputRequestTypeDef](./type_defs.md#startvectorenrichmentjobinputrequesttypedef)
- [StartVectorEnrichmentJobOutputTypeDef](./type_defs.md#startvectorenrichmentjoboutputtypedef)
- [ResamplingConfigInputUnionTypeDef](./type_defs.md#resamplingconfiginputuniontypedef)
- [JobConfigInputOutputTypeDef](./type_defs.md#jobconfiginputoutputtypedef)
- [StackConfigInputUnionTypeDef](./type_defs.md#stackconfiginputuniontypedef)
- [AreaOfInterestGeometryUnionTypeDef](./type_defs.md#areaofinterestgeometryuniontypedef)
- [PropertyFiltersOutputTypeDef](./type_defs.md#propertyfiltersoutputtypedef)
- [PropertyFiltersTypeDef](./type_defs.md#propertyfilterstypedef)
- [BandMathConfigInputUnionTypeDef](./type_defs.md#bandmathconfiginputuniontypedef)
- [AreaOfInterestTypeDef](./type_defs.md#areaofinteresttypedef)
- [RasterDataCollectionQueryOutputTypeDef](./type_defs.md#rasterdatacollectionqueryoutputtypedef)
- [PropertyFiltersUnionTypeDef](./type_defs.md#propertyfiltersuniontypedef)
- [JobConfigInputTypeDef](./type_defs.md#jobconfiginputtypedef)
- [AreaOfInterestUnionTypeDef](./type_defs.md#areaofinterestuniontypedef)
- [InputConfigOutputTypeDef](./type_defs.md#inputconfigoutputtypedef)
- [RasterDataCollectionQueryInputTypeDef](./type_defs.md#rasterdatacollectionqueryinputtypedef)
- [RasterDataCollectionQueryWithBandFilterInputTypeDef](./type_defs.md#rasterdatacollectionquerywithbandfilterinputtypedef)
- [GetEarthObservationJobOutputTypeDef](./type_defs.md#getearthobservationjoboutputtypedef)
- [StartEarthObservationJobOutputTypeDef](./type_defs.md#startearthobservationjoboutputtypedef)
- [InputConfigInputTypeDef](./type_defs.md#inputconfiginputtypedef)
- [SearchRasterDataCollectionInputRequestTypeDef](./type_defs.md#searchrasterdatacollectioninputrequesttypedef)
- [StartEarthObservationJobInputRequestTypeDef](./type_defs.md#startearthobservationjobinputrequesttypedef)
