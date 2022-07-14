# Paginators

> [Index](../README.md) > [Glacier](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Glacier](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
    type annotations stubs module [types-aiobotocore-glacier](https://pypi.org/project/types-aiobotocore-glacier/).

## ListJobsPaginator

Type annotations and code completion for `#!python session.client("glacier").get_paginator("list_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListJobs)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_glacier.paginator import ListJobsPaginator

session = Session()

session = get_session()
async with session.client("glacier") as client:  # (1)
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsOutputTypeDef
        print(item)  # (3)
```

1. client: [GlacierClient](./client.md)
2. paginator: [ListJobsPaginator](./paginators.md#listjobspaginator)
3. item: [:material-code-braces: ListJobsOutputTypeDef](./type_defs.md#listjobsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    accountId: str,
    vaultName: str,
    statuscode: str = ...,
    completed: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListJobsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobsOutputTypeDef](./type_defs.md#listjobsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListJobsInputListJobsPaginateTypeDef = {  # (1)
    "accountId": ...,
    "vaultName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsInputListJobsPaginateTypeDef](./type_defs.md#listjobsinputlistjobspaginatetypedef) 
## ListMultipartUploadsPaginator

Type annotations and code completion for `#!python session.client("glacier").get_paginator("list_multipart_uploads")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListMultipartUploads)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_glacier.paginator import ListMultipartUploadsPaginator

session = Session()

session = get_session()
async with session.client("glacier") as client:  # (1)
    paginator: ListMultipartUploadsPaginator = client.get_paginator("list_multipart_uploads")  # (2)
    async for item in paginator.paginate(...):
        item: ListMultipartUploadsOutputTypeDef
        print(item)  # (3)
```

1. client: [GlacierClient](./client.md)
2. paginator: [ListMultipartUploadsPaginator](./paginators.md#listmultipartuploadspaginator)
3. item: [:material-code-braces: ListMultipartUploadsOutputTypeDef](./type_defs.md#listmultipartuploadsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListMultipartUploadsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    accountId: str,
    vaultName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMultipartUploadsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMultipartUploadsOutputTypeDef](./type_defs.md#listmultipartuploadsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef = {  # (1)
    "accountId": ...,
    "vaultName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef](./type_defs.md#listmultipartuploadsinputlistmultipartuploadspaginatetypedef) 
## ListPartsPaginator

Type annotations and code completion for `#!python session.client("glacier").get_paginator("list_parts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListParts)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_glacier.paginator import ListPartsPaginator

session = Session()

session = get_session()
async with session.client("glacier") as client:  # (1)
    paginator: ListPartsPaginator = client.get_paginator("list_parts")  # (2)
    async for item in paginator.paginate(...):
        item: ListPartsOutputTypeDef
        print(item)  # (3)
```

1. client: [GlacierClient](./client.md)
2. paginator: [ListPartsPaginator](./paginators.md#listpartspaginator)
3. item: [:material-code-braces: ListPartsOutputTypeDef](./type_defs.md#listpartsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListPartsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    accountId: str,
    vaultName: str,
    uploadId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPartsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPartsOutputTypeDef](./type_defs.md#listpartsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListPartsInputListPartsPaginateTypeDef = {  # (1)
    "accountId": ...,
    "vaultName": ...,
    "uploadId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPartsInputListPartsPaginateTypeDef](./type_defs.md#listpartsinputlistpartspaginatetypedef) 
## ListVaultsPaginator

Type annotations and code completion for `#!python session.client("glacier").get_paginator("list_vaults")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListVaults)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_glacier.paginator import ListVaultsPaginator

session = Session()

session = get_session()
async with session.client("glacier") as client:  # (1)
    paginator: ListVaultsPaginator = client.get_paginator("list_vaults")  # (2)
    async for item in paginator.paginate(...):
        item: ListVaultsOutputTypeDef
        print(item)  # (3)
```

1. client: [GlacierClient](./client.md)
2. paginator: [ListVaultsPaginator](./paginators.md#listvaultspaginator)
3. item: [:material-code-braces: ListVaultsOutputTypeDef](./type_defs.md#listvaultsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListVaultsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    accountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListVaultsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListVaultsOutputTypeDef](./type_defs.md#listvaultsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListVaultsInputListVaultsPaginateTypeDef = {  # (1)
    "accountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVaultsInputListVaultsPaginateTypeDef](./type_defs.md#listvaultsinputlistvaultspaginatetypedef) 
