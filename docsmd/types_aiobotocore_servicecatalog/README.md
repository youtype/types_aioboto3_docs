# ServiceCatalog module

> [Index](../README.md) > ServiceCatalog


!!! note ""

    Auto-generated documentation for [ServiceCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#servicecatalog)
    type annotations stubs module [types-aiobotocore-servicecatalog](https://pypi.org/project/types-aiobotocore-servicecatalog/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `ServiceCatalog` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `ServiceCatalog` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[servicecatalog]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[servicecatalog]'

# standalone installation
python -m pip install types-aiobotocore-servicecatalog
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-servicecatalog
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ServiceCatalogClient

Type annotations and code completion for  `#!python session.client("servicecatalog")` as [ServiceCatalogClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client)

```python
# ServiceCatalogClient usage example

from aioboto3.session import Session

from types_aiobotocore_servicecatalog.client import ServiceCatalogClient


session = Session()
async with session.client("servicecatalog") as client:
    client: ServiceCatalogClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("servicecatalog").get_paginator("...")`.

```python
# ListAcceptedPortfolioSharesPaginator usage example

from types_aiobotocore_servicecatalog.paginator import ListAcceptedPortfolioSharesPaginator

def get_list_accepted_portfolio_shares_paginator() -> ListAcceptedPortfolioSharesPaginator:
    return client.get_paginator("list_accepted_portfolio_shares"))
```

- [ListAcceptedPortfolioSharesPaginator](./paginators.md#listacceptedportfoliosharespaginator)
- [ListConstraintsForPortfolioPaginator](./paginators.md#listconstraintsforportfoliopaginator)
- [ListLaunchPathsPaginator](./paginators.md#listlaunchpathspaginator)
- [ListOrganizationPortfolioAccessPaginator](./paginators.md#listorganizationportfolioaccesspaginator)
- [ListPortfoliosForProductPaginator](./paginators.md#listportfoliosforproductpaginator)
- [ListPortfoliosPaginator](./paginators.md#listportfoliospaginator)
- [ListPrincipalsForPortfolioPaginator](./paginators.md#listprincipalsforportfoliopaginator)
- [ListProvisionedProductPlansPaginator](./paginators.md#listprovisionedproductplanspaginator)
- [ListProvisioningArtifactsForServiceActionPaginator](./paginators.md#listprovisioningartifactsforserviceactionpaginator)
- [ListRecordHistoryPaginator](./paginators.md#listrecordhistorypaginator)
- [ListResourcesForTagOptionPaginator](./paginators.md#listresourcesfortagoptionpaginator)
- [ListServiceActionsForProvisioningArtifactPaginator](./paginators.md#listserviceactionsforprovisioningartifactpaginator)
- [ListServiceActionsPaginator](./paginators.md#listserviceactionspaginator)
- [ListTagOptionsPaginator](./paginators.md#listtagoptionspaginator)
- [ScanProvisionedProductsPaginator](./paginators.md#scanprovisionedproductspaginator)
- [SearchProductsAsAdminPaginator](./paginators.md#searchproductsasadminpaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccessLevelFilterKeyType usage example

from types_aiobotocore_servicecatalog.literals import AccessLevelFilterKeyType

def get_value() -> AccessLevelFilterKeyType:
    return "Account"
```

- [AccessLevelFilterKeyType](./literals.md#accesslevelfilterkeytype)
- [AccessStatusType](./literals.md#accessstatustype)
- [ChangeActionType](./literals.md#changeactiontype)
- [CopyOptionType](./literals.md#copyoptiontype)
- [CopyProductStatusType](./literals.md#copyproductstatustype)
- [DescribePortfolioShareTypeType](./literals.md#describeportfoliosharetypetype)
- [EngineWorkflowStatusType](./literals.md#engineworkflowstatustype)
- [EvaluationTypeType](./literals.md#evaluationtypetype)
- [LastSyncStatusType](./literals.md#lastsyncstatustype)
- [ListAcceptedPortfolioSharesPaginatorName](./literals.md#listacceptedportfoliosharespaginatorname)
- [ListConstraintsForPortfolioPaginatorName](./literals.md#listconstraintsforportfoliopaginatorname)
- [ListLaunchPathsPaginatorName](./literals.md#listlaunchpathspaginatorname)
- [ListOrganizationPortfolioAccessPaginatorName](./literals.md#listorganizationportfolioaccesspaginatorname)
- [ListPortfoliosForProductPaginatorName](./literals.md#listportfoliosforproductpaginatorname)
- [ListPortfoliosPaginatorName](./literals.md#listportfoliospaginatorname)
- [ListPrincipalsForPortfolioPaginatorName](./literals.md#listprincipalsforportfoliopaginatorname)
- [ListProvisionedProductPlansPaginatorName](./literals.md#listprovisionedproductplanspaginatorname)
- [ListProvisioningArtifactsForServiceActionPaginatorName](./literals.md#listprovisioningartifactsforserviceactionpaginatorname)
- [ListRecordHistoryPaginatorName](./literals.md#listrecordhistorypaginatorname)
- [ListResourcesForTagOptionPaginatorName](./literals.md#listresourcesfortagoptionpaginatorname)
- [ListServiceActionsForProvisioningArtifactPaginatorName](./literals.md#listserviceactionsforprovisioningartifactpaginatorname)
- [ListServiceActionsPaginatorName](./literals.md#listserviceactionspaginatorname)
- [ListTagOptionsPaginatorName](./literals.md#listtagoptionspaginatorname)
- [OrganizationNodeTypeType](./literals.md#organizationnodetypetype)
- [PortfolioShareTypeType](./literals.md#portfoliosharetypetype)
- [PrincipalTypeType](./literals.md#principaltypetype)
- [ProductSourceType](./literals.md#productsourcetype)
- [ProductTypeType](./literals.md#producttypetype)
- [ProductViewFilterByType](./literals.md#productviewfilterbytype)
- [ProductViewSortByType](./literals.md#productviewsortbytype)
- [PropertyKeyType](./literals.md#propertykeytype)
- [ProvisionedProductPlanStatusType](./literals.md#provisionedproductplanstatustype)
- [ProvisionedProductPlanTypeType](./literals.md#provisionedproductplantypetype)
- [ProvisionedProductStatusType](./literals.md#provisionedproductstatustype)
- [ProvisionedProductViewFilterByType](./literals.md#provisionedproductviewfilterbytype)
- [ProvisioningArtifactGuidanceType](./literals.md#provisioningartifactguidancetype)
- [ProvisioningArtifactPropertyNameType](./literals.md#provisioningartifactpropertynametype)
- [ProvisioningArtifactTypeType](./literals.md#provisioningartifacttypetype)
- [RecordStatusType](./literals.md#recordstatustype)
- [ReplacementType](./literals.md#replacementtype)
- [RequiresRecreationType](./literals.md#requiresrecreationtype)
- [ResourceAttributeType](./literals.md#resourceattributetype)
- [ScanProvisionedProductsPaginatorName](./literals.md#scanprovisionedproductspaginatorname)
- [SearchProductsAsAdminPaginatorName](./literals.md#searchproductsasadminpaginatorname)
- [ServiceActionAssociationErrorCodeType](./literals.md#serviceactionassociationerrorcodetype)
- [ServiceActionDefinitionKeyType](./literals.md#serviceactiondefinitionkeytype)
- [ServiceActionDefinitionTypeType](./literals.md#serviceactiondefinitiontypetype)
- [ShareStatusType](./literals.md#sharestatustype)
- [SortOrderType](./literals.md#sortordertype)
- [SourceTypeType](./literals.md#sourcetypetype)
- [StackInstanceStatusType](./literals.md#stackinstancestatustype)
- [StackSetOperationTypeType](./literals.md#stacksetoperationtypetype)
- [StatusType](./literals.md#statustype)
- [ServiceCatalogServiceName](./literals.md#servicecatalogservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AcceptPortfolioShareInputRequestTypeDef](./type_defs.md#acceptportfolioshareinputrequesttypedef)
- [AccessLevelFilterTypeDef](./type_defs.md#accesslevelfiltertypedef)
- [AssociateBudgetWithResourceInputRequestTypeDef](./type_defs.md#associatebudgetwithresourceinputrequesttypedef)
- [AssociatePrincipalWithPortfolioInputRequestTypeDef](./type_defs.md#associateprincipalwithportfolioinputrequesttypedef)
- [AssociateProductWithPortfolioInputRequestTypeDef](./type_defs.md#associateproductwithportfolioinputrequesttypedef)
- [AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef](./type_defs.md#associateserviceactionwithprovisioningartifactinputrequesttypedef)
- [AssociateTagOptionWithResourceInputRequestTypeDef](./type_defs.md#associatetagoptionwithresourceinputrequesttypedef)
- [ServiceActionAssociationTypeDef](./type_defs.md#serviceactionassociationtypedef)
- [FailedServiceActionAssociationTypeDef](./type_defs.md#failedserviceactionassociationtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BudgetDetailTypeDef](./type_defs.md#budgetdetailtypedef)
- [CloudWatchDashboardTypeDef](./type_defs.md#cloudwatchdashboardtypedef)
- [CodeStarParametersTypeDef](./type_defs.md#codestarparameterstypedef)
- [ConstraintDetailTypeDef](./type_defs.md#constraintdetailtypedef)
- [ConstraintSummaryTypeDef](./type_defs.md#constraintsummarytypedef)
- [CopyProductInputRequestTypeDef](./type_defs.md#copyproductinputrequesttypedef)
- [CreateConstraintInputRequestTypeDef](./type_defs.md#createconstraintinputrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [PortfolioDetailTypeDef](./type_defs.md#portfoliodetailtypedef)
- [OrganizationNodeTypeDef](./type_defs.md#organizationnodetypedef)
- [ProvisioningArtifactPropertiesTypeDef](./type_defs.md#provisioningartifactpropertiestypedef)
- [ProvisioningArtifactDetailTypeDef](./type_defs.md#provisioningartifactdetailtypedef)
- [UpdateProvisioningParameterTypeDef](./type_defs.md#updateprovisioningparametertypedef)
- [CreateServiceActionInputRequestTypeDef](./type_defs.md#createserviceactioninputrequesttypedef)
- [CreateTagOptionInputRequestTypeDef](./type_defs.md#createtagoptioninputrequesttypedef)
- [TagOptionDetailTypeDef](./type_defs.md#tagoptiondetailtypedef)
- [DeleteConstraintInputRequestTypeDef](./type_defs.md#deleteconstraintinputrequesttypedef)
- [DeletePortfolioInputRequestTypeDef](./type_defs.md#deleteportfolioinputrequesttypedef)
- [DeleteProductInputRequestTypeDef](./type_defs.md#deleteproductinputrequesttypedef)
- [DeleteProvisionedProductPlanInputRequestTypeDef](./type_defs.md#deleteprovisionedproductplaninputrequesttypedef)
- [DeleteProvisioningArtifactInputRequestTypeDef](./type_defs.md#deleteprovisioningartifactinputrequesttypedef)
- [DeleteServiceActionInputRequestTypeDef](./type_defs.md#deleteserviceactioninputrequesttypedef)
- [DeleteTagOptionInputRequestTypeDef](./type_defs.md#deletetagoptioninputrequesttypedef)
- [DescribeConstraintInputRequestTypeDef](./type_defs.md#describeconstraintinputrequesttypedef)
- [DescribeCopyProductStatusInputRequestTypeDef](./type_defs.md#describecopyproductstatusinputrequesttypedef)
- [DescribePortfolioInputRequestTypeDef](./type_defs.md#describeportfolioinputrequesttypedef)
- [DescribePortfolioShareStatusInputRequestTypeDef](./type_defs.md#describeportfoliosharestatusinputrequesttypedef)
- [DescribePortfolioSharesInputRequestTypeDef](./type_defs.md#describeportfoliosharesinputrequesttypedef)
- [PortfolioShareDetailTypeDef](./type_defs.md#portfoliosharedetailtypedef)
- [DescribeProductAsAdminInputRequestTypeDef](./type_defs.md#describeproductasadmininputrequesttypedef)
- [ProvisioningArtifactSummaryTypeDef](./type_defs.md#provisioningartifactsummarytypedef)
- [DescribeProductInputRequestTypeDef](./type_defs.md#describeproductinputrequesttypedef)
- [LaunchPathTypeDef](./type_defs.md#launchpathtypedef)
- [ProductViewSummaryTypeDef](./type_defs.md#productviewsummarytypedef)
- [ProvisioningArtifactTypeDef](./type_defs.md#provisioningartifacttypedef)
- [DescribeProductViewInputRequestTypeDef](./type_defs.md#describeproductviewinputrequesttypedef)
- [DescribeProvisionedProductInputRequestTypeDef](./type_defs.md#describeprovisionedproductinputrequesttypedef)
- [ProvisionedProductDetailTypeDef](./type_defs.md#provisionedproductdetailtypedef)
- [DescribeProvisionedProductPlanInputRequestTypeDef](./type_defs.md#describeprovisionedproductplaninputrequesttypedef)
- [DescribeProvisioningArtifactInputRequestTypeDef](./type_defs.md#describeprovisioningartifactinputrequesttypedef)
- [DescribeProvisioningParametersInputRequestTypeDef](./type_defs.md#describeprovisioningparametersinputrequesttypedef)
- [ProvisioningArtifactOutputTypeDef](./type_defs.md#provisioningartifactoutputtypedef)
- [ProvisioningArtifactPreferencesTypeDef](./type_defs.md#provisioningartifactpreferencestypedef)
- [TagOptionSummaryTypeDef](./type_defs.md#tagoptionsummarytypedef)
- [UsageInstructionTypeDef](./type_defs.md#usageinstructiontypedef)
- [DescribeRecordInputRequestTypeDef](./type_defs.md#describerecordinputrequesttypedef)
- [RecordOutputTypeDef](./type_defs.md#recordoutputtypedef)
- [DescribeServiceActionExecutionParametersInputRequestTypeDef](./type_defs.md#describeserviceactionexecutionparametersinputrequesttypedef)
- [ExecutionParameterTypeDef](./type_defs.md#executionparametertypedef)
- [DescribeServiceActionInputRequestTypeDef](./type_defs.md#describeserviceactioninputrequesttypedef)
- [DescribeTagOptionInputRequestTypeDef](./type_defs.md#describetagoptioninputrequesttypedef)
- [DisassociateBudgetFromResourceInputRequestTypeDef](./type_defs.md#disassociatebudgetfromresourceinputrequesttypedef)
- [DisassociatePrincipalFromPortfolioInputRequestTypeDef](./type_defs.md#disassociateprincipalfromportfolioinputrequesttypedef)
- [DisassociateProductFromPortfolioInputRequestTypeDef](./type_defs.md#disassociateproductfromportfolioinputrequesttypedef)
- [DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef](./type_defs.md#disassociateserviceactionfromprovisioningartifactinputrequesttypedef)
- [DisassociateTagOptionFromResourceInputRequestTypeDef](./type_defs.md#disassociatetagoptionfromresourceinputrequesttypedef)
- [UniqueTagResourceIdentifierTypeDef](./type_defs.md#uniquetagresourceidentifiertypedef)
- [ExecuteProvisionedProductPlanInputRequestTypeDef](./type_defs.md#executeprovisionedproductplaninputrequesttypedef)
- [ExecuteProvisionedProductServiceActionInputRequestTypeDef](./type_defs.md#executeprovisionedproductserviceactioninputrequesttypedef)
- [GetProvisionedProductOutputsInputRequestTypeDef](./type_defs.md#getprovisionedproductoutputsinputrequesttypedef)
- [ImportAsProvisionedProductInputRequestTypeDef](./type_defs.md#importasprovisionedproductinputrequesttypedef)
- [LastSyncTypeDef](./type_defs.md#lastsynctypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAcceptedPortfolioSharesInputRequestTypeDef](./type_defs.md#listacceptedportfoliosharesinputrequesttypedef)
- [ListBudgetsForResourceInputRequestTypeDef](./type_defs.md#listbudgetsforresourceinputrequesttypedef)
- [ListConstraintsForPortfolioInputRequestTypeDef](./type_defs.md#listconstraintsforportfolioinputrequesttypedef)
- [ListLaunchPathsInputRequestTypeDef](./type_defs.md#listlaunchpathsinputrequesttypedef)
- [ListOrganizationPortfolioAccessInputRequestTypeDef](./type_defs.md#listorganizationportfolioaccessinputrequesttypedef)
- [ListPortfolioAccessInputRequestTypeDef](./type_defs.md#listportfolioaccessinputrequesttypedef)
- [ListPortfoliosForProductInputRequestTypeDef](./type_defs.md#listportfoliosforproductinputrequesttypedef)
- [ListPortfoliosInputRequestTypeDef](./type_defs.md#listportfoliosinputrequesttypedef)
- [ListPrincipalsForPortfolioInputRequestTypeDef](./type_defs.md#listprincipalsforportfolioinputrequesttypedef)
- [PrincipalTypeDef](./type_defs.md#principaltypedef)
- [ProvisionedProductPlanSummaryTypeDef](./type_defs.md#provisionedproductplansummarytypedef)
- [ListProvisioningArtifactsForServiceActionInputRequestTypeDef](./type_defs.md#listprovisioningartifactsforserviceactioninputrequesttypedef)
- [ListProvisioningArtifactsInputRequestTypeDef](./type_defs.md#listprovisioningartifactsinputrequesttypedef)
- [ListRecordHistorySearchFilterTypeDef](./type_defs.md#listrecordhistorysearchfiltertypedef)
- [ListResourcesForTagOptionInputRequestTypeDef](./type_defs.md#listresourcesfortagoptioninputrequesttypedef)
- [ResourceDetailTypeDef](./type_defs.md#resourcedetailtypedef)
- [ListServiceActionsForProvisioningArtifactInputRequestTypeDef](./type_defs.md#listserviceactionsforprovisioningartifactinputrequesttypedef)
- [ServiceActionSummaryTypeDef](./type_defs.md#serviceactionsummarytypedef)
- [ListServiceActionsInputRequestTypeDef](./type_defs.md#listserviceactionsinputrequesttypedef)
- [ListStackInstancesForProvisionedProductInputRequestTypeDef](./type_defs.md#liststackinstancesforprovisionedproductinputrequesttypedef)
- [StackInstanceTypeDef](./type_defs.md#stackinstancetypedef)
- [ListTagOptionsFiltersTypeDef](./type_defs.md#listtagoptionsfilterstypedef)
- [NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef](./type_defs.md#notifyterminateprovisionedproductengineworkflowresultinputrequesttypedef)
- [ParameterConstraintsTypeDef](./type_defs.md#parameterconstraintstypedef)
- [ProductViewAggregationValueTypeDef](./type_defs.md#productviewaggregationvaluetypedef)
- [ProvisioningParameterTypeDef](./type_defs.md#provisioningparametertypedef)
- [ProvisioningPreferencesTypeDef](./type_defs.md#provisioningpreferencestypedef)
- [RecordErrorTypeDef](./type_defs.md#recorderrortypedef)
- [RecordTagTypeDef](./type_defs.md#recordtagtypedef)
- [RejectPortfolioShareInputRequestTypeDef](./type_defs.md#rejectportfolioshareinputrequesttypedef)
- [ResourceTargetDefinitionTypeDef](./type_defs.md#resourcetargetdefinitiontypedef)
- [SearchProductsAsAdminInputRequestTypeDef](./type_defs.md#searchproductsasadmininputrequesttypedef)
- [SearchProductsInputRequestTypeDef](./type_defs.md#searchproductsinputrequesttypedef)
- [ShareErrorTypeDef](./type_defs.md#shareerrortypedef)
- [TerminateProvisionedProductInputRequestTypeDef](./type_defs.md#terminateprovisionedproductinputrequesttypedef)
- [UpdateConstraintInputRequestTypeDef](./type_defs.md#updateconstraintinputrequesttypedef)
- [UpdateProvisioningPreferencesTypeDef](./type_defs.md#updateprovisioningpreferencestypedef)
- [UpdateProvisionedProductPropertiesInputRequestTypeDef](./type_defs.md#updateprovisionedproductpropertiesinputrequesttypedef)
- [UpdateProvisioningArtifactInputRequestTypeDef](./type_defs.md#updateprovisioningartifactinputrequesttypedef)
- [UpdateServiceActionInputRequestTypeDef](./type_defs.md#updateserviceactioninputrequesttypedef)
- [UpdateTagOptionInputRequestTypeDef](./type_defs.md#updatetagoptioninputrequesttypedef)
- [ListProvisionedProductPlansInputRequestTypeDef](./type_defs.md#listprovisionedproductplansinputrequesttypedef)
- [ScanProvisionedProductsInputRequestTypeDef](./type_defs.md#scanprovisionedproductsinputrequesttypedef)
- [SearchProvisionedProductsInputRequestTypeDef](./type_defs.md#searchprovisionedproductsinputrequesttypedef)
- [BatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef](./type_defs.md#batchassociateserviceactionwithprovisioningartifactinputrequesttypedef)
- [BatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef](./type_defs.md#batchdisassociateserviceactionfromprovisioningartifactinputrequesttypedef)
- [BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef](./type_defs.md#batchassociateserviceactionwithprovisioningartifactoutputtypedef)
- [BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef](./type_defs.md#batchdisassociateserviceactionfromprovisioningartifactoutputtypedef)
- [CopyProductOutputTypeDef](./type_defs.md#copyproductoutputtypedef)
- [CreatePortfolioShareOutputTypeDef](./type_defs.md#createportfolioshareoutputtypedef)
- [CreateProvisionedProductPlanOutputTypeDef](./type_defs.md#createprovisionedproductplanoutputtypedef)
- [DeletePortfolioShareOutputTypeDef](./type_defs.md#deleteportfolioshareoutputtypedef)
- [DescribeCopyProductStatusOutputTypeDef](./type_defs.md#describecopyproductstatusoutputtypedef)
- [GetAWSOrganizationsAccessStatusOutputTypeDef](./type_defs.md#getawsorganizationsaccessstatusoutputtypedef)
- [ListPortfolioAccessOutputTypeDef](./type_defs.md#listportfolioaccessoutputtypedef)
- [UpdatePortfolioShareOutputTypeDef](./type_defs.md#updateportfolioshareoutputtypedef)
- [UpdateProvisionedProductPropertiesOutputTypeDef](./type_defs.md#updateprovisionedproductpropertiesoutputtypedef)
- [ListBudgetsForResourceOutputTypeDef](./type_defs.md#listbudgetsforresourceoutputtypedef)
- [SourceConnectionParametersTypeDef](./type_defs.md#sourceconnectionparameterstypedef)
- [CreateConstraintOutputTypeDef](./type_defs.md#createconstraintoutputtypedef)
- [DescribeConstraintOutputTypeDef](./type_defs.md#describeconstraintoutputtypedef)
- [ListConstraintsForPortfolioOutputTypeDef](./type_defs.md#listconstraintsforportfoliooutputtypedef)
- [UpdateConstraintOutputTypeDef](./type_defs.md#updateconstraintoutputtypedef)
- [CreatePortfolioInputRequestTypeDef](./type_defs.md#createportfolioinputrequesttypedef)
- [LaunchPathSummaryTypeDef](./type_defs.md#launchpathsummarytypedef)
- [ProvisionedProductAttributeTypeDef](./type_defs.md#provisionedproductattributetypedef)
- [UpdatePortfolioInputRequestTypeDef](./type_defs.md#updateportfolioinputrequesttypedef)
- [CreatePortfolioOutputTypeDef](./type_defs.md#createportfoliooutputtypedef)
- [ListAcceptedPortfolioSharesOutputTypeDef](./type_defs.md#listacceptedportfoliosharesoutputtypedef)
- [ListPortfoliosForProductOutputTypeDef](./type_defs.md#listportfoliosforproductoutputtypedef)
- [ListPortfoliosOutputTypeDef](./type_defs.md#listportfoliosoutputtypedef)
- [UpdatePortfolioOutputTypeDef](./type_defs.md#updateportfoliooutputtypedef)
- [CreatePortfolioShareInputRequestTypeDef](./type_defs.md#createportfolioshareinputrequesttypedef)
- [DeletePortfolioShareInputRequestTypeDef](./type_defs.md#deleteportfolioshareinputrequesttypedef)
- [ListOrganizationPortfolioAccessOutputTypeDef](./type_defs.md#listorganizationportfolioaccessoutputtypedef)
- [UpdatePortfolioShareInputRequestTypeDef](./type_defs.md#updateportfolioshareinputrequesttypedef)
- [CreateProvisioningArtifactInputRequestTypeDef](./type_defs.md#createprovisioningartifactinputrequesttypedef)
- [CreateProvisioningArtifactOutputTypeDef](./type_defs.md#createprovisioningartifactoutputtypedef)
- [ListProvisioningArtifactsOutputTypeDef](./type_defs.md#listprovisioningartifactsoutputtypedef)
- [UpdateProvisioningArtifactOutputTypeDef](./type_defs.md#updateprovisioningartifactoutputtypedef)
- [CreateProvisionedProductPlanInputRequestTypeDef](./type_defs.md#createprovisionedproductplaninputrequesttypedef)
- [ProvisionedProductPlanDetailsTypeDef](./type_defs.md#provisionedproductplandetailstypedef)
- [CreateTagOptionOutputTypeDef](./type_defs.md#createtagoptionoutputtypedef)
- [DescribePortfolioOutputTypeDef](./type_defs.md#describeportfoliooutputtypedef)
- [DescribeTagOptionOutputTypeDef](./type_defs.md#describetagoptionoutputtypedef)
- [ListTagOptionsOutputTypeDef](./type_defs.md#listtagoptionsoutputtypedef)
- [UpdateTagOptionOutputTypeDef](./type_defs.md#updatetagoptionoutputtypedef)
- [DescribePortfolioSharesOutputTypeDef](./type_defs.md#describeportfoliosharesoutputtypedef)
- [DescribeProductOutputTypeDef](./type_defs.md#describeproductoutputtypedef)
- [DescribeProductViewOutputTypeDef](./type_defs.md#describeproductviewoutputtypedef)
- [ProvisioningArtifactViewTypeDef](./type_defs.md#provisioningartifactviewtypedef)
- [DescribeProvisionedProductOutputTypeDef](./type_defs.md#describeprovisionedproductoutputtypedef)
- [ScanProvisionedProductsOutputTypeDef](./type_defs.md#scanprovisionedproductsoutputtypedef)
- [GetProvisionedProductOutputsOutputTypeDef](./type_defs.md#getprovisionedproductoutputsoutputtypedef)
- [NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef](./type_defs.md#notifyupdateprovisionedproductengineworkflowresultinputrequesttypedef)
- [DescribeServiceActionExecutionParametersOutputTypeDef](./type_defs.md#describeserviceactionexecutionparametersoutputtypedef)
- [EngineWorkflowResourceIdentifierTypeDef](./type_defs.md#engineworkflowresourceidentifiertypedef)
- [ListAcceptedPortfolioSharesInputPaginateTypeDef](./type_defs.md#listacceptedportfoliosharesinputpaginatetypedef)
- [ListConstraintsForPortfolioInputPaginateTypeDef](./type_defs.md#listconstraintsforportfolioinputpaginatetypedef)
- [ListLaunchPathsInputPaginateTypeDef](./type_defs.md#listlaunchpathsinputpaginatetypedef)
- [ListOrganizationPortfolioAccessInputPaginateTypeDef](./type_defs.md#listorganizationportfolioaccessinputpaginatetypedef)
- [ListPortfoliosForProductInputPaginateTypeDef](./type_defs.md#listportfoliosforproductinputpaginatetypedef)
- [ListPortfoliosInputPaginateTypeDef](./type_defs.md#listportfoliosinputpaginatetypedef)
- [ListPrincipalsForPortfolioInputPaginateTypeDef](./type_defs.md#listprincipalsforportfolioinputpaginatetypedef)
- [ListProvisionedProductPlansInputPaginateTypeDef](./type_defs.md#listprovisionedproductplansinputpaginatetypedef)
- [ListProvisioningArtifactsForServiceActionInputPaginateTypeDef](./type_defs.md#listprovisioningartifactsforserviceactioninputpaginatetypedef)
- [ListResourcesForTagOptionInputPaginateTypeDef](./type_defs.md#listresourcesfortagoptioninputpaginatetypedef)
- [ListServiceActionsForProvisioningArtifactInputPaginateTypeDef](./type_defs.md#listserviceactionsforprovisioningartifactinputpaginatetypedef)
- [ListServiceActionsInputPaginateTypeDef](./type_defs.md#listserviceactionsinputpaginatetypedef)
- [ScanProvisionedProductsInputPaginateTypeDef](./type_defs.md#scanprovisionedproductsinputpaginatetypedef)
- [SearchProductsAsAdminInputPaginateTypeDef](./type_defs.md#searchproductsasadmininputpaginatetypedef)
- [ListPrincipalsForPortfolioOutputTypeDef](./type_defs.md#listprincipalsforportfoliooutputtypedef)
- [ListProvisionedProductPlansOutputTypeDef](./type_defs.md#listprovisionedproductplansoutputtypedef)
- [ListRecordHistoryInputPaginateTypeDef](./type_defs.md#listrecordhistoryinputpaginatetypedef)
- [ListRecordHistoryInputRequestTypeDef](./type_defs.md#listrecordhistoryinputrequesttypedef)
- [ListResourcesForTagOptionOutputTypeDef](./type_defs.md#listresourcesfortagoptionoutputtypedef)
- [ListServiceActionsForProvisioningArtifactOutputTypeDef](./type_defs.md#listserviceactionsforprovisioningartifactoutputtypedef)
- [ListServiceActionsOutputTypeDef](./type_defs.md#listserviceactionsoutputtypedef)
- [ServiceActionDetailTypeDef](./type_defs.md#serviceactiondetailtypedef)
- [ListStackInstancesForProvisionedProductOutputTypeDef](./type_defs.md#liststackinstancesforprovisionedproductoutputtypedef)
- [ListTagOptionsInputPaginateTypeDef](./type_defs.md#listtagoptionsinputpaginatetypedef)
- [ListTagOptionsInputRequestTypeDef](./type_defs.md#listtagoptionsinputrequesttypedef)
- [ProvisioningArtifactParameterTypeDef](./type_defs.md#provisioningartifactparametertypedef)
- [SearchProductsOutputTypeDef](./type_defs.md#searchproductsoutputtypedef)
- [ProvisionProductInputRequestTypeDef](./type_defs.md#provisionproductinputrequesttypedef)
- [RecordDetailTypeDef](./type_defs.md#recorddetailtypedef)
- [ResourceChangeDetailTypeDef](./type_defs.md#resourcechangedetailtypedef)
- [ShareDetailsTypeDef](./type_defs.md#sharedetailstypedef)
- [UpdateProvisionedProductInputRequestTypeDef](./type_defs.md#updateprovisionedproductinputrequesttypedef)
- [SourceConnectionDetailTypeDef](./type_defs.md#sourceconnectiondetailtypedef)
- [SourceConnectionTypeDef](./type_defs.md#sourceconnectiontypedef)
- [ListLaunchPathsOutputTypeDef](./type_defs.md#listlaunchpathsoutputtypedef)
- [SearchProvisionedProductsOutputTypeDef](./type_defs.md#searchprovisionedproductsoutputtypedef)
- [ListProvisioningArtifactsForServiceActionOutputTypeDef](./type_defs.md#listprovisioningartifactsforserviceactionoutputtypedef)
- [NotifyProvisionProductEngineWorkflowResultInputRequestTypeDef](./type_defs.md#notifyprovisionproductengineworkflowresultinputrequesttypedef)
- [CreateServiceActionOutputTypeDef](./type_defs.md#createserviceactionoutputtypedef)
- [DescribeServiceActionOutputTypeDef](./type_defs.md#describeserviceactionoutputtypedef)
- [UpdateServiceActionOutputTypeDef](./type_defs.md#updateserviceactionoutputtypedef)
- [DescribeProvisioningArtifactOutputTypeDef](./type_defs.md#describeprovisioningartifactoutputtypedef)
- [DescribeProvisioningParametersOutputTypeDef](./type_defs.md#describeprovisioningparametersoutputtypedef)
- [DescribeRecordOutputTypeDef](./type_defs.md#describerecordoutputtypedef)
- [ExecuteProvisionedProductPlanOutputTypeDef](./type_defs.md#executeprovisionedproductplanoutputtypedef)
- [ExecuteProvisionedProductServiceActionOutputTypeDef](./type_defs.md#executeprovisionedproductserviceactionoutputtypedef)
- [ImportAsProvisionedProductOutputTypeDef](./type_defs.md#importasprovisionedproductoutputtypedef)
- [ListRecordHistoryOutputTypeDef](./type_defs.md#listrecordhistoryoutputtypedef)
- [ProvisionProductOutputTypeDef](./type_defs.md#provisionproductoutputtypedef)
- [TerminateProvisionedProductOutputTypeDef](./type_defs.md#terminateprovisionedproductoutputtypedef)
- [UpdateProvisionedProductOutputTypeDef](./type_defs.md#updateprovisionedproductoutputtypedef)
- [ResourceChangeTypeDef](./type_defs.md#resourcechangetypedef)
- [DescribePortfolioShareStatusOutputTypeDef](./type_defs.md#describeportfoliosharestatusoutputtypedef)
- [ProductViewDetailTypeDef](./type_defs.md#productviewdetailtypedef)
- [CreateProductInputRequestTypeDef](./type_defs.md#createproductinputrequesttypedef)
- [UpdateProductInputRequestTypeDef](./type_defs.md#updateproductinputrequesttypedef)
- [DescribeProvisionedProductPlanOutputTypeDef](./type_defs.md#describeprovisionedproductplanoutputtypedef)
- [CreateProductOutputTypeDef](./type_defs.md#createproductoutputtypedef)
- [DescribeProductAsAdminOutputTypeDef](./type_defs.md#describeproductasadminoutputtypedef)
- [SearchProductsAsAdminOutputTypeDef](./type_defs.md#searchproductsasadminoutputtypedef)
- [UpdateProductOutputTypeDef](./type_defs.md#updateproductoutputtypedef)
