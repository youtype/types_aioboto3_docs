# Examples

> [Index](../README.md) > [Snowball](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Snowball](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#snowball)
    type annotations stubs module [types-aiobotocore-snowball](https://pypi.org/project/types-aiobotocore-snowball/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[snowball]` package installed.

Write your `Snowball` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SnowballClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("snowball") as client:  # (1)
    result = await client.create_address()  # (2)
```

1. client: [SnowballClient](./client.md)
2. result: [:material-code-braces: CreateAddressResultTypeDef](./type_defs.md#createaddressresulttypedef)



#### Paginator usage example

```python
# DescribeAddressesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("snowball") as client:  # (1)
    paginator = client.get_paginator("describe_addresses")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SnowballClient](./client.md)
2. paginator: [DescribeAddressesPaginator](./paginators.md#describeaddressespaginator)
3. item: [:material-code-braces: DescribeAddressesResultTypeDef](./type_defs.md#describeaddressesresulttypedef)




### Explicit type annotations

With `types-aioboto3-lite[snowball]`
or a standalone `types_aiobotocore_snowball` package, you have to explicitly specify
`client: SnowballClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SnowballClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_snowball.client import SnowballClient
from types_aiobotocore_snowball.type_defs import CreateAddressResultTypeDef
from types_aiobotocore_snowball.type_defs import CreateAddressRequestTypeDef


session = Session()

client: SnowballClient
async with session.client("snowball") as client:  # (1)
    kwargs: CreateAddressRequestTypeDef = {...}  # (2)
    result: CreateAddressResultTypeDef = await client.create_address(**kwargs)  # (3)
```

1. client: [SnowballClient](./client.md)
2. kwargs: [:material-code-braces: CreateAddressRequestTypeDef](./type_defs.md#createaddressrequesttypedef)
3. result: [:material-code-braces: CreateAddressResultTypeDef](./type_defs.md#createaddressresulttypedef)



#### Paginator usage example

```python
# DescribeAddressesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_snowball.client import SnowballClient
from types_aiobotocore_snowball.paginator import DescribeAddressesPaginator
from types_aiobotocore_snowball.type_defs import DescribeAddressesResultTypeDef


session = Session()

client: SnowballClient
async with session.client("snowball") as client:  # (1)
    paginator: DescribeAddressesPaginator = client.get_paginator("describe_addresses")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAddressesResultTypeDef
        print(item)  # (3)
```

1. client: [SnowballClient](./client.md)
2. paginator: [DescribeAddressesPaginator](./paginators.md#describeaddressespaginator)
3. item: [:material-code-braces: DescribeAddressesResultTypeDef](./type_defs.md#describeaddressesresulttypedef)




