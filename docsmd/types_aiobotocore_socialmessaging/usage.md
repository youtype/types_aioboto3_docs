# Examples

> [Index](../README.md) > [EndUserMessagingSocial](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EndUserMessagingSocial](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging.html#endusermessagingsocial)
    type annotations stubs module [types-aiobotocore-socialmessaging](https://pypi.org/project/types-aiobotocore-socialmessaging/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[socialmessaging]` package installed.

Write your `EndUserMessagingSocial` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# EndUserMessagingSocialClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("socialmessaging") as client:  # (1)
    result = await client.associate_whatsapp_business_account()  # (2)
```

1. client: [EndUserMessagingSocialClient](./client.md)
2. result: [:material-code-braces: AssociateWhatsAppBusinessAccountOutputTypeDef](./type_defs.md#associatewhatsappbusinessaccountoutputtypedef)



#### Paginator usage example

```python
# ListLinkedWhatsAppBusinessAccountsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("socialmessaging") as client:  # (1)
    paginator = client.get_paginator("list_linked_whatsapp_business_accounts")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [EndUserMessagingSocialClient](./client.md)
2. paginator: [ListLinkedWhatsAppBusinessAccountsPaginator](./paginators.md#listlinkedwhatsappbusinessaccountspaginator)
3. item: [:material-code-braces: ListLinkedWhatsAppBusinessAccountsOutputTypeDef](./type_defs.md#listlinkedwhatsappbusinessaccountsoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[socialmessaging]`
or a standalone `types_aiobotocore_socialmessaging` package, you have to explicitly specify
`client: EndUserMessagingSocialClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# EndUserMessagingSocialClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_socialmessaging.client import EndUserMessagingSocialClient
from types_aiobotocore_socialmessaging.type_defs import AssociateWhatsAppBusinessAccountOutputTypeDef
from types_aiobotocore_socialmessaging.type_defs import AssociateWhatsAppBusinessAccountInputTypeDef


session = Session()

client: EndUserMessagingSocialClient
async with session.client("socialmessaging") as client:  # (1)
    kwargs: AssociateWhatsAppBusinessAccountInputTypeDef = {...}  # (2)
    result: AssociateWhatsAppBusinessAccountOutputTypeDef = await client.associate_whatsapp_business_account(**kwargs)  # (3)
```

1. client: [EndUserMessagingSocialClient](./client.md)
2. kwargs: [:material-code-braces: AssociateWhatsAppBusinessAccountInputTypeDef](./type_defs.md#associatewhatsappbusinessaccountinputtypedef)
3. result: [:material-code-braces: AssociateWhatsAppBusinessAccountOutputTypeDef](./type_defs.md#associatewhatsappbusinessaccountoutputtypedef)



#### Paginator usage example

```python
# ListLinkedWhatsAppBusinessAccountsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_socialmessaging.client import EndUserMessagingSocialClient
from types_aiobotocore_socialmessaging.paginator import ListLinkedWhatsAppBusinessAccountsPaginator
from types_aiobotocore_socialmessaging.type_defs import ListLinkedWhatsAppBusinessAccountsOutputTypeDef


session = Session()

client: EndUserMessagingSocialClient
async with session.client("socialmessaging") as client:  # (1)
    paginator: ListLinkedWhatsAppBusinessAccountsPaginator = client.get_paginator("list_linked_whatsapp_business_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListLinkedWhatsAppBusinessAccountsOutputTypeDef
        print(item)  # (3)
```

1. client: [EndUserMessagingSocialClient](./client.md)
2. paginator: [ListLinkedWhatsAppBusinessAccountsPaginator](./paginators.md#listlinkedwhatsappbusinessaccountspaginator)
3. item: [:material-code-braces: ListLinkedWhatsAppBusinessAccountsOutputTypeDef](./type_defs.md#listlinkedwhatsappbusinessaccountsoutputtypedef)




