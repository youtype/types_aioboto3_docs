# MarketplaceEntitlementServiceClient

> [Index](../README.md) > [MarketplaceEntitlementService](./README.md) > MarketplaceEntitlementServiceClient

!!! note ""

    Auto-generated documentation for [MarketplaceEntitlementService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#marketplaceentitlementservice)
    type annotations stubs module [types-aiobotocore-marketplace-entitlement](https://pypi.org/project/types-aiobotocore-marketplace-entitlement/).

## MarketplaceEntitlementServiceClient

Type annotations and code completion for `#!python session.client("marketplace-entitlement")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client)

```python
# MarketplaceEntitlementServiceClient usage example

from aioboto3.session import Session
from types_aiobotocore_marketplace_entitlement.client import MarketplaceEntitlementServiceClient

session = Session()
async with session.client("marketplace-entitlement") as client:
    client: MarketplaceEntitlementServiceClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("marketplace-entitlement").exceptions` structure.

```python
# MarketplaceEntitlementServiceClient.exceptions usage example

async with session.client("marketplace-entitlement") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.InternalServiceErrorException,
        client.exceptions.InvalidParameterException,
        client.exceptions.ThrottlingException,
    ) as e:
        print(e)
```

```python
# MarketplaceEntitlementServiceClient.exceptions type checking example

from types_aiobotocore_marketplace_entitlement.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("marketplace-entitlement").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("marketplace-entitlement").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client)

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


### get\_entitlements

GetEntitlements retrieves entitlement values for a given product.

Type annotations and code completion for `#!python session.client("marketplace-entitlement").get_entitlements` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client)

```python
# get_entitlements method definition

await def get_entitlements(
    self,
    *,
    ProductCode: str,
    Filter: Mapping[GetEntitlementFilterNameType, Sequence[str]] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetEntitlementsResultTypeDef:  # (2)
    ...
```

1. See `Mapping[GetEntitlementFilterNameType, Sequence[str]]`
2. See [:material-code-braces: GetEntitlementsResultTypeDef](./type_defs.md#getentitlementsresulttypedef)


```python
# get_entitlements method usage example with argument unpacking

kwargs: GetEntitlementsRequestTypeDef = {  # (1)
    "ProductCode": ...,
}

parent.get_entitlements(**kwargs)
```

1. See [:material-code-braces: GetEntitlementsRequestTypeDef](./type_defs.md#getentitlementsrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("marketplace-entitlement").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("marketplace-entitlement").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client)

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




### get_paginator

Type annotations and code completion for `#!python session.client("marketplace-entitlement").get_paginator` method with overloads.

- `client.get_paginator("get_entitlements")` -> [GetEntitlementsPaginator](./paginators.md#getentitlementspaginator)



