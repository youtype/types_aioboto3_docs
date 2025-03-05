# Examples

> [Index](../README.md) > [ElasticsearchService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ElasticsearchService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#elasticsearchservice)
    type annotations stubs module [types-aiobotocore-es](https://pypi.org/project/types-aiobotocore-es/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[es]` package installed.

Write your `ElasticsearchService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ElasticsearchServiceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("es") as client:  # (1)
    result = await client.accept_inbound_cross_cluster_search_connection()  # (2)
```

1. client: [ElasticsearchServiceClient](./client.md)
2. result: [:material-code-braces: AcceptInboundCrossClusterSearchConnectionResponseTypeDef](./type_defs.md#acceptinboundcrossclustersearchconnectionresponsetypedef)



#### Paginator usage example

```python
# DescribeReservedElasticsearchInstanceOfferingsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("es") as client:  # (1)
    paginator = client.get_paginator("describe_reserved_elasticsearch_instance_offerings")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ElasticsearchServiceClient](./client.md)
2. paginator: [DescribeReservedElasticsearchInstanceOfferingsPaginator](./paginators.md#describereservedelasticsearchinstanceofferingspaginator)
3. item: [:material-code-braces: DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef](./type_defs.md#describereservedelasticsearchinstanceofferingsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[es]`
or a standalone `types_aiobotocore_es` package, you have to explicitly specify
`client: ElasticsearchServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ElasticsearchServiceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_es.client import ElasticsearchServiceClient
from types_aiobotocore_es.type_defs import AcceptInboundCrossClusterSearchConnectionResponseTypeDef
from types_aiobotocore_es.type_defs import AcceptInboundCrossClusterSearchConnectionRequestTypeDef


session = Session()

client: ElasticsearchServiceClient
async with session.client("es") as client:  # (1)
    kwargs: AcceptInboundCrossClusterSearchConnectionRequestTypeDef = {...}  # (2)
    result: AcceptInboundCrossClusterSearchConnectionResponseTypeDef = await client.accept_inbound_cross_cluster_search_connection(**kwargs)  # (3)
```

1. client: [ElasticsearchServiceClient](./client.md)
2. kwargs: [:material-code-braces: AcceptInboundCrossClusterSearchConnectionRequestTypeDef](./type_defs.md#acceptinboundcrossclustersearchconnectionrequesttypedef)
3. result: [:material-code-braces: AcceptInboundCrossClusterSearchConnectionResponseTypeDef](./type_defs.md#acceptinboundcrossclustersearchconnectionresponsetypedef)



#### Paginator usage example

```python
# DescribeReservedElasticsearchInstanceOfferingsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_es.client import ElasticsearchServiceClient
from types_aiobotocore_es.paginator import DescribeReservedElasticsearchInstanceOfferingsPaginator
from types_aiobotocore_es.type_defs import DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef


session = Session()

client: ElasticsearchServiceClient
async with session.client("es") as client:  # (1)
    paginator: DescribeReservedElasticsearchInstanceOfferingsPaginator = client.get_paginator("describe_reserved_elasticsearch_instance_offerings")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef
        print(item)  # (3)
```

1. client: [ElasticsearchServiceClient](./client.md)
2. paginator: [DescribeReservedElasticsearchInstanceOfferingsPaginator](./paginators.md#describereservedelasticsearchinstanceofferingspaginator)
3. item: [:material-code-braces: DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef](./type_defs.md#describereservedelasticsearchinstanceofferingsresponsetypedef)




