# BillingClient

> [Index](../README.md) > [Billing](./README.md) > BillingClient

!!! note ""

    Auto-generated documentation for [Billing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#billing)
    type annotations stubs module [types-aiobotocore-billing](https://pypi.org/project/types-aiobotocore-billing/).

## BillingClient

Type annotations and code completion for `#!python session.client("billing")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#Billing.Client)

```python
# BillingClient usage example

from aioboto3.session import Session
from types_aiobotocore_billing.client import BillingClient

session = Session()
async with session.client("billing") as client:
    client: BillingClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("billing").exceptions` structure.

```python
# BillingClient.exceptions usage example

async with session.client("billing") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.InternalServerException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# BillingClient.exceptions type checking example

from types_aiobotocore_billing.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("billing").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#Billing.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("billing").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#Billing.Client)

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


### list\_billing\_views

Lists the billing views available for a given time period.

Type annotations and code completion for `#!python session.client("billing").list_billing_views` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#Billing.Client)

```python
# list_billing_views method definition

await def list_billing_views(
    self,
    *,
    activeTimeRange: ActiveTimeRangeTypeDef,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListBillingViewsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ActiveTimeRangeTypeDef](./type_defs.md#activetimerangetypedef) 
2. See [:material-code-braces: ListBillingViewsResponseTypeDef](./type_defs.md#listbillingviewsresponsetypedef) 


```python
# list_billing_views method usage example with argument unpacking

kwargs: ListBillingViewsRequestRequestTypeDef = {  # (1)
    "activeTimeRange": ...,
}

parent.list_billing_views(**kwargs)
```

1. See [:material-code-braces: ListBillingViewsRequestRequestTypeDef](./type_defs.md#listbillingviewsrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("billing").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#Billing.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("billing").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#Billing.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("billing").get_paginator` method with overloads.

- `client.get_paginator("list_billing_views")` -> [ListBillingViewsPaginator](./paginators.md#listbillingviewspaginator)



