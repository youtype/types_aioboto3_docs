# BillingConductor module

> [Index](../README.md) > BillingConductor


!!! note ""

    Auto-generated documentation for [BillingConductor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#billingconductor)
    type annotations stubs module [types-aiobotocore-billingconductor](https://pypi.org/project/types-aiobotocore-billingconductor/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `BillingConductor` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `BillingConductor` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[billingconductor]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[billingconductor]'

# standalone installation
python -m pip install types-aiobotocore-billingconductor
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-billingconductor
```

## Usage

Code samples can be found in [Examples](./usage.md).

## BillingConductorClient

Type annotations and code completion for  `#!python session.client("billingconductor")` as [BillingConductorClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client)

```python
# BillingConductorClient usage example

from aioboto3.session import Session

from types_aiobotocore_billingconductor.client import BillingConductorClient


session = Session()
async with session.client("billingconductor") as client:
    client: BillingConductorClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("billingconductor").get_paginator("...")`.

```python
# ListAccountAssociationsPaginator usage example

from types_aiobotocore_billingconductor.paginator import ListAccountAssociationsPaginator

def get_list_account_associations_paginator() -> ListAccountAssociationsPaginator:
    return client.get_paginator("list_account_associations"))
```

- [ListAccountAssociationsPaginator](./paginators.md#listaccountassociationspaginator)
- [ListBillingGroupCostReportsPaginator](./paginators.md#listbillinggroupcostreportspaginator)
- [ListBillingGroupsPaginator](./paginators.md#listbillinggroupspaginator)
- [ListCustomLineItemVersionsPaginator](./paginators.md#listcustomlineitemversionspaginator)
- [ListCustomLineItemsPaginator](./paginators.md#listcustomlineitemspaginator)
- [ListPricingPlansAssociatedWithPricingRulePaginator](./paginators.md#listpricingplansassociatedwithpricingrulepaginator)
- [ListPricingPlansPaginator](./paginators.md#listpricingplanspaginator)
- [ListPricingRulesAssociatedToPricingPlanPaginator](./paginators.md#listpricingrulesassociatedtopricingplanpaginator)
- [ListPricingRulesPaginator](./paginators.md#listpricingrulespaginator)
- [ListResourcesAssociatedToCustomLineItemPaginator](./paginators.md#listresourcesassociatedtocustomlineitempaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AssociateResourceErrorReasonType usage example

from types_aiobotocore_billingconductor.literals import AssociateResourceErrorReasonType

def get_value() -> AssociateResourceErrorReasonType:
    return "ILLEGAL_CUSTOMLINEITEM"
```

- [AssociateResourceErrorReasonType](./literals.md#associateresourceerrorreasontype)
- [BillingGroupStatusType](./literals.md#billinggroupstatustype)
- [CurrencyCodeType](./literals.md#currencycodetype)
- [CustomLineItemRelationshipType](./literals.md#customlineitemrelationshiptype)
- [CustomLineItemTypeType](./literals.md#customlineitemtypetype)
- [GroupByAttributeNameType](./literals.md#groupbyattributenametype)
- [LineItemFilterAttributeNameType](./literals.md#lineitemfilterattributenametype)
- [LineItemFilterValueType](./literals.md#lineitemfiltervaluetype)
- [ListAccountAssociationsPaginatorName](./literals.md#listaccountassociationspaginatorname)
- [ListBillingGroupCostReportsPaginatorName](./literals.md#listbillinggroupcostreportspaginatorname)
- [ListBillingGroupsPaginatorName](./literals.md#listbillinggroupspaginatorname)
- [ListCustomLineItemVersionsPaginatorName](./literals.md#listcustomlineitemversionspaginatorname)
- [ListCustomLineItemsPaginatorName](./literals.md#listcustomlineitemspaginatorname)
- [ListPricingPlansAssociatedWithPricingRulePaginatorName](./literals.md#listpricingplansassociatedwithpricingrulepaginatorname)
- [ListPricingPlansPaginatorName](./literals.md#listpricingplanspaginatorname)
- [ListPricingRulesAssociatedToPricingPlanPaginatorName](./literals.md#listpricingrulesassociatedtopricingplanpaginatorname)
- [ListPricingRulesPaginatorName](./literals.md#listpricingrulespaginatorname)
- [ListResourcesAssociatedToCustomLineItemPaginatorName](./literals.md#listresourcesassociatedtocustomlineitempaginatorname)
- [MatchOptionType](./literals.md#matchoptiontype)
- [PricingRuleScopeType](./literals.md#pricingrulescopetype)
- [PricingRuleTypeType](./literals.md#pricingruletypetype)
- [BillingConductorServiceName](./literals.md#billingconductorservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccountAssociationsListElementTypeDef](./type_defs.md#accountassociationslistelementtypedef)
- [AccountGroupingTypeDef](./type_defs.md#accountgroupingtypedef)
- [AssociateAccountsInputRequestTypeDef](./type_defs.md#associateaccountsinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AssociatePricingRulesInputRequestTypeDef](./type_defs.md#associatepricingrulesinputrequesttypedef)
- [AssociateResourceErrorTypeDef](./type_defs.md#associateresourceerrortypedef)
- [AttributeTypeDef](./type_defs.md#attributetypedef)
- [CustomLineItemBillingPeriodRangeTypeDef](./type_defs.md#customlineitembillingperiodrangetypedef)
- [BillingGroupCostReportElementTypeDef](./type_defs.md#billinggroupcostreportelementtypedef)
- [ComputationPreferenceTypeDef](./type_defs.md#computationpreferencetypedef)
- [ListBillingGroupAccountGroupingTypeDef](./type_defs.md#listbillinggroupaccountgroupingtypedef)
- [BillingPeriodRangeTypeDef](./type_defs.md#billingperiodrangetypedef)
- [CreateFreeTierConfigTypeDef](./type_defs.md#createfreetierconfigtypedef)
- [CreatePricingPlanInputRequestTypeDef](./type_defs.md#createpricingplaninputrequesttypedef)
- [CustomLineItemFlatChargeDetailsTypeDef](./type_defs.md#customlineitemflatchargedetailstypedef)
- [CustomLineItemPercentageChargeDetailsTypeDef](./type_defs.md#customlineitempercentagechargedetailstypedef)
- [DeleteBillingGroupInputRequestTypeDef](./type_defs.md#deletebillinggroupinputrequesttypedef)
- [DeletePricingPlanInputRequestTypeDef](./type_defs.md#deletepricingplaninputrequesttypedef)
- [DeletePricingRuleInputRequestTypeDef](./type_defs.md#deletepricingruleinputrequesttypedef)
- [DisassociateAccountsInputRequestTypeDef](./type_defs.md#disassociateaccountsinputrequesttypedef)
- [DisassociatePricingRulesInputRequestTypeDef](./type_defs.md#disassociatepricingrulesinputrequesttypedef)
- [FreeTierConfigTypeDef](./type_defs.md#freetierconfigtypedef)
- [LineItemFilterOutputTypeDef](./type_defs.md#lineitemfilteroutputtypedef)
- [LineItemFilterTypeDef](./type_defs.md#lineitemfiltertypedef)
- [ListAccountAssociationsFilterTypeDef](./type_defs.md#listaccountassociationsfiltertypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListBillingGroupCostReportsFilterTypeDef](./type_defs.md#listbillinggroupcostreportsfiltertypedef)
- [ListBillingGroupsFilterTypeDef](./type_defs.md#listbillinggroupsfiltertypedef)
- [ListCustomLineItemFlatChargeDetailsTypeDef](./type_defs.md#listcustomlineitemflatchargedetailstypedef)
- [ListCustomLineItemPercentageChargeDetailsTypeDef](./type_defs.md#listcustomlineitempercentagechargedetailstypedef)
- [ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef](./type_defs.md#listcustomlineitemversionsbillingperiodrangefiltertypedef)
- [ListCustomLineItemsFilterTypeDef](./type_defs.md#listcustomlineitemsfiltertypedef)
- [ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef](./type_defs.md#listpricingplansassociatedwithpricingruleinputrequesttypedef)
- [ListPricingPlansFilterTypeDef](./type_defs.md#listpricingplansfiltertypedef)
- [PricingPlanListElementTypeDef](./type_defs.md#pricingplanlistelementtypedef)
- [ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef](./type_defs.md#listpricingrulesassociatedtopricingplaninputrequesttypedef)
- [ListPricingRulesFilterTypeDef](./type_defs.md#listpricingrulesfiltertypedef)
- [ListResourcesAssociatedToCustomLineItemFilterTypeDef](./type_defs.md#listresourcesassociatedtocustomlineitemfiltertypedef)
- [ListResourcesAssociatedToCustomLineItemResponseElementTypeDef](./type_defs.md#listresourcesassociatedtocustomlineitemresponseelementtypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateBillingGroupAccountGroupingTypeDef](./type_defs.md#updatebillinggroupaccountgroupingtypedef)
- [UpdateCustomLineItemFlatChargeDetailsTypeDef](./type_defs.md#updatecustomlineitemflatchargedetailstypedef)
- [UpdateCustomLineItemPercentageChargeDetailsTypeDef](./type_defs.md#updatecustomlineitempercentagechargedetailstypedef)
- [UpdateFreeTierConfigTypeDef](./type_defs.md#updatefreetierconfigtypedef)
- [UpdatePricingPlanInputRequestTypeDef](./type_defs.md#updatepricingplaninputrequesttypedef)
- [AssociateAccountsOutputTypeDef](./type_defs.md#associateaccountsoutputtypedef)
- [AssociatePricingRulesOutputTypeDef](./type_defs.md#associatepricingrulesoutputtypedef)
- [CreateBillingGroupOutputTypeDef](./type_defs.md#createbillinggroupoutputtypedef)
- [CreateCustomLineItemOutputTypeDef](./type_defs.md#createcustomlineitemoutputtypedef)
- [CreatePricingPlanOutputTypeDef](./type_defs.md#createpricingplanoutputtypedef)
- [CreatePricingRuleOutputTypeDef](./type_defs.md#createpricingruleoutputtypedef)
- [DeleteBillingGroupOutputTypeDef](./type_defs.md#deletebillinggroupoutputtypedef)
- [DeleteCustomLineItemOutputTypeDef](./type_defs.md#deletecustomlineitemoutputtypedef)
- [DeletePricingPlanOutputTypeDef](./type_defs.md#deletepricingplanoutputtypedef)
- [DeletePricingRuleOutputTypeDef](./type_defs.md#deletepricingruleoutputtypedef)
- [DisassociateAccountsOutputTypeDef](./type_defs.md#disassociateaccountsoutputtypedef)
- [DisassociatePricingRulesOutputTypeDef](./type_defs.md#disassociatepricingrulesoutputtypedef)
- [ListAccountAssociationsOutputTypeDef](./type_defs.md#listaccountassociationsoutputtypedef)
- [ListPricingPlansAssociatedWithPricingRuleOutputTypeDef](./type_defs.md#listpricingplansassociatedwithpricingruleoutputtypedef)
- [ListPricingRulesAssociatedToPricingPlanOutputTypeDef](./type_defs.md#listpricingrulesassociatedtopricingplanoutputtypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdatePricingPlanOutputTypeDef](./type_defs.md#updatepricingplanoutputtypedef)
- [AssociateResourceResponseElementTypeDef](./type_defs.md#associateresourceresponseelementtypedef)
- [DisassociateResourceResponseElementTypeDef](./type_defs.md#disassociateresourceresponseelementtypedef)
- [BillingGroupCostReportResultElementTypeDef](./type_defs.md#billinggroupcostreportresultelementtypedef)
- [BatchAssociateResourcesToCustomLineItemInputRequestTypeDef](./type_defs.md#batchassociateresourcestocustomlineiteminputrequesttypedef)
- [BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef](./type_defs.md#batchdisassociateresourcesfromcustomlineiteminputrequesttypedef)
- [DeleteCustomLineItemInputRequestTypeDef](./type_defs.md#deletecustomlineiteminputrequesttypedef)
- [ListBillingGroupCostReportsOutputTypeDef](./type_defs.md#listbillinggroupcostreportsoutputtypedef)
- [CreateBillingGroupInputRequestTypeDef](./type_defs.md#createbillinggroupinputrequesttypedef)
- [BillingGroupListElementTypeDef](./type_defs.md#billinggrouplistelementtypedef)
- [GetBillingGroupCostReportInputRequestTypeDef](./type_defs.md#getbillinggroupcostreportinputrequesttypedef)
- [CreateTieringInputTypeDef](./type_defs.md#createtieringinputtypedef)
- [TieringTypeDef](./type_defs.md#tieringtypedef)
- [LineItemFilterUnionTypeDef](./type_defs.md#lineitemfilteruniontypedef)
- [ListAccountAssociationsInputRequestTypeDef](./type_defs.md#listaccountassociationsinputrequesttypedef)
- [ListAccountAssociationsInputPaginateTypeDef](./type_defs.md#listaccountassociationsinputpaginatetypedef)
- [ListPricingPlansAssociatedWithPricingRuleInputPaginateTypeDef](./type_defs.md#listpricingplansassociatedwithpricingruleinputpaginatetypedef)
- [ListPricingRulesAssociatedToPricingPlanInputPaginateTypeDef](./type_defs.md#listpricingrulesassociatedtopricingplaninputpaginatetypedef)
- [ListBillingGroupCostReportsInputPaginateTypeDef](./type_defs.md#listbillinggroupcostreportsinputpaginatetypedef)
- [ListBillingGroupCostReportsInputRequestTypeDef](./type_defs.md#listbillinggroupcostreportsinputrequesttypedef)
- [ListBillingGroupsInputPaginateTypeDef](./type_defs.md#listbillinggroupsinputpaginatetypedef)
- [ListBillingGroupsInputRequestTypeDef](./type_defs.md#listbillinggroupsinputrequesttypedef)
- [ListCustomLineItemChargeDetailsTypeDef](./type_defs.md#listcustomlineitemchargedetailstypedef)
- [ListCustomLineItemVersionsFilterTypeDef](./type_defs.md#listcustomlineitemversionsfiltertypedef)
- [ListCustomLineItemsInputPaginateTypeDef](./type_defs.md#listcustomlineitemsinputpaginatetypedef)
- [ListCustomLineItemsInputRequestTypeDef](./type_defs.md#listcustomlineitemsinputrequesttypedef)
- [ListPricingPlansInputPaginateTypeDef](./type_defs.md#listpricingplansinputpaginatetypedef)
- [ListPricingPlansInputRequestTypeDef](./type_defs.md#listpricingplansinputrequesttypedef)
- [ListPricingPlansOutputTypeDef](./type_defs.md#listpricingplansoutputtypedef)
- [ListPricingRulesInputPaginateTypeDef](./type_defs.md#listpricingrulesinputpaginatetypedef)
- [ListPricingRulesInputRequestTypeDef](./type_defs.md#listpricingrulesinputrequesttypedef)
- [ListResourcesAssociatedToCustomLineItemInputPaginateTypeDef](./type_defs.md#listresourcesassociatedtocustomlineiteminputpaginatetypedef)
- [ListResourcesAssociatedToCustomLineItemInputRequestTypeDef](./type_defs.md#listresourcesassociatedtocustomlineiteminputrequesttypedef)
- [ListResourcesAssociatedToCustomLineItemOutputTypeDef](./type_defs.md#listresourcesassociatedtocustomlineitemoutputtypedef)
- [UpdateBillingGroupInputRequestTypeDef](./type_defs.md#updatebillinggroupinputrequesttypedef)
- [UpdateBillingGroupOutputTypeDef](./type_defs.md#updatebillinggroupoutputtypedef)
- [UpdateTieringInputTypeDef](./type_defs.md#updatetieringinputtypedef)
- [BatchAssociateResourcesToCustomLineItemOutputTypeDef](./type_defs.md#batchassociateresourcestocustomlineitemoutputtypedef)
- [BatchDisassociateResourcesFromCustomLineItemOutputTypeDef](./type_defs.md#batchdisassociateresourcesfromcustomlineitemoutputtypedef)
- [GetBillingGroupCostReportOutputTypeDef](./type_defs.md#getbillinggroupcostreportoutputtypedef)
- [ListBillingGroupsOutputTypeDef](./type_defs.md#listbillinggroupsoutputtypedef)
- [CreatePricingRuleInputRequestTypeDef](./type_defs.md#createpricingruleinputrequesttypedef)
- [PricingRuleListElementTypeDef](./type_defs.md#pricingrulelistelementtypedef)
- [CustomLineItemChargeDetailsTypeDef](./type_defs.md#customlineitemchargedetailstypedef)
- [UpdateCustomLineItemChargeDetailsTypeDef](./type_defs.md#updatecustomlineitemchargedetailstypedef)
- [CustomLineItemListElementTypeDef](./type_defs.md#customlineitemlistelementtypedef)
- [CustomLineItemVersionListElementTypeDef](./type_defs.md#customlineitemversionlistelementtypedef)
- [UpdateCustomLineItemOutputTypeDef](./type_defs.md#updatecustomlineitemoutputtypedef)
- [ListCustomLineItemVersionsInputPaginateTypeDef](./type_defs.md#listcustomlineitemversionsinputpaginatetypedef)
- [ListCustomLineItemVersionsInputRequestTypeDef](./type_defs.md#listcustomlineitemversionsinputrequesttypedef)
- [UpdatePricingRuleInputRequestTypeDef](./type_defs.md#updatepricingruleinputrequesttypedef)
- [UpdatePricingRuleOutputTypeDef](./type_defs.md#updatepricingruleoutputtypedef)
- [ListPricingRulesOutputTypeDef](./type_defs.md#listpricingrulesoutputtypedef)
- [CreateCustomLineItemInputRequestTypeDef](./type_defs.md#createcustomlineiteminputrequesttypedef)
- [UpdateCustomLineItemInputRequestTypeDef](./type_defs.md#updatecustomlineiteminputrequesttypedef)
- [ListCustomLineItemsOutputTypeDef](./type_defs.md#listcustomlineitemsoutputtypedef)
- [ListCustomLineItemVersionsOutputTypeDef](./type_defs.md#listcustomlineitemversionsoutputtypedef)
