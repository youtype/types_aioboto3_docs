# IoTTwinMaker module

> [Index](../README.md) > IoTTwinMaker


!!! note ""

    Auto-generated documentation for [IoTTwinMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
    type annotations stubs module [types-aiobotocore-iottwinmaker](https://pypi.org/project/types-aiobotocore-iottwinmaker/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `IoTTwinMaker` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[iottwinmaker]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[iottwinmaker]'


# standalone installation
python -m pip install types-aiobotocore-iottwinmaker
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-iottwinmaker
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IoTTwinMakerClient

Type annotations and code completion for  `#!python session.client("iottwinmaker")` as [IoTTwinMakerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client)

```python
# IoTTwinMakerClient usage example

from aioboto3.session import Session

from types_aiobotocore_iottwinmaker.client import IoTTwinMakerClient


session = Session()
async with session.client("iottwinmaker") as client:
    client: IoTTwinMakerClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ColumnTypeType usage example

from types_aiobotocore_iottwinmaker.literals import ColumnTypeType

def get_value() -> ColumnTypeType:
    return "EDGE"
```

- [ColumnTypeType](./literals.md#columntypetype)
- [ComponentUpdateTypeType](./literals.md#componentupdatetypetype)
- [DestinationTypeType](./literals.md#destinationtypetype)
- [ErrorCodeType](./literals.md#errorcodetype)
- [GroupTypeType](./literals.md#grouptypetype)
- [InterpolationTypeType](./literals.md#interpolationtypetype)
- [MetadataTransferJobStateType](./literals.md#metadatatransferjobstatetype)
- [OrderByTimeType](./literals.md#orderbytimetype)
- [OrderType](./literals.md#ordertype)
- [ParentEntityUpdateTypeType](./literals.md#parententityupdatetypetype)
- [PricingModeType](./literals.md#pricingmodetype)
- [PricingTierType](./literals.md#pricingtiertype)
- [PropertyGroupUpdateTypeType](./literals.md#propertygroupupdatetypetype)
- [PropertyUpdateTypeType](./literals.md#propertyupdatetypetype)
- [SceneErrorCodeType](./literals.md#sceneerrorcodetype)
- [ScopeType](./literals.md#scopetype)
- [SourceTypeType](./literals.md#sourcetypetype)
- [StateType](./literals.md#statetype)
- [SyncJobStateType](./literals.md#syncjobstatetype)
- [SyncResourceStateType](./literals.md#syncresourcestatetype)
- [SyncResourceTypeType](./literals.md#syncresourcetypetype)
- [TypeType](./literals.md#typetype)
- [UpdateReasonType](./literals.md#updatereasontype)
- [IoTTwinMakerServiceName](./literals.md#iottwinmakerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BundleInformationTypeDef](./type_defs.md#bundleinformationtypedef)
- [CancelMetadataTransferJobRequestRequestTypeDef](./type_defs.md#cancelmetadatatransferjobrequestrequesttypedef)
- [MetadataTransferJobProgressTypeDef](./type_defs.md#metadatatransferjobprogresstypedef)
- [ColumnDescriptionTypeDef](./type_defs.md#columndescriptiontypedef)
- [ComponentPropertyGroupRequestTypeDef](./type_defs.md#componentpropertygrouprequesttypedef)
- [ComponentPropertyGroupResponseTypeDef](./type_defs.md#componentpropertygroupresponsetypedef)
- [CompositeComponentTypeRequestTypeDef](./type_defs.md#compositecomponenttyperequesttypedef)
- [CompositeComponentTypeResponseTypeDef](./type_defs.md#compositecomponenttyperesponsetypedef)
- [PropertyDefinitionRequestTypeDef](./type_defs.md#propertydefinitionrequesttypedef)
- [PropertyGroupRequestTypeDef](./type_defs.md#propertygrouprequesttypedef)
- [CreateSceneRequestRequestTypeDef](./type_defs.md#createscenerequestrequesttypedef)
- [CreateSyncJobRequestRequestTypeDef](./type_defs.md#createsyncjobrequestrequesttypedef)
- [CreateWorkspaceRequestRequestTypeDef](./type_defs.md#createworkspacerequestrequesttypedef)
- [LambdaFunctionTypeDef](./type_defs.md#lambdafunctiontypedef)
- [RelationshipTypeDef](./type_defs.md#relationshiptypedef)
- [RelationshipValueTypeDef](./type_defs.md#relationshipvaluetypedef)
- [DeleteComponentTypeRequestRequestTypeDef](./type_defs.md#deletecomponenttyperequestrequesttypedef)
- [DeleteEntityRequestRequestTypeDef](./type_defs.md#deleteentityrequestrequesttypedef)
- [DeleteSceneRequestRequestTypeDef](./type_defs.md#deletescenerequestrequesttypedef)
- [DeleteSyncJobRequestRequestTypeDef](./type_defs.md#deletesyncjobrequestrequesttypedef)
- [DeleteWorkspaceRequestRequestTypeDef](./type_defs.md#deleteworkspacerequestrequesttypedef)
- [IotTwinMakerDestinationConfigurationTypeDef](./type_defs.md#iottwinmakerdestinationconfigurationtypedef)
- [S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef)
- [EntityPropertyReferenceTypeDef](./type_defs.md#entitypropertyreferencetypedef)
- [ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef)
- [ExecuteQueryRequestRequestTypeDef](./type_defs.md#executequeryrequestrequesttypedef)
- [RowTypeDef](./type_defs.md#rowtypedef)
- [FilterByAssetModelTypeDef](./type_defs.md#filterbyassetmodeltypedef)
- [FilterByAssetTypeDef](./type_defs.md#filterbyassettypedef)
- [FilterByComponentTypeTypeDef](./type_defs.md#filterbycomponenttypetypedef)
- [FilterByEntityTypeDef](./type_defs.md#filterbyentitytypedef)
- [GetComponentTypeRequestRequestTypeDef](./type_defs.md#getcomponenttyperequestrequesttypedef)
- [PropertyDefinitionResponseTypeDef](./type_defs.md#propertydefinitionresponsetypedef)
- [PropertyGroupResponseTypeDef](./type_defs.md#propertygroupresponsetypedef)
- [GetEntityRequestRequestTypeDef](./type_defs.md#getentityrequestrequesttypedef)
- [GetMetadataTransferJobRequestRequestTypeDef](./type_defs.md#getmetadatatransferjobrequestrequesttypedef)
- [InterpolationParametersTypeDef](./type_defs.md#interpolationparameterstypedef)
- [PropertyFilterTypeDef](./type_defs.md#propertyfiltertypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [GetSceneRequestRequestTypeDef](./type_defs.md#getscenerequestrequesttypedef)
- [SceneErrorTypeDef](./type_defs.md#sceneerrortypedef)
- [GetSyncJobRequestRequestTypeDef](./type_defs.md#getsyncjobrequestrequesttypedef)
- [GetWorkspaceRequestRequestTypeDef](./type_defs.md#getworkspacerequestrequesttypedef)
- [ListComponentTypesFilterTypeDef](./type_defs.md#listcomponenttypesfiltertypedef)
- [ListComponentsRequestRequestTypeDef](./type_defs.md#listcomponentsrequestrequesttypedef)
- [ListEntitiesFilterTypeDef](./type_defs.md#listentitiesfiltertypedef)
- [ListMetadataTransferJobsFilterTypeDef](./type_defs.md#listmetadatatransferjobsfiltertypedef)
- [ListPropertiesRequestRequestTypeDef](./type_defs.md#listpropertiesrequestrequesttypedef)
- [ListScenesRequestRequestTypeDef](./type_defs.md#listscenesrequestrequesttypedef)
- [SceneSummaryTypeDef](./type_defs.md#scenesummarytypedef)
- [ListSyncJobsRequestRequestTypeDef](./type_defs.md#listsyncjobsrequestrequesttypedef)
- [SyncResourceFilterTypeDef](./type_defs.md#syncresourcefiltertypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListWorkspacesRequestRequestTypeDef](./type_defs.md#listworkspacesrequestrequesttypedef)
- [WorkspaceSummaryTypeDef](./type_defs.md#workspacesummarytypedef)
- [OrderByTypeDef](./type_defs.md#orderbytypedef)
- [ParentEntityUpdateRequestTypeDef](./type_defs.md#parententityupdaterequesttypedef)
- [S3SourceConfigurationTypeDef](./type_defs.md#s3sourceconfigurationtypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdatePricingPlanRequestRequestTypeDef](./type_defs.md#updatepricingplanrequestrequesttypedef)
- [UpdateSceneRequestRequestTypeDef](./type_defs.md#updatescenerequestrequesttypedef)
- [UpdateWorkspaceRequestRequestTypeDef](./type_defs.md#updateworkspacerequestrequesttypedef)
- [CreateComponentTypeResponseTypeDef](./type_defs.md#createcomponenttyperesponsetypedef)
- [CreateEntityResponseTypeDef](./type_defs.md#createentityresponsetypedef)
- [CreateSceneResponseTypeDef](./type_defs.md#createsceneresponsetypedef)
- [CreateSyncJobResponseTypeDef](./type_defs.md#createsyncjobresponsetypedef)
- [CreateWorkspaceResponseTypeDef](./type_defs.md#createworkspaceresponsetypedef)
- [DeleteComponentTypeResponseTypeDef](./type_defs.md#deletecomponenttyperesponsetypedef)
- [DeleteEntityResponseTypeDef](./type_defs.md#deleteentityresponsetypedef)
- [DeleteSyncJobResponseTypeDef](./type_defs.md#deletesyncjobresponsetypedef)
- [DeleteWorkspaceResponseTypeDef](./type_defs.md#deleteworkspaceresponsetypedef)
- [GetWorkspaceResponseTypeDef](./type_defs.md#getworkspaceresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdateComponentTypeResponseTypeDef](./type_defs.md#updatecomponenttyperesponsetypedef)
- [UpdateEntityResponseTypeDef](./type_defs.md#updateentityresponsetypedef)
- [UpdateSceneResponseTypeDef](./type_defs.md#updatesceneresponsetypedef)
- [UpdateWorkspaceResponseTypeDef](./type_defs.md#updateworkspaceresponsetypedef)
- [PricingPlanTypeDef](./type_defs.md#pricingplantypedef)
- [PropertyRequestTypeDef](./type_defs.md#propertyrequesttypedef)
- [DataConnectorTypeDef](./type_defs.md#dataconnectortypedef)
- [DataTypeTypeDef](./type_defs.md#datatypetypedef)
- [DataValueTypeDef](./type_defs.md#datavaluetypedef)
- [DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef)
- [PropertyLatestValueTypeDef](./type_defs.md#propertylatestvaluetypedef)
- [MetadataTransferJobStatusTypeDef](./type_defs.md#metadatatransferjobstatustypedef)
- [StatusTypeDef](./type_defs.md#statustypedef)
- [SyncJobStatusTypeDef](./type_defs.md#syncjobstatustypedef)
- [SyncResourceStatusTypeDef](./type_defs.md#syncresourcestatustypedef)
- [ExecuteQueryResponseTypeDef](./type_defs.md#executequeryresponsetypedef)
- [IotSiteWiseSourceConfigurationFilterTypeDef](./type_defs.md#iotsitewisesourceconfigurationfiltertypedef)
- [IotTwinMakerSourceConfigurationFilterTypeDef](./type_defs.md#iottwinmakersourceconfigurationfiltertypedef)
- [PropertyResponseTypeDef](./type_defs.md#propertyresponsetypedef)
- [PropertySummaryTypeDef](./type_defs.md#propertysummarytypedef)
- [GetPropertyValueHistoryRequestRequestTypeDef](./type_defs.md#getpropertyvaluehistoryrequestrequesttypedef)
- [PropertyValueTypeDef](./type_defs.md#propertyvaluetypedef)
- [GetSceneResponseTypeDef](./type_defs.md#getsceneresponsetypedef)
- [ListComponentTypesRequestRequestTypeDef](./type_defs.md#listcomponenttypesrequestrequesttypedef)
- [ListEntitiesRequestRequestTypeDef](./type_defs.md#listentitiesrequestrequesttypedef)
- [ListMetadataTransferJobsRequestRequestTypeDef](./type_defs.md#listmetadatatransferjobsrequestrequesttypedef)
- [ListScenesResponseTypeDef](./type_defs.md#listscenesresponsetypedef)
- [ListSyncResourcesRequestRequestTypeDef](./type_defs.md#listsyncresourcesrequestrequesttypedef)
- [ListWorkspacesResponseTypeDef](./type_defs.md#listworkspacesresponsetypedef)
- [TabularConditionsTypeDef](./type_defs.md#tabularconditionstypedef)
- [GetPricingPlanResponseTypeDef](./type_defs.md#getpricingplanresponsetypedef)
- [UpdatePricingPlanResponseTypeDef](./type_defs.md#updatepricingplanresponsetypedef)
- [ComponentRequestTypeDef](./type_defs.md#componentrequesttypedef)
- [ComponentUpdateRequestTypeDef](./type_defs.md#componentupdaterequesttypedef)
- [CompositeComponentRequestTypeDef](./type_defs.md#compositecomponentrequesttypedef)
- [CompositeComponentUpdateRequestTypeDef](./type_defs.md#compositecomponentupdaterequesttypedef)
- [FunctionRequestTypeDef](./type_defs.md#functionrequesttypedef)
- [FunctionResponseTypeDef](./type_defs.md#functionresponsetypedef)
- [GetPropertyValueResponseTypeDef](./type_defs.md#getpropertyvalueresponsetypedef)
- [CancelMetadataTransferJobResponseTypeDef](./type_defs.md#cancelmetadatatransferjobresponsetypedef)
- [CreateMetadataTransferJobResponseTypeDef](./type_defs.md#createmetadatatransferjobresponsetypedef)
- [MetadataTransferJobSummaryTypeDef](./type_defs.md#metadatatransferjobsummarytypedef)
- [ComponentSummaryTypeDef](./type_defs.md#componentsummarytypedef)
- [ComponentTypeSummaryTypeDef](./type_defs.md#componenttypesummarytypedef)
- [EntitySummaryTypeDef](./type_defs.md#entitysummarytypedef)
- [GetSyncJobResponseTypeDef](./type_defs.md#getsyncjobresponsetypedef)
- [SyncJobSummaryTypeDef](./type_defs.md#syncjobsummarytypedef)
- [SyncResourceSummaryTypeDef](./type_defs.md#syncresourcesummarytypedef)
- [IotSiteWiseSourceConfigurationTypeDef](./type_defs.md#iotsitewisesourceconfigurationtypedef)
- [IotTwinMakerSourceConfigurationTypeDef](./type_defs.md#iottwinmakersourceconfigurationtypedef)
- [ListPropertiesResponseTypeDef](./type_defs.md#listpropertiesresponsetypedef)
- [PropertyValueEntryTypeDef](./type_defs.md#propertyvalueentrytypedef)
- [PropertyValueHistoryTypeDef](./type_defs.md#propertyvaluehistorytypedef)
- [GetPropertyValueRequestRequestTypeDef](./type_defs.md#getpropertyvaluerequestrequesttypedef)
- [CreateEntityRequestRequestTypeDef](./type_defs.md#createentityrequestrequesttypedef)
- [UpdateEntityRequestRequestTypeDef](./type_defs.md#updateentityrequestrequesttypedef)
- [CreateComponentTypeRequestRequestTypeDef](./type_defs.md#createcomponenttyperequestrequesttypedef)
- [UpdateComponentTypeRequestRequestTypeDef](./type_defs.md#updatecomponenttyperequestrequesttypedef)
- [GetComponentTypeResponseTypeDef](./type_defs.md#getcomponenttyperesponsetypedef)
- [ListMetadataTransferJobsResponseTypeDef](./type_defs.md#listmetadatatransferjobsresponsetypedef)
- [ComponentResponseTypeDef](./type_defs.md#componentresponsetypedef)
- [ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef)
- [ListComponentTypesResponseTypeDef](./type_defs.md#listcomponenttypesresponsetypedef)
- [ListEntitiesResponseTypeDef](./type_defs.md#listentitiesresponsetypedef)
- [ListSyncJobsResponseTypeDef](./type_defs.md#listsyncjobsresponsetypedef)
- [ListSyncResourcesResponseTypeDef](./type_defs.md#listsyncresourcesresponsetypedef)
- [SourceConfigurationTypeDef](./type_defs.md#sourceconfigurationtypedef)
- [BatchPutPropertyErrorTypeDef](./type_defs.md#batchputpropertyerrortypedef)
- [BatchPutPropertyValuesRequestRequestTypeDef](./type_defs.md#batchputpropertyvaluesrequestrequesttypedef)
- [GetPropertyValueHistoryResponseTypeDef](./type_defs.md#getpropertyvaluehistoryresponsetypedef)
- [GetEntityResponseTypeDef](./type_defs.md#getentityresponsetypedef)
- [CreateMetadataTransferJobRequestRequestTypeDef](./type_defs.md#createmetadatatransferjobrequestrequesttypedef)
- [GetMetadataTransferJobResponseTypeDef](./type_defs.md#getmetadatatransferjobresponsetypedef)
- [BatchPutPropertyErrorEntryTypeDef](./type_defs.md#batchputpropertyerrorentrytypedef)
- [BatchPutPropertyValuesResponseTypeDef](./type_defs.md#batchputpropertyvaluesresponsetypedef)

