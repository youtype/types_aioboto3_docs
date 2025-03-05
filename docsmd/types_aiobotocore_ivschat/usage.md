# Examples

> [Index](../README.md) > [Ivschat](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Ivschat](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
    type annotations stubs module [types-aiobotocore-ivschat](https://pypi.org/project/types-aiobotocore-ivschat/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[ivschat]` package installed.

Write your `Ivschat` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# IvschatClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("ivschat") as client:  # (1)
    result = await client.create_chat_token()  # (2)
```

1. client: [IvschatClient](./client.md)
2. result: [:material-code-braces: CreateChatTokenResponseTypeDef](./type_defs.md#createchattokenresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[ivschat]`
or a standalone `types_aiobotocore_ivschat` package, you have to explicitly specify
`client: IvschatClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# IvschatClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ivschat.client import IvschatClient
from types_aiobotocore_ivschat.type_defs import CreateChatTokenResponseTypeDef
from types_aiobotocore_ivschat.type_defs import CreateChatTokenRequestTypeDef


session = Session()

client: IvschatClient
async with session.client("ivschat") as client:  # (1)
    kwargs: CreateChatTokenRequestTypeDef = {...}  # (2)
    result: CreateChatTokenResponseTypeDef = await client.create_chat_token(**kwargs)  # (3)
```

1. client: [IvschatClient](./client.md)
2. kwargs: [:material-code-braces: CreateChatTokenRequestTypeDef](./type_defs.md#createchattokenrequesttypedef)
3. result: [:material-code-braces: CreateChatTokenResponseTypeDef](./type_defs.md#createchattokenresponsetypedef)






