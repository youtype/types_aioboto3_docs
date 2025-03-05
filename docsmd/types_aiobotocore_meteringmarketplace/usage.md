# Examples

> [Index](../README.md) > [MarketplaceMetering](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MarketplaceMetering](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#marketplacemetering)
    type annotations stubs module [types-aiobotocore-meteringmarketplace](https://pypi.org/project/types-aiobotocore-meteringmarketplace/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[meteringmarketplace]` package installed.

Write your `MarketplaceMetering` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# MarketplaceMeteringClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("meteringmarketplace") as client:  # (1)
    result = await client.batch_meter_usage()  # (2)
```

1. client: [MarketplaceMeteringClient](./client.md)
2. result: [:material-code-braces: BatchMeterUsageResultTypeDef](./type_defs.md#batchmeterusageresulttypedef)






### Explicit type annotations

With `types-aioboto3-lite[meteringmarketplace]`
or a standalone `types_aiobotocore_meteringmarketplace` package, you have to explicitly specify
`client: MarketplaceMeteringClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# MarketplaceMeteringClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_meteringmarketplace.client import MarketplaceMeteringClient
from types_aiobotocore_meteringmarketplace.type_defs import BatchMeterUsageResultTypeDef
from types_aiobotocore_meteringmarketplace.type_defs import BatchMeterUsageRequestTypeDef


session = Session()

client: MarketplaceMeteringClient
async with session.client("meteringmarketplace") as client:  # (1)
    kwargs: BatchMeterUsageRequestTypeDef = {...}  # (2)
    result: BatchMeterUsageResultTypeDef = await client.batch_meter_usage(**kwargs)  # (3)
```

1. client: [MarketplaceMeteringClient](./client.md)
2. kwargs: [:material-code-braces: BatchMeterUsageRequestTypeDef](./type_defs.md#batchmeterusagerequesttypedef)
3. result: [:material-code-braces: BatchMeterUsageResultTypeDef](./type_defs.md#batchmeterusageresulttypedef)






