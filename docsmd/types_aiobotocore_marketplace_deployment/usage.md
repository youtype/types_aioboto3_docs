# Examples

> [Index](../README.md) > [MarketplaceDeploymentService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MarketplaceDeploymentService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-deployment.html#marketplacedeploymentservice)
    type annotations stubs module [types-aiobotocore-marketplace-deployment](https://pypi.org/project/types-aiobotocore-marketplace-deployment/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[marketplace-deployment]` package installed.

Write your `MarketplaceDeploymentService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# MarketplaceDeploymentServiceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("marketplace-deployment") as client:  # (1)
    result = await client.list_tags_for_resource()  # (2)
```

1. client: [MarketplaceDeploymentServiceClient](./client.md)
2. result: [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[marketplace-deployment]`
or a standalone `types_aiobotocore_marketplace_deployment` package, you have to explicitly specify
`client: MarketplaceDeploymentServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# MarketplaceDeploymentServiceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_marketplace_deployment.client import MarketplaceDeploymentServiceClient
from types_aiobotocore_marketplace_deployment.type_defs import ListTagsForResourceResponseTypeDef
from types_aiobotocore_marketplace_deployment.type_defs import ListTagsForResourceRequestTypeDef


session = Session()

client: MarketplaceDeploymentServiceClient
async with session.client("marketplace-deployment") as client:  # (1)
    kwargs: ListTagsForResourceRequestTypeDef = {...}  # (2)
    result: ListTagsForResourceResponseTypeDef = await client.list_tags_for_resource(**kwargs)  # (3)
```

1. client: [MarketplaceDeploymentServiceClient](./client.md)
2. kwargs: [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
3. result: [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)






