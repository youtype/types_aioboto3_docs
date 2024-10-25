# Examples

> [Index](../README.md) > [ConnectCases](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ConnectCases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
    type annotations stubs module [types-aiobotocore-connectcases](https://pypi.org/project/types-aiobotocore-connectcases/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[connectcases]` package installed.

Write your `ConnectCases` code as usual,
type checking and code completion should work out of the box.



```python
# ConnectCasesClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("connectcases") as client:  # (1)
    result = await client.batch_get_field()  # (2)
```

1. client: [ConnectCasesClient](./client.md)
2. result: [:material-code-braces: BatchGetFieldResponseTypeDef](./type_defs.md#batchgetfieldresponsetypedef) 



```python
# SearchCasesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("connectcases") as client:  # (1)
    paginator = client.get_paginator("search_cases")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ConnectCasesClient](./client.md)
2. paginator: [SearchCasesPaginator](./paginators.md#searchcasespaginator)
3. item: [:material-code-braces: SearchCasesResponseTypeDef](./type_defs.md#searchcasesresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[connectcases]`
or a standalone `types_aiobotocore_connectcases` package, you have to explicitly specify
`client: ConnectCasesClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ConnectCasesClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_connectcases.client import ConnectCasesClient
from types_aiobotocore_connectcases.type_defs import BatchGetFieldResponseTypeDef
from types_aiobotocore_connectcases.type_defs import BatchGetFieldRequestRequestTypeDef


session = Session()

client: ConnectCasesClient
async with session.client("connectcases") as client:  # (1)
    kwargs: BatchGetFieldRequestRequestTypeDef = {...}  # (2)
    result: BatchGetFieldResponseTypeDef = await client.batch_get_field(**kwargs)  # (3)
```

1. client: [ConnectCasesClient](./client.md)
2. kwargs: [:material-code-braces: BatchGetFieldRequestRequestTypeDef](./type_defs.md#batchgetfieldrequestrequesttypedef) 
3. result: [:material-code-braces: BatchGetFieldResponseTypeDef](./type_defs.md#batchgetfieldresponsetypedef) 



```python
# SearchCasesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_connectcases.client import ConnectCasesClient
from types_aiobotocore_connectcases.paginator import SearchCasesPaginator
from types_aiobotocore_connectcases.type_defs import SearchCasesResponseTypeDef


session = Session()

client: ConnectCasesClient
async with session.client("connectcases") as client:  # (1)
    paginator: SearchCasesPaginator = client.get_paginator("search_cases")  # (2)
    async for item in paginator.paginate(...):
        item: SearchCasesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectCasesClient](./client.md)
2. paginator: [SearchCasesPaginator](./paginators.md#searchcasespaginator)
3. item: [:material-code-braces: SearchCasesResponseTypeDef](./type_defs.md#searchcasesresponsetypedef) 




