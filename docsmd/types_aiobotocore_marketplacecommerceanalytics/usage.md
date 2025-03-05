# Examples

> [Index](../README.md) > [MarketplaceCommerceAnalytics](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MarketplaceCommerceAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#marketplacecommerceanalytics)
    type annotations stubs module [types-aiobotocore-marketplacecommerceanalytics](https://pypi.org/project/types-aiobotocore-marketplacecommerceanalytics/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[marketplacecommerceanalytics]` package installed.

Write your `MarketplaceCommerceAnalytics` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# MarketplaceCommerceAnalyticsClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("marketplacecommerceanalytics") as client:  # (1)
    result = await client.generate_data_set()  # (2)
```

1. client: [MarketplaceCommerceAnalyticsClient](./client.md)
2. result: [:material-code-braces: GenerateDataSetResultTypeDef](./type_defs.md#generatedatasetresulttypedef)






### Explicit type annotations

With `types-aioboto3-lite[marketplacecommerceanalytics]`
or a standalone `types_aiobotocore_marketplacecommerceanalytics` package, you have to explicitly specify
`client: MarketplaceCommerceAnalyticsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# MarketplaceCommerceAnalyticsClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_marketplacecommerceanalytics.client import MarketplaceCommerceAnalyticsClient
from types_aiobotocore_marketplacecommerceanalytics.type_defs import GenerateDataSetResultTypeDef
from types_aiobotocore_marketplacecommerceanalytics.type_defs import GenerateDataSetRequestTypeDef


session = Session()

client: MarketplaceCommerceAnalyticsClient
async with session.client("marketplacecommerceanalytics") as client:  # (1)
    kwargs: GenerateDataSetRequestTypeDef = {...}  # (2)
    result: GenerateDataSetResultTypeDef = await client.generate_data_set(**kwargs)  # (3)
```

1. client: [MarketplaceCommerceAnalyticsClient](./client.md)
2. kwargs: [:material-code-braces: GenerateDataSetRequestTypeDef](./type_defs.md#generatedatasetrequesttypedef)
3. result: [:material-code-braces: GenerateDataSetResultTypeDef](./type_defs.md#generatedatasetresulttypedef)






