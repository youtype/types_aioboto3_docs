# MarketplaceCatalogClient

> [Index](../README.md) > [MarketplaceCatalog](./README.md) > MarketplaceCatalogClient

!!! note ""

    Auto-generated documentation for [MarketplaceCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
    type annotations stubs module [types-aiobotocore-marketplace-catalog](https://pypi.org/project/types-aiobotocore-marketplace-catalog/).

## MarketplaceCatalogClient

Type annotations and code completion for `#!python session.client("marketplace-catalog")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

```python title="Usage example"
from aioboto3.session import Session
from types_aiobotocore_marketplace_catalog.client import MarketplaceCatalogClient

session = Session()
async with session.client("marketplace-catalog") as client:
    client: MarketplaceCatalogClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("marketplace-catalog").exceptions` structure.

```python title="Usage example"
async with session.client("marketplace-catalog") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.InternalServiceException,
        client.ResourceInUseException,
        client.ResourceNotFoundException,
        client.ResourceNotSupportedException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_marketplace_catalog.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.client("marketplace-catalog").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_change\_set

Used to cancel an open change request.

Type annotations and code completion for `#!python session.client("marketplace-catalog").cancel_change_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.cancel_change_set)

```python title="Method definition"
await def cancel_change_set(
    self,
    *,
    Catalog: str,
    ChangeSetId: str,
) -> CancelChangeSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelChangeSetResponseTypeDef](./type_defs.md#cancelchangesetresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: CancelChangeSetRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ChangeSetId": ...,
}

parent.cancel_change_set(**kwargs)
```

1. See [:material-code-braces: CancelChangeSetRequestRequestTypeDef](./type_defs.md#cancelchangesetrequestrequesttypedef) 

### describe\_change\_set

Provides information about a given change set.

Type annotations and code completion for `#!python session.client("marketplace-catalog").describe_change_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.describe_change_set)

```python title="Method definition"
await def describe_change_set(
    self,
    *,
    Catalog: str,
    ChangeSetId: str,
) -> DescribeChangeSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeChangeSetResponseTypeDef](./type_defs.md#describechangesetresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeChangeSetRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ChangeSetId": ...,
}

parent.describe_change_set(**kwargs)
```

1. See [:material-code-braces: DescribeChangeSetRequestRequestTypeDef](./type_defs.md#describechangesetrequestrequesttypedef) 

### describe\_entity

Returns the metadata and content of the entity.

Type annotations and code completion for `#!python session.client("marketplace-catalog").describe_entity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.describe_entity)

```python title="Method definition"
await def describe_entity(
    self,
    *,
    Catalog: str,
    EntityId: str,
) -> DescribeEntityResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEntityResponseTypeDef](./type_defs.md#describeentityresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEntityRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "EntityId": ...,
}

parent.describe_entity(**kwargs)
```

1. See [:material-code-braces: DescribeEntityRequestRequestTypeDef](./type_defs.md#describeentityrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.client("marketplace-catalog").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.generate_presigned_url)

```python title="Method definition"
await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### list\_change\_sets

Returns the list of change sets owned by the account being used to make the
call.

Type annotations and code completion for `#!python session.client("marketplace-catalog").list_change_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.list_change_sets)

```python title="Method definition"
await def list_change_sets(
    self,
    *,
    Catalog: str,
    FilterList: Sequence[FilterTypeDef] = ...,  # (1)
    Sort: SortTypeDef = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListChangeSetsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: ListChangeSetsResponseTypeDef](./type_defs.md#listchangesetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListChangeSetsRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
}

parent.list_change_sets(**kwargs)
```

1. See [:material-code-braces: ListChangeSetsRequestRequestTypeDef](./type_defs.md#listchangesetsrequestrequesttypedef) 

### list\_entities

Provides the list of entities of a given type.

Type annotations and code completion for `#!python session.client("marketplace-catalog").list_entities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.list_entities)

```python title="Method definition"
await def list_entities(
    self,
    *,
    Catalog: str,
    EntityType: str,
    FilterList: Sequence[FilterTypeDef] = ...,  # (1)
    Sort: SortTypeDef = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListEntitiesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: ListEntitiesResponseTypeDef](./type_defs.md#listentitiesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListEntitiesRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "EntityType": ...,
}

parent.list_entities(**kwargs)
```

1. See [:material-code-braces: ListEntitiesRequestRequestTypeDef](./type_defs.md#listentitiesrequestrequesttypedef) 

### start\_change\_set

This operation allows you to request changes for your entities.

Type annotations and code completion for `#!python session.client("marketplace-catalog").start_change_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.start_change_set)

```python title="Method definition"
await def start_change_set(
    self,
    *,
    Catalog: str,
    ChangeSet: Sequence[ChangeTypeDef],  # (1)
    ChangeSetName: str = ...,
    ClientRequestToken: str = ...,
) -> StartChangeSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ChangeTypeDef](./type_defs.md#changetypedef) 
2. See [:material-code-braces: StartChangeSetResponseTypeDef](./type_defs.md#startchangesetresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: StartChangeSetRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ChangeSet": ...,
}

parent.start_change_set(**kwargs)
```

1. See [:material-code-braces: StartChangeSetRequestRequestTypeDef](./type_defs.md#startchangesetrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("marketplace-catalog").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> MarketplaceCatalogClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("marketplace-catalog").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





