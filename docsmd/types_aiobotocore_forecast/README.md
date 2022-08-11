# ForecastService module

> [Index](../README.md) > ForecastService


!!! note ""

    Auto-generated documentation for [ForecastService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
    type annotations stubs module [types-aiobotocore-forecast](https://pypi.org/project/types-aiobotocore-forecast/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `ForecastService` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[forecast]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[forecast]'


# standalone installation
python -m pip install types-aiobotocore-forecast
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-forecast
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ForecastServiceClient

Type annotations and code completion for  `#!python session.client("forecast")` as [ForecastServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_forecast.client import ForecastServiceClient


session = Session()
async with session.client("forecast") as client:
    client: ForecastServiceClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("forecast").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_forecast.paginator import ListDatasetGroupsPaginator

def get_list_dataset_groups_paginator() -> ListDatasetGroupsPaginator:
    return client.get_paginator("list_dataset_groups"))
```

- [ListDatasetGroupsPaginator](./paginators.md#listdatasetgroupspaginator)
- [ListDatasetImportJobsPaginator](./paginators.md#listdatasetimportjobspaginator)
- [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
- [ListForecastExportJobsPaginator](./paginators.md#listforecastexportjobspaginator)
- [ListForecastsPaginator](./paginators.md#listforecastspaginator)
- [ListPredictorBacktestExportJobsPaginator](./paginators.md#listpredictorbacktestexportjobspaginator)
- [ListPredictorsPaginator](./paginators.md#listpredictorspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_forecast.literals import AttributeTypeType

def get_value() -> AttributeTypeType:
    return "float"
```

- [AttributeTypeType](./literals.md#attributetypetype)
- [AutoMLOverrideStrategyType](./literals.md#automloverridestrategytype)
- [DatasetTypeType](./literals.md#datasettypetype)
- [DomainType](./literals.md#domaintype)
- [EvaluationTypeType](./literals.md#evaluationtypetype)
- [FeaturizationMethodNameType](./literals.md#featurizationmethodnametype)
- [FilterConditionStringType](./literals.md#filterconditionstringtype)
- [ListDatasetGroupsPaginatorName](./literals.md#listdatasetgroupspaginatorname)
- [ListDatasetImportJobsPaginatorName](./literals.md#listdatasetimportjobspaginatorname)
- [ListDatasetsPaginatorName](./literals.md#listdatasetspaginatorname)
- [ListForecastExportJobsPaginatorName](./literals.md#listforecastexportjobspaginatorname)
- [ListForecastsPaginatorName](./literals.md#listforecastspaginatorname)
- [ListPredictorBacktestExportJobsPaginatorName](./literals.md#listpredictorbacktestexportjobspaginatorname)
- [ListPredictorsPaginatorName](./literals.md#listpredictorspaginatorname)
- [OptimizationMetricType](./literals.md#optimizationmetrictype)
- [ScalingTypeType](./literals.md#scalingtypetype)
- [StateType](./literals.md#statetype)
- [TimePointGranularityType](./literals.md#timepointgranularitytype)
- [TimeSeriesGranularityType](./literals.md#timeseriesgranularitytype)
- [ForecastServiceServiceName](./literals.md#forecastserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_forecast.type_defs import AdditionalDatasetTypeDef

def get_value() -> AdditionalDatasetTypeDef:
    return {
        "Name": ...,
    }
```

- [AdditionalDatasetTypeDef](./type_defs.md#additionaldatasettypedef)
- [AttributeConfigTypeDef](./type_defs.md#attributeconfigtypedef)
- [CategoricalParameterRangeTypeDef](./type_defs.md#categoricalparameterrangetypedef)
- [ContinuousParameterRangeTypeDef](./type_defs.md#continuousparameterrangetypedef)
- [EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ExplainabilityConfigTypeDef](./type_defs.md#explainabilityconfigtypedef)
- [EvaluationParametersTypeDef](./type_defs.md#evaluationparameterstypedef)
- [S3ConfigTypeDef](./type_defs.md#s3configtypedef)
- [DatasetGroupSummaryTypeDef](./type_defs.md#datasetgroupsummarytypedef)
- [DatasetSummaryTypeDef](./type_defs.md#datasetsummarytypedef)
- [DeleteDatasetGroupRequestRequestTypeDef](./type_defs.md#deletedatasetgrouprequestrequesttypedef)
- [DeleteDatasetImportJobRequestRequestTypeDef](./type_defs.md#deletedatasetimportjobrequestrequesttypedef)
- [DeleteDatasetRequestRequestTypeDef](./type_defs.md#deletedatasetrequestrequesttypedef)
- [DeleteExplainabilityExportRequestRequestTypeDef](./type_defs.md#deleteexplainabilityexportrequestrequesttypedef)
- [DeleteExplainabilityRequestRequestTypeDef](./type_defs.md#deleteexplainabilityrequestrequesttypedef)
- [DeleteForecastExportJobRequestRequestTypeDef](./type_defs.md#deleteforecastexportjobrequestrequesttypedef)
- [DeleteForecastRequestRequestTypeDef](./type_defs.md#deleteforecastrequestrequesttypedef)
- [DeletePredictorBacktestExportJobRequestRequestTypeDef](./type_defs.md#deletepredictorbacktestexportjobrequestrequesttypedef)
- [DeletePredictorRequestRequestTypeDef](./type_defs.md#deletepredictorrequestrequesttypedef)
- [DeleteResourceTreeRequestRequestTypeDef](./type_defs.md#deleteresourcetreerequestrequesttypedef)
- [DescribeAutoPredictorRequestRequestTypeDef](./type_defs.md#describeautopredictorrequestrequesttypedef)
- [ExplainabilityInfoTypeDef](./type_defs.md#explainabilityinfotypedef)
- [ReferencePredictorSummaryTypeDef](./type_defs.md#referencepredictorsummarytypedef)
- [DescribeDatasetGroupRequestRequestTypeDef](./type_defs.md#describedatasetgrouprequestrequesttypedef)
- [DescribeDatasetImportJobRequestRequestTypeDef](./type_defs.md#describedatasetimportjobrequestrequesttypedef)
- [StatisticsTypeDef](./type_defs.md#statisticstypedef)
- [DescribeDatasetRequestRequestTypeDef](./type_defs.md#describedatasetrequestrequesttypedef)
- [DescribeExplainabilityExportRequestRequestTypeDef](./type_defs.md#describeexplainabilityexportrequestrequesttypedef)
- [DescribeExplainabilityRequestRequestTypeDef](./type_defs.md#describeexplainabilityrequestrequesttypedef)
- [DescribeForecastExportJobRequestRequestTypeDef](./type_defs.md#describeforecastexportjobrequestrequesttypedef)
- [DescribeForecastRequestRequestTypeDef](./type_defs.md#describeforecastrequestrequesttypedef)
- [DescribePredictorBacktestExportJobRequestRequestTypeDef](./type_defs.md#describepredictorbacktestexportjobrequestrequesttypedef)
- [DescribePredictorRequestRequestTypeDef](./type_defs.md#describepredictorrequestrequesttypedef)
- [ErrorMetricTypeDef](./type_defs.md#errormetrictypedef)
- [FeaturizationMethodTypeDef](./type_defs.md#featurizationmethodtypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [ForecastSummaryTypeDef](./type_defs.md#forecastsummarytypedef)
- [GetAccuracyMetricsRequestRequestTypeDef](./type_defs.md#getaccuracymetricsrequestrequesttypedef)
- [SupplementaryFeatureTypeDef](./type_defs.md#supplementaryfeaturetypedef)
- [IntegerParameterRangeTypeDef](./type_defs.md#integerparameterrangetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListDatasetGroupsRequestRequestTypeDef](./type_defs.md#listdatasetgroupsrequestrequesttypedef)
- [ListDatasetsRequestRequestTypeDef](./type_defs.md#listdatasetsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [WeightedQuantileLossTypeDef](./type_defs.md#weightedquantilelosstypedef)
- [TestWindowSummaryTypeDef](./type_defs.md#testwindowsummarytypedef)
- [SchemaAttributeTypeDef](./type_defs.md#schemaattributetypedef)
- [StopResourceRequestRequestTypeDef](./type_defs.md#stopresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateDatasetGroupRequestRequestTypeDef](./type_defs.md#updatedatasetgrouprequestrequesttypedef)
- [DataConfigTypeDef](./type_defs.md#dataconfigtypedef)
- [CreateDatasetGroupRequestRequestTypeDef](./type_defs.md#createdatasetgrouprequestrequesttypedef)
- [CreateForecastRequestRequestTypeDef](./type_defs.md#createforecastrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateAutoPredictorResponseTypeDef](./type_defs.md#createautopredictorresponsetypedef)
- [CreateDatasetGroupResponseTypeDef](./type_defs.md#createdatasetgroupresponsetypedef)
- [CreateDatasetImportJobResponseTypeDef](./type_defs.md#createdatasetimportjobresponsetypedef)
- [CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef)
- [CreateExplainabilityExportResponseTypeDef](./type_defs.md#createexplainabilityexportresponsetypedef)
- [CreateExplainabilityResponseTypeDef](./type_defs.md#createexplainabilityresponsetypedef)
- [CreateForecastExportJobResponseTypeDef](./type_defs.md#createforecastexportjobresponsetypedef)
- [CreateForecastResponseTypeDef](./type_defs.md#createforecastresponsetypedef)
- [CreatePredictorBacktestExportJobResponseTypeDef](./type_defs.md#createpredictorbacktestexportjobresponsetypedef)
- [CreatePredictorResponseTypeDef](./type_defs.md#createpredictorresponsetypedef)
- [DescribeDatasetGroupResponseTypeDef](./type_defs.md#describedatasetgroupresponsetypedef)
- [DescribeForecastResponseTypeDef](./type_defs.md#describeforecastresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ExplainabilitySummaryTypeDef](./type_defs.md#explainabilitysummarytypedef)
- [DataDestinationTypeDef](./type_defs.md#datadestinationtypedef)
- [DataSourceTypeDef](./type_defs.md#datasourcetypedef)
- [ListDatasetGroupsResponseTypeDef](./type_defs.md#listdatasetgroupsresponsetypedef)
- [ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef)
- [PredictorSummaryTypeDef](./type_defs.md#predictorsummarytypedef)
- [FeaturizationTypeDef](./type_defs.md#featurizationtypedef)
- [ListDatasetImportJobsRequestRequestTypeDef](./type_defs.md#listdatasetimportjobsrequestrequesttypedef)
- [ListExplainabilitiesRequestRequestTypeDef](./type_defs.md#listexplainabilitiesrequestrequesttypedef)
- [ListExplainabilityExportsRequestRequestTypeDef](./type_defs.md#listexplainabilityexportsrequestrequesttypedef)
- [ListForecastExportJobsRequestRequestTypeDef](./type_defs.md#listforecastexportjobsrequestrequesttypedef)
- [ListForecastsRequestRequestTypeDef](./type_defs.md#listforecastsrequestrequesttypedef)
- [ListPredictorBacktestExportJobsRequestRequestTypeDef](./type_defs.md#listpredictorbacktestexportjobsrequestrequesttypedef)
- [ListPredictorsRequestRequestTypeDef](./type_defs.md#listpredictorsrequestrequesttypedef)
- [ListForecastsResponseTypeDef](./type_defs.md#listforecastsresponsetypedef)
- [InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef)
- [ParameterRangesTypeDef](./type_defs.md#parameterrangestypedef)
- [ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef](./type_defs.md#listdatasetgroupsrequestlistdatasetgroupspaginatetypedef)
- [ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef](./type_defs.md#listdatasetimportjobsrequestlistdatasetimportjobspaginatetypedef)
- [ListDatasetsRequestListDatasetsPaginateTypeDef](./type_defs.md#listdatasetsrequestlistdatasetspaginatetypedef)
- [ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef](./type_defs.md#listforecastexportjobsrequestlistforecastexportjobspaginatetypedef)
- [ListForecastsRequestListForecastsPaginateTypeDef](./type_defs.md#listforecastsrequestlistforecastspaginatetypedef)
- [ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef](./type_defs.md#listpredictorbacktestexportjobsrequestlistpredictorbacktestexportjobspaginatetypedef)
- [ListPredictorsRequestListPredictorsPaginateTypeDef](./type_defs.md#listpredictorsrequestlistpredictorspaginatetypedef)
- [MetricsTypeDef](./type_defs.md#metricstypedef)
- [PredictorExecutionTypeDef](./type_defs.md#predictorexecutiontypedef)
- [SchemaTypeDef](./type_defs.md#schematypedef)
- [CreateAutoPredictorRequestRequestTypeDef](./type_defs.md#createautopredictorrequestrequesttypedef)
- [DescribeAutoPredictorResponseTypeDef](./type_defs.md#describeautopredictorresponsetypedef)
- [ListExplainabilitiesResponseTypeDef](./type_defs.md#listexplainabilitiesresponsetypedef)
- [CreateExplainabilityExportRequestRequestTypeDef](./type_defs.md#createexplainabilityexportrequestrequesttypedef)
- [CreateForecastExportJobRequestRequestTypeDef](./type_defs.md#createforecastexportjobrequestrequesttypedef)
- [CreatePredictorBacktestExportJobRequestRequestTypeDef](./type_defs.md#createpredictorbacktestexportjobrequestrequesttypedef)
- [DescribeExplainabilityExportResponseTypeDef](./type_defs.md#describeexplainabilityexportresponsetypedef)
- [DescribeForecastExportJobResponseTypeDef](./type_defs.md#describeforecastexportjobresponsetypedef)
- [DescribePredictorBacktestExportJobResponseTypeDef](./type_defs.md#describepredictorbacktestexportjobresponsetypedef)
- [ExplainabilityExportSummaryTypeDef](./type_defs.md#explainabilityexportsummarytypedef)
- [ForecastExportJobSummaryTypeDef](./type_defs.md#forecastexportjobsummarytypedef)
- [PredictorBacktestExportJobSummaryTypeDef](./type_defs.md#predictorbacktestexportjobsummarytypedef)
- [CreateDatasetImportJobRequestRequestTypeDef](./type_defs.md#createdatasetimportjobrequestrequesttypedef)
- [DatasetImportJobSummaryTypeDef](./type_defs.md#datasetimportjobsummarytypedef)
- [DescribeDatasetImportJobResponseTypeDef](./type_defs.md#describedatasetimportjobresponsetypedef)
- [ListPredictorsResponseTypeDef](./type_defs.md#listpredictorsresponsetypedef)
- [FeaturizationConfigTypeDef](./type_defs.md#featurizationconfigtypedef)
- [HyperParameterTuningJobConfigTypeDef](./type_defs.md#hyperparametertuningjobconfigtypedef)
- [WindowSummaryTypeDef](./type_defs.md#windowsummarytypedef)
- [PredictorExecutionDetailsTypeDef](./type_defs.md#predictorexecutiondetailstypedef)
- [CreateDatasetRequestRequestTypeDef](./type_defs.md#createdatasetrequestrequesttypedef)
- [CreateExplainabilityRequestRequestTypeDef](./type_defs.md#createexplainabilityrequestrequesttypedef)
- [DescribeDatasetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef)
- [DescribeExplainabilityResponseTypeDef](./type_defs.md#describeexplainabilityresponsetypedef)
- [ListExplainabilityExportsResponseTypeDef](./type_defs.md#listexplainabilityexportsresponsetypedef)
- [ListForecastExportJobsResponseTypeDef](./type_defs.md#listforecastexportjobsresponsetypedef)
- [ListPredictorBacktestExportJobsResponseTypeDef](./type_defs.md#listpredictorbacktestexportjobsresponsetypedef)
- [ListDatasetImportJobsResponseTypeDef](./type_defs.md#listdatasetimportjobsresponsetypedef)
- [CreatePredictorRequestRequestTypeDef](./type_defs.md#createpredictorrequestrequesttypedef)
- [EvaluationResultTypeDef](./type_defs.md#evaluationresulttypedef)
- [DescribePredictorResponseTypeDef](./type_defs.md#describepredictorresponsetypedef)
- [GetAccuracyMetricsResponseTypeDef](./type_defs.md#getaccuracymetricsresponsetypedef)

