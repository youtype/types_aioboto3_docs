# Examples

> [Index](../README.md) > [CodeCatalyst](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodeCatalyst](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#codecatalyst)
    type annotations stubs module [types-aiobotocore-codecatalyst](https://pypi.org/project/types-aiobotocore-codecatalyst/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[codecatalyst]` package installed.

Write your `CodeCatalyst` code as usual,
type checking and code completion should work out of the box.



```python
# CodeCatalystClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("codecatalyst") as client:  # (1)
    result = await client.create_access_token()  # (2)
```

1. client: [CodeCatalystClient](./client.md)
2. result: [:material-code-braces: CreateAccessTokenResponseTypeDef](./type_defs.md#createaccesstokenresponsetypedef) 



```python
# ListAccessTokensPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("codecatalyst") as client:  # (1)
    paginator = client.get_paginator("list_access_tokens")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CodeCatalystClient](./client.md)
2. paginator: [ListAccessTokensPaginator](./paginators.md#listaccesstokenspaginator)
3. item: [:material-code-braces: ListAccessTokensResponseTypeDef](./type_defs.md#listaccesstokensresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[codecatalyst]`
or a standalone `types_aiobotocore_codecatalyst` package, you have to explicitly specify
`client: CodeCatalystClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CodeCatalystClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_codecatalyst.client import CodeCatalystClient
from types_aiobotocore_codecatalyst.type_defs import CreateAccessTokenResponseTypeDef
from types_aiobotocore_codecatalyst.type_defs import CreateAccessTokenRequestRequestTypeDef


session = Session()

client: CodeCatalystClient
async with session.client("codecatalyst") as client:  # (1)
    kwargs: CreateAccessTokenRequestRequestTypeDef = {...}  # (2)
    result: CreateAccessTokenResponseTypeDef = await client.create_access_token(**kwargs)  # (3)
```

1. client: [CodeCatalystClient](./client.md)
2. kwargs: [:material-code-braces: CreateAccessTokenRequestRequestTypeDef](./type_defs.md#createaccesstokenrequestrequesttypedef) 
3. result: [:material-code-braces: CreateAccessTokenResponseTypeDef](./type_defs.md#createaccesstokenresponsetypedef) 



```python
# ListAccessTokensPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_codecatalyst.client import CodeCatalystClient
from types_aiobotocore_codecatalyst.paginator import ListAccessTokensPaginator
from types_aiobotocore_codecatalyst.type_defs import ListAccessTokensResponseTypeDef


session = Session()

client: CodeCatalystClient
async with session.client("codecatalyst") as client:  # (1)
    paginator: ListAccessTokensPaginator = client.get_paginator("list_access_tokens")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccessTokensResponseTypeDef
        print(item)  # (3)
```

1. client: [CodeCatalystClient](./client.md)
2. paginator: [ListAccessTokensPaginator](./paginators.md#listaccesstokenspaginator)
3. item: [:material-code-braces: ListAccessTokensResponseTypeDef](./type_defs.md#listaccesstokensresponsetypedef) 



