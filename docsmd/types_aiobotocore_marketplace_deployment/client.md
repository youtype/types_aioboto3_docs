# MarketplaceDeploymentServiceClient

> [Index](../README.md) > [MarketplaceDeploymentService](./README.md) > MarketplaceDeploymentServiceClient

!!! note ""

    Auto-generated documentation for [MarketplaceDeploymentService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-deployment.html#marketplacedeploymentservice)
    type annotations stubs module [types-aiobotocore-marketplace-deployment](https://pypi.org/project/types-aiobotocore-marketplace-deployment/).

## MarketplaceDeploymentServiceClient

Type annotations and code completion for `#!python session.client("marketplace-deployment")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-deployment.html#MarketplaceDeploymentService.Client)

```python
# MarketplaceDeploymentServiceClient usage example

from aioboto3.session import Session
from types_aiobotocore_marketplace_deployment.client import MarketplaceDeploymentServiceClient

session = Session()
async with session.client("marketplace-deployment") as client:
    client: MarketplaceDeploymentServiceClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("marketplace-deployment").exceptions` structure.

```python
# MarketplaceDeploymentServiceClient.exceptions usage example

async with session.client("marketplace-deployment") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# MarketplaceDeploymentServiceClient.exceptions type checking example

from types_aiobotocore_marketplace_deployment.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("marketplace-deployment").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-deployment.html#MarketplaceDeploymentService.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("marketplace-deployment").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-deployment.html#MarketplaceDeploymentService.Client)

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


### list\_tags\_for\_resource

Lists all tags that have been added to a deployment parameter resource.

Type annotations and code completion for `#!python session.client("marketplace-deployment").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-deployment.html#MarketplaceDeploymentService.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### put\_deployment\_parameter

Creates or updates a deployment parameter and is targeted by
<code>catalog</code> and <code>agreementId</code>.

Type annotations and code completion for `#!python session.client("marketplace-deployment").put_deployment_parameter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-deployment.html#MarketplaceDeploymentService.Client)

```python
# put_deployment_parameter method definition

await def put_deployment_parameter(
    self,
    *,
    agreementId: str,
    catalog: str,
    deploymentParameter: DeploymentParameterInputTypeDef,  # (1)
    productId: str,
    clientToken: str = ...,
    expirationDate: TimestampTypeDef = ...,
    tags: Mapping[str, str] = ...,
) -> PutDeploymentParameterResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DeploymentParameterInputTypeDef](./type_defs.md#deploymentparameterinputtypedef) 
2. See [:material-code-braces: PutDeploymentParameterResponseTypeDef](./type_defs.md#putdeploymentparameterresponsetypedef) 


```python
# put_deployment_parameter method usage example with argument unpacking

kwargs: PutDeploymentParameterRequestRequestTypeDef = {  # (1)
    "agreementId": ...,
    "catalog": ...,
    "deploymentParameter": ...,
    "productId": ...,
}

parent.put_deployment_parameter(**kwargs)
```

1. See [:material-code-braces: PutDeploymentParameterRequestRequestTypeDef](./type_defs.md#putdeploymentparameterrequestrequesttypedef) 

### tag\_resource

Tags a resource.

Type annotations and code completion for `#!python session.client("marketplace-deployment").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-deployment.html#MarketplaceDeploymentService.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str] = ...,
) -> dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes a tag or list of tags from a resource.

Type annotations and code completion for `#!python session.client("marketplace-deployment").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-deployment.html#MarketplaceDeploymentService.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("marketplace-deployment").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-deployment.html#MarketplaceDeploymentService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("marketplace-deployment").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-deployment.html#MarketplaceDeploymentService.Client)

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




