# PricingClient

> [Index](../README.md) > [Pricing](./README.md) > PricingClient

!!! note ""

    Auto-generated documentation for [Pricing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#pricing)
    type annotations stubs module [types-aiobotocore-pricing](https://pypi.org/project/types-aiobotocore-pricing/).

## PricingClient

Type annotations and code completion for `#!python session.client("pricing")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client)

```python
# PricingClient usage example

from aioboto3.session import Session
from types_aiobotocore_pricing.client import PricingClient

session = Session()
async with session.client("pricing") as client:
    client: PricingClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("pricing").exceptions` structure.

```python
# PricingClient.exceptions usage example

async with session.client("pricing") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ExpiredNextTokenException,
        client.exceptions.InternalErrorException,
        client.exceptions.InvalidNextTokenException,
        client.exceptions.InvalidParameterException,
        client.exceptions.NotFoundException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ThrottlingException,
    ) as e:
        print(e)
```

```python
# PricingClient.exceptions type checking example

from types_aiobotocore_pricing.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("pricing").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("pricing").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client)

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


### describe\_services

Returns the metadata for one service or a list of the metadata for all services.

Type annotations and code completion for `#!python session.client("pricing").describe_services` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client)

```python
# describe_services method definition

await def describe_services(
    self,
    *,
    ServiceCode: str = ...,
    FormatVersion: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeServicesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeServicesResponseTypeDef](./type_defs.md#describeservicesresponsetypedef) 


```python
# describe_services method usage example with argument unpacking

kwargs: DescribeServicesRequestRequestTypeDef = {  # (1)
    "ServiceCode": ...,
}

parent.describe_services(**kwargs)
```

1. See [:material-code-braces: DescribeServicesRequestRequestTypeDef](./type_defs.md#describeservicesrequestrequesttypedef) 

### get\_attribute\_values

Returns a list of attribute values.

Type annotations and code completion for `#!python session.client("pricing").get_attribute_values` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client)

```python
# get_attribute_values method definition

await def get_attribute_values(
    self,
    *,
    ServiceCode: str,
    AttributeName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetAttributeValuesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAttributeValuesResponseTypeDef](./type_defs.md#getattributevaluesresponsetypedef) 


```python
# get_attribute_values method usage example with argument unpacking

kwargs: GetAttributeValuesRequestRequestTypeDef = {  # (1)
    "ServiceCode": ...,
    "AttributeName": ...,
}

parent.get_attribute_values(**kwargs)
```

1. See [:material-code-braces: GetAttributeValuesRequestRequestTypeDef](./type_defs.md#getattributevaluesrequestrequesttypedef) 

### get\_price\_list\_file\_url

<i> <b>This feature is in preview release and is subject to change.

Type annotations and code completion for `#!python session.client("pricing").get_price_list_file_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client)

```python
# get_price_list_file_url method definition

await def get_price_list_file_url(
    self,
    *,
    PriceListArn: str,
    FileFormat: str,
) -> GetPriceListFileUrlResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPriceListFileUrlResponseTypeDef](./type_defs.md#getpricelistfileurlresponsetypedef) 


```python
# get_price_list_file_url method usage example with argument unpacking

kwargs: GetPriceListFileUrlRequestRequestTypeDef = {  # (1)
    "PriceListArn": ...,
    "FileFormat": ...,
}

parent.get_price_list_file_url(**kwargs)
```

1. See [:material-code-braces: GetPriceListFileUrlRequestRequestTypeDef](./type_defs.md#getpricelistfileurlrequestrequesttypedef) 

### get\_products

Returns a list of all products that match the filter criteria.

Type annotations and code completion for `#!python session.client("pricing").get_products` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client)

```python
# get_products method definition

await def get_products(
    self,
    *,
    ServiceCode: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    FormatVersion: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetProductsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: GetProductsResponseTypeDef](./type_defs.md#getproductsresponsetypedef) 


```python
# get_products method usage example with argument unpacking

kwargs: GetProductsRequestRequestTypeDef = {  # (1)
    "ServiceCode": ...,
}

parent.get_products(**kwargs)
```

1. See [:material-code-braces: GetProductsRequestRequestTypeDef](./type_defs.md#getproductsrequestrequesttypedef) 

### list\_price\_lists

<i> <b>This feature is in preview release and is subject to change.

Type annotations and code completion for `#!python session.client("pricing").list_price_lists` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client)

```python
# list_price_lists method definition

await def list_price_lists(
    self,
    *,
    ServiceCode: str,
    EffectiveDate: TimestampTypeDef,
    CurrencyCode: str,
    RegionCode: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListPriceListsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPriceListsResponseTypeDef](./type_defs.md#listpricelistsresponsetypedef) 


```python
# list_price_lists method usage example with argument unpacking

kwargs: ListPriceListsRequestRequestTypeDef = {  # (1)
    "ServiceCode": ...,
    "EffectiveDate": ...,
    "CurrencyCode": ...,
}

parent.list_price_lists(**kwargs)
```

1. See [:material-code-braces: ListPriceListsRequestRequestTypeDef](./type_defs.md#listpricelistsrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("pricing").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("pricing").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client)

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

Type annotations and code completion for `#!python session.client("pricing").get_paginator` method with overloads.

- `client.get_paginator("describe_services")` -> [DescribeServicesPaginator](./paginators.md#describeservicespaginator)
- `client.get_paginator("get_attribute_values")` -> [GetAttributeValuesPaginator](./paginators.md#getattributevaluespaginator)
- `client.get_paginator("get_products")` -> [GetProductsPaginator](./paginators.md#getproductspaginator)
- `client.get_paginator("list_price_lists")` -> [ListPriceListsPaginator](./paginators.md#listpricelistspaginator)


