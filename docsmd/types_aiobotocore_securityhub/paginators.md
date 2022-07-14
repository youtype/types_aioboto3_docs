# Paginators

> [Index](../README.md) > [SecurityHub](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SecurityHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
    type annotations stubs module [types-aiobotocore-securityhub](https://pypi.org/project/types-aiobotocore-securityhub/).

## DescribeActionTargetsPaginator

Type annotations and code completion for `#!python session.client("securityhub").get_paginator("describe_action_targets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeActionTargets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_securityhub.paginator import DescribeActionTargetsPaginator

session = Session()

session = get_session()
async with session.client("securityhub") as client:  # (1)
    paginator: DescribeActionTargetsPaginator = client.get_paginator("describe_action_targets")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeActionTargetsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [DescribeActionTargetsPaginator](./paginators.md#describeactiontargetspaginator)
3. item: [:material-code-braces: DescribeActionTargetsResponseTypeDef](./type_defs.md#describeactiontargetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeActionTargetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ActionTargetArns: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeActionTargetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeActionTargetsResponseTypeDef](./type_defs.md#describeactiontargetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef = {  # (1)
    "ActionTargetArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef](./type_defs.md#describeactiontargetsrequestdescribeactiontargetspaginatetypedef) 
## DescribeProductsPaginator

Type annotations and code completion for `#!python session.client("securityhub").get_paginator("describe_products")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeProducts)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_securityhub.paginator import DescribeProductsPaginator

session = Session()

session = get_session()
async with session.client("securityhub") as client:  # (1)
    paginator: DescribeProductsPaginator = client.get_paginator("describe_products")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeProductsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [DescribeProductsPaginator](./paginators.md#describeproductspaginator)
3. item: [:material-code-braces: DescribeProductsResponseTypeDef](./type_defs.md#describeproductsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeProductsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ProductArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeProductsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeProductsResponseTypeDef](./type_defs.md#describeproductsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeProductsRequestDescribeProductsPaginateTypeDef = {  # (1)
    "ProductArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeProductsRequestDescribeProductsPaginateTypeDef](./type_defs.md#describeproductsrequestdescribeproductspaginatetypedef) 
## DescribeStandardsPaginator

Type annotations and code completion for `#!python session.client("securityhub").get_paginator("describe_standards")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandards)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_securityhub.paginator import DescribeStandardsPaginator

session = Session()

session = get_session()
async with session.client("securityhub") as client:  # (1)
    paginator: DescribeStandardsPaginator = client.get_paginator("describe_standards")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeStandardsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [DescribeStandardsPaginator](./paginators.md#describestandardspaginator)
3. item: [:material-code-braces: DescribeStandardsResponseTypeDef](./type_defs.md#describestandardsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeStandardsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeStandardsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeStandardsResponseTypeDef](./type_defs.md#describestandardsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeStandardsRequestDescribeStandardsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeStandardsRequestDescribeStandardsPaginateTypeDef](./type_defs.md#describestandardsrequestdescribestandardspaginatetypedef) 
## DescribeStandardsControlsPaginator

Type annotations and code completion for `#!python session.client("securityhub").get_paginator("describe_standards_controls")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandardsControls)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_securityhub.paginator import DescribeStandardsControlsPaginator

session = Session()

session = get_session()
async with session.client("securityhub") as client:  # (1)
    paginator: DescribeStandardsControlsPaginator = client.get_paginator("describe_standards_controls")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeStandardsControlsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [DescribeStandardsControlsPaginator](./paginators.md#describestandardscontrolspaginator)
3. item: [:material-code-braces: DescribeStandardsControlsResponseTypeDef](./type_defs.md#describestandardscontrolsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeStandardsControlsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    StandardsSubscriptionArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeStandardsControlsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeStandardsControlsResponseTypeDef](./type_defs.md#describestandardscontrolsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef = {  # (1)
    "StandardsSubscriptionArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef](./type_defs.md#describestandardscontrolsrequestdescribestandardscontrolspaginatetypedef) 
## GetEnabledStandardsPaginator

Type annotations and code completion for `#!python session.client("securityhub").get_paginator("get_enabled_standards")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetEnabledStandards)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_securityhub.paginator import GetEnabledStandardsPaginator

session = Session()

session = get_session()
async with session.client("securityhub") as client:  # (1)
    paginator: GetEnabledStandardsPaginator = client.get_paginator("get_enabled_standards")  # (2)
    async for item in paginator.paginate(...):
        item: GetEnabledStandardsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [GetEnabledStandardsPaginator](./paginators.md#getenabledstandardspaginator)
3. item: [:material-code-braces: GetEnabledStandardsResponseTypeDef](./type_defs.md#getenabledstandardsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetEnabledStandardsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    StandardsSubscriptionArns: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetEnabledStandardsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetEnabledStandardsResponseTypeDef](./type_defs.md#getenabledstandardsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef = {  # (1)
    "StandardsSubscriptionArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef](./type_defs.md#getenabledstandardsrequestgetenabledstandardspaginatetypedef) 
## GetFindingsPaginator

Type annotations and code completion for `#!python session.client("securityhub").get_paginator("get_findings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_securityhub.paginator import GetFindingsPaginator

session = Session()

session = get_session()
async with session.client("securityhub") as client:  # (1)
    paginator: GetFindingsPaginator = client.get_paginator("get_findings")  # (2)
    async for item in paginator.paginate(...):
        item: GetFindingsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [GetFindingsPaginator](./paginators.md#getfindingspaginator)
3. item: [:material-code-braces: GetFindingsResponseTypeDef](./type_defs.md#getfindingsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetFindingsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: AwsSecurityFindingFiltersTypeDef = ...,  # (1)
    SortCriteria: Sequence[SortCriterionTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[GetFindingsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: AwsSecurityFindingFiltersTypeDef](./type_defs.md#awssecurityfindingfilterstypedef) 
2. See [:material-code-braces: SortCriterionTypeDef](./type_defs.md#sortcriteriontypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: GetFindingsResponseTypeDef](./type_defs.md#getfindingsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetFindingsRequestGetFindingsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetFindingsRequestGetFindingsPaginateTypeDef](./type_defs.md#getfindingsrequestgetfindingspaginatetypedef) 
## GetInsightsPaginator

Type annotations and code completion for `#!python session.client("securityhub").get_paginator("get_insights")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetInsights)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_securityhub.paginator import GetInsightsPaginator

session = Session()

session = get_session()
async with session.client("securityhub") as client:  # (1)
    paginator: GetInsightsPaginator = client.get_paginator("get_insights")  # (2)
    async for item in paginator.paginate(...):
        item: GetInsightsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [GetInsightsPaginator](./paginators.md#getinsightspaginator)
3. item: [:material-code-braces: GetInsightsResponseTypeDef](./type_defs.md#getinsightsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetInsightsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InsightArns: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetInsightsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetInsightsResponseTypeDef](./type_defs.md#getinsightsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetInsightsRequestGetInsightsPaginateTypeDef = {  # (1)
    "InsightArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetInsightsRequestGetInsightsPaginateTypeDef](./type_defs.md#getinsightsrequestgetinsightspaginatetypedef) 
## ListEnabledProductsForImportPaginator

Type annotations and code completion for `#!python session.client("securityhub").get_paginator("list_enabled_products_for_import")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListEnabledProductsForImport)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_securityhub.paginator import ListEnabledProductsForImportPaginator

session = Session()

session = get_session()
async with session.client("securityhub") as client:  # (1)
    paginator: ListEnabledProductsForImportPaginator = client.get_paginator("list_enabled_products_for_import")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnabledProductsForImportResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [ListEnabledProductsForImportPaginator](./paginators.md#listenabledproductsforimportpaginator)
3. item: [:material-code-braces: ListEnabledProductsForImportResponseTypeDef](./type_defs.md#listenabledproductsforimportresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEnabledProductsForImportPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEnabledProductsForImportResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEnabledProductsForImportResponseTypeDef](./type_defs.md#listenabledproductsforimportresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef](./type_defs.md#listenabledproductsforimportrequestlistenabledproductsforimportpaginatetypedef) 
## ListFindingAggregatorsPaginator

Type annotations and code completion for `#!python session.client("securityhub").get_paginator("list_finding_aggregators")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListFindingAggregators)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_securityhub.paginator import ListFindingAggregatorsPaginator

session = Session()

session = get_session()
async with session.client("securityhub") as client:  # (1)
    paginator: ListFindingAggregatorsPaginator = client.get_paginator("list_finding_aggregators")  # (2)
    async for item in paginator.paginate(...):
        item: ListFindingAggregatorsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [ListFindingAggregatorsPaginator](./paginators.md#listfindingaggregatorspaginator)
3. item: [:material-code-braces: ListFindingAggregatorsResponseTypeDef](./type_defs.md#listfindingaggregatorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFindingAggregatorsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListFindingAggregatorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFindingAggregatorsResponseTypeDef](./type_defs.md#listfindingaggregatorsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef](./type_defs.md#listfindingaggregatorsrequestlistfindingaggregatorspaginatetypedef) 
## ListInvitationsPaginator

Type annotations and code completion for `#!python session.client("securityhub").get_paginator("list_invitations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListInvitations)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_securityhub.paginator import ListInvitationsPaginator

session = Session()

session = get_session()
async with session.client("securityhub") as client:  # (1)
    paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")  # (2)
    async for item in paginator.paginate(...):
        item: ListInvitationsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [ListInvitationsPaginator](./paginators.md#listinvitationspaginator)
3. item: [:material-code-braces: ListInvitationsResponseTypeDef](./type_defs.md#listinvitationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInvitationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListInvitationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInvitationsResponseTypeDef](./type_defs.md#listinvitationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListInvitationsRequestListInvitationsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInvitationsRequestListInvitationsPaginateTypeDef](./type_defs.md#listinvitationsrequestlistinvitationspaginatetypedef) 
## ListMembersPaginator

Type annotations and code completion for `#!python session.client("securityhub").get_paginator("list_members")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListMembers)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_securityhub.paginator import ListMembersPaginator

session = Session()

session = get_session()
async with session.client("securityhub") as client:  # (1)
    paginator: ListMembersPaginator = client.get_paginator("list_members")  # (2)
    async for item in paginator.paginate(...):
        item: ListMembersResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [ListMembersPaginator](./paginators.md#listmemberspaginator)
3. item: [:material-code-braces: ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMembersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    OnlyAssociated: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMembersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListMembersRequestListMembersPaginateTypeDef = {  # (1)
    "OnlyAssociated": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMembersRequestListMembersPaginateTypeDef](./type_defs.md#listmembersrequestlistmemberspaginatetypedef) 
## ListOrganizationAdminAccountsPaginator

Type annotations and code completion for `#!python session.client("securityhub").get_paginator("list_organization_admin_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListOrganizationAdminAccounts)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_securityhub.paginator import ListOrganizationAdminAccountsPaginator

session = Session()

session = get_session()
async with session.client("securityhub") as client:  # (1)
    paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListOrganizationAdminAccountsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [ListOrganizationAdminAccountsPaginator](./paginators.md#listorganizationadminaccountspaginator)
3. item: [:material-code-braces: ListOrganizationAdminAccountsResponseTypeDef](./type_defs.md#listorganizationadminaccountsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListOrganizationAdminAccountsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListOrganizationAdminAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOrganizationAdminAccountsResponseTypeDef](./type_defs.md#listorganizationadminaccountsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef](./type_defs.md#listorganizationadminaccountsrequestlistorganizationadminaccountspaginatetypedef) 
