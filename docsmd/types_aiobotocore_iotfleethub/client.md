# IoTFleetHubClient

> [Index](../README.md) > [IoTFleetHub](./README.md) > IoTFleetHubClient

!!! note ""

    Auto-generated documentation for [IoTFleetHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#iotfleethub)
    type annotations stubs module [types-aiobotocore-iotfleethub](https://pypi.org/project/types-aiobotocore-iotfleethub/).

## IoTFleetHubClient

Type annotations and code completion for `#!python session.client("iotfleethub")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client)

```python
# IoTFleetHubClient usage example

from aioboto3.session import Session
from types_aiobotocore_iotfleethub.client import IoTFleetHubClient

session = Session()
async with session.client("iotfleethub") as client:
    client: IoTFleetHubClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("iotfleethub").exceptions` structure.

```python
# IoTFleetHubClient.exceptions usage example

async with session.client("iotfleethub") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalFailureException,
        client.exceptions.InvalidRequestException,
        client.exceptions.LimitExceededException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ThrottlingException,
    ) as e:
        print(e)
```

```python
# IoTFleetHubClient.exceptions type checking example

from types_aiobotocore_iotfleethub.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("iotfleethub").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("iotfleethub").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client)

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


### create\_application

Creates a Fleet Hub for IoT Device Management web application.

Type annotations and code completion for `#!python session.client("iotfleethub").create_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client)

```python
# create_application method definition

await def create_application(
    self,
    *,
    applicationName: str,
    roleArn: str,
    applicationDescription: str = ...,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef) 


```python
# create_application method usage example with argument unpacking

kwargs: CreateApplicationRequestRequestTypeDef = {  # (1)
    "applicationName": ...,
    "roleArn": ...,
}

parent.create_application(**kwargs)
```

1. See [:material-code-braces: CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef) 

### delete\_application

Deletes a Fleet Hub for IoT Device Management web application.

Type annotations and code completion for `#!python session.client("iotfleethub").delete_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client)

```python
# delete_application method definition

await def delete_application(
    self,
    *,
    applicationId: str,
    clientToken: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_application method usage example with argument unpacking

kwargs: DeleteApplicationRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.delete_application(**kwargs)
```

1. See [:material-code-braces: DeleteApplicationRequestRequestTypeDef](./type_defs.md#deleteapplicationrequestrequesttypedef) 

### describe\_application

Gets information about a Fleet Hub for IoT Device Management web application.

Type annotations and code completion for `#!python session.client("iotfleethub").describe_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client)

```python
# describe_application method definition

await def describe_application(
    self,
    *,
    applicationId: str,
) -> DescribeApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeApplicationResponseTypeDef](./type_defs.md#describeapplicationresponsetypedef) 


```python
# describe_application method usage example with argument unpacking

kwargs: DescribeApplicationRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.describe_application(**kwargs)
```

1. See [:material-code-braces: DescribeApplicationRequestRequestTypeDef](./type_defs.md#describeapplicationrequestrequesttypedef) 

### list\_applications

Gets a list of Fleet Hub for IoT Device Management web applications for the
current account.

Type annotations and code completion for `#!python session.client("iotfleethub").list_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client)

```python
# list_applications method definition

await def list_applications(
    self,
    *,
    nextToken: str = ...,
) -> ListApplicationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


```python
# list_applications method usage example with argument unpacking

kwargs: ListApplicationsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_applications(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestRequestTypeDef](./type_defs.md#listapplicationsrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags for the specified resource.

Type annotations and code completion for `#!python session.client("iotfleethub").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client)

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

### tag\_resource

Adds to or modifies the tags of the specified resource.

Type annotations and code completion for `#!python session.client("iotfleethub").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client)

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

Removes the specified tags (metadata) from the resource.

Type annotations and code completion for `#!python session.client("iotfleethub").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client)

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

### update\_application

Updates information about a Fleet Hub for IoT Device Management web application.

Type annotations and code completion for `#!python session.client("iotfleethub").update_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client)

```python
# update_application method definition

await def update_application(
    self,
    *,
    applicationId: str,
    applicationName: str = ...,
    applicationDescription: str = ...,
    clientToken: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# update_application method usage example with argument unpacking

kwargs: UpdateApplicationRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.update_application(**kwargs)
```

1. See [:material-code-braces: UpdateApplicationRequestRequestTypeDef](./type_defs.md#updateapplicationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("iotfleethub").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("iotfleethub").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client)

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

Type annotations and code completion for `#!python session.client("iotfleethub").get_paginator` method with overloads.

- `client.get_paginator("list_applications")` -> [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)


