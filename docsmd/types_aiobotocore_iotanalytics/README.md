# IoTAnalytics module

> [Index](../README.md) > IoTAnalytics


!!! note ""

    Auto-generated documentation for [IoTAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
    type annotations stubs module [types-aiobotocore-iotanalytics](https://pypi.org/project/types-aiobotocore-iotanalytics/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `IoTAnalytics` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[iotanalytics]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[iotanalytics]'


# standalone installation
python -m pip install types-aiobotocore-iotanalytics
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-iotanalytics
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IoTAnalyticsClient

Type annotations and code completion for  `#!python session.client("iotanalytics")` as [IoTAnalyticsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iotanalytics.client import IoTAnalyticsClient


session = Session()
async with session.client("iotanalytics") as client:
    client: IoTAnalyticsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("iotanalytics").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_iotanalytics.paginator import ListChannelsPaginator

def get_list_channels_paginator() -> ListChannelsPaginator:
    return client.get_paginator("list_channels"))
```

- [ListChannelsPaginator](./paginators.md#listchannelspaginator)
- [ListDatasetContentsPaginator](./paginators.md#listdatasetcontentspaginator)
- [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
- [ListDatastoresPaginator](./paginators.md#listdatastorespaginator)
- [ListPipelinesPaginator](./paginators.md#listpipelinespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_iotanalytics.literals import ChannelStatusType

def get_value() -> ChannelStatusType:
    return "ACTIVE"
```

- [ChannelStatusType](./literals.md#channelstatustype)
- [ComputeTypeType](./literals.md#computetypetype)
- [DatasetActionTypeType](./literals.md#datasetactiontypetype)
- [DatasetContentStateType](./literals.md#datasetcontentstatetype)
- [DatasetStatusType](./literals.md#datasetstatustype)
- [DatastoreStatusType](./literals.md#datastorestatustype)
- [FileFormatTypeType](./literals.md#fileformattypetype)
- [ListChannelsPaginatorName](./literals.md#listchannelspaginatorname)
- [ListDatasetContentsPaginatorName](./literals.md#listdatasetcontentspaginatorname)
- [ListDatasetsPaginatorName](./literals.md#listdatasetspaginatorname)
- [ListDatastoresPaginatorName](./literals.md#listdatastorespaginatorname)
- [ListPipelinesPaginatorName](./literals.md#listpipelinespaginatorname)
- [LoggingLevelType](./literals.md#loggingleveltype)
- [ReprocessingStatusType](./literals.md#reprocessingstatustype)
- [IoTAnalyticsServiceName](./literals.md#iotanalyticsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_iotanalytics.type_defs import AddAttributesActivityTypeDef

def get_value() -> AddAttributesActivityTypeDef:
    return {
        "name": ...,
        "attributes": ...,
    }
```

- [AddAttributesActivityTypeDef](./type_defs.md#addattributesactivitytypedef)
- [BatchPutMessageErrorEntryTypeDef](./type_defs.md#batchputmessageerrorentrytypedef)
- [MessageTypeDef](./type_defs.md#messagetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CancelPipelineReprocessingRequestRequestTypeDef](./type_defs.md#cancelpipelinereprocessingrequestrequesttypedef)
- [ChannelActivityTypeDef](./type_defs.md#channelactivitytypedef)
- [ChannelMessagesTypeDef](./type_defs.md#channelmessagestypedef)
- [EstimatedResourceSizeTypeDef](./type_defs.md#estimatedresourcesizetypedef)
- [CustomerManagedChannelS3StorageSummaryTypeDef](./type_defs.md#customermanagedchannels3storagesummarytypedef)
- [CustomerManagedChannelS3StorageTypeDef](./type_defs.md#customermanagedchannels3storagetypedef)
- [RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef)
- [ColumnTypeDef](./type_defs.md#columntypedef)
- [ResourceConfigurationTypeDef](./type_defs.md#resourceconfigurationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [CreateDatasetContentRequestRequestTypeDef](./type_defs.md#createdatasetcontentrequestrequesttypedef)
- [VersioningConfigurationTypeDef](./type_defs.md#versioningconfigurationtypedef)
- [CustomerManagedDatastoreS3StorageSummaryTypeDef](./type_defs.md#customermanageddatastores3storagesummarytypedef)
- [CustomerManagedDatastoreS3StorageTypeDef](./type_defs.md#customermanageddatastores3storagetypedef)
- [DatasetActionSummaryTypeDef](./type_defs.md#datasetactionsummarytypedef)
- [IotEventsDestinationConfigurationTypeDef](./type_defs.md#ioteventsdestinationconfigurationtypedef)
- [DatasetContentStatusTypeDef](./type_defs.md#datasetcontentstatustypedef)
- [DatasetContentVersionValueTypeDef](./type_defs.md#datasetcontentversionvaluetypedef)
- [DatasetEntryTypeDef](./type_defs.md#datasetentrytypedef)
- [ScheduleTypeDef](./type_defs.md#scheduletypedef)
- [TriggeringDatasetTypeDef](./type_defs.md#triggeringdatasettypedef)
- [DatastoreActivityTypeDef](./type_defs.md#datastoreactivitytypedef)
- [IotSiteWiseCustomerManagedDatastoreS3StorageSummaryTypeDef](./type_defs.md#iotsitewisecustomermanageddatastores3storagesummarytypedef)
- [IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef](./type_defs.md#iotsitewisecustomermanageddatastores3storagetypedef)
- [PartitionTypeDef](./type_defs.md#partitiontypedef)
- [TimestampPartitionTypeDef](./type_defs.md#timestamppartitiontypedef)
- [DeleteChannelRequestRequestTypeDef](./type_defs.md#deletechannelrequestrequesttypedef)
- [DeleteDatasetContentRequestRequestTypeDef](./type_defs.md#deletedatasetcontentrequestrequesttypedef)
- [DeleteDatasetRequestRequestTypeDef](./type_defs.md#deletedatasetrequestrequesttypedef)
- [DeleteDatastoreRequestRequestTypeDef](./type_defs.md#deletedatastorerequestrequesttypedef)
- [DeletePipelineRequestRequestTypeDef](./type_defs.md#deletepipelinerequestrequesttypedef)
- [DeltaTimeSessionWindowConfigurationTypeDef](./type_defs.md#deltatimesessionwindowconfigurationtypedef)
- [DeltaTimeTypeDef](./type_defs.md#deltatimetypedef)
- [DescribeChannelRequestRequestTypeDef](./type_defs.md#describechannelrequestrequesttypedef)
- [DescribeDatasetRequestRequestTypeDef](./type_defs.md#describedatasetrequestrequesttypedef)
- [DescribeDatastoreRequestRequestTypeDef](./type_defs.md#describedatastorerequestrequesttypedef)
- [LoggingOptionsTypeDef](./type_defs.md#loggingoptionstypedef)
- [DescribePipelineRequestRequestTypeDef](./type_defs.md#describepipelinerequestrequesttypedef)
- [DeviceRegistryEnrichActivityTypeDef](./type_defs.md#deviceregistryenrichactivitytypedef)
- [DeviceShadowEnrichActivityTypeDef](./type_defs.md#deviceshadowenrichactivitytypedef)
- [FilterActivityTypeDef](./type_defs.md#filteractivitytypedef)
- [GetDatasetContentRequestRequestTypeDef](./type_defs.md#getdatasetcontentrequestrequesttypedef)
- [GlueConfigurationTypeDef](./type_defs.md#glueconfigurationtypedef)
- [LambdaActivityTypeDef](./type_defs.md#lambdaactivitytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListChannelsRequestRequestTypeDef](./type_defs.md#listchannelsrequestrequesttypedef)
- [ListDatasetContentsRequestRequestTypeDef](./type_defs.md#listdatasetcontentsrequestrequesttypedef)
- [ListDatasetsRequestRequestTypeDef](./type_defs.md#listdatasetsrequestrequesttypedef)
- [ListDatastoresRequestRequestTypeDef](./type_defs.md#listdatastoresrequestrequesttypedef)
- [ListPipelinesRequestRequestTypeDef](./type_defs.md#listpipelinesrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [MathActivityTypeDef](./type_defs.md#mathactivitytypedef)
- [OutputFileUriValueTypeDef](./type_defs.md#outputfileurivaluetypedef)
- [RemoveAttributesActivityTypeDef](./type_defs.md#removeattributesactivitytypedef)
- [SelectAttributesActivityTypeDef](./type_defs.md#selectattributesactivitytypedef)
- [ReprocessingSummaryTypeDef](./type_defs.md#reprocessingsummarytypedef)
- [SampleChannelDataRequestRequestTypeDef](./type_defs.md#samplechanneldatarequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [BatchPutMessageRequestRequestTypeDef](./type_defs.md#batchputmessagerequestrequesttypedef)
- [BatchPutMessageResponseTypeDef](./type_defs.md#batchputmessageresponsetypedef)
- [CreateDatasetContentResponseTypeDef](./type_defs.md#createdatasetcontentresponsetypedef)
- [CreatePipelineResponseTypeDef](./type_defs.md#createpipelineresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [RunPipelineActivityResponseTypeDef](./type_defs.md#runpipelineactivityresponsetypedef)
- [SampleChannelDataResponseTypeDef](./type_defs.md#samplechanneldataresponsetypedef)
- [StartPipelineReprocessingResponseTypeDef](./type_defs.md#startpipelinereprocessingresponsetypedef)
- [StartPipelineReprocessingRequestRequestTypeDef](./type_defs.md#startpipelinereprocessingrequestrequesttypedef)
- [ChannelStatisticsTypeDef](./type_defs.md#channelstatisticstypedef)
- [DatastoreStatisticsTypeDef](./type_defs.md#datastorestatisticstypedef)
- [ChannelStorageSummaryTypeDef](./type_defs.md#channelstoragesummarytypedef)
- [ChannelStorageTypeDef](./type_defs.md#channelstoragetypedef)
- [CreateChannelResponseTypeDef](./type_defs.md#createchannelresponsetypedef)
- [CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef)
- [CreateDatastoreResponseTypeDef](./type_defs.md#createdatastoreresponsetypedef)
- [SchemaDefinitionTypeDef](./type_defs.md#schemadefinitiontypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [DatasetContentSummaryTypeDef](./type_defs.md#datasetcontentsummarytypedef)
- [GetDatasetContentResponseTypeDef](./type_defs.md#getdatasetcontentresponsetypedef)
- [DatasetTriggerTypeDef](./type_defs.md#datasettriggertypedef)
- [DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef](./type_defs.md#datastoreiotsitewisemultilayerstoragesummarytypedef)
- [DatastoreIotSiteWiseMultiLayerStorageTypeDef](./type_defs.md#datastoreiotsitewisemultilayerstoragetypedef)
- [DatastorePartitionTypeDef](./type_defs.md#datastorepartitiontypedef)
- [LateDataRuleConfigurationTypeDef](./type_defs.md#latedataruleconfigurationtypedef)
- [QueryFilterTypeDef](./type_defs.md#queryfiltertypedef)
- [DescribeLoggingOptionsResponseTypeDef](./type_defs.md#describeloggingoptionsresponsetypedef)
- [PutLoggingOptionsRequestRequestTypeDef](./type_defs.md#putloggingoptionsrequestrequesttypedef)
- [S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef)
- [ListChannelsRequestListChannelsPaginateTypeDef](./type_defs.md#listchannelsrequestlistchannelspaginatetypedef)
- [ListDatasetContentsRequestListDatasetContentsPaginateTypeDef](./type_defs.md#listdatasetcontentsrequestlistdatasetcontentspaginatetypedef)
- [ListDatasetsRequestListDatasetsPaginateTypeDef](./type_defs.md#listdatasetsrequestlistdatasetspaginatetypedef)
- [ListDatastoresRequestListDatastoresPaginateTypeDef](./type_defs.md#listdatastoresrequestlistdatastorespaginatetypedef)
- [ListPipelinesRequestListPipelinesPaginateTypeDef](./type_defs.md#listpipelinesrequestlistpipelinespaginatetypedef)
- [VariableTypeDef](./type_defs.md#variabletypedef)
- [PipelineActivityTypeDef](./type_defs.md#pipelineactivitytypedef)
- [PipelineSummaryTypeDef](./type_defs.md#pipelinesummarytypedef)
- [ChannelSummaryTypeDef](./type_defs.md#channelsummarytypedef)
- [ChannelTypeDef](./type_defs.md#channeltypedef)
- [CreateChannelRequestRequestTypeDef](./type_defs.md#createchannelrequestrequesttypedef)
- [UpdateChannelRequestRequestTypeDef](./type_defs.md#updatechannelrequestrequesttypedef)
- [ParquetConfigurationTypeDef](./type_defs.md#parquetconfigurationtypedef)
- [ListDatasetContentsResponseTypeDef](./type_defs.md#listdatasetcontentsresponsetypedef)
- [DatasetSummaryTypeDef](./type_defs.md#datasetsummarytypedef)
- [DatastoreStorageSummaryTypeDef](./type_defs.md#datastorestoragesummarytypedef)
- [DatastoreStorageTypeDef](./type_defs.md#datastorestoragetypedef)
- [DatastorePartitionsTypeDef](./type_defs.md#datastorepartitionstypedef)
- [LateDataRuleTypeDef](./type_defs.md#latedataruletypedef)
- [SqlQueryDatasetActionTypeDef](./type_defs.md#sqlquerydatasetactiontypedef)
- [DatasetContentDeliveryDestinationTypeDef](./type_defs.md#datasetcontentdeliverydestinationtypedef)
- [ContainerDatasetActionTypeDef](./type_defs.md#containerdatasetactiontypedef)
- [CreatePipelineRequestRequestTypeDef](./type_defs.md#createpipelinerequestrequesttypedef)
- [PipelineTypeDef](./type_defs.md#pipelinetypedef)
- [RunPipelineActivityRequestRequestTypeDef](./type_defs.md#runpipelineactivityrequestrequesttypedef)
- [UpdatePipelineRequestRequestTypeDef](./type_defs.md#updatepipelinerequestrequesttypedef)
- [ListPipelinesResponseTypeDef](./type_defs.md#listpipelinesresponsetypedef)
- [ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef)
- [DescribeChannelResponseTypeDef](./type_defs.md#describechannelresponsetypedef)
- [FileFormatConfigurationTypeDef](./type_defs.md#fileformatconfigurationtypedef)
- [ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef)
- [DatastoreSummaryTypeDef](./type_defs.md#datastoresummarytypedef)
- [DatasetContentDeliveryRuleTypeDef](./type_defs.md#datasetcontentdeliveryruletypedef)
- [DatasetActionTypeDef](./type_defs.md#datasetactiontypedef)
- [DescribePipelineResponseTypeDef](./type_defs.md#describepipelineresponsetypedef)
- [CreateDatastoreRequestRequestTypeDef](./type_defs.md#createdatastorerequestrequesttypedef)
- [DatastoreTypeDef](./type_defs.md#datastoretypedef)
- [UpdateDatastoreRequestRequestTypeDef](./type_defs.md#updatedatastorerequestrequesttypedef)
- [ListDatastoresResponseTypeDef](./type_defs.md#listdatastoresresponsetypedef)
- [CreateDatasetRequestRequestTypeDef](./type_defs.md#createdatasetrequestrequesttypedef)
- [DatasetTypeDef](./type_defs.md#datasettypedef)
- [UpdateDatasetRequestRequestTypeDef](./type_defs.md#updatedatasetrequestrequesttypedef)
- [DescribeDatastoreResponseTypeDef](./type_defs.md#describedatastoreresponsetypedef)
- [DescribeDatasetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef)

