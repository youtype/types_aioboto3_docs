# ElasticInferenceClient

> [Index](../README.md) > [ElasticInference](./README.md) > ElasticInferenceClient

!!! note ""

    Auto-generated documentation for [ElasticInference](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
    type annotations stubs module [types-aiobotocore-elastic-inference](https://pypi.org/project/types-aiobotocore-elastic-inference/).

## ElasticInferenceClient

Type annotations and code completion for `#!python session.client("elastic-inference")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client)

```python title="Usage example"
from aioboto3.session import Session
from types_aiobotocore_elastic_inference.client import ElasticInferenceClient

session = Session()
async with session.client("elastic-inference") as client:
    client: ElasticInferenceClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("elastic-inference").exceptions` structure.

```python title="Usage example"
async with session.client("elastic-inference") as client:
    try:
        do_something(client)
    except (
            client.BadRequestException,
        client.ClientError,
        client.InternalServerException,
        client.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_elastic_inference.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.client("elastic-inference").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### describe\_accelerator\_offerings

Describes the locations in which a given accelerator type or set of types is
present in a given region.

Type annotations and code completion for `#!python session.client("elastic-inference").describe_accelerator_offerings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.describe_accelerator_offerings)

```python title="Method definition"
await def describe_accelerator_offerings(
    self,
    *,
    locationType: LocationTypeType,  # (1)
    acceleratorTypes: Sequence[str] = ...,
) -> DescribeAcceleratorOfferingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LocationTypeType](./literals.md#locationtypetype) 
2. See [:material-code-braces: DescribeAcceleratorOfferingsResponseTypeDef](./type_defs.md#describeacceleratorofferingsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeAcceleratorOfferingsRequestRequestTypeDef = {  # (1)
    "locationType": ...,
}

parent.describe_accelerator_offerings(**kwargs)
```

1. See [:material-code-braces: DescribeAcceleratorOfferingsRequestRequestTypeDef](./type_defs.md#describeacceleratorofferingsrequestrequesttypedef) 

### describe\_accelerator\_types

Describes the accelerator types available in a given region, as well as their
characteristics, such as memory and throughput.

Type annotations and code completion for `#!python session.client("elastic-inference").describe_accelerator_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.describe_accelerator_types)

```python title="Method definition"
await def describe_accelerator_types(
    self,
) -> DescribeAcceleratorTypesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAcceleratorTypesResponseTypeDef](./type_defs.md#describeacceleratortypesresponsetypedef) 

### describe\_accelerators

Describes information over a provided set of accelerators belonging to an
account.

Type annotations and code completion for `#!python session.client("elastic-inference").describe_accelerators` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.describe_accelerators)

```python title="Method definition"
await def describe_accelerators(
    self,
    *,
    acceleratorIds: Sequence[str] = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeAcceleratorsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeAcceleratorsResponseTypeDef](./type_defs.md#describeacceleratorsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeAcceleratorsRequestRequestTypeDef = {  # (1)
    "acceleratorIds": ...,
}

parent.describe_accelerators(**kwargs)
```

1. See [:material-code-braces: DescribeAcceleratorsRequestRequestTypeDef](./type_defs.md#describeacceleratorsrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.client("elastic-inference").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.generate_presigned_url)

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


### list\_tags\_for\_resource

Returns all tags of an Elastic Inference Accelerator.

Type annotations and code completion for `#!python session.client("elastic-inference").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.list_tags_for_resource)

```python title="Method definition"
await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### tag\_resource

Adds the specified tags to an Elastic Inference Accelerator.

Type annotations and code completion for `#!python session.client("elastic-inference").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.tag_resource)

```python title="Method definition"
await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python title="Usage example with kwargs"
kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes the specified tags from an Elastic Inference Accelerator.

Type annotations and code completion for `#!python session.client("elastic-inference").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.untag_resource)

```python title="Method definition"
await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python title="Usage example with kwargs"
kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("elastic-inference").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> ElasticInferenceClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("elastic-inference").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("elastic-inference").get_paginator` method with overloads.

- `client.get_paginator("describe_accelerators")` -> [DescribeAcceleratorsPaginator](./paginators.md#describeacceleratorspaginator)



