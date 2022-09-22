# Paginators

> [Index](../README.md) > [GuardDuty](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [GuardDuty](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
    type annotations stubs module [types-aiobotocore-guardduty](https://pypi.org/project/types-aiobotocore-guardduty/).

## DescribeMalwareScansPaginator

Type annotations and code completion for `#!python session.client("guardduty").get_paginator("describe_malware_scans")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.DescribeMalwareScans)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_guardduty.paginator import DescribeMalwareScansPaginator

session = Session()

session = get_session()
async with session.client("guardduty") as client:  # (1)
    paginator: DescribeMalwareScansPaginator = client.get_paginator("describe_malware_scans")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeMalwareScansResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
2. paginator: [DescribeMalwareScansPaginator](./paginators.md#describemalwarescanspaginator)
3. item: [:material-code-braces: DescribeMalwareScansResponseTypeDef](./type_defs.md#describemalwarescansresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeMalwareScansPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DetectorId: str,
    FilterCriteria: FilterCriteriaTypeDef = ...,  # (1)
    SortCriteria: SortCriteriaTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[DescribeMalwareScansResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeMalwareScansResponseTypeDef](./type_defs.md#describemalwarescansresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef = {  # (1)
    "DetectorId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef](./type_defs.md#describemalwarescansrequestdescribemalwarescanspaginatetypedef) 
## ListDetectorsPaginator

Type annotations and code completion for `#!python session.client("guardduty").get_paginator("list_detectors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListDetectors)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_guardduty.paginator import ListDetectorsPaginator

session = Session()

session = get_session()
async with session.client("guardduty") as client:  # (1)
    paginator: ListDetectorsPaginator = client.get_paginator("list_detectors")  # (2)
    async for item in paginator.paginate(...):
        item: ListDetectorsResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
2. paginator: [ListDetectorsPaginator](./paginators.md#listdetectorspaginator)
3. item: [:material-code-braces: ListDetectorsResponseTypeDef](./type_defs.md#listdetectorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDetectorsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDetectorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDetectorsResponseTypeDef](./type_defs.md#listdetectorsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDetectorsRequestListDetectorsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDetectorsRequestListDetectorsPaginateTypeDef](./type_defs.md#listdetectorsrequestlistdetectorspaginatetypedef) 
## ListFiltersPaginator

Type annotations and code completion for `#!python session.client("guardduty").get_paginator("list_filters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFilters)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_guardduty.paginator import ListFiltersPaginator

session = Session()

session = get_session()
async with session.client("guardduty") as client:  # (1)
    paginator: ListFiltersPaginator = client.get_paginator("list_filters")  # (2)
    async for item in paginator.paginate(...):
        item: ListFiltersResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
2. paginator: [ListFiltersPaginator](./paginators.md#listfilterspaginator)
3. item: [:material-code-braces: ListFiltersResponseTypeDef](./type_defs.md#listfiltersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFiltersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DetectorId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListFiltersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFiltersResponseTypeDef](./type_defs.md#listfiltersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListFiltersRequestListFiltersPaginateTypeDef = {  # (1)
    "DetectorId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFiltersRequestListFiltersPaginateTypeDef](./type_defs.md#listfiltersrequestlistfilterspaginatetypedef) 
## ListFindingsPaginator

Type annotations and code completion for `#!python session.client("guardduty").get_paginator("list_findings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFindings)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_guardduty.paginator import ListFindingsPaginator

session = Session()

session = get_session()
async with session.client("guardduty") as client:  # (1)
    paginator: ListFindingsPaginator = client.get_paginator("list_findings")  # (2)
    async for item in paginator.paginate(...):
        item: ListFindingsResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
2. paginator: [ListFindingsPaginator](./paginators.md#listfindingspaginator)
3. item: [:material-code-braces: ListFindingsResponseTypeDef](./type_defs.md#listfindingsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFindingsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DetectorId: str,
    FindingCriteria: FindingCriteriaTypeDef = ...,  # (1)
    SortCriteria: SortCriteriaTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListFindingsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FindingCriteriaTypeDef](./type_defs.md#findingcriteriatypedef) 
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListFindingsResponseTypeDef](./type_defs.md#listfindingsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListFindingsRequestListFindingsPaginateTypeDef = {  # (1)
    "DetectorId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFindingsRequestListFindingsPaginateTypeDef](./type_defs.md#listfindingsrequestlistfindingspaginatetypedef) 
## ListIPSetsPaginator

Type annotations and code completion for `#!python session.client("guardduty").get_paginator("list_ip_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListIPSets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_guardduty.paginator import ListIPSetsPaginator

session = Session()

session = get_session()
async with session.client("guardduty") as client:  # (1)
    paginator: ListIPSetsPaginator = client.get_paginator("list_ip_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListIPSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
2. paginator: [ListIPSetsPaginator](./paginators.md#listipsetspaginator)
3. item: [:material-code-braces: ListIPSetsResponseTypeDef](./type_defs.md#listipsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListIPSetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DetectorId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListIPSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIPSetsResponseTypeDef](./type_defs.md#listipsetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListIPSetsRequestListIPSetsPaginateTypeDef = {  # (1)
    "DetectorId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIPSetsRequestListIPSetsPaginateTypeDef](./type_defs.md#listipsetsrequestlistipsetspaginatetypedef) 
## ListInvitationsPaginator

Type annotations and code completion for `#!python session.client("guardduty").get_paginator("list_invitations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListInvitations)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_guardduty.paginator import ListInvitationsPaginator

session = Session()

session = get_session()
async with session.client("guardduty") as client:  # (1)
    paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")  # (2)
    async for item in paginator.paginate(...):
        item: ListInvitationsResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
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

Type annotations and code completion for `#!python session.client("guardduty").get_paginator("list_members")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListMembers)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_guardduty.paginator import ListMembersPaginator

session = Session()

session = get_session()
async with session.client("guardduty") as client:  # (1)
    paginator: ListMembersPaginator = client.get_paginator("list_members")  # (2)
    async for item in paginator.paginate(...):
        item: ListMembersResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
2. paginator: [ListMembersPaginator](./paginators.md#listmemberspaginator)
3. item: [:material-code-braces: ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMembersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DetectorId: str,
    OnlyAssociated: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMembersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListMembersRequestListMembersPaginateTypeDef = {  # (1)
    "DetectorId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMembersRequestListMembersPaginateTypeDef](./type_defs.md#listmembersrequestlistmemberspaginatetypedef) 
## ListOrganizationAdminAccountsPaginator

Type annotations and code completion for `#!python session.client("guardduty").get_paginator("list_organization_admin_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListOrganizationAdminAccounts)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_guardduty.paginator import ListOrganizationAdminAccountsPaginator

session = Session()

session = get_session()
async with session.client("guardduty") as client:  # (1)
    paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListOrganizationAdminAccountsResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
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
## ListThreatIntelSetsPaginator

Type annotations and code completion for `#!python session.client("guardduty").get_paginator("list_threat_intel_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListThreatIntelSets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_guardduty.paginator import ListThreatIntelSetsPaginator

session = Session()

session = get_session()
async with session.client("guardduty") as client:  # (1)
    paginator: ListThreatIntelSetsPaginator = client.get_paginator("list_threat_intel_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListThreatIntelSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
2. paginator: [ListThreatIntelSetsPaginator](./paginators.md#listthreatintelsetspaginator)
3. item: [:material-code-braces: ListThreatIntelSetsResponseTypeDef](./type_defs.md#listthreatintelsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListThreatIntelSetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DetectorId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListThreatIntelSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListThreatIntelSetsResponseTypeDef](./type_defs.md#listthreatintelsetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = {  # (1)
    "DetectorId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef](./type_defs.md#listthreatintelsetsrequestlistthreatintelsetspaginatetypedef) 
