# Examples

> [Index](../README.md) > [S3](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [S3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#s3)
    type annotations stubs module [types-aiobotocore-s3](https://pypi.org/project/types-aiobotocore-s3/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[s3]` package installed.

Write your `S3` code as usual,
type checking and code completion should work out of the box.



```python
# S3Client usage example

from aioboto3.session import Session


session = Session()

async with session.client("s3") as client:  # (1)
    result = await client.abort_multipart_upload()  # (2)
```

1. client: [S3Client](./client.md)
2. result: [:material-code-braces: AbortMultipartUploadOutputTypeDef](./type_defs.md#abortmultipartuploadoutputtypedef) 



```python
# ListBucketsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("s3") as client:  # (1)
    paginator = client.get_paginator("list_buckets")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [S3Client](./client.md)
2. paginator: [ListBucketsPaginator](./paginators.md#listbucketspaginator)
3. item: [:material-code-braces: ListBucketsOutputTypeDef](./type_defs.md#listbucketsoutputtypedef) 



```python
# BucketExistsWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("s3") as client:  # (1)
    waiter = client.get_waiter("bucket_exists")  # (2)
    await waiter.wait()
```

1. client: [S3Client](./client.md)
2. waiter: [BucketExistsWaiter](./waiters.md#bucketexistswaiter)


### Explicit type annotations

With `types-aioboto3-lite[s3]`
or a standalone `types_aiobotocore_s3` package, you have to explicitly specify
`client: S3Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# S3Client usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_s3.client import S3Client
from types_aiobotocore_s3.type_defs import AbortMultipartUploadOutputTypeDef
from types_aiobotocore_s3.type_defs import AbortMultipartUploadRequestRequestTypeDef


session = Session()

client: S3Client
async with session.client("s3") as client:  # (1)
    kwargs: AbortMultipartUploadRequestRequestTypeDef = {...}  # (2)
    result: AbortMultipartUploadOutputTypeDef = await client.abort_multipart_upload(**kwargs)  # (3)
```

1. client: [S3Client](./client.md)
2. kwargs: [:material-code-braces: AbortMultipartUploadRequestRequestTypeDef](./type_defs.md#abortmultipartuploadrequestrequesttypedef) 
3. result: [:material-code-braces: AbortMultipartUploadOutputTypeDef](./type_defs.md#abortmultipartuploadoutputtypedef) 



```python
# ListBucketsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_s3.client import S3Client
from types_aiobotocore_s3.paginator import ListBucketsPaginator
from types_aiobotocore_s3.type_defs import ListBucketsOutputTypeDef


session = Session()

client: S3Client
async with session.client("s3") as client:  # (1)
    paginator: ListBucketsPaginator = client.get_paginator("list_buckets")  # (2)
    async for item in paginator.paginate(...):
        item: ListBucketsOutputTypeDef
        print(item)  # (3)
```

1. client: [S3Client](./client.md)
2. paginator: [ListBucketsPaginator](./paginators.md#listbucketspaginator)
3. item: [:material-code-braces: ListBucketsOutputTypeDef](./type_defs.md#listbucketsoutputtypedef) 



```python
# BucketExistsWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_s3.client import S3Client
from types_aiobotocore_s3.waiter import BucketExistsWaiter


session = Session()

async with session.client("s3") as client:  # (1)
    waiter = client.get_waiter("bucket_exists")  # (2)
    await waiter.wait()
```

1. client: [S3Client](./client.md)
2. waiter: [BucketExistsWaiter](./waiters.md#bucketexistswaiter)



## Service Resource

### Implicit type annotations

Can be used with `types-aioboto3[s3]` package installed.


```python
# S3ServiceResource usage example

from aioboto3.session import Session


session = Session()

async with session.resource("s3") as resource:  # (1)
    result = resource.get_available_subresources()  # (2)
```

1. resource: [S3ServiceResource](./service_resource.md)
2. result: 



```python
# ServiceResourceBucketsCollection usage example

from aioboto3.session import Session


session = Session()
resource = session.resource("s3")  # (1)

collection = resource.buckets  # (2)
for item in collection:
    print(item)  # (3)
```

1. resource: [S3ServiceResource](./service_resource.md)
2. collection: [S3ServiceResource](./service_resource.md#serviceresourcebucketscollection)
3. item: Bucket


### Explicit type annotations

With `types-aioboto3-lite[s3]`
or a standalone `types_aiobotocore_s3` package, you have to explicitly specify
`resource: S3ServiceResource` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.



```python
# S3ServiceResource usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_s3.service_resource import S3ServiceResource
from types_aiobotocore_s3.service_resource import get_available_subresources


session = Session()

resource: S3ServiceResource
async with session.resource("s3") as resource:  # (1)
    result: get_available_subresources = resource.get_available_subresources() # (2)
```

1. resource: [S3ServiceResource](./service_resource.md)
2. result: 



```python
# ServiceResourceBucketsCollection usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_s3.service_resource import S3ServiceResource
from types_aiobotocore_s3.service_resource import ServiceResourceBucketsCollection
from types_aiobotocore_s3.service_resource import Bucket


session = Session()

resource: S3ServiceResource
async with session.resource("s3") as resource:  # (1)
    collection: ServiceResourceBucketsCollection = resource.buckets  # (2)
    for item in collection:
        item: Bucket
        print(item)  # (3)
```

1. resource: [S3ServiceResource](./service_resource.md)
2. collection: [S3ServiceResource](./service_resource.md#serviceresourcebucketscollection)
3. item: Bucket
