# ForecastQueryServiceClient

> [Index](../README.md) > [ForecastQueryService](./README.md) > ForecastQueryServiceClient

!!! note ""

    Auto-generated documentation for [ForecastQueryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#forecastqueryservice)
    type annotations stubs module [types-aiobotocore-forecastquery](https://pypi.org/project/types-aiobotocore-forecastquery/).

## ForecastQueryServiceClient

Type annotations and code completion for `#!python session.client("forecastquery")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client)

```python
# ForecastQueryServiceClient usage example

from aioboto3.session import Session
from types_aiobotocore_forecastquery.client import ForecastQueryServiceClient

session = Session()
async with session.client("forecastquery") as client:
    client: ForecastQueryServiceClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("forecastquery").exceptions` structure.

```python
# ForecastQueryServiceClient.exceptions usage example

async with session.client("forecastquery") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.InvalidInputException,
        client.exceptions.InvalidNextTokenException,
        client.exceptions.LimitExceededException,
        client.exceptions.ResourceInUseException,
        client.exceptions.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python
# ForecastQueryServiceClient.exceptions type checking example

from types_aiobotocore_forecastquery.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("forecastquery").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("forecastquery").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### query\_forecast

Retrieves a forecast for a single item, filtered by the supplied criteria.

Type annotations and code completion for `#!python session.client("forecastquery").query_forecast` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client)

```python
# query_forecast method definition

await def query_forecast(
    self,
    *,
    ForecastArn: str,
    Filters: Mapping[str, str],
    StartDate: str = ...,
    EndDate: str = ...,
    NextToken: str = ...,
) -> QueryForecastResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: QueryForecastResponseTypeDef](./type_defs.md#queryforecastresponsetypedef)


```python
# query_forecast method usage example with argument unpacking

kwargs: QueryForecastRequestTypeDef = {  # (1)
    "ForecastArn": ...,
    "Filters": ...,
}

parent.query_forecast(**kwargs)
```

1. See [:material-code-braces: QueryForecastRequestTypeDef](./type_defs.md#queryforecastrequesttypedef)

### query\_what\_if\_forecast

Retrieves a what-if forecast.

Type annotations and code completion for `#!python session.client("forecastquery").query_what_if_forecast` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client)

```python
# query_what_if_forecast method definition

await def query_what_if_forecast(
    self,
    *,
    WhatIfForecastArn: str,
    Filters: Mapping[str, str],
    StartDate: str = ...,
    EndDate: str = ...,
    NextToken: str = ...,
) -> QueryWhatIfForecastResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: QueryWhatIfForecastResponseTypeDef](./type_defs.md#querywhatifforecastresponsetypedef)


```python
# query_what_if_forecast method usage example with argument unpacking

kwargs: QueryWhatIfForecastRequestTypeDef = {  # (1)
    "WhatIfForecastArn": ...,
    "Filters": ...,
}

parent.query_what_if_forecast(**kwargs)
```

1. See [:material-code-braces: QueryWhatIfForecastRequestTypeDef](./type_defs.md#querywhatifforecastrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("forecastquery").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("forecastquery").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```





