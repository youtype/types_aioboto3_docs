# Paginators

> [Index](../README.md) > [OpsWorks](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [OpsWorks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#opsworks)
    type annotations stubs module [types-aiobotocore-opsworks](https://pypi.org/project/types-aiobotocore-opsworks/).

## DescribeEcsClustersPaginator

Type annotations and code completion for `#!python session.client("opsworks").get_paginator("describe_ecs_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/paginator/DescribeEcsClusters.html#OpsWorks.Paginator.DescribeEcsClusters)

```python
# DescribeEcsClustersPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_opsworks.paginator import DescribeEcsClustersPaginator

session = Session()

session = get_session()
async with session.client("opsworks") as client:  # (1)
    paginator: DescribeEcsClustersPaginator = client.get_paginator("describe_ecs_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEcsClustersResultTypeDef
        print(item)  # (3)
```

1. client: [OpsWorksClient](./client.md)
2. paginator: [DescribeEcsClustersPaginator](./paginators.md#describeecsclusterspaginator)
3. item: `AioPageIterator[DescribeEcsClustersResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeEcsClustersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    EcsClusterArns: Sequence[str] = ...,
    StackId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeEcsClustersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeEcsClustersResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEcsClustersRequestPaginateTypeDef = {  # (1)
    "EcsClusterArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEcsClustersRequestPaginateTypeDef](./type_defs.md#describeecsclustersrequestpaginatetypedef)
