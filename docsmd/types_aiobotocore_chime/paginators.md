# Paginators

> [Index](../README.md) > [Chime](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Chime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#chime)
    type annotations stubs module [types-aiobotocore-chime](https://pypi.org/project/types-aiobotocore-chime/).

## ListAccountsPaginator

Type annotations and code completion for `#!python session.client("chime").get_paginator("list_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/paginator/ListAccounts.html#Chime.Paginator.ListAccounts)

```python
# ListAccountsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_chime.paginator import ListAccountsPaginator

session = Session()

session = get_session()
async with session.client("chime") as client:  # (1)
    paginator: ListAccountsPaginator = client.get_paginator("list_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccountsResponseTypeDef
        print(item)  # (3)
```

1. client: [ChimeClient](./client.md)
2. paginator: [ListAccountsPaginator](./paginators.md#listaccountspaginator)
3. item: [:material-code-braces: ListAccountsResponseTypeDef](./type_defs.md#listaccountsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAccountsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Name: str = ...,
    UserEmail: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccountsResponseTypeDef](./type_defs.md#listaccountsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAccountsRequestPaginateTypeDef = {  # (1)
    "Name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountsRequestPaginateTypeDef](./type_defs.md#listaccountsrequestpaginatetypedef) 
## ListUsersPaginator

Type annotations and code completion for `#!python session.client("chime").get_paginator("list_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/paginator/ListUsers.html#Chime.Paginator.ListUsers)

```python
# ListUsersPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_chime.paginator import ListUsersPaginator

session = Session()

session = get_session()
async with session.client("chime") as client:  # (1)
    paginator: ListUsersPaginator = client.get_paginator("list_users")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [ChimeClient](./client.md)
2. paginator: [ListUsersPaginator](./paginators.md#listuserspaginator)
3. item: [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountId: str,
    UserEmail: str = ...,
    UserType: UserTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListUsersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListUsersRequestPaginateTypeDef = {  # (1)
    "AccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestPaginateTypeDef](./type_defs.md#listusersrequestpaginatetypedef) 