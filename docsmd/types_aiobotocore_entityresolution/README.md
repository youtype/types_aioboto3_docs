# EntityResolution module

> [Index](../README.md) > EntityResolution


!!! note ""

    Auto-generated documentation for [EntityResolution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
    type annotations stubs module [types-aiobotocore-entityresolution](https://pypi.org/project/types-aiobotocore-entityresolution/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `EntityResolution` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[entityresolution]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[entityresolution]'


# standalone installation
python -m pip install types-aiobotocore-entityresolution
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-entityresolution
```

## Usage

Code samples can be found in [Examples](./usage.md).

## EntityResolutionClient

Type annotations and code completion for  `#!python session.client("entityresolution")` as [EntityResolutionClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client)

```python
# EntityResolutionClient usage example

from aioboto3.session import Session

from types_aiobotocore_entityresolution.client import EntityResolutionClient


session = Session()
async with session.client("entityresolution") as client:
    client: EntityResolutionClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("entityresolution").get_paginator("...")`.

```python
# ListIdMappingJobsPaginator usage example

from types_aiobotocore_entityresolution.paginator import ListIdMappingJobsPaginator

def get_list_id_mapping_jobs_paginator() -> ListIdMappingJobsPaginator:
    return client.get_paginator("list_id_mapping_jobs"))
```

- [ListIdMappingJobsPaginator](./paginators.md#listidmappingjobspaginator)
- [ListIdMappingWorkflowsPaginator](./paginators.md#listidmappingworkflowspaginator)
- [ListMatchingJobsPaginator](./paginators.md#listmatchingjobspaginator)
- [ListMatchingWorkflowsPaginator](./paginators.md#listmatchingworkflowspaginator)
- [ListProviderServicesPaginator](./paginators.md#listproviderservicespaginator)
- [ListSchemaMappingsPaginator](./paginators.md#listschemamappingspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AttributeMatchingModelType usage example

from types_aiobotocore_entityresolution.literals import AttributeMatchingModelType

def get_value() -> AttributeMatchingModelType:
    return "MANY_TO_MANY"
```

- [AttributeMatchingModelType](./literals.md#attributematchingmodeltype)
- [IdMappingTypeType](./literals.md#idmappingtypetype)
- [IncrementalRunTypeType](./literals.md#incrementalruntypetype)
- [JobStatusType](./literals.md#jobstatustype)
- [ListIdMappingJobsPaginatorName](./literals.md#listidmappingjobspaginatorname)
- [ListIdMappingWorkflowsPaginatorName](./literals.md#listidmappingworkflowspaginatorname)
- [ListMatchingJobsPaginatorName](./literals.md#listmatchingjobspaginatorname)
- [ListMatchingWorkflowsPaginatorName](./literals.md#listmatchingworkflowspaginatorname)
- [ListProviderServicesPaginatorName](./literals.md#listproviderservicespaginatorname)
- [ListSchemaMappingsPaginatorName](./literals.md#listschemamappingspaginatorname)
- [ResolutionTypeType](./literals.md#resolutiontypetype)
- [SchemaAttributeTypeType](./literals.md#schemaattributetypetype)
- [ServiceTypeType](./literals.md#servicetypetype)
- [EntityResolutionServiceName](./literals.md#entityresolutionservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [IdMappingWorkflowInputSourceTypeDef](./type_defs.md#idmappingworkflowinputsourcetypedef)
- [IdMappingWorkflowOutputSourceTypeDef](./type_defs.md#idmappingworkflowoutputsourcetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef)
- [InputSourceTypeDef](./type_defs.md#inputsourcetypedef)
- [SchemaInputAttributeTypeDef](./type_defs.md#schemainputattributetypedef)
- [DeleteIdMappingWorkflowInputRequestTypeDef](./type_defs.md#deleteidmappingworkflowinputrequesttypedef)
- [DeleteMatchingWorkflowInputRequestTypeDef](./type_defs.md#deletematchingworkflowinputrequesttypedef)
- [DeleteSchemaMappingInputRequestTypeDef](./type_defs.md#deleteschemamappinginputrequesttypedef)
- [ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef)
- [GetIdMappingJobInputRequestTypeDef](./type_defs.md#getidmappingjobinputrequesttypedef)
- [IdMappingJobMetricsTypeDef](./type_defs.md#idmappingjobmetricstypedef)
- [GetIdMappingWorkflowInputRequestTypeDef](./type_defs.md#getidmappingworkflowinputrequesttypedef)
- [GetMatchIdInputRequestTypeDef](./type_defs.md#getmatchidinputrequesttypedef)
- [GetMatchingJobInputRequestTypeDef](./type_defs.md#getmatchingjobinputrequesttypedef)
- [JobMetricsTypeDef](./type_defs.md#jobmetricstypedef)
- [GetMatchingWorkflowInputRequestTypeDef](./type_defs.md#getmatchingworkflowinputrequesttypedef)
- [GetProviderServiceInputRequestTypeDef](./type_defs.md#getproviderserviceinputrequesttypedef)
- [ProviderIntermediateDataAccessConfigurationTypeDef](./type_defs.md#providerintermediatedataaccessconfigurationtypedef)
- [GetSchemaMappingInputRequestTypeDef](./type_defs.md#getschemamappinginputrequesttypedef)
- [IdMappingWorkflowSummaryTypeDef](./type_defs.md#idmappingworkflowsummarytypedef)
- [IntermediateSourceConfigurationTypeDef](./type_defs.md#intermediatesourceconfigurationtypedef)
- [JobSummaryTypeDef](./type_defs.md#jobsummarytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListIdMappingJobsInputRequestTypeDef](./type_defs.md#listidmappingjobsinputrequesttypedef)
- [ListIdMappingWorkflowsInputRequestTypeDef](./type_defs.md#listidmappingworkflowsinputrequesttypedef)
- [ListMatchingJobsInputRequestTypeDef](./type_defs.md#listmatchingjobsinputrequesttypedef)
- [ListMatchingWorkflowsInputRequestTypeDef](./type_defs.md#listmatchingworkflowsinputrequesttypedef)
- [MatchingWorkflowSummaryTypeDef](./type_defs.md#matchingworkflowsummarytypedef)
- [ListProviderServicesInputRequestTypeDef](./type_defs.md#listproviderservicesinputrequesttypedef)
- [ProviderServiceSummaryTypeDef](./type_defs.md#providerservicesummarytypedef)
- [ListSchemaMappingsInputRequestTypeDef](./type_defs.md#listschemamappingsinputrequesttypedef)
- [SchemaMappingSummaryTypeDef](./type_defs.md#schemamappingsummarytypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [OutputAttributeTypeDef](./type_defs.md#outputattributetypedef)
- [ProviderMarketplaceConfigurationTypeDef](./type_defs.md#providermarketplaceconfigurationtypedef)
- [RuleTypeDef](./type_defs.md#ruletypedef)
- [StartIdMappingJobInputRequestTypeDef](./type_defs.md#startidmappingjobinputrequesttypedef)
- [StartMatchingJobInputRequestTypeDef](./type_defs.md#startmatchingjobinputrequesttypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [DeleteIdMappingWorkflowOutputTypeDef](./type_defs.md#deleteidmappingworkflowoutputtypedef)
- [DeleteMatchingWorkflowOutputTypeDef](./type_defs.md#deletematchingworkflowoutputtypedef)
- [DeleteSchemaMappingOutputTypeDef](./type_defs.md#deleteschemamappingoutputtypedef)
- [GetMatchIdOutputTypeDef](./type_defs.md#getmatchidoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [StartIdMappingJobOutputTypeDef](./type_defs.md#startidmappingjoboutputtypedef)
- [StartMatchingJobOutputTypeDef](./type_defs.md#startmatchingjoboutputtypedef)
- [CreateSchemaMappingInputRequestTypeDef](./type_defs.md#createschemamappinginputrequesttypedef)
- [CreateSchemaMappingOutputTypeDef](./type_defs.md#createschemamappingoutputtypedef)
- [GetSchemaMappingOutputTypeDef](./type_defs.md#getschemamappingoutputtypedef)
- [UpdateSchemaMappingInputRequestTypeDef](./type_defs.md#updateschemamappinginputrequesttypedef)
- [UpdateSchemaMappingOutputTypeDef](./type_defs.md#updateschemamappingoutputtypedef)
- [GetIdMappingJobOutputTypeDef](./type_defs.md#getidmappingjoboutputtypedef)
- [GetMatchingJobOutputTypeDef](./type_defs.md#getmatchingjoboutputtypedef)
- [ListIdMappingWorkflowsOutputTypeDef](./type_defs.md#listidmappingworkflowsoutputtypedef)
- [ProviderPropertiesTypeDef](./type_defs.md#providerpropertiestypedef)
- [ListIdMappingJobsOutputTypeDef](./type_defs.md#listidmappingjobsoutputtypedef)
- [ListMatchingJobsOutputTypeDef](./type_defs.md#listmatchingjobsoutputtypedef)
- [ListIdMappingJobsInputListIdMappingJobsPaginateTypeDef](./type_defs.md#listidmappingjobsinputlistidmappingjobspaginatetypedef)
- [ListIdMappingWorkflowsInputListIdMappingWorkflowsPaginateTypeDef](./type_defs.md#listidmappingworkflowsinputlistidmappingworkflowspaginatetypedef)
- [ListMatchingJobsInputListMatchingJobsPaginateTypeDef](./type_defs.md#listmatchingjobsinputlistmatchingjobspaginatetypedef)
- [ListMatchingWorkflowsInputListMatchingWorkflowsPaginateTypeDef](./type_defs.md#listmatchingworkflowsinputlistmatchingworkflowspaginatetypedef)
- [ListProviderServicesInputListProviderServicesPaginateTypeDef](./type_defs.md#listproviderservicesinputlistproviderservicespaginatetypedef)
- [ListSchemaMappingsInputListSchemaMappingsPaginateTypeDef](./type_defs.md#listschemamappingsinputlistschemamappingspaginatetypedef)
- [ListMatchingWorkflowsOutputTypeDef](./type_defs.md#listmatchingworkflowsoutputtypedef)
- [ListProviderServicesOutputTypeDef](./type_defs.md#listproviderservicesoutputtypedef)
- [ListSchemaMappingsOutputTypeDef](./type_defs.md#listschemamappingsoutputtypedef)
- [OutputSourceTypeDef](./type_defs.md#outputsourcetypedef)
- [ProviderEndpointConfigurationTypeDef](./type_defs.md#providerendpointconfigurationtypedef)
- [RuleBasedPropertiesTypeDef](./type_defs.md#rulebasedpropertiestypedef)
- [IdMappingTechniquesTypeDef](./type_defs.md#idmappingtechniquestypedef)
- [GetProviderServiceOutputTypeDef](./type_defs.md#getproviderserviceoutputtypedef)
- [ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef)
- [CreateIdMappingWorkflowInputRequestTypeDef](./type_defs.md#createidmappingworkflowinputrequesttypedef)
- [CreateIdMappingWorkflowOutputTypeDef](./type_defs.md#createidmappingworkflowoutputtypedef)
- [GetIdMappingWorkflowOutputTypeDef](./type_defs.md#getidmappingworkflowoutputtypedef)
- [UpdateIdMappingWorkflowInputRequestTypeDef](./type_defs.md#updateidmappingworkflowinputrequesttypedef)
- [UpdateIdMappingWorkflowOutputTypeDef](./type_defs.md#updateidmappingworkflowoutputtypedef)
- [CreateMatchingWorkflowInputRequestTypeDef](./type_defs.md#creatematchingworkflowinputrequesttypedef)
- [CreateMatchingWorkflowOutputTypeDef](./type_defs.md#creatematchingworkflowoutputtypedef)
- [GetMatchingWorkflowOutputTypeDef](./type_defs.md#getmatchingworkflowoutputtypedef)
- [UpdateMatchingWorkflowInputRequestTypeDef](./type_defs.md#updatematchingworkflowinputrequesttypedef)
- [UpdateMatchingWorkflowOutputTypeDef](./type_defs.md#updatematchingworkflowoutputtypedef)

