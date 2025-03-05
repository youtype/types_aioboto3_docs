# Paginators

> [Index](../README.md) > [EndUserMessagingSocial](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [EndUserMessagingSocial](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging.html#endusermessagingsocial)
    type annotations stubs module [types-aiobotocore-socialmessaging](https://pypi.org/project/types-aiobotocore-socialmessaging/).

## ListLinkedWhatsAppBusinessAccountsPaginator

Type annotations and code completion for `#!python session.client("socialmessaging").get_paginator("list_linked_whatsapp_business_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging/paginator/ListLinkedWhatsAppBusinessAccounts.html#EndUserMessagingSocial.Paginator.ListLinkedWhatsAppBusinessAccounts)

```python
# ListLinkedWhatsAppBusinessAccountsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_socialmessaging.paginator import ListLinkedWhatsAppBusinessAccountsPaginator

session = Session()

session = get_session()
async with session.client("socialmessaging") as client:  # (1)
    paginator: ListLinkedWhatsAppBusinessAccountsPaginator = client.get_paginator("list_linked_whatsapp_business_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListLinkedWhatsAppBusinessAccountsOutputTypeDef
        print(item)  # (3)
```

1. client: [EndUserMessagingSocialClient](./client.md)
2. paginator: [ListLinkedWhatsAppBusinessAccountsPaginator](./paginators.md#listlinkedwhatsappbusinessaccountspaginator)
3. item: `AioPageIterator[ListLinkedWhatsAppBusinessAccountsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListLinkedWhatsAppBusinessAccountsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListLinkedWhatsAppBusinessAccountsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListLinkedWhatsAppBusinessAccountsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListLinkedWhatsAppBusinessAccountsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLinkedWhatsAppBusinessAccountsInputPaginateTypeDef](./type_defs.md#listlinkedwhatsappbusinessaccountsinputpaginatetypedef)
