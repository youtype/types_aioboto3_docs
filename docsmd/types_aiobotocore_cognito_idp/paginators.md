# Paginators

> [Index](../README.md) > [CognitoIdentityProvider](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CognitoIdentityProvider](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
    type annotations stubs module [types-aiobotocore-cognito-idp](https://pypi.org/project/types-aiobotocore-cognito-idp/).

## AdminListGroupsForUserPaginator

Type annotations and code completion for `#!python session.client("cognito-idp").get_paginator("admin_list_groups_for_user")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_cognito_idp.paginator import AdminListGroupsForUserPaginator

session = Session()

session = get_session()
async with session.client("cognito-idp") as client:  # (1)
    paginator: AdminListGroupsForUserPaginator = client.get_paginator("admin_list_groups_for_user")  # (2)
    async for item in paginator.paginate(...):
        item: AdminListGroupsForUserResponseTypeDef
        print(item)  # (3)
```

1. client: [CognitoIdentityProviderClient](./client.md)
2. paginator: [AdminListGroupsForUserPaginator](./paginators.md#adminlistgroupsforuserpaginator)
3. item: [:material-code-braces: AdminListGroupsForUserResponseTypeDef](./type_defs.md#adminlistgroupsforuserresponsetypedef) 


### paginate

Type annotations and code completion for `#!python AdminListGroupsForUserPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Username: str,
    UserPoolId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[AdminListGroupsForUserResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: AdminListGroupsForUserResponseTypeDef](./type_defs.md#adminlistgroupsforuserresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = {  # (1)
    "Username": ...,
    "UserPoolId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef](./type_defs.md#adminlistgroupsforuserrequestadminlistgroupsforuserpaginatetypedef) 
## AdminListUserAuthEventsPaginator

Type annotations and code completion for `#!python session.client("cognito-idp").get_paginator("admin_list_user_auth_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_cognito_idp.paginator import AdminListUserAuthEventsPaginator

session = Session()

session = get_session()
async with session.client("cognito-idp") as client:  # (1)
    paginator: AdminListUserAuthEventsPaginator = client.get_paginator("admin_list_user_auth_events")  # (2)
    async for item in paginator.paginate(...):
        item: AdminListUserAuthEventsResponseTypeDef
        print(item)  # (3)
```

1. client: [CognitoIdentityProviderClient](./client.md)
2. paginator: [AdminListUserAuthEventsPaginator](./paginators.md#adminlistuserautheventspaginator)
3. item: [:material-code-braces: AdminListUserAuthEventsResponseTypeDef](./type_defs.md#adminlistuserautheventsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python AdminListUserAuthEventsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    UserPoolId: str,
    Username: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[AdminListUserAuthEventsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: AdminListUserAuthEventsResponseTypeDef](./type_defs.md#adminlistuserautheventsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef](./type_defs.md#adminlistuserautheventsrequestadminlistuserautheventspaginatetypedef) 
## ListGroupsPaginator

Type annotations and code completion for `#!python session.client("cognito-idp").get_paginator("list_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_cognito_idp.paginator import ListGroupsPaginator

session = Session()

session = get_session()
async with session.client("cognito-idp") as client:  # (1)
    paginator: ListGroupsPaginator = client.get_paginator("list_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [CognitoIdentityProviderClient](./client.md)
2. paginator: [ListGroupsPaginator](./paginators.md#listgroupspaginator)
3. item: [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    UserPoolId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListGroupsRequestListGroupsPaginateTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestListGroupsPaginateTypeDef](./type_defs.md#listgroupsrequestlistgroupspaginatetypedef) 
## ListIdentityProvidersPaginator

Type annotations and code completion for `#!python session.client("cognito-idp").get_paginator("list_identity_providers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_cognito_idp.paginator import ListIdentityProvidersPaginator

session = Session()

session = get_session()
async with session.client("cognito-idp") as client:  # (1)
    paginator: ListIdentityProvidersPaginator = client.get_paginator("list_identity_providers")  # (2)
    async for item in paginator.paginate(...):
        item: ListIdentityProvidersResponseTypeDef
        print(item)  # (3)
```

1. client: [CognitoIdentityProviderClient](./client.md)
2. paginator: [ListIdentityProvidersPaginator](./paginators.md#listidentityproviderspaginator)
3. item: [:material-code-braces: ListIdentityProvidersResponseTypeDef](./type_defs.md#listidentityprovidersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListIdentityProvidersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    UserPoolId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListIdentityProvidersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIdentityProvidersResponseTypeDef](./type_defs.md#listidentityprovidersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef](./type_defs.md#listidentityprovidersrequestlistidentityproviderspaginatetypedef) 
## ListResourceServersPaginator

Type annotations and code completion for `#!python session.client("cognito-idp").get_paginator("list_resource_servers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_cognito_idp.paginator import ListResourceServersPaginator

session = Session()

session = get_session()
async with session.client("cognito-idp") as client:  # (1)
    paginator: ListResourceServersPaginator = client.get_paginator("list_resource_servers")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceServersResponseTypeDef
        print(item)  # (3)
```

1. client: [CognitoIdentityProviderClient](./client.md)
2. paginator: [ListResourceServersPaginator](./paginators.md#listresourceserverspaginator)
3. item: [:material-code-braces: ListResourceServersResponseTypeDef](./type_defs.md#listresourceserversresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResourceServersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    UserPoolId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListResourceServersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResourceServersResponseTypeDef](./type_defs.md#listresourceserversresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListResourceServersRequestListResourceServersPaginateTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceServersRequestListResourceServersPaginateTypeDef](./type_defs.md#listresourceserversrequestlistresourceserverspaginatetypedef) 
## ListUserPoolClientsPaginator

Type annotations and code completion for `#!python session.client("cognito-idp").get_paginator("list_user_pool_clients")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_cognito_idp.paginator import ListUserPoolClientsPaginator

session = Session()

session = get_session()
async with session.client("cognito-idp") as client:  # (1)
    paginator: ListUserPoolClientsPaginator = client.get_paginator("list_user_pool_clients")  # (2)
    async for item in paginator.paginate(...):
        item: ListUserPoolClientsResponseTypeDef
        print(item)  # (3)
```

1. client: [CognitoIdentityProviderClient](./client.md)
2. paginator: [ListUserPoolClientsPaginator](./paginators.md#listuserpoolclientspaginator)
3. item: [:material-code-braces: ListUserPoolClientsResponseTypeDef](./type_defs.md#listuserpoolclientsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUserPoolClientsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    UserPoolId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListUserPoolClientsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUserPoolClientsResponseTypeDef](./type_defs.md#listuserpoolclientsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef](./type_defs.md#listuserpoolclientsrequestlistuserpoolclientspaginatetypedef) 
## ListUserPoolsPaginator

Type annotations and code completion for `#!python session.client("cognito-idp").get_paginator("list_user_pools")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_cognito_idp.paginator import ListUserPoolsPaginator

session = Session()

session = get_session()
async with session.client("cognito-idp") as client:  # (1)
    paginator: ListUserPoolsPaginator = client.get_paginator("list_user_pools")  # (2)
    async for item in paginator.paginate(...):
        item: ListUserPoolsResponseTypeDef
        print(item)  # (3)
```

1. client: [CognitoIdentityProviderClient](./client.md)
2. paginator: [ListUserPoolsPaginator](./paginators.md#listuserpoolspaginator)
3. item: [:material-code-braces: ListUserPoolsResponseTypeDef](./type_defs.md#listuserpoolsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUserPoolsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListUserPoolsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUserPoolsResponseTypeDef](./type_defs.md#listuserpoolsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListUserPoolsRequestListUserPoolsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUserPoolsRequestListUserPoolsPaginateTypeDef](./type_defs.md#listuserpoolsrequestlistuserpoolspaginatetypedef) 
## ListUsersPaginator

Type annotations and code completion for `#!python session.client("cognito-idp").get_paginator("list_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsers)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_cognito_idp.paginator import ListUsersPaginator

session = Session()

session = get_session()
async with session.client("cognito-idp") as client:  # (1)
    paginator: ListUsersPaginator = client.get_paginator("list_users")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [CognitoIdentityProviderClient](./client.md)
2. paginator: [ListUsersPaginator](./paginators.md#listuserspaginator)
3. item: [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUsersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    UserPoolId: str,
    AttributesToGet: Sequence[str] = ...,
    Filter: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListUsersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListUsersRequestListUsersPaginateTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestListUsersPaginateTypeDef](./type_defs.md#listusersrequestlistuserspaginatetypedef) 
## ListUsersInGroupPaginator

Type annotations and code completion for `#!python session.client("cognito-idp").get_paginator("list_users_in_group")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_cognito_idp.paginator import ListUsersInGroupPaginator

session = Session()

session = get_session()
async with session.client("cognito-idp") as client:  # (1)
    paginator: ListUsersInGroupPaginator = client.get_paginator("list_users_in_group")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsersInGroupResponseTypeDef
        print(item)  # (3)
```

1. client: [CognitoIdentityProviderClient](./client.md)
2. paginator: [ListUsersInGroupPaginator](./paginators.md#listusersingrouppaginator)
3. item: [:material-code-braces: ListUsersInGroupResponseTypeDef](./type_defs.md#listusersingroupresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUsersInGroupPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    UserPoolId: str,
    GroupName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListUsersInGroupResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUsersInGroupResponseTypeDef](./type_defs.md#listusersingroupresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListUsersInGroupRequestListUsersInGroupPaginateTypeDef = {  # (1)
    "UserPoolId": ...,
    "GroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsersInGroupRequestListUsersInGroupPaginateTypeDef](./type_defs.md#listusersingrouprequestlistusersingrouppaginatetypedef) 
