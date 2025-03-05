# Examples

> [Index](../README.md) > [APIGateway](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [APIGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#apigateway)
    type annotations stubs module [types-aiobotocore-apigateway](https://pypi.org/project/types-aiobotocore-apigateway/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[apigateway]` package installed.

Write your `APIGateway` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# APIGatewayClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("apigateway") as client:  # (1)
    result = await client.create_api_key()  # (2)
```

1. client: [APIGatewayClient](./client.md)
2. result: [:material-code-braces: ApiKeyResponseTypeDef](./type_defs.md#apikeyresponsetypedef)



#### Paginator usage example

```python
# GetApiKeysPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("apigateway") as client:  # (1)
    paginator = client.get_paginator("get_api_keys")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetApiKeysPaginator](./paginators.md#getapikeyspaginator)
3. item: [:material-code-braces: ApiKeysTypeDef](./type_defs.md#apikeystypedef)




### Explicit type annotations

With `types-aioboto3-lite[apigateway]`
or a standalone `types_aiobotocore_apigateway` package, you have to explicitly specify
`client: APIGatewayClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# APIGatewayClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_apigateway.client import APIGatewayClient
from types_aiobotocore_apigateway.type_defs import ApiKeyResponseTypeDef
from types_aiobotocore_apigateway.type_defs import CreateApiKeyRequestTypeDef


session = Session()

client: APIGatewayClient
async with session.client("apigateway") as client:  # (1)
    kwargs: CreateApiKeyRequestTypeDef = {...}  # (2)
    result: ApiKeyResponseTypeDef = await client.create_api_key(**kwargs)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. kwargs: [:material-code-braces: CreateApiKeyRequestTypeDef](./type_defs.md#createapikeyrequesttypedef)
3. result: [:material-code-braces: ApiKeyResponseTypeDef](./type_defs.md#apikeyresponsetypedef)



#### Paginator usage example

```python
# GetApiKeysPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_apigateway.client import APIGatewayClient
from types_aiobotocore_apigateway.paginator import GetApiKeysPaginator
from types_aiobotocore_apigateway.type_defs import ApiKeysTypeDef


session = Session()

client: APIGatewayClient
async with session.client("apigateway") as client:  # (1)
    paginator: GetApiKeysPaginator = client.get_paginator("get_api_keys")  # (2)
    async for item in paginator.paginate(...):
        item: ApiKeysTypeDef
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetApiKeysPaginator](./paginators.md#getapikeyspaginator)
3. item: [:material-code-braces: ApiKeysTypeDef](./type_defs.md#apikeystypedef)




