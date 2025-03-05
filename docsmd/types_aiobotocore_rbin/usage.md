# Examples

> [Index](../README.md) > [RecycleBin](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [RecycleBin](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#recyclebin)
    type annotations stubs module [types-aiobotocore-rbin](https://pypi.org/project/types-aiobotocore-rbin/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[rbin]` package installed.

Write your `RecycleBin` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# RecycleBinClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("rbin") as client:  # (1)
    result = await client.create_rule()  # (2)
```

1. client: [RecycleBinClient](./client.md)
2. result: [:material-code-braces: CreateRuleResponseTypeDef](./type_defs.md#createruleresponsetypedef)



#### Paginator usage example

```python
# ListRulesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("rbin") as client:  # (1)
    paginator = client.get_paginator("list_rules")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [RecycleBinClient](./client.md)
2. paginator: [ListRulesPaginator](./paginators.md#listrulespaginator)
3. item: [:material-code-braces: ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[rbin]`
or a standalone `types_aiobotocore_rbin` package, you have to explicitly specify
`client: RecycleBinClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# RecycleBinClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_rbin.client import RecycleBinClient
from types_aiobotocore_rbin.type_defs import CreateRuleResponseTypeDef
from types_aiobotocore_rbin.type_defs import CreateRuleRequestTypeDef


session = Session()

client: RecycleBinClient
async with session.client("rbin") as client:  # (1)
    kwargs: CreateRuleRequestTypeDef = {...}  # (2)
    result: CreateRuleResponseTypeDef = await client.create_rule(**kwargs)  # (3)
```

1. client: [RecycleBinClient](./client.md)
2. kwargs: [:material-code-braces: CreateRuleRequestTypeDef](./type_defs.md#createrulerequesttypedef)
3. result: [:material-code-braces: CreateRuleResponseTypeDef](./type_defs.md#createruleresponsetypedef)



#### Paginator usage example

```python
# ListRulesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_rbin.client import RecycleBinClient
from types_aiobotocore_rbin.paginator import ListRulesPaginator
from types_aiobotocore_rbin.type_defs import ListRulesResponseTypeDef


session = Session()

client: RecycleBinClient
async with session.client("rbin") as client:  # (1)
    paginator: ListRulesPaginator = client.get_paginator("list_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [RecycleBinClient](./client.md)
2. paginator: [ListRulesPaginator](./paginators.md#listrulespaginator)
3. item: [:material-code-braces: ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef)




