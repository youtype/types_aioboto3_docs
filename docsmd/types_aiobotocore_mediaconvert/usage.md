# Examples

> [Index](../README.md) > [MediaConvert](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MediaConvert](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#mediaconvert)
    type annotations stubs module [types-aiobotocore-mediaconvert](https://pypi.org/project/types-aiobotocore-mediaconvert/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[mediaconvert]` package installed.

Write your `MediaConvert` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# MediaConvertClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("mediaconvert") as client:  # (1)
    result = await client.create_job()  # (2)
```

1. client: [MediaConvertClient](./client.md)
2. result: [:material-code-braces: CreateJobResponseTypeDef](./type_defs.md#createjobresponsetypedef)



#### Paginator usage example

```python
# DescribeEndpointsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("mediaconvert") as client:  # (1)
    paginator = client.get_paginator("describe_endpoints")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MediaConvertClient](./client.md)
2. paginator: [DescribeEndpointsPaginator](./paginators.md#describeendpointspaginator)
3. item: [:material-code-braces: DescribeEndpointsResponseTypeDef](./type_defs.md#describeendpointsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[mediaconvert]`
or a standalone `types_aiobotocore_mediaconvert` package, you have to explicitly specify
`client: MediaConvertClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# MediaConvertClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_mediaconvert.client import MediaConvertClient
from types_aiobotocore_mediaconvert.type_defs import CreateJobResponseTypeDef
from types_aiobotocore_mediaconvert.type_defs import CreateJobRequestTypeDef


session = Session()

client: MediaConvertClient
async with session.client("mediaconvert") as client:  # (1)
    kwargs: CreateJobRequestTypeDef = {...}  # (2)
    result: CreateJobResponseTypeDef = await client.create_job(**kwargs)  # (3)
```

1. client: [MediaConvertClient](./client.md)
2. kwargs: [:material-code-braces: CreateJobRequestTypeDef](./type_defs.md#createjobrequesttypedef)
3. result: [:material-code-braces: CreateJobResponseTypeDef](./type_defs.md#createjobresponsetypedef)



#### Paginator usage example

```python
# DescribeEndpointsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_mediaconvert.client import MediaConvertClient
from types_aiobotocore_mediaconvert.paginator import DescribeEndpointsPaginator
from types_aiobotocore_mediaconvert.type_defs import DescribeEndpointsResponseTypeDef


session = Session()

client: MediaConvertClient
async with session.client("mediaconvert") as client:  # (1)
    paginator: DescribeEndpointsPaginator = client.get_paginator("describe_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEndpointsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConvertClient](./client.md)
2. paginator: [DescribeEndpointsPaginator](./paginators.md#describeendpointspaginator)
3. item: [:material-code-braces: DescribeEndpointsResponseTypeDef](./type_defs.md#describeendpointsresponsetypedef)




