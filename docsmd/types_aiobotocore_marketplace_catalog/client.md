# MarketplaceCatalogClient

> [Index](../README.md) > [MarketplaceCatalog](./README.md) > MarketplaceCatalogClient

!!! note ""

    Auto-generated documentation for [MarketplaceCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#marketplacecatalog)
    type annotations stubs module [types-aiobotocore-marketplace-catalog](https://pypi.org/project/types-aiobotocore-marketplace-catalog/).

## MarketplaceCatalogClient

Type annotations and code completion for `#!python session.client("marketplace-catalog")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

```python
# MarketplaceCatalogClient usage example

from aioboto3.session import Session
from types_aiobotocore_marketplace_catalog.client import MarketplaceCatalogClient

session = Session()
async with session.client("marketplace-catalog") as client:
    client: MarketplaceCatalogClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("marketplace-catalog").exceptions` structure.

```python
# MarketplaceCatalogClient.exceptions usage example

async with session.client("marketplace-catalog") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.InternalServiceException,
        client.exceptions.ResourceInUseException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ResourceNotSupportedException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# MarketplaceCatalogClient.exceptions type checking example

from types_aiobotocore_marketplace_catalog.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("marketplace-catalog").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("marketplace-catalog").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

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


### batch\_describe\_entities

Returns metadata and content for multiple entities.

Type annotations and code completion for `#!python session.client("marketplace-catalog").batch_describe_entities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

```python
# batch_describe_entities method definition

await def batch_describe_entities(
    self,
    *,
    EntityRequestList: Sequence[EntityRequestTypeDef],  # (1)
) -> BatchDescribeEntitiesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EntityRequestTypeDef](./type_defs.md#entityrequesttypedef) 
2. See [:material-code-braces: BatchDescribeEntitiesResponseTypeDef](./type_defs.md#batchdescribeentitiesresponsetypedef) 


```python
# batch_describe_entities method usage example with argument unpacking

kwargs: BatchDescribeEntitiesRequestRequestTypeDef = {  # (1)
    "EntityRequestList": ...,
}

parent.batch_describe_entities(**kwargs)
```

1. See [:material-code-braces: BatchDescribeEntitiesRequestRequestTypeDef](./type_defs.md#batchdescribeentitiesrequestrequesttypedef) 

### cancel\_change\_set

Used to cancel an open change request.

Type annotations and code completion for `#!python session.client("marketplace-catalog").cancel_change_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

```python
# cancel_change_set method definition

await def cancel_change_set(
    self,
    *,
    Catalog: str,
    ChangeSetId: str,
) -> CancelChangeSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelChangeSetResponseTypeDef](./type_defs.md#cancelchangesetresponsetypedef) 


```python
# cancel_change_set method usage example with argument unpacking

kwargs: CancelChangeSetRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ChangeSetId": ...,
}

parent.cancel_change_set(**kwargs)
```

1. See [:material-code-braces: CancelChangeSetRequestRequestTypeDef](./type_defs.md#cancelchangesetrequestrequesttypedef) 

### delete\_resource\_policy

Deletes a resource-based policy on an entity that is identified by its resource
ARN.

Type annotations and code completion for `#!python session.client("marketplace-catalog").delete_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

```python
# delete_resource_policy method definition

await def delete_resource_policy(
    self,
    *,
    ResourceArn: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_resource_policy method usage example with argument unpacking

kwargs: DeleteResourcePolicyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.delete_resource_policy(**kwargs)
```

1. See [:material-code-braces: DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef) 

### describe\_change\_set

Provides information about a given change set.

Type annotations and code completion for `#!python session.client("marketplace-catalog").describe_change_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

```python
# describe_change_set method definition

await def describe_change_set(
    self,
    *,
    Catalog: str,
    ChangeSetId: str,
) -> DescribeChangeSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeChangeSetResponseTypeDef](./type_defs.md#describechangesetresponsetypedef) 


```python
# describe_change_set method usage example with argument unpacking

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

```python
# describe_entity method definition

await def describe_entity(
    self,
    *,
    Catalog: str,
    EntityId: str,
) -> DescribeEntityResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEntityResponseTypeDef](./type_defs.md#describeentityresponsetypedef) 


```python
# describe_entity method usage example with argument unpacking

kwargs: DescribeEntityRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "EntityId": ...,
}

parent.describe_entity(**kwargs)
```

1. See [:material-code-braces: DescribeEntityRequestRequestTypeDef](./type_defs.md#describeentityrequestrequesttypedef) 

### get\_resource\_policy

Gets a resource-based policy of an entity that is identified by its resource
ARN.

Type annotations and code completion for `#!python session.client("marketplace-catalog").get_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

```python
# get_resource_policy method definition

await def get_resource_policy(
    self,
    *,
    ResourceArn: str,
) -> GetResourcePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResourcePolicyResponseTypeDef](./type_defs.md#getresourcepolicyresponsetypedef) 


```python
# get_resource_policy method usage example with argument unpacking

kwargs: GetResourcePolicyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_resource_policy(**kwargs)
```

1. See [:material-code-braces: GetResourcePolicyRequestRequestTypeDef](./type_defs.md#getresourcepolicyrequestrequesttypedef) 

### list\_change\_sets

Returns the list of change sets owned by the account being used to make the
call.

Type annotations and code completion for `#!python session.client("marketplace-catalog").list_change_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

```python
# list_change_sets method definition

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


```python
# list_change_sets method usage example with argument unpacking

kwargs: ListChangeSetsRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
}

parent.list_change_sets(**kwargs)
```

1. See [:material-code-braces: ListChangeSetsRequestRequestTypeDef](./type_defs.md#listchangesetsrequestrequesttypedef) 

### list\_entities

Provides the list of entities of a given type.

Type annotations and code completion for `#!python session.client("marketplace-catalog").list_entities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

```python
# list_entities method definition

await def list_entities(
    self,
    *,
    Catalog: str,
    EntityType: str,
    FilterList: Sequence[FilterTypeDef] = ...,  # (1)
    Sort: SortTypeDef = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
    OwnershipType: OwnershipTypeType = ...,  # (3)
    EntityTypeFilters: EntityTypeFiltersTypeDef = ...,  # (4)
    EntityTypeSort: EntityTypeSortTypeDef = ...,  # (5)
) -> ListEntitiesResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-brackets: OwnershipTypeType](./literals.md#ownershiptypetype) 
4. See [:material-code-braces: EntityTypeFiltersTypeDef](./type_defs.md#entitytypefilterstypedef) 
5. See [:material-code-braces: EntityTypeSortTypeDef](./type_defs.md#entitytypesorttypedef) 
6. See [:material-code-braces: ListEntitiesResponseTypeDef](./type_defs.md#listentitiesresponsetypedef) 


```python
# list_entities method usage example with argument unpacking

kwargs: ListEntitiesRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "EntityType": ...,
}

parent.list_entities(**kwargs)
```

1. See [:material-code-braces: ListEntitiesRequestRequestTypeDef](./type_defs.md#listentitiesrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists all tags that have been added to a resource (either an <a
href="https://docs.aws.amazon.com/marketplace-catalog/latest/api-reference/welcome.html#catalog-api-entities">entity</a>
or <a
href="https://docs.aws.amazon.com/marketplace-catalog/latest/api-reference/welcome.html#working-with-chang...

Type annotations and code completion for `#!python session.client("marketplace-catalog").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### put\_resource\_policy

Attaches a resource-based policy to an entity.

Type annotations and code completion for `#!python session.client("marketplace-catalog").put_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

```python
# put_resource_policy method definition

await def put_resource_policy(
    self,
    *,
    ResourceArn: str,
    Policy: str,
) -> dict[str, Any]:
    ...
```



```python
# put_resource_policy method usage example with argument unpacking

kwargs: PutResourcePolicyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Policy": ...,
}

parent.put_resource_policy(**kwargs)
```

1. See [:material-code-braces: PutResourcePolicyRequestRequestTypeDef](./type_defs.md#putresourcepolicyrequestrequesttypedef) 

### start\_change\_set

Allows you to request changes for your entities.

Type annotations and code completion for `#!python session.client("marketplace-catalog").start_change_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

```python
# start_change_set method definition

await def start_change_set(
    self,
    *,
    Catalog: str,
    ChangeSet: Sequence[ChangeTypeDef],  # (1)
    ChangeSetName: str = ...,
    ClientRequestToken: str = ...,
    ChangeSetTags: Sequence[TagTypeDef] = ...,  # (2)
    Intent: IntentType = ...,  # (3)
) -> StartChangeSetResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ChangeTypeDef](./type_defs.md#changetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: IntentType](./literals.md#intenttype) 
4. See [:material-code-braces: StartChangeSetResponseTypeDef](./type_defs.md#startchangesetresponsetypedef) 


```python
# start_change_set method usage example with argument unpacking

kwargs: StartChangeSetRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ChangeSet": ...,
}

parent.start_change_set(**kwargs)
```

1. See [:material-code-braces: StartChangeSetRequestRequestTypeDef](./type_defs.md#startchangesetrequestrequesttypedef) 

### tag\_resource

Tags a resource (either an <a
href="https://docs.aws.amazon.com/marketplace-catalog/latest/api-reference/welcome.html#catalog-api-entities">entity</a>
or <a
href="https://docs.aws.amazon.com/marketplace-catalog/latest/api-reference/welcome.html#working-with-change-sets">change
set</a>).

Type annotations and code completion for `#!python session.client("marketplace-catalog").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes a tag or list of tags from a resource (either an <a
href="https://docs.aws.amazon.com/marketplace-catalog/latest/api-reference/welcome.html#catalog-api-entities">entity</a>
or <a
href="https://docs.aws.amazon.com/marketplace-catalog/latest/api-reference/welcome.html#working-with-change-se...

Type annotations and code completion for `#!python session.client("marketplace-catalog").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("marketplace-catalog").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("marketplace-catalog").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

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

Type annotations and code completion for `#!python session.client("marketplace-catalog").get_paginator` method with overloads.

- `client.get_paginator("list_change_sets")` -> [ListChangeSetsPaginator](./paginators.md#listchangesetspaginator)
- `client.get_paginator("list_entities")` -> [ListEntitiesPaginator](./paginators.md#listentitiespaginator)


