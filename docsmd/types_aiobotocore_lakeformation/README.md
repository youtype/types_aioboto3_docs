# LakeFormation module

> [Index](../README.md) > LakeFormation


!!! note ""

    Auto-generated documentation for [LakeFormation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
    type annotations stubs module [types-aiobotocore-lakeformation](https://pypi.org/project/types-aiobotocore-lakeformation/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `LakeFormation` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[lakeformation]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[lakeformation]'


# standalone installation
python -m pip install types-aiobotocore-lakeformation
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-lakeformation
```

## Usage

Code samples can be found in [Examples](./usage.md).

## LakeFormationClient

Type annotations and code completion for  `#!python session.client("lakeformation")` as [LakeFormationClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# LakeFormationClient usage example

from aioboto3.session import Session

from types_aiobotocore_lakeformation.client import LakeFormationClient


session = Session()
async with session.client("lakeformation") as client:
    client: LakeFormationClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("lakeformation").get_paginator("...")`.

```python
# GetWorkUnitsPaginator usage example

from types_aiobotocore_lakeformation.paginator import GetWorkUnitsPaginator

def get_get_work_units_paginator() -> GetWorkUnitsPaginator:
    return client.get_paginator("get_work_units"))
```

- [GetWorkUnitsPaginator](./paginators.md#getworkunitspaginator)
- [ListDataCellsFilterPaginator](./paginators.md#listdatacellsfilterpaginator)
- [ListLFTagsPaginator](./paginators.md#listlftagspaginator)
- [SearchDatabasesByLFTagsPaginator](./paginators.md#searchdatabasesbylftagspaginator)
- [SearchTablesByLFTagsPaginator](./paginators.md#searchtablesbylftagspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ApplicationStatusType usage example

from types_aiobotocore_lakeformation.literals import ApplicationStatusType

def get_value() -> ApplicationStatusType:
    return "DISABLED"
```

- [ApplicationStatusType](./literals.md#applicationstatustype)
- [ComparisonOperatorType](./literals.md#comparisonoperatortype)
- [DataLakeResourceTypeType](./literals.md#datalakeresourcetypetype)
- [EnableStatusType](./literals.md#enablestatustype)
- [FieldNameStringType](./literals.md#fieldnamestringtype)
- [GetWorkUnitsPaginatorName](./literals.md#getworkunitspaginatorname)
- [ListDataCellsFilterPaginatorName](./literals.md#listdatacellsfilterpaginatorname)
- [ListLFTagsPaginatorName](./literals.md#listlftagspaginatorname)
- [OptimizerTypeType](./literals.md#optimizertypetype)
- [PermissionType](./literals.md#permissiontype)
- [PermissionTypeType](./literals.md#permissiontypetype)
- [QueryStateStringType](./literals.md#querystatestringtype)
- [ResourceShareTypeType](./literals.md#resourcesharetypetype)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [SearchDatabasesByLFTagsPaginatorName](./literals.md#searchdatabasesbylftagspaginatorname)
- [SearchTablesByLFTagsPaginatorName](./literals.md#searchtablesbylftagspaginatorname)
- [TransactionStatusFilterType](./literals.md#transactionstatusfiltertype)
- [TransactionStatusType](./literals.md#transactionstatustype)
- [TransactionTypeType](./literals.md#transactiontypetype)
- [LakeFormationServiceName](./literals.md#lakeformationservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [LFTagPairTypeDef](./type_defs.md#lftagpairtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AddObjectInputTypeDef](./type_defs.md#addobjectinputtypedef)
- [AssumeDecoratedRoleWithSAMLRequestRequestTypeDef](./type_defs.md#assumedecoratedrolewithsamlrequestrequesttypedef)
- [AuditContextTypeDef](./type_defs.md#auditcontexttypedef)
- [ErrorDetailTypeDef](./type_defs.md#errordetailtypedef)
- [DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef)
- [CancelTransactionRequestRequestTypeDef](./type_defs.md#canceltransactionrequestrequesttypedef)
- [LFTagPairPaginatorTypeDef](./type_defs.md#lftagpairpaginatortypedef)
- [ColumnWildcardPaginatorTypeDef](./type_defs.md#columnwildcardpaginatortypedef)
- [ColumnWildcardTypeDef](./type_defs.md#columnwildcardtypedef)
- [CommitTransactionRequestRequestTypeDef](./type_defs.md#committransactionrequestrequesttypedef)
- [CreateLFTagRequestRequestTypeDef](./type_defs.md#createlftagrequestrequesttypedef)
- [ExternalFilteringConfigurationTypeDef](./type_defs.md#externalfilteringconfigurationtypedef)
- [RowFilterPaginatorTypeDef](./type_defs.md#rowfilterpaginatortypedef)
- [DataCellsFilterResourceTypeDef](./type_defs.md#datacellsfilterresourcetypedef)
- [RowFilterTypeDef](./type_defs.md#rowfiltertypedef)
- [DataLocationResourceTypeDef](./type_defs.md#datalocationresourcetypedef)
- [DatabaseResourceTypeDef](./type_defs.md#databaseresourcetypedef)
- [DeleteDataCellsFilterRequestRequestTypeDef](./type_defs.md#deletedatacellsfilterrequestrequesttypedef)
- [DeleteLFTagRequestRequestTypeDef](./type_defs.md#deletelftagrequestrequesttypedef)
- [DeleteLakeFormationIdentityCenterConfigurationRequestRequestTypeDef](./type_defs.md#deletelakeformationidentitycenterconfigurationrequestrequesttypedef)
- [DeleteObjectInputTypeDef](./type_defs.md#deleteobjectinputtypedef)
- [VirtualObjectTypeDef](./type_defs.md#virtualobjecttypedef)
- [DeregisterResourceRequestRequestTypeDef](./type_defs.md#deregisterresourcerequestrequesttypedef)
- [DescribeLakeFormationIdentityCenterConfigurationRequestRequestTypeDef](./type_defs.md#describelakeformationidentitycenterconfigurationrequestrequesttypedef)
- [DescribeResourceRequestRequestTypeDef](./type_defs.md#describeresourcerequestrequesttypedef)
- [ResourceInfoTypeDef](./type_defs.md#resourceinfotypedef)
- [DescribeTransactionRequestRequestTypeDef](./type_defs.md#describetransactionrequestrequesttypedef)
- [TransactionDescriptionTypeDef](./type_defs.md#transactiondescriptiontypedef)
- [DetailsMapTypeDef](./type_defs.md#detailsmaptypedef)
- [ExecutionStatisticsTypeDef](./type_defs.md#executionstatisticstypedef)
- [ExtendTransactionRequestRequestTypeDef](./type_defs.md#extendtransactionrequestrequesttypedef)
- [FilterConditionTypeDef](./type_defs.md#filterconditiontypedef)
- [GetDataCellsFilterRequestRequestTypeDef](./type_defs.md#getdatacellsfilterrequestrequesttypedef)
- [GetDataLakeSettingsRequestRequestTypeDef](./type_defs.md#getdatalakesettingsrequestrequesttypedef)
- [GetEffectivePermissionsForPathRequestRequestTypeDef](./type_defs.md#geteffectivepermissionsforpathrequestrequesttypedef)
- [GetLFTagRequestRequestTypeDef](./type_defs.md#getlftagrequestrequesttypedef)
- [GetQueryStateRequestRequestTypeDef](./type_defs.md#getquerystaterequestrequesttypedef)
- [GetQueryStatisticsRequestRequestTypeDef](./type_defs.md#getquerystatisticsrequestrequesttypedef)
- [PlanningStatisticsTypeDef](./type_defs.md#planningstatisticstypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [PartitionValueListTypeDef](./type_defs.md#partitionvaluelisttypedef)
- [GetWorkUnitResultsRequestRequestTypeDef](./type_defs.md#getworkunitresultsrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetWorkUnitsRequestRequestTypeDef](./type_defs.md#getworkunitsrequestrequesttypedef)
- [WorkUnitRangeTypeDef](./type_defs.md#workunitrangetypedef)
- [LFTagKeyResourceTypeDef](./type_defs.md#lftagkeyresourcetypedef)
- [LFTagTypeDef](./type_defs.md#lftagtypedef)
- [TableResourceTypeDef](./type_defs.md#tableresourcetypedef)
- [ListLFTagsRequestRequestTypeDef](./type_defs.md#listlftagsrequestrequesttypedef)
- [ListTableStorageOptimizersRequestRequestTypeDef](./type_defs.md#listtablestorageoptimizersrequestrequesttypedef)
- [StorageOptimizerTypeDef](./type_defs.md#storageoptimizertypedef)
- [ListTransactionsRequestRequestTypeDef](./type_defs.md#listtransactionsrequestrequesttypedef)
- [TableObjectTypeDef](./type_defs.md#tableobjecttypedef)
- [RegisterResourceRequestRequestTypeDef](./type_defs.md#registerresourcerequestrequesttypedef)
- [StartTransactionRequestRequestTypeDef](./type_defs.md#starttransactionrequestrequesttypedef)
- [UpdateLFTagRequestRequestTypeDef](./type_defs.md#updatelftagrequestrequesttypedef)
- [UpdateResourceRequestRequestTypeDef](./type_defs.md#updateresourcerequestrequesttypedef)
- [UpdateTableStorageOptimizerRequestRequestTypeDef](./type_defs.md#updatetablestorageoptimizerrequestrequesttypedef)
- [ColumnLFTagTypeDef](./type_defs.md#columnlftagtypedef)
- [AssumeDecoratedRoleWithSAMLResponseTypeDef](./type_defs.md#assumedecoratedrolewithsamlresponsetypedef)
- [CommitTransactionResponseTypeDef](./type_defs.md#committransactionresponsetypedef)
- [CreateLakeFormationIdentityCenterConfigurationResponseTypeDef](./type_defs.md#createlakeformationidentitycenterconfigurationresponsetypedef)
- [GetLFTagResponseTypeDef](./type_defs.md#getlftagresponsetypedef)
- [GetQueryStateResponseTypeDef](./type_defs.md#getquerystateresponsetypedef)
- [GetTemporaryGluePartitionCredentialsResponseTypeDef](./type_defs.md#gettemporarygluepartitioncredentialsresponsetypedef)
- [GetTemporaryGlueTableCredentialsResponseTypeDef](./type_defs.md#gettemporarygluetablecredentialsresponsetypedef)
- [GetWorkUnitResultsResponseTypeDef](./type_defs.md#getworkunitresultsresponsetypedef)
- [ListLFTagsResponseTypeDef](./type_defs.md#listlftagsresponsetypedef)
- [StartQueryPlanningResponseTypeDef](./type_defs.md#startqueryplanningresponsetypedef)
- [StartTransactionResponseTypeDef](./type_defs.md#starttransactionresponsetypedef)
- [UpdateTableStorageOptimizerResponseTypeDef](./type_defs.md#updatetablestorageoptimizerresponsetypedef)
- [LFTagErrorTypeDef](./type_defs.md#lftagerrortypedef)
- [PrincipalPermissionsTypeDef](./type_defs.md#principalpermissionstypedef)
- [ColumnLFTagPaginatorTypeDef](./type_defs.md#columnlftagpaginatortypedef)
- [ListLFTagsResponsePaginatorTypeDef](./type_defs.md#listlftagsresponsepaginatortypedef)
- [TableWithColumnsResourceTypeDef](./type_defs.md#tablewithcolumnsresourcetypedef)
- [CreateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef](./type_defs.md#createlakeformationidentitycenterconfigurationrequestrequesttypedef)
- [DescribeLakeFormationIdentityCenterConfigurationResponseTypeDef](./type_defs.md#describelakeformationidentitycenterconfigurationresponsetypedef)
- [UpdateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef](./type_defs.md#updatelakeformationidentitycenterconfigurationrequestrequesttypedef)
- [DataCellsFilterPaginatorTypeDef](./type_defs.md#datacellsfilterpaginatortypedef)
- [DataCellsFilterTypeDef](./type_defs.md#datacellsfiltertypedef)
- [TaggedDatabasePaginatorTypeDef](./type_defs.md#taggeddatabasepaginatortypedef)
- [TaggedDatabaseTypeDef](./type_defs.md#taggeddatabasetypedef)
- [WriteOperationTypeDef](./type_defs.md#writeoperationtypedef)
- [DeleteObjectsOnCancelRequestRequestTypeDef](./type_defs.md#deleteobjectsoncancelrequestrequesttypedef)
- [DescribeResourceResponseTypeDef](./type_defs.md#describeresourceresponsetypedef)
- [ListResourcesResponseTypeDef](./type_defs.md#listresourcesresponsetypedef)
- [DescribeTransactionResponseTypeDef](./type_defs.md#describetransactionresponsetypedef)
- [ListTransactionsResponseTypeDef](./type_defs.md#listtransactionsresponsetypedef)
- [ListResourcesRequestRequestTypeDef](./type_defs.md#listresourcesrequestrequesttypedef)
- [GetQueryStatisticsResponseTypeDef](./type_defs.md#getquerystatisticsresponsetypedef)
- [GetTableObjectsRequestRequestTypeDef](./type_defs.md#gettableobjectsrequestrequesttypedef)
- [QueryPlanningContextTypeDef](./type_defs.md#queryplanningcontexttypedef)
- [QuerySessionContextTypeDef](./type_defs.md#querysessioncontexttypedef)
- [GetTemporaryGluePartitionCredentialsRequestRequestTypeDef](./type_defs.md#gettemporarygluepartitioncredentialsrequestrequesttypedef)
- [GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef](./type_defs.md#getworkunitsrequestgetworkunitspaginatetypedef)
- [ListLFTagsRequestListLFTagsPaginateTypeDef](./type_defs.md#listlftagsrequestlistlftagspaginatetypedef)
- [GetWorkUnitsResponseTypeDef](./type_defs.md#getworkunitsresponsetypedef)
- [LFTagPolicyResourceTypeDef](./type_defs.md#lftagpolicyresourcetypedef)
- [SearchDatabasesByLFTagsRequestRequestTypeDef](./type_defs.md#searchdatabasesbylftagsrequestrequesttypedef)
- [SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef](./type_defs.md#searchdatabasesbylftagsrequestsearchdatabasesbylftagspaginatetypedef)
- [SearchTablesByLFTagsRequestRequestTypeDef](./type_defs.md#searchtablesbylftagsrequestrequesttypedef)
- [SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef](./type_defs.md#searchtablesbylftagsrequestsearchtablesbylftagspaginatetypedef)
- [ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef](./type_defs.md#listdatacellsfilterrequestlistdatacellsfilterpaginatetypedef)
- [ListDataCellsFilterRequestRequestTypeDef](./type_defs.md#listdatacellsfilterrequestrequesttypedef)
- [ListTableStorageOptimizersResponseTypeDef](./type_defs.md#listtablestorageoptimizersresponsetypedef)
- [PartitionObjectsTypeDef](./type_defs.md#partitionobjectstypedef)
- [GetResourceLFTagsResponseTypeDef](./type_defs.md#getresourcelftagsresponsetypedef)
- [TaggedTableTypeDef](./type_defs.md#taggedtabletypedef)
- [AddLFTagsToResourceResponseTypeDef](./type_defs.md#addlftagstoresourceresponsetypedef)
- [RemoveLFTagsFromResourceResponseTypeDef](./type_defs.md#removelftagsfromresourceresponsetypedef)
- [DataLakeSettingsTypeDef](./type_defs.md#datalakesettingstypedef)
- [TaggedTablePaginatorTypeDef](./type_defs.md#taggedtablepaginatortypedef)
- [ListDataCellsFilterResponsePaginatorTypeDef](./type_defs.md#listdatacellsfilterresponsepaginatortypedef)
- [CreateDataCellsFilterRequestRequestTypeDef](./type_defs.md#createdatacellsfilterrequestrequesttypedef)
- [GetDataCellsFilterResponseTypeDef](./type_defs.md#getdatacellsfilterresponsetypedef)
- [ListDataCellsFilterResponseTypeDef](./type_defs.md#listdatacellsfilterresponsetypedef)
- [UpdateDataCellsFilterRequestRequestTypeDef](./type_defs.md#updatedatacellsfilterrequestrequesttypedef)
- [SearchDatabasesByLFTagsResponsePaginatorTypeDef](./type_defs.md#searchdatabasesbylftagsresponsepaginatortypedef)
- [SearchDatabasesByLFTagsResponseTypeDef](./type_defs.md#searchdatabasesbylftagsresponsetypedef)
- [UpdateTableObjectsRequestRequestTypeDef](./type_defs.md#updatetableobjectsrequestrequesttypedef)
- [StartQueryPlanningRequestRequestTypeDef](./type_defs.md#startqueryplanningrequestrequesttypedef)
- [GetTemporaryGlueTableCredentialsRequestRequestTypeDef](./type_defs.md#gettemporarygluetablecredentialsrequestrequesttypedef)
- [ResourceTypeDef](./type_defs.md#resourcetypedef)
- [GetTableObjectsResponseTypeDef](./type_defs.md#gettableobjectsresponsetypedef)
- [SearchTablesByLFTagsResponseTypeDef](./type_defs.md#searchtablesbylftagsresponsetypedef)
- [GetDataLakeSettingsResponseTypeDef](./type_defs.md#getdatalakesettingsresponsetypedef)
- [PutDataLakeSettingsRequestRequestTypeDef](./type_defs.md#putdatalakesettingsrequestrequesttypedef)
- [SearchTablesByLFTagsResponsePaginatorTypeDef](./type_defs.md#searchtablesbylftagsresponsepaginatortypedef)
- [AddLFTagsToResourceRequestRequestTypeDef](./type_defs.md#addlftagstoresourcerequestrequesttypedef)
- [BatchPermissionsRequestEntryTypeDef](./type_defs.md#batchpermissionsrequestentrytypedef)
- [CreateLakeFormationOptInRequestRequestTypeDef](./type_defs.md#createlakeformationoptinrequestrequesttypedef)
- [DeleteLakeFormationOptInRequestRequestTypeDef](./type_defs.md#deletelakeformationoptinrequestrequesttypedef)
- [GetResourceLFTagsRequestRequestTypeDef](./type_defs.md#getresourcelftagsrequestrequesttypedef)
- [GrantPermissionsRequestRequestTypeDef](./type_defs.md#grantpermissionsrequestrequesttypedef)
- [LakeFormationOptInsInfoTypeDef](./type_defs.md#lakeformationoptinsinfotypedef)
- [ListLakeFormationOptInsRequestRequestTypeDef](./type_defs.md#listlakeformationoptinsrequestrequesttypedef)
- [ListPermissionsRequestRequestTypeDef](./type_defs.md#listpermissionsrequestrequesttypedef)
- [PrincipalResourcePermissionsTypeDef](./type_defs.md#principalresourcepermissionstypedef)
- [RemoveLFTagsFromResourceRequestRequestTypeDef](./type_defs.md#removelftagsfromresourcerequestrequesttypedef)
- [RevokePermissionsRequestRequestTypeDef](./type_defs.md#revokepermissionsrequestrequesttypedef)
- [BatchGrantPermissionsRequestRequestTypeDef](./type_defs.md#batchgrantpermissionsrequestrequesttypedef)
- [BatchPermissionsFailureEntryTypeDef](./type_defs.md#batchpermissionsfailureentrytypedef)
- [BatchRevokePermissionsRequestRequestTypeDef](./type_defs.md#batchrevokepermissionsrequestrequesttypedef)
- [ListLakeFormationOptInsResponseTypeDef](./type_defs.md#listlakeformationoptinsresponsetypedef)
- [GetEffectivePermissionsForPathResponseTypeDef](./type_defs.md#geteffectivepermissionsforpathresponsetypedef)
- [ListPermissionsResponseTypeDef](./type_defs.md#listpermissionsresponsetypedef)
- [BatchGrantPermissionsResponseTypeDef](./type_defs.md#batchgrantpermissionsresponsetypedef)
- [BatchRevokePermissionsResponseTypeDef](./type_defs.md#batchrevokepermissionsresponsetypedef)

