# ConnectCases module

> [Index](../README.md) > ConnectCases


!!! note ""

    Auto-generated documentation for [ConnectCases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
    type annotations stubs module [types-aiobotocore-connectcases](https://pypi.org/project/types-aiobotocore-connectcases/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `ConnectCases` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[connectcases]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[connectcases]'


# standalone installation
python -m pip install types-aiobotocore-connectcases
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-connectcases
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ConnectCasesClient

Type annotations and code completion for  `#!python session.client("connectcases")` as [ConnectCasesClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client)

```python
# ConnectCasesClient usage example

from aioboto3.session import Session

from types_aiobotocore_connectcases.client import ConnectCasesClient


session = Session()
async with session.client("connectcases") as client:
    client: ConnectCasesClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("connectcases").get_paginator("...")`.

```python
# SearchCasesPaginator usage example

from types_aiobotocore_connectcases.paginator import SearchCasesPaginator

def get_search_cases_paginator() -> SearchCasesPaginator:
    return client.get_paginator("search_cases"))
```

- [SearchCasesPaginator](./paginators.md#searchcasespaginator)
- [SearchRelatedItemsPaginator](./paginators.md#searchrelateditemspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AuditEventTypeType usage example

from types_aiobotocore_connectcases.literals import AuditEventTypeType

def get_value() -> AuditEventTypeType:
    return "Case.Created"
```

- [AuditEventTypeType](./literals.md#auditeventtypetype)
- [CommentBodyTextTypeType](./literals.md#commentbodytexttypetype)
- [DomainStatusType](./literals.md#domainstatustype)
- [FieldNamespaceType](./literals.md#fieldnamespacetype)
- [FieldTypeType](./literals.md#fieldtypetype)
- [OrderType](./literals.md#ordertype)
- [RelatedItemTypeType](./literals.md#relateditemtypetype)
- [SearchCasesPaginatorName](./literals.md#searchcasespaginatorname)
- [SearchRelatedItemsPaginatorName](./literals.md#searchrelateditemspaginatorname)
- [TemplateStatusType](./literals.md#templatestatustype)
- [ConnectCasesServiceName](./literals.md#connectcasesservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AuditEventFieldValueUnionTypeDef](./type_defs.md#auditeventfieldvalueuniontypedef)
- [UserUnionTypeDef](./type_defs.md#useruniontypedef)
- [FieldIdentifierTypeDef](./type_defs.md#fieldidentifiertypedef)
- [FieldErrorTypeDef](./type_defs.md#fielderrortypedef)
- [GetFieldResponseTypeDef](./type_defs.md#getfieldresponsetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [FieldOptionTypeDef](./type_defs.md#fieldoptiontypedef)
- [FieldOptionErrorTypeDef](./type_defs.md#fieldoptionerrortypedef)
- [CaseSummaryTypeDef](./type_defs.md#casesummarytypedef)
- [CommentContentTypeDef](./type_defs.md#commentcontenttypedef)
- [ContactContentTypeDef](./type_defs.md#contactcontenttypedef)
- [ContactFilterTypeDef](./type_defs.md#contactfiltertypedef)
- [ContactTypeDef](./type_defs.md#contacttypedef)
- [CreateDomainRequestRequestTypeDef](./type_defs.md#createdomainrequestrequesttypedef)
- [CreateFieldRequestRequestTypeDef](./type_defs.md#createfieldrequestrequesttypedef)
- [LayoutConfigurationTypeDef](./type_defs.md#layoutconfigurationtypedef)
- [RequiredFieldTypeDef](./type_defs.md#requiredfieldtypedef)
- [DeleteDomainRequestRequestTypeDef](./type_defs.md#deletedomainrequestrequesttypedef)
- [DomainSummaryTypeDef](./type_defs.md#domainsummarytypedef)
- [RelatedItemEventIncludedDataTypeDef](./type_defs.md#relateditemeventincludeddatatypedef)
- [FieldItemTypeDef](./type_defs.md#fielditemtypedef)
- [FieldSummaryTypeDef](./type_defs.md#fieldsummarytypedef)
- [FieldValueUnionTypeDef](./type_defs.md#fieldvalueuniontypedef)
- [GetCaseAuditEventsRequestRequestTypeDef](./type_defs.md#getcaseauditeventsrequestrequesttypedef)
- [GetCaseEventConfigurationRequestRequestTypeDef](./type_defs.md#getcaseeventconfigurationrequestrequesttypedef)
- [GetDomainRequestRequestTypeDef](./type_defs.md#getdomainrequestrequesttypedef)
- [GetLayoutRequestRequestTypeDef](./type_defs.md#getlayoutrequestrequesttypedef)
- [GetTemplateRequestRequestTypeDef](./type_defs.md#gettemplaterequestrequesttypedef)
- [LayoutSummaryTypeDef](./type_defs.md#layoutsummarytypedef)
- [ListCasesForContactRequestRequestTypeDef](./type_defs.md#listcasesforcontactrequestrequesttypedef)
- [ListDomainsRequestRequestTypeDef](./type_defs.md#listdomainsrequestrequesttypedef)
- [ListFieldOptionsRequestRequestTypeDef](./type_defs.md#listfieldoptionsrequestrequesttypedef)
- [ListFieldsRequestRequestTypeDef](./type_defs.md#listfieldsrequestrequesttypedef)
- [ListLayoutsRequestRequestTypeDef](./type_defs.md#listlayoutsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTemplatesRequestRequestTypeDef](./type_defs.md#listtemplatesrequestrequesttypedef)
- [TemplateSummaryTypeDef](./type_defs.md#templatesummarytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [SortTypeDef](./type_defs.md#sorttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateFieldRequestRequestTypeDef](./type_defs.md#updatefieldrequestrequesttypedef)
- [AuditEventFieldTypeDef](./type_defs.md#auditeventfieldtypedef)
- [AuditEventPerformedByTypeDef](./type_defs.md#auditeventperformedbytypedef)
- [BatchGetFieldRequestRequestTypeDef](./type_defs.md#batchgetfieldrequestrequesttypedef)
- [CaseEventIncludedDataTypeDef](./type_defs.md#caseeventincludeddatatypedef)
- [GetCaseRequestRequestTypeDef](./type_defs.md#getcaserequestrequesttypedef)
- [BatchGetFieldResponseTypeDef](./type_defs.md#batchgetfieldresponsetypedef)
- [CreateCaseResponseTypeDef](./type_defs.md#createcaseresponsetypedef)
- [CreateDomainResponseTypeDef](./type_defs.md#createdomainresponsetypedef)
- [CreateFieldResponseTypeDef](./type_defs.md#createfieldresponsetypedef)
- [CreateLayoutResponseTypeDef](./type_defs.md#createlayoutresponsetypedef)
- [CreateRelatedItemResponseTypeDef](./type_defs.md#createrelateditemresponsetypedef)
- [CreateTemplateResponseTypeDef](./type_defs.md#createtemplateresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetDomainResponseTypeDef](./type_defs.md#getdomainresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [BatchPutFieldOptionsRequestRequestTypeDef](./type_defs.md#batchputfieldoptionsrequestrequesttypedef)
- [ListFieldOptionsResponseTypeDef](./type_defs.md#listfieldoptionsresponsetypedef)
- [BatchPutFieldOptionsResponseTypeDef](./type_defs.md#batchputfieldoptionsresponsetypedef)
- [ListCasesForContactResponseTypeDef](./type_defs.md#listcasesforcontactresponsetypedef)
- [RelatedItemContentTypeDef](./type_defs.md#relateditemcontenttypedef)
- [RelatedItemTypeFilterTypeDef](./type_defs.md#relateditemtypefiltertypedef)
- [RelatedItemInputContentTypeDef](./type_defs.md#relatediteminputcontenttypedef)
- [CreateTemplateRequestRequestTypeDef](./type_defs.md#createtemplaterequestrequesttypedef)
- [GetTemplateResponseTypeDef](./type_defs.md#gettemplateresponsetypedef)
- [UpdateTemplateRequestRequestTypeDef](./type_defs.md#updatetemplaterequestrequesttypedef)
- [ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef)
- [FieldGroupTypeDef](./type_defs.md#fieldgrouptypedef)
- [ListFieldsResponseTypeDef](./type_defs.md#listfieldsresponsetypedef)
- [FieldValueTypeDef](./type_defs.md#fieldvaluetypedef)
- [ListLayoutsResponseTypeDef](./type_defs.md#listlayoutsresponsetypedef)
- [ListTemplatesResponseTypeDef](./type_defs.md#listtemplatesresponsetypedef)
- [SearchCasesRequestRequestTypeDef](./type_defs.md#searchcasesrequestrequesttypedef)
- [AuditEventTypeDef](./type_defs.md#auditeventtypedef)
- [EventIncludedDataTypeDef](./type_defs.md#eventincludeddatatypedef)
- [SearchRelatedItemsResponseItemTypeDef](./type_defs.md#searchrelateditemsresponseitemtypedef)
- [SearchRelatedItemsRequestRequestTypeDef](./type_defs.md#searchrelateditemsrequestrequesttypedef)
- [SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef](./type_defs.md#searchrelateditemsrequestsearchrelateditemspaginatetypedef)
- [CreateRelatedItemRequestRequestTypeDef](./type_defs.md#createrelateditemrequestrequesttypedef)
- [SectionTypeDef](./type_defs.md#sectiontypedef)
- [CreateCaseRequestRequestTypeDef](./type_defs.md#createcaserequestrequesttypedef)
- [FieldFilterTypeDef](./type_defs.md#fieldfiltertypedef)
- [GetCaseResponseTypeDef](./type_defs.md#getcaseresponsetypedef)
- [SearchCasesResponseItemTypeDef](./type_defs.md#searchcasesresponseitemtypedef)
- [UpdateCaseRequestRequestTypeDef](./type_defs.md#updatecaserequestrequesttypedef)
- [GetCaseAuditEventsResponseTypeDef](./type_defs.md#getcaseauditeventsresponsetypedef)
- [EventBridgeConfigurationTypeDef](./type_defs.md#eventbridgeconfigurationtypedef)
- [SearchRelatedItemsResponseTypeDef](./type_defs.md#searchrelateditemsresponsetypedef)
- [LayoutSectionsTypeDef](./type_defs.md#layoutsectionstypedef)
- [CaseFilterTypeDef](./type_defs.md#casefiltertypedef)
- [SearchCasesResponseTypeDef](./type_defs.md#searchcasesresponsetypedef)
- [GetCaseEventConfigurationResponseTypeDef](./type_defs.md#getcaseeventconfigurationresponsetypedef)
- [PutCaseEventConfigurationRequestRequestTypeDef](./type_defs.md#putcaseeventconfigurationrequestrequesttypedef)
- [BasicLayoutTypeDef](./type_defs.md#basiclayouttypedef)
- [SearchCasesRequestSearchCasesPaginateTypeDef](./type_defs.md#searchcasesrequestsearchcasespaginatetypedef)
- [LayoutContentTypeDef](./type_defs.md#layoutcontenttypedef)
- [CreateLayoutRequestRequestTypeDef](./type_defs.md#createlayoutrequestrequesttypedef)
- [GetLayoutResponseTypeDef](./type_defs.md#getlayoutresponsetypedef)
- [UpdateLayoutRequestRequestTypeDef](./type_defs.md#updatelayoutrequestrequesttypedef)

