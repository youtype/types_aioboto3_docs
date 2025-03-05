# Examples

> [Index](../README.md) > [ForecastQueryService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ForecastQueryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#forecastqueryservice)
    type annotations stubs module [types-aiobotocore-forecastquery](https://pypi.org/project/types-aiobotocore-forecastquery/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[forecastquery]` package installed.

Write your `ForecastQueryService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ForecastQueryServiceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("forecastquery") as client:  # (1)
    result = await client.query_forecast()  # (2)
```

1. client: [ForecastQueryServiceClient](./client.md)
2. result: [:material-code-braces: QueryForecastResponseTypeDef](./type_defs.md#queryforecastresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[forecastquery]`
or a standalone `types_aiobotocore_forecastquery` package, you have to explicitly specify
`client: ForecastQueryServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ForecastQueryServiceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_forecastquery.client import ForecastQueryServiceClient
from types_aiobotocore_forecastquery.type_defs import QueryForecastResponseTypeDef
from types_aiobotocore_forecastquery.type_defs import QueryForecastRequestTypeDef


session = Session()

client: ForecastQueryServiceClient
async with session.client("forecastquery") as client:  # (1)
    kwargs: QueryForecastRequestTypeDef = {...}  # (2)
    result: QueryForecastResponseTypeDef = await client.query_forecast(**kwargs)  # (3)
```

1. client: [ForecastQueryServiceClient](./client.md)
2. kwargs: [:material-code-braces: QueryForecastRequestTypeDef](./type_defs.md#queryforecastrequesttypedef)
3. result: [:material-code-braces: QueryForecastResponseTypeDef](./type_defs.md#queryforecastresponsetypedef)






