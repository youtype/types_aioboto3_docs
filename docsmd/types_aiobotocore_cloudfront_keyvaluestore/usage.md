# Examples

> [Index](../README.md) > [CloudFrontKeyValueStore](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudFrontKeyValueStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore.html#cloudfrontkeyvaluestore)
    type annotations stubs module [types-aiobotocore-cloudfront-keyvaluestore](https://pypi.org/project/types-aiobotocore-cloudfront-keyvaluestore/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[cloudfront-keyvaluestore]` package installed.

Write your `CloudFrontKeyValueStore` code as usual,
type checking and code completion should work out of the box.



```python
# CloudFrontKeyValueStoreClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("cloudfront-keyvaluestore") as client:  # (1)
    result = await client.delete_key()  # (2)
```

1. client: [CloudFrontKeyValueStoreClient](./client.md)
2. result: [:material-code-braces: DeleteKeyResponseTypeDef](./type_defs.md#deletekeyresponsetypedef) 



```python
# ListKeysPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("cloudfront-keyvaluestore") as client:  # (1)
    paginator = client.get_paginator("list_keys")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudFrontKeyValueStoreClient](./client.md)
2. paginator: [ListKeysPaginator](./paginators.md#listkeyspaginator)
3. item: [:material-code-braces: ListKeysResponseTypeDef](./type_defs.md#listkeysresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[cloudfront-keyvaluestore]`
or a standalone `types_aiobotocore_cloudfront_keyvaluestore` package, you have to explicitly specify
`client: CloudFrontKeyValueStoreClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CloudFrontKeyValueStoreClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_cloudfront_keyvaluestore.client import CloudFrontKeyValueStoreClient
from types_aiobotocore_cloudfront_keyvaluestore.type_defs import DeleteKeyResponseTypeDef
from types_aiobotocore_cloudfront_keyvaluestore.type_defs import DeleteKeyRequestRequestTypeDef


session = Session()

client: CloudFrontKeyValueStoreClient
async with session.client("cloudfront-keyvaluestore") as client:  # (1)
    kwargs: DeleteKeyRequestRequestTypeDef = {...}  # (2)
    result: DeleteKeyResponseTypeDef = await client.delete_key(**kwargs)  # (3)
```

1. client: [CloudFrontKeyValueStoreClient](./client.md)
2. kwargs: [:material-code-braces: DeleteKeyRequestRequestTypeDef](./type_defs.md#deletekeyrequestrequesttypedef) 
3. result: [:material-code-braces: DeleteKeyResponseTypeDef](./type_defs.md#deletekeyresponsetypedef) 



```python
# ListKeysPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_cloudfront_keyvaluestore.client import CloudFrontKeyValueStoreClient
from types_aiobotocore_cloudfront_keyvaluestore.paginator import ListKeysPaginator
from types_aiobotocore_cloudfront_keyvaluestore.type_defs import ListKeysResponseTypeDef


session = Session()

client: CloudFrontKeyValueStoreClient
async with session.client("cloudfront-keyvaluestore") as client:  # (1)
    paginator: ListKeysPaginator = client.get_paginator("list_keys")  # (2)
    async for item in paginator.paginate(...):
        item: ListKeysResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudFrontKeyValueStoreClient](./client.md)
2. paginator: [ListKeysPaginator](./paginators.md#listkeyspaginator)
3. item: [:material-code-braces: ListKeysResponseTypeDef](./type_defs.md#listkeysresponsetypedef) 



