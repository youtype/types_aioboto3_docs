# Examples

> [Index](../README.md) > [Glacier](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Glacier](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#glacier)
    type annotations stubs module [types-aiobotocore-glacier](https://pypi.org/project/types-aiobotocore-glacier/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[glacier]` package installed.

Write your `Glacier` code as usual,
type checking and code completion should work out of the box.



```python
# GlacierClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("glacier") as client:  # (1)
    result = await client.abort_multipart_upload()  # (2)
```

1. client: [GlacierClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# ListJobsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("glacier") as client:  # (1)
    paginator = client.get_paginator("list_jobs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [GlacierClient](./client.md)
2. paginator: [ListJobsPaginator](./paginators.md#listjobspaginator)
3. item: [:material-code-braces: ListJobsOutputTypeDef](./type_defs.md#listjobsoutputtypedef) 



```python
# VaultExistsWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("glacier") as client:  # (1)
    waiter = client.get_waiter("vault_exists")  # (2)
    await waiter.wait()
```

1. client: [GlacierClient](./client.md)
2. waiter: [VaultExistsWaiter](./waiters.md#vaultexistswaiter)


### Explicit type annotations

With `types-aioboto3-lite[glacier]`
or a standalone `types_aiobotocore_glacier` package, you have to explicitly specify
`client: GlacierClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# GlacierClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_glacier.client import GlacierClient
from types_aiobotocore_glacier.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_glacier.type_defs import AbortMultipartUploadInputRequestTypeDef


session = Session()

client: GlacierClient
async with session.client("glacier") as client:  # (1)
    kwargs: AbortMultipartUploadInputRequestTypeDef = {...}  # (2)
    result: EmptyResponseMetadataTypeDef = await client.abort_multipart_upload(**kwargs)  # (3)
```

1. client: [GlacierClient](./client.md)
2. kwargs: [:material-code-braces: AbortMultipartUploadInputRequestTypeDef](./type_defs.md#abortmultipartuploadinputrequesttypedef) 
3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# ListJobsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_glacier.client import GlacierClient
from types_aiobotocore_glacier.paginator import ListJobsPaginator
from types_aiobotocore_glacier.type_defs import ListJobsOutputTypeDef


session = Session()

client: GlacierClient
async with session.client("glacier") as client:  # (1)
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsOutputTypeDef
        print(item)  # (3)
```

1. client: [GlacierClient](./client.md)
2. paginator: [ListJobsPaginator](./paginators.md#listjobspaginator)
3. item: [:material-code-braces: ListJobsOutputTypeDef](./type_defs.md#listjobsoutputtypedef) 



```python
# VaultExistsWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_glacier.client import GlacierClient
from types_aiobotocore_glacier.waiter import VaultExistsWaiter


session = Session()

async with session.client("glacier") as client:  # (1)
    waiter = client.get_waiter("vault_exists")  # (2)
    await waiter.wait()
```

1. client: [GlacierClient](./client.md)
2. waiter: [VaultExistsWaiter](./waiters.md#vaultexistswaiter)



## Service Resource

### Implicit type annotations

Can be used with `types-aioboto3[glacier]` package installed.


```python
# GlacierServiceResource usage example

from aioboto3.session import Session


session = Session()

async with session.resource("glacier") as resource:  # (1)
    result = resource.get_available_subresources()  # (2)
```

1. resource: [GlacierServiceResource](./service_resource.md)
2. result: 



```python
# ServiceResourceVaultsCollection usage example

from aioboto3.session import Session


session = Session()
resource = session.resource("glacier")  # (1)

collection = resource.vaults  # (2)
for item in collection:
    print(item)  # (3)
```

1. resource: [GlacierServiceResource](./service_resource.md)
2. collection: [GlacierServiceResource](./service_resource.md#serviceresourcevaultscollection)
3. item: Vault


### Explicit type annotations

With `types-aioboto3-lite[glacier]`
or a standalone `types_aiobotocore_glacier` package, you have to explicitly specify
`resource: GlacierServiceResource` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.



```python
# GlacierServiceResource usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_glacier.service_resource import GlacierServiceResource
from types_aiobotocore_glacier.service_resource import get_available_subresources


session = Session()

resource: GlacierServiceResource
async with session.resource("glacier") as resource:  # (1)
    result: get_available_subresources = resource.get_available_subresources() # (2)
```

1. resource: [GlacierServiceResource](./service_resource.md)
2. result: 



```python
# ServiceResourceVaultsCollection usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_glacier.service_resource import GlacierServiceResource
from types_aiobotocore_glacier.service_resource import ServiceResourceVaultsCollection
from types_aiobotocore_glacier.service_resource import Vault


session = Session()

resource: GlacierServiceResource
async with session.resource("glacier") as resource:  # (1)
    collection: ServiceResourceVaultsCollection = resource.vaults  # (2)
    for item in collection:
        item: Vault
        print(item)  # (3)
```

1. resource: [GlacierServiceResource](./service_resource.md)
2. collection: [GlacierServiceResource](./service_resource.md#serviceresourcevaultscollection)
3. item: Vault
