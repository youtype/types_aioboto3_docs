# Examples

> [Index](../README.md) > [S3Outposts](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [S3Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#s3outposts)
    type annotations stubs module [types-aiobotocore-s3outposts](https://pypi.org/project/types-aiobotocore-s3outposts/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[s3outposts]` package installed.

Write your `S3Outposts` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# S3OutpostsClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("s3outposts") as client:  # (1)
    result = await client.create_endpoint()  # (2)
```

1. client: [S3OutpostsClient](./client.md)
2. result: [:material-code-braces: CreateEndpointResultTypeDef](./type_defs.md#createendpointresulttypedef)



#### Paginator usage example

```python
# ListEndpointsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("s3outposts") as client:  # (1)
    paginator = client.get_paginator("list_endpoints")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [S3OutpostsClient](./client.md)
2. paginator: [ListEndpointsPaginator](./paginators.md#listendpointspaginator)
3. item: [:material-code-braces: ListEndpointsResultTypeDef](./type_defs.md#listendpointsresulttypedef)




### Explicit type annotations

With `types-aioboto3-lite[s3outposts]`
or a standalone `types_aiobotocore_s3outposts` package, you have to explicitly specify
`client: S3OutpostsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# S3OutpostsClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_s3outposts.client import S3OutpostsClient
from types_aiobotocore_s3outposts.type_defs import CreateEndpointResultTypeDef
from types_aiobotocore_s3outposts.type_defs import CreateEndpointRequestTypeDef


session = Session()

client: S3OutpostsClient
async with session.client("s3outposts") as client:  # (1)
    kwargs: CreateEndpointRequestTypeDef = {...}  # (2)
    result: CreateEndpointResultTypeDef = await client.create_endpoint(**kwargs)  # (3)
```

1. client: [S3OutpostsClient](./client.md)
2. kwargs: [:material-code-braces: CreateEndpointRequestTypeDef](./type_defs.md#createendpointrequesttypedef)
3. result: [:material-code-braces: CreateEndpointResultTypeDef](./type_defs.md#createendpointresulttypedef)



#### Paginator usage example

```python
# ListEndpointsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_s3outposts.client import S3OutpostsClient
from types_aiobotocore_s3outposts.paginator import ListEndpointsPaginator
from types_aiobotocore_s3outposts.type_defs import ListEndpointsResultTypeDef


session = Session()

client: S3OutpostsClient
async with session.client("s3outposts") as client:  # (1)
    paginator: ListEndpointsPaginator = client.get_paginator("list_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: ListEndpointsResultTypeDef
        print(item)  # (3)
```

1. client: [S3OutpostsClient](./client.md)
2. paginator: [ListEndpointsPaginator](./paginators.md#listendpointspaginator)
3. item: [:material-code-braces: ListEndpointsResultTypeDef](./type_defs.md#listendpointsresulttypedef)




