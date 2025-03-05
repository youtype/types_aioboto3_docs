# Examples

> [Index](../README.md) > [FIS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [FIS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#fis)
    type annotations stubs module [types-aiobotocore-fis](https://pypi.org/project/types-aiobotocore-fis/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[fis]` package installed.

Write your `FIS` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# FISClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("fis") as client:  # (1)
    result = await client.create_experiment_template()  # (2)
```

1. client: [FISClient](./client.md)
2. result: [:material-code-braces: CreateExperimentTemplateResponseTypeDef](./type_defs.md#createexperimenttemplateresponsetypedef)



#### Paginator usage example

```python
# ListActionsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("fis") as client:  # (1)
    paginator = client.get_paginator("list_actions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [FISClient](./client.md)
2. paginator: [ListActionsPaginator](./paginators.md#listactionspaginator)
3. item: [:material-code-braces: ListActionsResponseTypeDef](./type_defs.md#listactionsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[fis]`
or a standalone `types_aiobotocore_fis` package, you have to explicitly specify
`client: FISClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# FISClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_fis.client import FISClient
from types_aiobotocore_fis.type_defs import CreateExperimentTemplateResponseTypeDef
from types_aiobotocore_fis.type_defs import CreateExperimentTemplateRequestTypeDef


session = Session()

client: FISClient
async with session.client("fis") as client:  # (1)
    kwargs: CreateExperimentTemplateRequestTypeDef = {...}  # (2)
    result: CreateExperimentTemplateResponseTypeDef = await client.create_experiment_template(**kwargs)  # (3)
```

1. client: [FISClient](./client.md)
2. kwargs: [:material-code-braces: CreateExperimentTemplateRequestTypeDef](./type_defs.md#createexperimenttemplaterequesttypedef)
3. result: [:material-code-braces: CreateExperimentTemplateResponseTypeDef](./type_defs.md#createexperimenttemplateresponsetypedef)



#### Paginator usage example

```python
# ListActionsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_fis.client import FISClient
from types_aiobotocore_fis.paginator import ListActionsPaginator
from types_aiobotocore_fis.type_defs import ListActionsResponseTypeDef


session = Session()

client: FISClient
async with session.client("fis") as client:  # (1)
    paginator: ListActionsPaginator = client.get_paginator("list_actions")  # (2)
    async for item in paginator.paginate(...):
        item: ListActionsResponseTypeDef
        print(item)  # (3)
```

1. client: [FISClient](./client.md)
2. paginator: [ListActionsPaginator](./paginators.md#listactionspaginator)
3. item: [:material-code-braces: ListActionsResponseTypeDef](./type_defs.md#listactionsresponsetypedef)




