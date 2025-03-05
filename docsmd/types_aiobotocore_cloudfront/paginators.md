# Paginators

> [Index](../README.md) > [CloudFront](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudFront](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#cloudfront)
    type annotations stubs module [types-aiobotocore-cloudfront](https://pypi.org/project/types-aiobotocore-cloudfront/).

## ListCloudFrontOriginAccessIdentitiesPaginator

Type annotations and code completion for `#!python session.client("cloudfront").get_paginator("list_cloud_front_origin_access_identities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront/paginator/ListCloudFrontOriginAccessIdentities.html#CloudFront.Paginator.ListCloudFrontOriginAccessIdentities)

```python
# ListCloudFrontOriginAccessIdentitiesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_cloudfront.paginator import ListCloudFrontOriginAccessIdentitiesPaginator

session = Session()

session = get_session()
async with session.client("cloudfront") as client:  # (1)
    paginator: ListCloudFrontOriginAccessIdentitiesPaginator = client.get_paginator("list_cloud_front_origin_access_identities")  # (2)
    async for item in paginator.paginate(...):
        item: ListCloudFrontOriginAccessIdentitiesResultTypeDef
        print(item)  # (3)
```

1. client: [CloudFrontClient](./client.md)
2. paginator: [ListCloudFrontOriginAccessIdentitiesPaginator](./paginators.md#listcloudfrontoriginaccessidentitiespaginator)
3. item: `AioPageIterator[ListCloudFrontOriginAccessIdentitiesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCloudFrontOriginAccessIdentitiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCloudFrontOriginAccessIdentitiesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCloudFrontOriginAccessIdentitiesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCloudFrontOriginAccessIdentitiesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCloudFrontOriginAccessIdentitiesRequestPaginateTypeDef](./type_defs.md#listcloudfrontoriginaccessidentitiesrequestpaginatetypedef)
## ListDistributionsPaginator

Type annotations and code completion for `#!python session.client("cloudfront").get_paginator("list_distributions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront/paginator/ListDistributions.html#CloudFront.Paginator.ListDistributions)

```python
# ListDistributionsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_cloudfront.paginator import ListDistributionsPaginator

session = Session()

session = get_session()
async with session.client("cloudfront") as client:  # (1)
    paginator: ListDistributionsPaginator = client.get_paginator("list_distributions")  # (2)
    async for item in paginator.paginate(...):
        item: ListDistributionsResultTypeDef
        print(item)  # (3)
```

1. client: [CloudFrontClient](./client.md)
2. paginator: [ListDistributionsPaginator](./paginators.md#listdistributionspaginator)
3. item: `AioPageIterator[ListDistributionsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDistributionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDistributionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDistributionsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDistributionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDistributionsRequestPaginateTypeDef](./type_defs.md#listdistributionsrequestpaginatetypedef)
## ListInvalidationsPaginator

Type annotations and code completion for `#!python session.client("cloudfront").get_paginator("list_invalidations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront/paginator/ListInvalidations.html#CloudFront.Paginator.ListInvalidations)

```python
# ListInvalidationsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_cloudfront.paginator import ListInvalidationsPaginator

session = Session()

session = get_session()
async with session.client("cloudfront") as client:  # (1)
    paginator: ListInvalidationsPaginator = client.get_paginator("list_invalidations")  # (2)
    async for item in paginator.paginate(...):
        item: ListInvalidationsResultTypeDef
        print(item)  # (3)
```

1. client: [CloudFrontClient](./client.md)
2. paginator: [ListInvalidationsPaginator](./paginators.md#listinvalidationspaginator)
3. item: `AioPageIterator[ListInvalidationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListInvalidationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DistributionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListInvalidationsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListInvalidationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListInvalidationsRequestPaginateTypeDef = {  # (1)
    "DistributionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInvalidationsRequestPaginateTypeDef](./type_defs.md#listinvalidationsrequestpaginatetypedef)
## ListKeyValueStoresPaginator

Type annotations and code completion for `#!python session.client("cloudfront").get_paginator("list_key_value_stores")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront/paginator/ListKeyValueStores.html#CloudFront.Paginator.ListKeyValueStores)

```python
# ListKeyValueStoresPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_cloudfront.paginator import ListKeyValueStoresPaginator

session = Session()

session = get_session()
async with session.client("cloudfront") as client:  # (1)
    paginator: ListKeyValueStoresPaginator = client.get_paginator("list_key_value_stores")  # (2)
    async for item in paginator.paginate(...):
        item: ListKeyValueStoresResultTypeDef
        print(item)  # (3)
```

1. client: [CloudFrontClient](./client.md)
2. paginator: [ListKeyValueStoresPaginator](./paginators.md#listkeyvaluestorespaginator)
3. item: `AioPageIterator[ListKeyValueStoresResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListKeyValueStoresPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Status: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListKeyValueStoresResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListKeyValueStoresResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListKeyValueStoresRequestPaginateTypeDef = {  # (1)
    "Status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListKeyValueStoresRequestPaginateTypeDef](./type_defs.md#listkeyvaluestoresrequestpaginatetypedef)
## ListPublicKeysPaginator

Type annotations and code completion for `#!python session.client("cloudfront").get_paginator("list_public_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront/paginator/ListPublicKeys.html#CloudFront.Paginator.ListPublicKeys)

```python
# ListPublicKeysPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_cloudfront.paginator import ListPublicKeysPaginator

session = Session()

session = get_session()
async with session.client("cloudfront") as client:  # (1)
    paginator: ListPublicKeysPaginator = client.get_paginator("list_public_keys")  # (2)
    async for item in paginator.paginate(...):
        item: ListPublicKeysResultTypeDef
        print(item)  # (3)
```

1. client: [CloudFrontClient](./client.md)
2. paginator: [ListPublicKeysPaginator](./paginators.md#listpublickeyspaginator)
3. item: `AioPageIterator[ListPublicKeysResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPublicKeysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPublicKeysResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPublicKeysResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPublicKeysRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPublicKeysRequestPaginateTypeDef](./type_defs.md#listpublickeysrequestpaginatetypedef)
## ListStreamingDistributionsPaginator

Type annotations and code completion for `#!python session.client("cloudfront").get_paginator("list_streaming_distributions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront/paginator/ListStreamingDistributions.html#CloudFront.Paginator.ListStreamingDistributions)

```python
# ListStreamingDistributionsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_cloudfront.paginator import ListStreamingDistributionsPaginator

session = Session()

session = get_session()
async with session.client("cloudfront") as client:  # (1)
    paginator: ListStreamingDistributionsPaginator = client.get_paginator("list_streaming_distributions")  # (2)
    async for item in paginator.paginate(...):
        item: ListStreamingDistributionsResultTypeDef
        print(item)  # (3)
```

1. client: [CloudFrontClient](./client.md)
2. paginator: [ListStreamingDistributionsPaginator](./paginators.md#liststreamingdistributionspaginator)
3. item: `AioPageIterator[ListStreamingDistributionsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListStreamingDistributionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListStreamingDistributionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListStreamingDistributionsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListStreamingDistributionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStreamingDistributionsRequestPaginateTypeDef](./type_defs.md#liststreamingdistributionsrequestpaginatetypedef)
