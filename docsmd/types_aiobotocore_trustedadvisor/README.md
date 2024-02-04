# TrustedAdvisorPublicAPI module

> [Index](../README.md) > TrustedAdvisorPublicAPI


!!! note ""

    Auto-generated documentation for [TrustedAdvisorPublicAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI)
    type annotations stubs module [types-aiobotocore-trustedadvisor](https://pypi.org/project/types-aiobotocore-trustedadvisor/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `TrustedAdvisorPublicAPI` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[trustedadvisor]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[trustedadvisor]'


# standalone installation
python -m pip install types-aiobotocore-trustedadvisor
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-trustedadvisor
```

## Usage

Code samples can be found in [Examples](./usage.md).

## TrustedAdvisorPublicAPIClient

Type annotations and code completion for  `#!python session.client("trustedadvisor")` as [TrustedAdvisorPublicAPIClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client)

```python
# TrustedAdvisorPublicAPIClient usage example

from aioboto3.session import Session

from types_aiobotocore_trustedadvisor.client import TrustedAdvisorPublicAPIClient


session = Session()
async with session.client("trustedadvisor") as client:
    client: TrustedAdvisorPublicAPIClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("trustedadvisor").get_paginator("...")`.

```python
# ListChecksPaginator usage example

from types_aiobotocore_trustedadvisor.paginator import ListChecksPaginator

def get_list_checks_paginator() -> ListChecksPaginator:
    return client.get_paginator("list_checks"))
```

- [ListChecksPaginator](./paginators.md#listcheckspaginator)
- [ListOrganizationRecommendationAccountsPaginator](./paginators.md#listorganizationrecommendationaccountspaginator)
- [ListOrganizationRecommendationResourcesPaginator](./paginators.md#listorganizationrecommendationresourcespaginator)
- [ListOrganizationRecommendationsPaginator](./paginators.md#listorganizationrecommendationspaginator)
- [ListRecommendationResourcesPaginator](./paginators.md#listrecommendationresourcespaginator)
- [ListRecommendationsPaginator](./paginators.md#listrecommendationspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ListChecksPaginatorName usage example

from types_aiobotocore_trustedadvisor.literals import ListChecksPaginatorName

def get_value() -> ListChecksPaginatorName:
    return "list_checks"
```

- [ListChecksPaginatorName](./literals.md#listcheckspaginatorname)
- [ListOrganizationRecommendationAccountsPaginatorName](./literals.md#listorganizationrecommendationaccountspaginatorname)
- [ListOrganizationRecommendationResourcesPaginatorName](./literals.md#listorganizationrecommendationresourcespaginatorname)
- [ListOrganizationRecommendationsPaginatorName](./literals.md#listorganizationrecommendationspaginatorname)
- [ListRecommendationResourcesPaginatorName](./literals.md#listrecommendationresourcespaginatorname)
- [ListRecommendationsPaginatorName](./literals.md#listrecommendationspaginatorname)
- [RecommendationLanguageType](./literals.md#recommendationlanguagetype)
- [RecommendationLifecycleStageType](./literals.md#recommendationlifecyclestagetype)
- [RecommendationPillarType](./literals.md#recommendationpillartype)
- [RecommendationSourceType](./literals.md#recommendationsourcetype)
- [RecommendationStatusType](./literals.md#recommendationstatustype)
- [RecommendationTypeType](./literals.md#recommendationtypetype)
- [ResourceStatusType](./literals.md#resourcestatustype)
- [UpdateRecommendationLifecycleStageReasonCodeType](./literals.md#updaterecommendationlifecyclestagereasoncodetype)
- [UpdateRecommendationLifecycleStageType](./literals.md#updaterecommendationlifecyclestagetype)
- [TrustedAdvisorPublicAPIServiceName](./literals.md#trustedadvisorpublicapiservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccountRecommendationLifecycleSummaryTypeDef](./type_defs.md#accountrecommendationlifecyclesummarytypedef)
- [CheckSummaryTypeDef](./type_defs.md#checksummarytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetOrganizationRecommendationRequestRequestTypeDef](./type_defs.md#getorganizationrecommendationrequestrequesttypedef)
- [GetRecommendationRequestRequestTypeDef](./type_defs.md#getrecommendationrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListChecksRequestRequestTypeDef](./type_defs.md#listchecksrequestrequesttypedef)
- [ListOrganizationRecommendationAccountsRequestRequestTypeDef](./type_defs.md#listorganizationrecommendationaccountsrequestrequesttypedef)
- [ListOrganizationRecommendationResourcesRequestRequestTypeDef](./type_defs.md#listorganizationrecommendationresourcesrequestrequesttypedef)
- [OrganizationRecommendationResourceSummaryTypeDef](./type_defs.md#organizationrecommendationresourcesummarytypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ListRecommendationResourcesRequestRequestTypeDef](./type_defs.md#listrecommendationresourcesrequestrequesttypedef)
- [RecommendationResourceSummaryTypeDef](./type_defs.md#recommendationresourcesummarytypedef)
- [RecommendationResourcesAggregatesTypeDef](./type_defs.md#recommendationresourcesaggregatestypedef)
- [RecommendationCostOptimizingAggregatesTypeDef](./type_defs.md#recommendationcostoptimizingaggregatestypedef)
- [UpdateOrganizationRecommendationLifecycleRequestRequestTypeDef](./type_defs.md#updateorganizationrecommendationlifecyclerequestrequesttypedef)
- [UpdateRecommendationLifecycleRequestRequestTypeDef](./type_defs.md#updaterecommendationlifecyclerequestrequesttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListChecksResponseTypeDef](./type_defs.md#listchecksresponsetypedef)
- [ListOrganizationRecommendationAccountsResponseTypeDef](./type_defs.md#listorganizationrecommendationaccountsresponsetypedef)
- [ListChecksRequestListChecksPaginateTypeDef](./type_defs.md#listchecksrequestlistcheckspaginatetypedef)
- [ListOrganizationRecommendationAccountsRequestListOrganizationRecommendationAccountsPaginateTypeDef](./type_defs.md#listorganizationrecommendationaccountsrequestlistorganizationrecommendationaccountspaginatetypedef)
- [ListOrganizationRecommendationResourcesRequestListOrganizationRecommendationResourcesPaginateTypeDef](./type_defs.md#listorganizationrecommendationresourcesrequestlistorganizationrecommendationresourcespaginatetypedef)
- [ListRecommendationResourcesRequestListRecommendationResourcesPaginateTypeDef](./type_defs.md#listrecommendationresourcesrequestlistrecommendationresourcespaginatetypedef)
- [ListOrganizationRecommendationResourcesResponseTypeDef](./type_defs.md#listorganizationrecommendationresourcesresponsetypedef)
- [ListOrganizationRecommendationsRequestListOrganizationRecommendationsPaginateTypeDef](./type_defs.md#listorganizationrecommendationsrequestlistorganizationrecommendationspaginatetypedef)
- [ListOrganizationRecommendationsRequestRequestTypeDef](./type_defs.md#listorganizationrecommendationsrequestrequesttypedef)
- [ListRecommendationsRequestListRecommendationsPaginateTypeDef](./type_defs.md#listrecommendationsrequestlistrecommendationspaginatetypedef)
- [ListRecommendationsRequestRequestTypeDef](./type_defs.md#listrecommendationsrequestrequesttypedef)
- [ListRecommendationResourcesResponseTypeDef](./type_defs.md#listrecommendationresourcesresponsetypedef)
- [RecommendationPillarSpecificAggregatesTypeDef](./type_defs.md#recommendationpillarspecificaggregatestypedef)
- [OrganizationRecommendationSummaryTypeDef](./type_defs.md#organizationrecommendationsummarytypedef)
- [OrganizationRecommendationTypeDef](./type_defs.md#organizationrecommendationtypedef)
- [RecommendationSummaryTypeDef](./type_defs.md#recommendationsummarytypedef)
- [RecommendationTypeDef](./type_defs.md#recommendationtypedef)
- [ListOrganizationRecommendationsResponseTypeDef](./type_defs.md#listorganizationrecommendationsresponsetypedef)
- [GetOrganizationRecommendationResponseTypeDef](./type_defs.md#getorganizationrecommendationresponsetypedef)
- [ListRecommendationsResponseTypeDef](./type_defs.md#listrecommendationsresponsetypedef)
- [GetRecommendationResponseTypeDef](./type_defs.md#getrecommendationresponsetypedef)

