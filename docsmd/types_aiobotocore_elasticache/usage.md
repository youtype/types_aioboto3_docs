# Examples

> [Index](../README.md) > [ElastiCache](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ElastiCache](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
    type annotations stubs module [types-aiobotocore-elasticache](https://pypi.org/project/types-aiobotocore-elasticache/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[elasticache]` package installed.

Write your `ElastiCache` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("elasticache") as client:  # (1)
        result = await client.add_tags_to_resource()  # (2)
    ```

    1. client: [ElastiCacheClient](./client.md)
    2. result: [:material-code-braces: TagListMessageTypeDef](./type_defs.md#taglistmessagetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("elasticache") as client:  # (1)
        paginator = client.get_paginator("describe_cache_clusters")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [ElastiCacheClient](./client.md)
    2. paginator: [DescribeCacheClustersPaginator](./paginators.md#describecacheclusterspaginator)
    3. item: [:material-code-braces: CacheClusterMessageTypeDef](./type_defs.md#cacheclustermessagetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("elasticache") as client:  # (1)
        waiter = client.get_waiter("cache_cluster_available")  # (2)
        await waiter.wait()
    ```

    1. client: [ElastiCacheClient](./client.md)
    2. waiter: [CacheClusterAvailableWaiter](./waiters.md#cacheclusteravailablewaiter)


### Explicit type annotations

With `types-aioboto3-lite[elasticache]`
or a standalone `types_aiobotocore_elasticache` package, you have to explicitly specify
`client: ElastiCacheClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_elasticache.client import ElastiCacheClient
    from types_aiobotocore_elasticache.type_defs import TagListMessageTypeDef
    from types_aiobotocore_elasticache.type_defs import AddTagsToResourceMessageRequestTypeDef


    session = Session()

    client: ElastiCacheClient
    async with session.client("elasticache") as client:  # (1)
        kwargs: AddTagsToResourceMessageRequestTypeDef = {...}  # (2)
        result: TagListMessageTypeDef = await client.add_tags_to_resource(**kwargs)  # (3)
    ```

    1. client: [ElastiCacheClient](./client.md)
    2. kwargs: [:material-code-braces: AddTagsToResourceMessageRequestTypeDef](./type_defs.md#addtagstoresourcemessagerequesttypedef) 
    3. result: [:material-code-braces: TagListMessageTypeDef](./type_defs.md#taglistmessagetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_elasticache.client import ElastiCacheClient
    from types_aiobotocore_elasticache.paginator import DescribeCacheClustersPaginator
    from types_aiobotocore_elasticache.type_defs import CacheClusterMessageTypeDef


    session = Session()

    client: ElastiCacheClient
    async with session.client("elasticache") as client:  # (1)
        paginator: DescribeCacheClustersPaginator = client.get_paginator("describe_cache_clusters")  # (2)
        async for item in paginator.paginate(...):
            item: CacheClusterMessageTypeDef
            print(item)  # (3)
    ```

    1. client: [ElastiCacheClient](./client.md)
    2. paginator: [DescribeCacheClustersPaginator](./paginators.md#describecacheclusterspaginator)
    3. item: [:material-code-braces: CacheClusterMessageTypeDef](./type_defs.md#cacheclustermessagetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_elasticache.client import ElastiCacheClient
    from types_aiobotocore_elasticache.waiter import CacheClusterAvailableWaiter


    session = Session()

    async with session.client("elasticache") as client:  # (1)
        waiter = client.get_waiter("cache_cluster_available")  # (2)
        await waiter.wait()
    ```

    1. client: [ElastiCacheClient](./client.md)
    2. waiter: [CacheClusterAvailableWaiter](./waiters.md#cacheclusteravailablewaiter)


