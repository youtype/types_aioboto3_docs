# Paginators

> [Index](../README.md) > [ElasticInference](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ElasticInference](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#elasticinference)
    type annotations stubs module [types-aiobotocore-elastic-inference](https://pypi.org/project/types-aiobotocore-elastic-inference/).

## DescribeAcceleratorsPaginator

Type annotations and code completion for `#!python session.client("elastic-inference").get_paginator("describe_accelerators")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference/paginator/DescribeAccelerators.html#ElasticInference.Paginator.DescribeAccelerators)

```python
# DescribeAcceleratorsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_elastic_inference.paginator import DescribeAcceleratorsPaginator

session = Session()

session = get_session()
async with session.client("elastic-inference") as client:  # (1)
    paginator: DescribeAcceleratorsPaginator = client.get_paginator("describe_accelerators")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAcceleratorsResponseTypeDef
        print(item)  # (3)
```

1. client: [ElasticInferenceClient](./client.md)
2. paginator: [DescribeAcceleratorsPaginator](./paginators.md#describeacceleratorspaginator)
3. item: [:material-code-braces: DescribeAcceleratorsResponseTypeDef](./type_defs.md#describeacceleratorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAcceleratorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    acceleratorIds: Sequence[str] = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeAcceleratorsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeAcceleratorsResponseTypeDef](./type_defs.md#describeacceleratorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAcceleratorsRequestPaginateTypeDef = {  # (1)
    "acceleratorIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAcceleratorsRequestPaginateTypeDef](./type_defs.md#describeacceleratorsrequestpaginatetypedef) 