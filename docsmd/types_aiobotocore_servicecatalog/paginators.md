# Paginators

> [Index](../README.md) > [ServiceCatalog](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ServiceCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
    type annotations stubs module [types-aiobotocore-servicecatalog](https://pypi.org/project/types-aiobotocore-servicecatalog/).

## ListAcceptedPortfolioSharesPaginator

Type annotations and code completion for `#!python session.client("servicecatalog").get_paginator("list_accepted_portfolio_shares")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListAcceptedPortfolioShares)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_servicecatalog.paginator import ListAcceptedPortfolioSharesPaginator

session = Session()

session = get_session()
async with session.client("servicecatalog") as client:  # (1)
    paginator: ListAcceptedPortfolioSharesPaginator = client.get_paginator("list_accepted_portfolio_shares")  # (2)
    async for item in paginator.paginate(...):
        item: ListAcceptedPortfolioSharesOutputTypeDef
        print(item)  # (3)
```

1. client: [ServiceCatalogClient](./client.md)
2. paginator: [ListAcceptedPortfolioSharesPaginator](./paginators.md#listacceptedportfoliosharespaginator)
3. item: [:material-code-braces: ListAcceptedPortfolioSharesOutputTypeDef](./type_defs.md#listacceptedportfoliosharesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListAcceptedPortfolioSharesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AcceptLanguage: str = ...,
    PortfolioShareType: PortfolioShareTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAcceptedPortfolioSharesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: PortfolioShareTypeType](./literals.md#portfoliosharetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAcceptedPortfolioSharesOutputTypeDef](./type_defs.md#listacceptedportfoliosharesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef = {  # (1)
    "AcceptLanguage": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef](./type_defs.md#listacceptedportfoliosharesinputlistacceptedportfoliosharespaginatetypedef) 
## ListConstraintsForPortfolioPaginator

Type annotations and code completion for `#!python session.client("servicecatalog").get_paginator("list_constraints_for_portfolio")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListConstraintsForPortfolio)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_servicecatalog.paginator import ListConstraintsForPortfolioPaginator

session = Session()

session = get_session()
async with session.client("servicecatalog") as client:  # (1)
    paginator: ListConstraintsForPortfolioPaginator = client.get_paginator("list_constraints_for_portfolio")  # (2)
    async for item in paginator.paginate(...):
        item: ListConstraintsForPortfolioOutputTypeDef
        print(item)  # (3)
```

1. client: [ServiceCatalogClient](./client.md)
2. paginator: [ListConstraintsForPortfolioPaginator](./paginators.md#listconstraintsforportfoliopaginator)
3. item: [:material-code-braces: ListConstraintsForPortfolioOutputTypeDef](./type_defs.md#listconstraintsforportfoliooutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListConstraintsForPortfolioPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PortfolioId: str,
    AcceptLanguage: str = ...,
    ProductId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListConstraintsForPortfolioOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConstraintsForPortfolioOutputTypeDef](./type_defs.md#listconstraintsforportfoliooutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef = {  # (1)
    "PortfolioId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef](./type_defs.md#listconstraintsforportfolioinputlistconstraintsforportfoliopaginatetypedef) 
## ListLaunchPathsPaginator

Type annotations and code completion for `#!python session.client("servicecatalog").get_paginator("list_launch_paths")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListLaunchPaths)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_servicecatalog.paginator import ListLaunchPathsPaginator

session = Session()

session = get_session()
async with session.client("servicecatalog") as client:  # (1)
    paginator: ListLaunchPathsPaginator = client.get_paginator("list_launch_paths")  # (2)
    async for item in paginator.paginate(...):
        item: ListLaunchPathsOutputTypeDef
        print(item)  # (3)
```

1. client: [ServiceCatalogClient](./client.md)
2. paginator: [ListLaunchPathsPaginator](./paginators.md#listlaunchpathspaginator)
3. item: [:material-code-braces: ListLaunchPathsOutputTypeDef](./type_defs.md#listlaunchpathsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListLaunchPathsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ProductId: str,
    AcceptLanguage: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListLaunchPathsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLaunchPathsOutputTypeDef](./type_defs.md#listlaunchpathsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListLaunchPathsInputListLaunchPathsPaginateTypeDef = {  # (1)
    "ProductId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLaunchPathsInputListLaunchPathsPaginateTypeDef](./type_defs.md#listlaunchpathsinputlistlaunchpathspaginatetypedef) 
## ListOrganizationPortfolioAccessPaginator

Type annotations and code completion for `#!python session.client("servicecatalog").get_paginator("list_organization_portfolio_access")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListOrganizationPortfolioAccess)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_servicecatalog.paginator import ListOrganizationPortfolioAccessPaginator

session = Session()

session = get_session()
async with session.client("servicecatalog") as client:  # (1)
    paginator: ListOrganizationPortfolioAccessPaginator = client.get_paginator("list_organization_portfolio_access")  # (2)
    async for item in paginator.paginate(...):
        item: ListOrganizationPortfolioAccessOutputTypeDef
        print(item)  # (3)
```

1. client: [ServiceCatalogClient](./client.md)
2. paginator: [ListOrganizationPortfolioAccessPaginator](./paginators.md#listorganizationportfolioaccesspaginator)
3. item: [:material-code-braces: ListOrganizationPortfolioAccessOutputTypeDef](./type_defs.md#listorganizationportfolioaccessoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListOrganizationPortfolioAccessPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PortfolioId: str,
    OrganizationNodeType: OrganizationNodeTypeType,  # (1)
    AcceptLanguage: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListOrganizationPortfolioAccessOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: OrganizationNodeTypeType](./literals.md#organizationnodetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListOrganizationPortfolioAccessOutputTypeDef](./type_defs.md#listorganizationportfolioaccessoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef = {  # (1)
    "PortfolioId": ...,
    "OrganizationNodeType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef](./type_defs.md#listorganizationportfolioaccessinputlistorganizationportfolioaccesspaginatetypedef) 
## ListPortfoliosPaginator

Type annotations and code completion for `#!python session.client("servicecatalog").get_paginator("list_portfolios")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPortfolios)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_servicecatalog.paginator import ListPortfoliosPaginator

session = Session()

session = get_session()
async with session.client("servicecatalog") as client:  # (1)
    paginator: ListPortfoliosPaginator = client.get_paginator("list_portfolios")  # (2)
    async for item in paginator.paginate(...):
        item: ListPortfoliosOutputTypeDef
        print(item)  # (3)
```

1. client: [ServiceCatalogClient](./client.md)
2. paginator: [ListPortfoliosPaginator](./paginators.md#listportfoliospaginator)
3. item: [:material-code-braces: ListPortfoliosOutputTypeDef](./type_defs.md#listportfoliosoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListPortfoliosPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AcceptLanguage: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPortfoliosOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPortfoliosOutputTypeDef](./type_defs.md#listportfoliosoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListPortfoliosInputListPortfoliosPaginateTypeDef = {  # (1)
    "AcceptLanguage": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPortfoliosInputListPortfoliosPaginateTypeDef](./type_defs.md#listportfoliosinputlistportfoliospaginatetypedef) 
## ListPortfoliosForProductPaginator

Type annotations and code completion for `#!python session.client("servicecatalog").get_paginator("list_portfolios_for_product")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPortfoliosForProduct)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_servicecatalog.paginator import ListPortfoliosForProductPaginator

session = Session()

session = get_session()
async with session.client("servicecatalog") as client:  # (1)
    paginator: ListPortfoliosForProductPaginator = client.get_paginator("list_portfolios_for_product")  # (2)
    async for item in paginator.paginate(...):
        item: ListPortfoliosForProductOutputTypeDef
        print(item)  # (3)
```

1. client: [ServiceCatalogClient](./client.md)
2. paginator: [ListPortfoliosForProductPaginator](./paginators.md#listportfoliosforproductpaginator)
3. item: [:material-code-braces: ListPortfoliosForProductOutputTypeDef](./type_defs.md#listportfoliosforproductoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListPortfoliosForProductPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ProductId: str,
    AcceptLanguage: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPortfoliosForProductOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPortfoliosForProductOutputTypeDef](./type_defs.md#listportfoliosforproductoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef = {  # (1)
    "ProductId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef](./type_defs.md#listportfoliosforproductinputlistportfoliosforproductpaginatetypedef) 
## ListPrincipalsForPortfolioPaginator

Type annotations and code completion for `#!python session.client("servicecatalog").get_paginator("list_principals_for_portfolio")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPrincipalsForPortfolio)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_servicecatalog.paginator import ListPrincipalsForPortfolioPaginator

session = Session()

session = get_session()
async with session.client("servicecatalog") as client:  # (1)
    paginator: ListPrincipalsForPortfolioPaginator = client.get_paginator("list_principals_for_portfolio")  # (2)
    async for item in paginator.paginate(...):
        item: ListPrincipalsForPortfolioOutputTypeDef
        print(item)  # (3)
```

1. client: [ServiceCatalogClient](./client.md)
2. paginator: [ListPrincipalsForPortfolioPaginator](./paginators.md#listprincipalsforportfoliopaginator)
3. item: [:material-code-braces: ListPrincipalsForPortfolioOutputTypeDef](./type_defs.md#listprincipalsforportfoliooutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListPrincipalsForPortfolioPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PortfolioId: str,
    AcceptLanguage: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPrincipalsForPortfolioOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPrincipalsForPortfolioOutputTypeDef](./type_defs.md#listprincipalsforportfoliooutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef = {  # (1)
    "PortfolioId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef](./type_defs.md#listprincipalsforportfolioinputlistprincipalsforportfoliopaginatetypedef) 
## ListProvisionedProductPlansPaginator

Type annotations and code completion for `#!python session.client("servicecatalog").get_paginator("list_provisioned_product_plans")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListProvisionedProductPlans)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_servicecatalog.paginator import ListProvisionedProductPlansPaginator

session = Session()

session = get_session()
async with session.client("servicecatalog") as client:  # (1)
    paginator: ListProvisionedProductPlansPaginator = client.get_paginator("list_provisioned_product_plans")  # (2)
    async for item in paginator.paginate(...):
        item: ListProvisionedProductPlansOutputTypeDef
        print(item)  # (3)
```

1. client: [ServiceCatalogClient](./client.md)
2. paginator: [ListProvisionedProductPlansPaginator](./paginators.md#listprovisionedproductplanspaginator)
3. item: [:material-code-braces: ListProvisionedProductPlansOutputTypeDef](./type_defs.md#listprovisionedproductplansoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListProvisionedProductPlansPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AcceptLanguage: str = ...,
    ProvisionProductId: str = ...,
    AccessLevelFilter: AccessLevelFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListProvisionedProductPlansOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: AccessLevelFilterTypeDef](./type_defs.md#accesslevelfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListProvisionedProductPlansOutputTypeDef](./type_defs.md#listprovisionedproductplansoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef = {  # (1)
    "AcceptLanguage": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef](./type_defs.md#listprovisionedproductplansinputlistprovisionedproductplanspaginatetypedef) 
## ListProvisioningArtifactsForServiceActionPaginator

Type annotations and code completion for `#!python session.client("servicecatalog").get_paginator("list_provisioning_artifacts_for_service_action")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListProvisioningArtifactsForServiceAction)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_servicecatalog.paginator import ListProvisioningArtifactsForServiceActionPaginator

session = Session()

session = get_session()
async with session.client("servicecatalog") as client:  # (1)
    paginator: ListProvisioningArtifactsForServiceActionPaginator = client.get_paginator("list_provisioning_artifacts_for_service_action")  # (2)
    async for item in paginator.paginate(...):
        item: ListProvisioningArtifactsForServiceActionOutputTypeDef
        print(item)  # (3)
```

1. client: [ServiceCatalogClient](./client.md)
2. paginator: [ListProvisioningArtifactsForServiceActionPaginator](./paginators.md#listprovisioningartifactsforserviceactionpaginator)
3. item: [:material-code-braces: ListProvisioningArtifactsForServiceActionOutputTypeDef](./type_defs.md#listprovisioningartifactsforserviceactionoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListProvisioningArtifactsForServiceActionPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ServiceActionId: str,
    AcceptLanguage: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListProvisioningArtifactsForServiceActionOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProvisioningArtifactsForServiceActionOutputTypeDef](./type_defs.md#listprovisioningartifactsforserviceactionoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef = {  # (1)
    "ServiceActionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef](./type_defs.md#listprovisioningartifactsforserviceactioninputlistprovisioningartifactsforserviceactionpaginatetypedef) 
## ListRecordHistoryPaginator

Type annotations and code completion for `#!python session.client("servicecatalog").get_paginator("list_record_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListRecordHistory)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_servicecatalog.paginator import ListRecordHistoryPaginator

session = Session()

session = get_session()
async with session.client("servicecatalog") as client:  # (1)
    paginator: ListRecordHistoryPaginator = client.get_paginator("list_record_history")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecordHistoryOutputTypeDef
        print(item)  # (3)
```

1. client: [ServiceCatalogClient](./client.md)
2. paginator: [ListRecordHistoryPaginator](./paginators.md#listrecordhistorypaginator)
3. item: [:material-code-braces: ListRecordHistoryOutputTypeDef](./type_defs.md#listrecordhistoryoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListRecordHistoryPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AcceptLanguage: str = ...,
    AccessLevelFilter: AccessLevelFilterTypeDef = ...,  # (1)
    SearchFilter: ListRecordHistorySearchFilterTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListRecordHistoryOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: AccessLevelFilterTypeDef](./type_defs.md#accesslevelfiltertypedef) 
2. See [:material-code-braces: ListRecordHistorySearchFilterTypeDef](./type_defs.md#listrecordhistorysearchfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListRecordHistoryOutputTypeDef](./type_defs.md#listrecordhistoryoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListRecordHistoryInputListRecordHistoryPaginateTypeDef = {  # (1)
    "AcceptLanguage": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecordHistoryInputListRecordHistoryPaginateTypeDef](./type_defs.md#listrecordhistoryinputlistrecordhistorypaginatetypedef) 
## ListResourcesForTagOptionPaginator

Type annotations and code completion for `#!python session.client("servicecatalog").get_paginator("list_resources_for_tag_option")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListResourcesForTagOption)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_servicecatalog.paginator import ListResourcesForTagOptionPaginator

session = Session()

session = get_session()
async with session.client("servicecatalog") as client:  # (1)
    paginator: ListResourcesForTagOptionPaginator = client.get_paginator("list_resources_for_tag_option")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourcesForTagOptionOutputTypeDef
        print(item)  # (3)
```

1. client: [ServiceCatalogClient](./client.md)
2. paginator: [ListResourcesForTagOptionPaginator](./paginators.md#listresourcesfortagoptionpaginator)
3. item: [:material-code-braces: ListResourcesForTagOptionOutputTypeDef](./type_defs.md#listresourcesfortagoptionoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListResourcesForTagOptionPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TagOptionId: str,
    ResourceType: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListResourcesForTagOptionOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResourcesForTagOptionOutputTypeDef](./type_defs.md#listresourcesfortagoptionoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef = {  # (1)
    "TagOptionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef](./type_defs.md#listresourcesfortagoptioninputlistresourcesfortagoptionpaginatetypedef) 
## ListServiceActionsPaginator

Type annotations and code completion for `#!python session.client("servicecatalog").get_paginator("list_service_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListServiceActions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_servicecatalog.paginator import ListServiceActionsPaginator

session = Session()

session = get_session()
async with session.client("servicecatalog") as client:  # (1)
    paginator: ListServiceActionsPaginator = client.get_paginator("list_service_actions")  # (2)
    async for item in paginator.paginate(...):
        item: ListServiceActionsOutputTypeDef
        print(item)  # (3)
```

1. client: [ServiceCatalogClient](./client.md)
2. paginator: [ListServiceActionsPaginator](./paginators.md#listserviceactionspaginator)
3. item: [:material-code-braces: ListServiceActionsOutputTypeDef](./type_defs.md#listserviceactionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListServiceActionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AcceptLanguage: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListServiceActionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListServiceActionsOutputTypeDef](./type_defs.md#listserviceactionsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListServiceActionsInputListServiceActionsPaginateTypeDef = {  # (1)
    "AcceptLanguage": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListServiceActionsInputListServiceActionsPaginateTypeDef](./type_defs.md#listserviceactionsinputlistserviceactionspaginatetypedef) 
## ListServiceActionsForProvisioningArtifactPaginator

Type annotations and code completion for `#!python session.client("servicecatalog").get_paginator("list_service_actions_for_provisioning_artifact")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListServiceActionsForProvisioningArtifact)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_servicecatalog.paginator import ListServiceActionsForProvisioningArtifactPaginator

session = Session()

session = get_session()
async with session.client("servicecatalog") as client:  # (1)
    paginator: ListServiceActionsForProvisioningArtifactPaginator = client.get_paginator("list_service_actions_for_provisioning_artifact")  # (2)
    async for item in paginator.paginate(...):
        item: ListServiceActionsForProvisioningArtifactOutputTypeDef
        print(item)  # (3)
```

1. client: [ServiceCatalogClient](./client.md)
2. paginator: [ListServiceActionsForProvisioningArtifactPaginator](./paginators.md#listserviceactionsforprovisioningartifactpaginator)
3. item: [:material-code-braces: ListServiceActionsForProvisioningArtifactOutputTypeDef](./type_defs.md#listserviceactionsforprovisioningartifactoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListServiceActionsForProvisioningArtifactPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ProductId: str,
    ProvisioningArtifactId: str,
    AcceptLanguage: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListServiceActionsForProvisioningArtifactOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListServiceActionsForProvisioningArtifactOutputTypeDef](./type_defs.md#listserviceactionsforprovisioningartifactoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef = {  # (1)
    "ProductId": ...,
    "ProvisioningArtifactId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef](./type_defs.md#listserviceactionsforprovisioningartifactinputlistserviceactionsforprovisioningartifactpaginatetypedef) 
## ListTagOptionsPaginator

Type annotations and code completion for `#!python session.client("servicecatalog").get_paginator("list_tag_options")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListTagOptions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_servicecatalog.paginator import ListTagOptionsPaginator

session = Session()

session = get_session()
async with session.client("servicecatalog") as client:  # (1)
    paginator: ListTagOptionsPaginator = client.get_paginator("list_tag_options")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagOptionsOutputTypeDef
        print(item)  # (3)
```

1. client: [ServiceCatalogClient](./client.md)
2. paginator: [ListTagOptionsPaginator](./paginators.md#listtagoptionspaginator)
3. item: [:material-code-braces: ListTagOptionsOutputTypeDef](./type_defs.md#listtagoptionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListTagOptionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: ListTagOptionsFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListTagOptionsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListTagOptionsFiltersTypeDef](./type_defs.md#listtagoptionsfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListTagOptionsOutputTypeDef](./type_defs.md#listtagoptionsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagOptionsInputListTagOptionsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagOptionsInputListTagOptionsPaginateTypeDef](./type_defs.md#listtagoptionsinputlisttagoptionspaginatetypedef) 
## ScanProvisionedProductsPaginator

Type annotations and code completion for `#!python session.client("servicecatalog").get_paginator("scan_provisioned_products")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ScanProvisionedProducts)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_servicecatalog.paginator import ScanProvisionedProductsPaginator

session = Session()

session = get_session()
async with session.client("servicecatalog") as client:  # (1)
    paginator: ScanProvisionedProductsPaginator = client.get_paginator("scan_provisioned_products")  # (2)
    async for item in paginator.paginate(...):
        item: ScanProvisionedProductsOutputTypeDef
        print(item)  # (3)
```

1. client: [ServiceCatalogClient](./client.md)
2. paginator: [ScanProvisionedProductsPaginator](./paginators.md#scanprovisionedproductspaginator)
3. item: [:material-code-braces: ScanProvisionedProductsOutputTypeDef](./type_defs.md#scanprovisionedproductsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ScanProvisionedProductsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AcceptLanguage: str = ...,
    AccessLevelFilter: AccessLevelFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ScanProvisionedProductsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: AccessLevelFilterTypeDef](./type_defs.md#accesslevelfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ScanProvisionedProductsOutputTypeDef](./type_defs.md#scanprovisionedproductsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef = {  # (1)
    "AcceptLanguage": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef](./type_defs.md#scanprovisionedproductsinputscanprovisionedproductspaginatetypedef) 
## SearchProductsAsAdminPaginator

Type annotations and code completion for `#!python session.client("servicecatalog").get_paginator("search_products_as_admin")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.SearchProductsAsAdmin)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_servicecatalog.paginator import SearchProductsAsAdminPaginator

session = Session()

session = get_session()
async with session.client("servicecatalog") as client:  # (1)
    paginator: SearchProductsAsAdminPaginator = client.get_paginator("search_products_as_admin")  # (2)
    async for item in paginator.paginate(...):
        item: SearchProductsAsAdminOutputTypeDef
        print(item)  # (3)
```

1. client: [ServiceCatalogClient](./client.md)
2. paginator: [SearchProductsAsAdminPaginator](./paginators.md#searchproductsasadminpaginator)
3. item: [:material-code-braces: SearchProductsAsAdminOutputTypeDef](./type_defs.md#searchproductsasadminoutputtypedef) 


### paginate

Type annotations and code completion for `#!python SearchProductsAsAdminPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AcceptLanguage: str = ...,
    PortfolioId: str = ...,
    Filters: Mapping[ProductViewFilterByType, Sequence[str]] = ...,  # (1)
    SortBy: ProductViewSortByType = ...,  # (2)
    SortOrder: SortOrderType = ...,  # (3)
    ProductSource: ProductSourceType = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> AsyncIterator[SearchProductsAsAdminOutputTypeDef]:  # (6)
    ...
```

1. See [:material-code-brackets: ProductViewFilterByType](./literals.md#productviewfilterbytype) 
2. See [:material-code-brackets: ProductViewSortByType](./literals.md#productviewsortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-brackets: ProductSourceType](./literals.md#productsourcetype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
6. See [:material-code-braces: SearchProductsAsAdminOutputTypeDef](./type_defs.md#searchproductsasadminoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef = {  # (1)
    "AcceptLanguage": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef](./type_defs.md#searchproductsasadmininputsearchproductsasadminpaginatetypedef) 
