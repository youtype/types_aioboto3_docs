# Examples

> [Index](../README.md) > [ECRPublic](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ECRPublic](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ecrpublic)
    type annotations stubs module [types-aiobotocore-ecr-public](https://pypi.org/project/types-aiobotocore-ecr-public/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[ecr-public]` package installed.

Write your `ECRPublic` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ECRPublicClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("ecr-public") as client:  # (1)
    result = await client.batch_check_layer_availability()  # (2)
```

1. client: [ECRPublicClient](./client.md)
2. result: [:material-code-braces: BatchCheckLayerAvailabilityResponseTypeDef](./type_defs.md#batchchecklayeravailabilityresponsetypedef)



#### Paginator usage example

```python
# DescribeImageTagsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("ecr-public") as client:  # (1)
    paginator = client.get_paginator("describe_image_tags")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ECRPublicClient](./client.md)
2. paginator: [DescribeImageTagsPaginator](./paginators.md#describeimagetagspaginator)
3. item: [:material-code-braces: DescribeImageTagsResponseTypeDef](./type_defs.md#describeimagetagsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[ecr-public]`
or a standalone `types_aiobotocore_ecr_public` package, you have to explicitly specify
`client: ECRPublicClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ECRPublicClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ecr_public.client import ECRPublicClient
from types_aiobotocore_ecr_public.type_defs import BatchCheckLayerAvailabilityResponseTypeDef
from types_aiobotocore_ecr_public.type_defs import BatchCheckLayerAvailabilityRequestTypeDef


session = Session()

client: ECRPublicClient
async with session.client("ecr-public") as client:  # (1)
    kwargs: BatchCheckLayerAvailabilityRequestTypeDef = {...}  # (2)
    result: BatchCheckLayerAvailabilityResponseTypeDef = await client.batch_check_layer_availability(**kwargs)  # (3)
```

1. client: [ECRPublicClient](./client.md)
2. kwargs: [:material-code-braces: BatchCheckLayerAvailabilityRequestTypeDef](./type_defs.md#batchchecklayeravailabilityrequesttypedef)
3. result: [:material-code-braces: BatchCheckLayerAvailabilityResponseTypeDef](./type_defs.md#batchchecklayeravailabilityresponsetypedef)



#### Paginator usage example

```python
# DescribeImageTagsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ecr_public.client import ECRPublicClient
from types_aiobotocore_ecr_public.paginator import DescribeImageTagsPaginator
from types_aiobotocore_ecr_public.type_defs import DescribeImageTagsResponseTypeDef


session = Session()

client: ECRPublicClient
async with session.client("ecr-public") as client:  # (1)
    paginator: DescribeImageTagsPaginator = client.get_paginator("describe_image_tags")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeImageTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [ECRPublicClient](./client.md)
2. paginator: [DescribeImageTagsPaginator](./paginators.md#describeimagetagspaginator)
3. item: [:material-code-braces: DescribeImageTagsResponseTypeDef](./type_defs.md#describeimagetagsresponsetypedef)




