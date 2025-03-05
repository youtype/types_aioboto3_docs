# Examples

> [Index](../README.md) > [Pricing](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Pricing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#pricing)
    type annotations stubs module [types-aiobotocore-pricing](https://pypi.org/project/types-aiobotocore-pricing/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[pricing]` package installed.

Write your `Pricing` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# PricingClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("pricing") as client:  # (1)
    result = await client.describe_services()  # (2)
```

1. client: [PricingClient](./client.md)
2. result: [:material-code-braces: DescribeServicesResponseTypeDef](./type_defs.md#describeservicesresponsetypedef)



#### Paginator usage example

```python
# DescribeServicesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("pricing") as client:  # (1)
    paginator = client.get_paginator("describe_services")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [PricingClient](./client.md)
2. paginator: [DescribeServicesPaginator](./paginators.md#describeservicespaginator)
3. item: [:material-code-braces: DescribeServicesResponseTypeDef](./type_defs.md#describeservicesresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[pricing]`
or a standalone `types_aiobotocore_pricing` package, you have to explicitly specify
`client: PricingClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# PricingClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_pricing.client import PricingClient
from types_aiobotocore_pricing.type_defs import DescribeServicesResponseTypeDef
from types_aiobotocore_pricing.type_defs import DescribeServicesRequestTypeDef


session = Session()

client: PricingClient
async with session.client("pricing") as client:  # (1)
    kwargs: DescribeServicesRequestTypeDef = {...}  # (2)
    result: DescribeServicesResponseTypeDef = await client.describe_services(**kwargs)  # (3)
```

1. client: [PricingClient](./client.md)
2. kwargs: [:material-code-braces: DescribeServicesRequestTypeDef](./type_defs.md#describeservicesrequesttypedef)
3. result: [:material-code-braces: DescribeServicesResponseTypeDef](./type_defs.md#describeservicesresponsetypedef)



#### Paginator usage example

```python
# DescribeServicesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_pricing.client import PricingClient
from types_aiobotocore_pricing.paginator import DescribeServicesPaginator
from types_aiobotocore_pricing.type_defs import DescribeServicesResponseTypeDef


session = Session()

client: PricingClient
async with session.client("pricing") as client:  # (1)
    paginator: DescribeServicesPaginator = client.get_paginator("describe_services")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeServicesResponseTypeDef
        print(item)  # (3)
```

1. client: [PricingClient](./client.md)
2. paginator: [DescribeServicesPaginator](./paginators.md#describeservicespaginator)
3. item: [:material-code-braces: DescribeServicesResponseTypeDef](./type_defs.md#describeservicesresponsetypedef)




