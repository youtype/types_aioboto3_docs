# Examples

> [Index](../README.md) > [Bedrock](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Bedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#bedrock)
    type annotations stubs module [types-aiobotocore-bedrock](https://pypi.org/project/types-aiobotocore-bedrock/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[bedrock]` package installed.

Write your `Bedrock` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# BedrockClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("bedrock") as client:  # (1)
    result = await client.batch_delete_evaluation_job()  # (2)
```

1. client: [BedrockClient](./client.md)
2. result: [:material-code-braces: BatchDeleteEvaluationJobResponseTypeDef](./type_defs.md#batchdeleteevaluationjobresponsetypedef)



#### Paginator usage example

```python
# ListCustomModelsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("bedrock") as client:  # (1)
    paginator = client.get_paginator("list_custom_models")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [BedrockClient](./client.md)
2. paginator: [ListCustomModelsPaginator](./paginators.md#listcustommodelspaginator)
3. item: [:material-code-braces: ListCustomModelsResponseTypeDef](./type_defs.md#listcustommodelsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[bedrock]`
or a standalone `types_aiobotocore_bedrock` package, you have to explicitly specify
`client: BedrockClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# BedrockClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_bedrock.client import BedrockClient
from types_aiobotocore_bedrock.type_defs import BatchDeleteEvaluationJobResponseTypeDef
from types_aiobotocore_bedrock.type_defs import BatchDeleteEvaluationJobRequestTypeDef


session = Session()

client: BedrockClient
async with session.client("bedrock") as client:  # (1)
    kwargs: BatchDeleteEvaluationJobRequestTypeDef = {...}  # (2)
    result: BatchDeleteEvaluationJobResponseTypeDef = await client.batch_delete_evaluation_job(**kwargs)  # (3)
```

1. client: [BedrockClient](./client.md)
2. kwargs: [:material-code-braces: BatchDeleteEvaluationJobRequestTypeDef](./type_defs.md#batchdeleteevaluationjobrequesttypedef)
3. result: [:material-code-braces: BatchDeleteEvaluationJobResponseTypeDef](./type_defs.md#batchdeleteevaluationjobresponsetypedef)



#### Paginator usage example

```python
# ListCustomModelsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_bedrock.client import BedrockClient
from types_aiobotocore_bedrock.paginator import ListCustomModelsPaginator
from types_aiobotocore_bedrock.type_defs import ListCustomModelsResponseTypeDef


session = Session()

client: BedrockClient
async with session.client("bedrock") as client:  # (1)
    paginator: ListCustomModelsPaginator = client.get_paginator("list_custom_models")  # (2)
    async for item in paginator.paginate(...):
        item: ListCustomModelsResponseTypeDef
        print(item)  # (3)
```

1. client: [BedrockClient](./client.md)
2. paginator: [ListCustomModelsPaginator](./paginators.md#listcustommodelspaginator)
3. item: [:material-code-braces: ListCustomModelsResponseTypeDef](./type_defs.md#listcustommodelsresponsetypedef)




