# Examples

> [Index](../README.md) > [MarketplaceReportingService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MarketplaceReportingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-reporting.html#marketplacereportingservice)
    type annotations stubs module [types-aiobotocore-marketplace-reporting](https://pypi.org/project/types-aiobotocore-marketplace-reporting/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[marketplace-reporting]` package installed.

Write your `MarketplaceReportingService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# MarketplaceReportingServiceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("marketplace-reporting") as client:  # (1)
    result = await client.get_buyer_dashboard()  # (2)
```

1. client: [MarketplaceReportingServiceClient](./client.md)
2. result: [:material-code-braces: GetBuyerDashboardOutputTypeDef](./type_defs.md#getbuyerdashboardoutputtypedef)






### Explicit type annotations

With `types-aioboto3-lite[marketplace-reporting]`
or a standalone `types_aiobotocore_marketplace_reporting` package, you have to explicitly specify
`client: MarketplaceReportingServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# MarketplaceReportingServiceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_marketplace_reporting.client import MarketplaceReportingServiceClient
from types_aiobotocore_marketplace_reporting.type_defs import GetBuyerDashboardOutputTypeDef
from types_aiobotocore_marketplace_reporting.type_defs import GetBuyerDashboardInputTypeDef


session = Session()

client: MarketplaceReportingServiceClient
async with session.client("marketplace-reporting") as client:  # (1)
    kwargs: GetBuyerDashboardInputTypeDef = {...}  # (2)
    result: GetBuyerDashboardOutputTypeDef = await client.get_buyer_dashboard(**kwargs)  # (3)
```

1. client: [MarketplaceReportingServiceClient](./client.md)
2. kwargs: [:material-code-braces: GetBuyerDashboardInputTypeDef](./type_defs.md#getbuyerdashboardinputtypedef)
3. result: [:material-code-braces: GetBuyerDashboardOutputTypeDef](./type_defs.md#getbuyerdashboardoutputtypedef)






