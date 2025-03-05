# Examples

> [Index](../README.md) > [OpenSearchServiceServerless](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [OpenSearchServiceServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#opensearchserviceserverless)
    type annotations stubs module [types-aiobotocore-opensearchserverless](https://pypi.org/project/types-aiobotocore-opensearchserverless/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[opensearchserverless]` package installed.

Write your `OpenSearchServiceServerless` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# OpenSearchServiceServerlessClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("opensearchserverless") as client:  # (1)
    result = await client.batch_get_collection()  # (2)
```

1. client: [OpenSearchServiceServerlessClient](./client.md)
2. result: [:material-code-braces: BatchGetCollectionResponseTypeDef](./type_defs.md#batchgetcollectionresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[opensearchserverless]`
or a standalone `types_aiobotocore_opensearchserverless` package, you have to explicitly specify
`client: OpenSearchServiceServerlessClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# OpenSearchServiceServerlessClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_opensearchserverless.client import OpenSearchServiceServerlessClient
from types_aiobotocore_opensearchserverless.type_defs import BatchGetCollectionResponseTypeDef
from types_aiobotocore_opensearchserverless.type_defs import BatchGetCollectionRequestTypeDef


session = Session()

client: OpenSearchServiceServerlessClient
async with session.client("opensearchserverless") as client:  # (1)
    kwargs: BatchGetCollectionRequestTypeDef = {...}  # (2)
    result: BatchGetCollectionResponseTypeDef = await client.batch_get_collection(**kwargs)  # (3)
```

1. client: [OpenSearchServiceServerlessClient](./client.md)
2. kwargs: [:material-code-braces: BatchGetCollectionRequestTypeDef](./type_defs.md#batchgetcollectionrequesttypedef)
3. result: [:material-code-braces: BatchGetCollectionResponseTypeDef](./type_defs.md#batchgetcollectionresponsetypedef)






