# Paginators

> [Index](../README.md) > [IAM](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IAM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
    type annotations stubs module [types-aiobotocore-iam](https://pypi.org/project/types-aiobotocore-iam/).

## GetAccountAuthorizationDetailsPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("get_account_authorization_details")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetAccountAuthorizationDetails)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import GetAccountAuthorizationDetailsPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: GetAccountAuthorizationDetailsPaginator = client.get_paginator("get_account_authorization_details")  # (2)
    async for item in paginator.paginate(...):
        item: GetAccountAuthorizationDetailsResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [GetAccountAuthorizationDetailsPaginator](./paginators.md#getaccountauthorizationdetailspaginator)
3. item: [:material-code-braces: GetAccountAuthorizationDetailsResponseTypeDef](./type_defs.md#getaccountauthorizationdetailsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetAccountAuthorizationDetailsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filter: Sequence[EntityTypeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetAccountAuthorizationDetailsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetAccountAuthorizationDetailsResponseTypeDef](./type_defs.md#getaccountauthorizationdetailsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef](./type_defs.md#getaccountauthorizationdetailsrequestgetaccountauthorizationdetailspaginatetypedef) 
## GetGroupPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("get_group")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetGroup)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import GetGroupPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: GetGroupPaginator = client.get_paginator("get_group")  # (2)
    async for item in paginator.paginate(...):
        item: GetGroupResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [GetGroupPaginator](./paginators.md#getgrouppaginator)
3. item: [:material-code-braces: GetGroupResponseTypeDef](./type_defs.md#getgroupresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetGroupPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GroupName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetGroupResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetGroupResponseTypeDef](./type_defs.md#getgroupresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetGroupRequestGetGroupPaginateTypeDef = {  # (1)
    "GroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetGroupRequestGetGroupPaginateTypeDef](./type_defs.md#getgrouprequestgetgrouppaginatetypedef) 
## ListAccessKeysPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_access_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccessKeys)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListAccessKeysPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListAccessKeysPaginator = client.get_paginator("list_access_keys")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccessKeysResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListAccessKeysPaginator](./paginators.md#listaccesskeyspaginator)
3. item: [:material-code-braces: ListAccessKeysResponseTypeDef](./type_defs.md#listaccesskeysresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAccessKeysPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    UserName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAccessKeysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccessKeysResponseTypeDef](./type_defs.md#listaccesskeysresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAccessKeysRequestListAccessKeysPaginateTypeDef = {  # (1)
    "UserName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccessKeysRequestListAccessKeysPaginateTypeDef](./type_defs.md#listaccesskeysrequestlistaccesskeyspaginatetypedef) 
## ListAccountAliasesPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_account_aliases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccountAliases)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListAccountAliasesPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListAccountAliasesPaginator = client.get_paginator("list_account_aliases")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccountAliasesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListAccountAliasesPaginator](./paginators.md#listaccountaliasespaginator)
3. item: [:material-code-braces: ListAccountAliasesResponseTypeDef](./type_defs.md#listaccountaliasesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAccountAliasesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAccountAliasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccountAliasesResponseTypeDef](./type_defs.md#listaccountaliasesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAccountAliasesRequestListAccountAliasesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountAliasesRequestListAccountAliasesPaginateTypeDef](./type_defs.md#listaccountaliasesrequestlistaccountaliasespaginatetypedef) 
## ListAttachedGroupPoliciesPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_attached_group_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedGroupPolicies)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListAttachedGroupPoliciesPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListAttachedGroupPoliciesPaginator = client.get_paginator("list_attached_group_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListAttachedGroupPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListAttachedGroupPoliciesPaginator](./paginators.md#listattachedgrouppoliciespaginator)
3. item: [:material-code-braces: ListAttachedGroupPoliciesResponseTypeDef](./type_defs.md#listattachedgrouppoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAttachedGroupPoliciesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GroupName: str,
    PathPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAttachedGroupPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAttachedGroupPoliciesResponseTypeDef](./type_defs.md#listattachedgrouppoliciesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef = {  # (1)
    "GroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef](./type_defs.md#listattachedgrouppoliciesrequestlistattachedgrouppoliciespaginatetypedef) 
## ListAttachedRolePoliciesPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_attached_role_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedRolePolicies)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListAttachedRolePoliciesPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListAttachedRolePoliciesPaginator = client.get_paginator("list_attached_role_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListAttachedRolePoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListAttachedRolePoliciesPaginator](./paginators.md#listattachedrolepoliciespaginator)
3. item: [:material-code-braces: ListAttachedRolePoliciesResponseTypeDef](./type_defs.md#listattachedrolepoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAttachedRolePoliciesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    RoleName: str,
    PathPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAttachedRolePoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAttachedRolePoliciesResponseTypeDef](./type_defs.md#listattachedrolepoliciesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef = {  # (1)
    "RoleName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef](./type_defs.md#listattachedrolepoliciesrequestlistattachedrolepoliciespaginatetypedef) 
## ListAttachedUserPoliciesPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_attached_user_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedUserPolicies)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListAttachedUserPoliciesPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListAttachedUserPoliciesPaginator = client.get_paginator("list_attached_user_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListAttachedUserPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListAttachedUserPoliciesPaginator](./paginators.md#listattacheduserpoliciespaginator)
3. item: [:material-code-braces: ListAttachedUserPoliciesResponseTypeDef](./type_defs.md#listattacheduserpoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAttachedUserPoliciesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    UserName: str,
    PathPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAttachedUserPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAttachedUserPoliciesResponseTypeDef](./type_defs.md#listattacheduserpoliciesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef = {  # (1)
    "UserName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef](./type_defs.md#listattacheduserpoliciesrequestlistattacheduserpoliciespaginatetypedef) 
## ListEntitiesForPolicyPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_entities_for_policy")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListEntitiesForPolicy)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListEntitiesForPolicyPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListEntitiesForPolicyPaginator = client.get_paginator("list_entities_for_policy")  # (2)
    async for item in paginator.paginate(...):
        item: ListEntitiesForPolicyResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListEntitiesForPolicyPaginator](./paginators.md#listentitiesforpolicypaginator)
3. item: [:material-code-braces: ListEntitiesForPolicyResponseTypeDef](./type_defs.md#listentitiesforpolicyresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEntitiesForPolicyPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PolicyArn: str,
    EntityFilter: EntityTypeType = ...,  # (1)
    PathPrefix: str = ...,
    PolicyUsageFilter: PolicyUsageTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListEntitiesForPolicyResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
2. See [:material-code-brackets: PolicyUsageTypeType](./literals.md#policyusagetypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListEntitiesForPolicyResponseTypeDef](./type_defs.md#listentitiesforpolicyresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef = {  # (1)
    "PolicyArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef](./type_defs.md#listentitiesforpolicyrequestlistentitiesforpolicypaginatetypedef) 
## ListGroupPoliciesPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_group_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupPolicies)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListGroupPoliciesPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListGroupPoliciesPaginator = client.get_paginator("list_group_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListGroupPoliciesPaginator](./paginators.md#listgrouppoliciespaginator)
3. item: [:material-code-braces: ListGroupPoliciesResponseTypeDef](./type_defs.md#listgrouppoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupPoliciesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GroupName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGroupPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGroupPoliciesResponseTypeDef](./type_defs.md#listgrouppoliciesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef = {  # (1)
    "GroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef](./type_defs.md#listgrouppoliciesrequestlistgrouppoliciespaginatetypedef) 
## ListGroupsPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroups)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListGroupsPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListGroupsPaginator = client.get_paginator("list_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListGroupsPaginator](./paginators.md#listgroupspaginator)
3. item: [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PathPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListGroupsRequestListGroupsPaginateTypeDef = {  # (1)
    "PathPrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestListGroupsPaginateTypeDef](./type_defs.md#listgroupsrequestlistgroupspaginatetypedef) 
## ListGroupsForUserPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_groups_for_user")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupsForUser)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListGroupsForUserPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListGroupsForUserPaginator = client.get_paginator("list_groups_for_user")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupsForUserResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListGroupsForUserPaginator](./paginators.md#listgroupsforuserpaginator)
3. item: [:material-code-braces: ListGroupsForUserResponseTypeDef](./type_defs.md#listgroupsforuserresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupsForUserPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    UserName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGroupsForUserResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGroupsForUserResponseTypeDef](./type_defs.md#listgroupsforuserresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListGroupsForUserRequestListGroupsForUserPaginateTypeDef = {  # (1)
    "UserName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupsForUserRequestListGroupsForUserPaginateTypeDef](./type_defs.md#listgroupsforuserrequestlistgroupsforuserpaginatetypedef) 
## ListInstanceProfilesPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_instance_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfiles)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListInstanceProfilesPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListInstanceProfilesPaginator = client.get_paginator("list_instance_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstanceProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListInstanceProfilesPaginator](./paginators.md#listinstanceprofilespaginator)
3. item: [:material-code-braces: ListInstanceProfilesResponseTypeDef](./type_defs.md#listinstanceprofilesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInstanceProfilesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PathPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListInstanceProfilesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInstanceProfilesResponseTypeDef](./type_defs.md#listinstanceprofilesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = {  # (1)
    "PathPrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef](./type_defs.md#listinstanceprofilesrequestlistinstanceprofilespaginatetypedef) 
## ListInstanceProfilesForRolePaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_instance_profiles_for_role")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfilesForRole)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListInstanceProfilesForRolePaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListInstanceProfilesForRolePaginator = client.get_paginator("list_instance_profiles_for_role")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstanceProfilesForRoleResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListInstanceProfilesForRolePaginator](./paginators.md#listinstanceprofilesforrolepaginator)
3. item: [:material-code-braces: ListInstanceProfilesForRoleResponseTypeDef](./type_defs.md#listinstanceprofilesforroleresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInstanceProfilesForRolePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    RoleName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListInstanceProfilesForRoleResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInstanceProfilesForRoleResponseTypeDef](./type_defs.md#listinstanceprofilesforroleresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef = {  # (1)
    "RoleName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef](./type_defs.md#listinstanceprofilesforrolerequestlistinstanceprofilesforrolepaginatetypedef) 
## ListMFADevicesPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_mfa_devices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADevices)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListMFADevicesPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListMFADevicesPaginator = client.get_paginator("list_mfa_devices")  # (2)
    async for item in paginator.paginate(...):
        item: ListMFADevicesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListMFADevicesPaginator](./paginators.md#listmfadevicespaginator)
3. item: [:material-code-braces: ListMFADevicesResponseTypeDef](./type_defs.md#listmfadevicesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMFADevicesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    UserName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMFADevicesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMFADevicesResponseTypeDef](./type_defs.md#listmfadevicesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListMFADevicesRequestListMFADevicesPaginateTypeDef = {  # (1)
    "UserName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMFADevicesRequestListMFADevicesPaginateTypeDef](./type_defs.md#listmfadevicesrequestlistmfadevicespaginatetypedef) 
## ListPoliciesPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicies)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListPoliciesPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListPoliciesPaginator = client.get_paginator("list_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListPoliciesPaginator](./paginators.md#listpoliciespaginator)
3. item: [:material-code-braces: ListPoliciesResponseTypeDef](./type_defs.md#listpoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPoliciesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Scope: policyScopeTypeType = ...,  # (1)
    OnlyAttached: bool = ...,
    PathPrefix: str = ...,
    PolicyUsageFilter: PolicyUsageTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListPoliciesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: policyScopeTypeType](./literals.md#policyscopetypetype) 
2. See [:material-code-brackets: PolicyUsageTypeType](./literals.md#policyusagetypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListPoliciesResponseTypeDef](./type_defs.md#listpoliciesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPoliciesRequestListPoliciesPaginateTypeDef = {  # (1)
    "Scope": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPoliciesRequestListPoliciesPaginateTypeDef](./type_defs.md#listpoliciesrequestlistpoliciespaginatetypedef) 
## ListPolicyVersionsPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_policy_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyVersions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListPolicyVersionsPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListPolicyVersionsPaginator = client.get_paginator("list_policy_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListPolicyVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListPolicyVersionsPaginator](./paginators.md#listpolicyversionspaginator)
3. item: [:material-code-braces: ListPolicyVersionsResponseTypeDef](./type_defs.md#listpolicyversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPolicyVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PolicyArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPolicyVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPolicyVersionsResponseTypeDef](./type_defs.md#listpolicyversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef = {  # (1)
    "PolicyArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef](./type_defs.md#listpolicyversionsrequestlistpolicyversionspaginatetypedef) 
## ListRolePoliciesPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_role_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRolePolicies)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListRolePoliciesPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListRolePoliciesPaginator = client.get_paginator("list_role_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListRolePoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListRolePoliciesPaginator](./paginators.md#listrolepoliciespaginator)
3. item: [:material-code-braces: ListRolePoliciesResponseTypeDef](./type_defs.md#listrolepoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRolePoliciesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    RoleName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRolePoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRolePoliciesResponseTypeDef](./type_defs.md#listrolepoliciesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRolePoliciesRequestListRolePoliciesPaginateTypeDef = {  # (1)
    "RoleName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRolePoliciesRequestListRolePoliciesPaginateTypeDef](./type_defs.md#listrolepoliciesrequestlistrolepoliciespaginatetypedef) 
## ListRolesPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_roles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoles)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListRolesPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListRolesPaginator = client.get_paginator("list_roles")  # (2)
    async for item in paginator.paginate(...):
        item: ListRolesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListRolesPaginator](./paginators.md#listrolespaginator)
3. item: [:material-code-braces: ListRolesResponseTypeDef](./type_defs.md#listrolesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRolesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PathPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRolesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRolesResponseTypeDef](./type_defs.md#listrolesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRolesRequestListRolesPaginateTypeDef = {  # (1)
    "PathPrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRolesRequestListRolesPaginateTypeDef](./type_defs.md#listrolesrequestlistrolespaginatetypedef) 
## ListSSHPublicKeysPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_ssh_public_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSSHPublicKeys)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListSSHPublicKeysPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListSSHPublicKeysPaginator = client.get_paginator("list_ssh_public_keys")  # (2)
    async for item in paginator.paginate(...):
        item: ListSSHPublicKeysResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListSSHPublicKeysPaginator](./paginators.md#listsshpublickeyspaginator)
3. item: [:material-code-braces: ListSSHPublicKeysResponseTypeDef](./type_defs.md#listsshpublickeysresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSSHPublicKeysPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    UserName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSSHPublicKeysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSSHPublicKeysResponseTypeDef](./type_defs.md#listsshpublickeysresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef = {  # (1)
    "UserName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef](./type_defs.md#listsshpublickeysrequestlistsshpublickeyspaginatetypedef) 
## ListServerCertificatesPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_server_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificates)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListServerCertificatesPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListServerCertificatesPaginator = client.get_paginator("list_server_certificates")  # (2)
    async for item in paginator.paginate(...):
        item: ListServerCertificatesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListServerCertificatesPaginator](./paginators.md#listservercertificatespaginator)
3. item: [:material-code-braces: ListServerCertificatesResponseTypeDef](./type_defs.md#listservercertificatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListServerCertificatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PathPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListServerCertificatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListServerCertificatesResponseTypeDef](./type_defs.md#listservercertificatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListServerCertificatesRequestListServerCertificatesPaginateTypeDef = {  # (1)
    "PathPrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListServerCertificatesRequestListServerCertificatesPaginateTypeDef](./type_defs.md#listservercertificatesrequestlistservercertificatespaginatetypedef) 
## ListSigningCertificatesPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_signing_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSigningCertificates)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListSigningCertificatesPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListSigningCertificatesPaginator = client.get_paginator("list_signing_certificates")  # (2)
    async for item in paginator.paginate(...):
        item: ListSigningCertificatesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListSigningCertificatesPaginator](./paginators.md#listsigningcertificatespaginator)
3. item: [:material-code-braces: ListSigningCertificatesResponseTypeDef](./type_defs.md#listsigningcertificatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSigningCertificatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    UserName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSigningCertificatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSigningCertificatesResponseTypeDef](./type_defs.md#listsigningcertificatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef = {  # (1)
    "UserName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef](./type_defs.md#listsigningcertificatesrequestlistsigningcertificatespaginatetypedef) 
## ListUserPoliciesPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_user_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserPolicies)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListUserPoliciesPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListUserPoliciesPaginator = client.get_paginator("list_user_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListUserPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListUserPoliciesPaginator](./paginators.md#listuserpoliciespaginator)
3. item: [:material-code-braces: ListUserPoliciesResponseTypeDef](./type_defs.md#listuserpoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUserPoliciesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    UserName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListUserPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUserPoliciesResponseTypeDef](./type_defs.md#listuserpoliciesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListUserPoliciesRequestListUserPoliciesPaginateTypeDef = {  # (1)
    "UserName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUserPoliciesRequestListUserPoliciesPaginateTypeDef](./type_defs.md#listuserpoliciesrequestlistuserpoliciespaginatetypedef) 
## ListUserTagsPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_user_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserTags)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListUserTagsPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListUserTagsPaginator = client.get_paginator("list_user_tags")  # (2)
    async for item in paginator.paginate(...):
        item: ListUserTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListUserTagsPaginator](./paginators.md#listusertagspaginator)
3. item: [:material-code-braces: ListUserTagsResponseTypeDef](./type_defs.md#listusertagsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUserTagsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    UserName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListUserTagsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUserTagsResponseTypeDef](./type_defs.md#listusertagsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListUserTagsRequestListUserTagsPaginateTypeDef = {  # (1)
    "UserName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUserTagsRequestListUserTagsPaginateTypeDef](./type_defs.md#listusertagsrequestlistusertagspaginatetypedef) 
## ListUsersPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUsers)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListUsersPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListUsersPaginator = client.get_paginator("list_users")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListUsersPaginator](./paginators.md#listuserspaginator)
3. item: [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUsersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PathPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListUsersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListUsersRequestListUsersPaginateTypeDef = {  # (1)
    "PathPrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestListUsersPaginateTypeDef](./type_defs.md#listusersrequestlistuserspaginatetypedef) 
## ListVirtualMFADevicesPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("list_virtual_mfa_devices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListVirtualMFADevices)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import ListVirtualMFADevicesPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: ListVirtualMFADevicesPaginator = client.get_paginator("list_virtual_mfa_devices")  # (2)
    async for item in paginator.paginate(...):
        item: ListVirtualMFADevicesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [ListVirtualMFADevicesPaginator](./paginators.md#listvirtualmfadevicespaginator)
3. item: [:material-code-braces: ListVirtualMFADevicesResponseTypeDef](./type_defs.md#listvirtualmfadevicesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListVirtualMFADevicesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AssignmentStatus: assignmentStatusTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListVirtualMFADevicesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: assignmentStatusTypeType](./literals.md#assignmentstatustypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListVirtualMFADevicesResponseTypeDef](./type_defs.md#listvirtualmfadevicesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef = {  # (1)
    "AssignmentStatus": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef](./type_defs.md#listvirtualmfadevicesrequestlistvirtualmfadevicespaginatetypedef) 
## SimulateCustomPolicyPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("simulate_custom_policy")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.SimulateCustomPolicy)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import SimulateCustomPolicyPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: SimulateCustomPolicyPaginator = client.get_paginator("simulate_custom_policy")  # (2)
    async for item in paginator.paginate(...):
        item: SimulatePolicyResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [SimulateCustomPolicyPaginator](./paginators.md#simulatecustompolicypaginator)
3. item: [:material-code-braces: SimulatePolicyResponseTypeDef](./type_defs.md#simulatepolicyresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SimulateCustomPolicyPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PolicyInputList: Sequence[str],
    ActionNames: Sequence[str],
    PermissionsBoundaryPolicyInputList: Sequence[str] = ...,
    ResourceArns: Sequence[str] = ...,
    ResourcePolicy: str = ...,
    ResourceOwner: str = ...,
    CallerArn: str = ...,
    ContextEntries: Sequence[ContextEntryTypeDef] = ...,  # (1)
    ResourceHandlingOption: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[SimulatePolicyResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ContextEntryTypeDef](./type_defs.md#contextentrytypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SimulatePolicyResponseTypeDef](./type_defs.md#simulatepolicyresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef = {  # (1)
    "PolicyInputList": ...,
    "ActionNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef](./type_defs.md#simulatecustompolicyrequestsimulatecustompolicypaginatetypedef) 
## SimulatePrincipalPolicyPaginator

Type annotations and code completion for `#!python session.client("iam").get_paginator("simulate_principal_policy")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.SimulatePrincipalPolicy)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.paginator import SimulatePrincipalPolicyPaginator

session = Session()

session = get_session()
async with session.client("iam") as client:  # (1)
    paginator: SimulatePrincipalPolicyPaginator = client.get_paginator("simulate_principal_policy")  # (2)
    async for item in paginator.paginate(...):
        item: SimulatePolicyResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMClient](./client.md)
2. paginator: [SimulatePrincipalPolicyPaginator](./paginators.md#simulateprincipalpolicypaginator)
3. item: [:material-code-braces: SimulatePolicyResponseTypeDef](./type_defs.md#simulatepolicyresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SimulatePrincipalPolicyPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PolicySourceArn: str,
    ActionNames: Sequence[str],
    PolicyInputList: Sequence[str] = ...,
    PermissionsBoundaryPolicyInputList: Sequence[str] = ...,
    ResourceArns: Sequence[str] = ...,
    ResourcePolicy: str = ...,
    ResourceOwner: str = ...,
    CallerArn: str = ...,
    ContextEntries: Sequence[ContextEntryTypeDef] = ...,  # (1)
    ResourceHandlingOption: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[SimulatePolicyResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ContextEntryTypeDef](./type_defs.md#contextentrytypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SimulatePolicyResponseTypeDef](./type_defs.md#simulatepolicyresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef = {  # (1)
    "PolicySourceArn": ...,
    "ActionNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef](./type_defs.md#simulateprincipalpolicyrequestsimulateprincipalpolicypaginatetypedef) 
