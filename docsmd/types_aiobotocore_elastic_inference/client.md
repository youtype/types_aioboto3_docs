# ElasticInferenceClient

> [Index](../README.md) > [ElasticInference](./README.md) > ElasticInferenceClient

!!! note ""

    Auto-generated documentation for [ElasticInference](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#elasticinference)
    type annotations stubs module [types-aiobotocore-elastic-inference](https://pypi.org/project/types-aiobotocore-elastic-inference/).

## ElasticInferenceClient

Type annotations and code completion for `#!python session.client("elastic-inference")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client)

```python
# ElasticInferenceClient usage example

from aioboto3.session import Session
from types_aiobotocore_elastic_inference.client import ElasticInferenceClient

session = Session()
async with session.client("elastic-inference") as client:
    client: ElasticInferenceClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("elastic-inference").exceptions` structure.

```python
# ElasticInferenceClient.exceptions usage example

async with session.client("elastic-inference") as client:
    try:
        do_something(client)
    except (
            client.exceptions.BadRequestException,
        client.exceptions.ClientError,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python
# ElasticInferenceClient.exceptions type checking example

from types_aiobotocore_elastic_inference.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("elastic-inference").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("elastic-inference").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client)

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


### describe\_accelerator\_offerings

Amazon Elastic Inference is no longer available.

Type annotations and code completion for `#!python session.client("elastic-inference").describe_accelerator_offerings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client)

```python
# describe_accelerator_offerings method definition

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


```python
# describe_accelerator_offerings method usage example with argument unpacking

kwargs: DescribeAcceleratorOfferingsRequestRequestTypeDef = {  # (1)
    "locationType": ...,
}

parent.describe_accelerator_offerings(**kwargs)
```

1. See [:material-code-braces: DescribeAcceleratorOfferingsRequestRequestTypeDef](./type_defs.md#describeacceleratorofferingsrequestrequesttypedef) 

### describe\_accelerator\_types

Amazon Elastic Inference is no longer available.

Type annotations and code completion for `#!python session.client("elastic-inference").describe_accelerator_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client)

```python
# describe_accelerator_types method definition

await def describe_accelerator_types(
    self,
) -> DescribeAcceleratorTypesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAcceleratorTypesResponseTypeDef](./type_defs.md#describeacceleratortypesresponsetypedef) 

### describe\_accelerators

Amazon Elastic Inference is no longer available.

Type annotations and code completion for `#!python session.client("elastic-inference").describe_accelerators` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client)

```python
# describe_accelerators method definition

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


```python
# describe_accelerators method usage example with argument unpacking

kwargs: DescribeAcceleratorsRequestRequestTypeDef = {  # (1)
    "acceleratorIds": ...,
}

parent.describe_accelerators(**kwargs)
```

1. See [:material-code-braces: DescribeAcceleratorsRequestRequestTypeDef](./type_defs.md#describeacceleratorsrequestrequesttypedef) 

### list\_tags\_for\_resource

Amazon Elastic Inference is no longer available.

Type annotations and code completion for `#!python session.client("elastic-inference").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### tag\_resource

Amazon Elastic Inference is no longer available.

Type annotations and code completion for `#!python session.client("elastic-inference").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Amazon Elastic Inference is no longer available.

Type annotations and code completion for `#!python session.client("elastic-inference").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client)

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



Type annotations and code completion for `#!python session.client("elastic-inference").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("elastic-inference").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client)

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

Type annotations and code completion for `#!python session.client("elastic-inference").get_paginator` method with overloads.

- `client.get_paginator("describe_accelerators")` -> [DescribeAcceleratorsPaginator](./paginators.md#describeacceleratorspaginator)


