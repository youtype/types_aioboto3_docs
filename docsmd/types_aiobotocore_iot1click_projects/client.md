# IoT1ClickProjectsClient

> [Index](../README.md) > [IoT1ClickProjects](./README.md) > IoT1ClickProjectsClient

!!! note ""

    Auto-generated documentation for [IoT1ClickProjects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#iot1clickprojects)
    type annotations stubs module [types-aiobotocore-iot1click-projects](https://pypi.org/project/types-aiobotocore-iot1click-projects/).

## IoT1ClickProjectsClient

Type annotations and code completion for `#!python session.client("iot1click-projects")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

```python
# IoT1ClickProjectsClient usage example

from aioboto3.session import Session
from types_aiobotocore_iot1click_projects.client import IoT1ClickProjectsClient

session = Session()
async with session.client("iot1click-projects") as client:
    client: IoT1ClickProjectsClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("iot1click-projects").exceptions` structure.

```python
# IoT1ClickProjectsClient.exceptions usage example

async with session.client("iot1click-projects") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.InternalFailureException,
        client.exceptions.InvalidRequestException,
        client.exceptions.ResourceConflictException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.TooManyRequestsException,
    ) as e:
        print(e)
```

```python
# IoT1ClickProjectsClient.exceptions type checking example

from types_aiobotocore_iot1click_projects.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("iot1click-projects").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("iot1click-projects").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

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


### associate\_device\_with\_placement

Associates a physical device with a placement.

Type annotations and code completion for `#!python session.client("iot1click-projects").associate_device_with_placement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

```python
# associate_device_with_placement method definition

await def associate_device_with_placement(
    self,
    *,
    projectName: str,
    placementName: str,
    deviceId: str,
    deviceTemplateName: str,
) -> dict[str, Any]:
    ...
```



```python
# associate_device_with_placement method usage example with argument unpacking

kwargs: AssociateDeviceWithPlacementRequestRequestTypeDef = {  # (1)
    "projectName": ...,
    "placementName": ...,
    "deviceId": ...,
    "deviceTemplateName": ...,
}

parent.associate_device_with_placement(**kwargs)
```

1. See [:material-code-braces: AssociateDeviceWithPlacementRequestRequestTypeDef](./type_defs.md#associatedevicewithplacementrequestrequesttypedef) 

### create\_placement

Creates an empty placement.

Type annotations and code completion for `#!python session.client("iot1click-projects").create_placement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

```python
# create_placement method definition

await def create_placement(
    self,
    *,
    placementName: str,
    projectName: str,
    attributes: Mapping[str, str] = ...,
) -> dict[str, Any]:
    ...
```



```python
# create_placement method usage example with argument unpacking

kwargs: CreatePlacementRequestRequestTypeDef = {  # (1)
    "placementName": ...,
    "projectName": ...,
}

parent.create_placement(**kwargs)
```

1. See [:material-code-braces: CreatePlacementRequestRequestTypeDef](./type_defs.md#createplacementrequestrequesttypedef) 

### create\_project

Creates an empty project with a placement template.

Type annotations and code completion for `#!python session.client("iot1click-projects").create_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

```python
# create_project method definition

await def create_project(
    self,
    *,
    projectName: str,
    description: str = ...,
    placementTemplate: PlacementTemplateTypeDef = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: PlacementTemplateTypeDef](./type_defs.md#placementtemplatetypedef) 


```python
# create_project method usage example with argument unpacking

kwargs: CreateProjectRequestRequestTypeDef = {  # (1)
    "projectName": ...,
}

parent.create_project(**kwargs)
```

1. See [:material-code-braces: CreateProjectRequestRequestTypeDef](./type_defs.md#createprojectrequestrequesttypedef) 

### delete\_placement

Deletes a placement.

Type annotations and code completion for `#!python session.client("iot1click-projects").delete_placement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

```python
# delete_placement method definition

await def delete_placement(
    self,
    *,
    placementName: str,
    projectName: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_placement method usage example with argument unpacking

kwargs: DeletePlacementRequestRequestTypeDef = {  # (1)
    "placementName": ...,
    "projectName": ...,
}

parent.delete_placement(**kwargs)
```

1. See [:material-code-braces: DeletePlacementRequestRequestTypeDef](./type_defs.md#deleteplacementrequestrequesttypedef) 

### delete\_project

Deletes a project.

Type annotations and code completion for `#!python session.client("iot1click-projects").delete_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

```python
# delete_project method definition

await def delete_project(
    self,
    *,
    projectName: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_project method usage example with argument unpacking

kwargs: DeleteProjectRequestRequestTypeDef = {  # (1)
    "projectName": ...,
}

parent.delete_project(**kwargs)
```

1. See [:material-code-braces: DeleteProjectRequestRequestTypeDef](./type_defs.md#deleteprojectrequestrequesttypedef) 

### describe\_placement

Describes a placement in a project.

Type annotations and code completion for `#!python session.client("iot1click-projects").describe_placement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

```python
# describe_placement method definition

await def describe_placement(
    self,
    *,
    placementName: str,
    projectName: str,
) -> DescribePlacementResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePlacementResponseTypeDef](./type_defs.md#describeplacementresponsetypedef) 


```python
# describe_placement method usage example with argument unpacking

kwargs: DescribePlacementRequestRequestTypeDef = {  # (1)
    "placementName": ...,
    "projectName": ...,
}

parent.describe_placement(**kwargs)
```

1. See [:material-code-braces: DescribePlacementRequestRequestTypeDef](./type_defs.md#describeplacementrequestrequesttypedef) 

### describe\_project

Returns an object describing a project.

Type annotations and code completion for `#!python session.client("iot1click-projects").describe_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

```python
# describe_project method definition

await def describe_project(
    self,
    *,
    projectName: str,
) -> DescribeProjectResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeProjectResponseTypeDef](./type_defs.md#describeprojectresponsetypedef) 


```python
# describe_project method usage example with argument unpacking

kwargs: DescribeProjectRequestRequestTypeDef = {  # (1)
    "projectName": ...,
}

parent.describe_project(**kwargs)
```

1. See [:material-code-braces: DescribeProjectRequestRequestTypeDef](./type_defs.md#describeprojectrequestrequesttypedef) 

### disassociate\_device\_from\_placement

Removes a physical device from a placement.

Type annotations and code completion for `#!python session.client("iot1click-projects").disassociate_device_from_placement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

```python
# disassociate_device_from_placement method definition

await def disassociate_device_from_placement(
    self,
    *,
    projectName: str,
    placementName: str,
    deviceTemplateName: str,
) -> dict[str, Any]:
    ...
```



```python
# disassociate_device_from_placement method usage example with argument unpacking

kwargs: DisassociateDeviceFromPlacementRequestRequestTypeDef = {  # (1)
    "projectName": ...,
    "placementName": ...,
    "deviceTemplateName": ...,
}

parent.disassociate_device_from_placement(**kwargs)
```

1. See [:material-code-braces: DisassociateDeviceFromPlacementRequestRequestTypeDef](./type_defs.md#disassociatedevicefromplacementrequestrequesttypedef) 

### get\_devices\_in\_placement

Returns an object enumerating the devices in a placement.

Type annotations and code completion for `#!python session.client("iot1click-projects").get_devices_in_placement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

```python
# get_devices_in_placement method definition

await def get_devices_in_placement(
    self,
    *,
    projectName: str,
    placementName: str,
) -> GetDevicesInPlacementResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDevicesInPlacementResponseTypeDef](./type_defs.md#getdevicesinplacementresponsetypedef) 


```python
# get_devices_in_placement method usage example with argument unpacking

kwargs: GetDevicesInPlacementRequestRequestTypeDef = {  # (1)
    "projectName": ...,
    "placementName": ...,
}

parent.get_devices_in_placement(**kwargs)
```

1. See [:material-code-braces: GetDevicesInPlacementRequestRequestTypeDef](./type_defs.md#getdevicesinplacementrequestrequesttypedef) 

### list\_placements

Lists the placement(s) of a project.

Type annotations and code completion for `#!python session.client("iot1click-projects").list_placements` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

```python
# list_placements method definition

await def list_placements(
    self,
    *,
    projectName: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListPlacementsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPlacementsResponseTypeDef](./type_defs.md#listplacementsresponsetypedef) 


```python
# list_placements method usage example with argument unpacking

kwargs: ListPlacementsRequestRequestTypeDef = {  # (1)
    "projectName": ...,
}

parent.list_placements(**kwargs)
```

1. See [:material-code-braces: ListPlacementsRequestRequestTypeDef](./type_defs.md#listplacementsrequestrequesttypedef) 

### list\_projects

Lists the AWS IoT 1-Click project(s) associated with your AWS account and
region.

Type annotations and code completion for `#!python session.client("iot1click-projects").list_projects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

```python
# list_projects method definition

await def list_projects(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListProjectsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef) 


```python
# list_projects method usage example with argument unpacking

kwargs: ListProjectsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_projects(**kwargs)
```

1. See [:material-code-braces: ListProjectsRequestRequestTypeDef](./type_defs.md#listprojectsrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags (metadata key/value pairs) which you have assigned to the
resource.

Type annotations and code completion for `#!python session.client("iot1click-projects").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

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

Creates or modifies tags for a resource.

Type annotations and code completion for `#!python session.client("iot1click-projects").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

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

Removes one or more tags (metadata key/value pairs) from a resource.

Type annotations and code completion for `#!python session.client("iot1click-projects").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

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

### update\_placement

Updates a placement with the given attributes.

Type annotations and code completion for `#!python session.client("iot1click-projects").update_placement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

```python
# update_placement method definition

await def update_placement(
    self,
    *,
    placementName: str,
    projectName: str,
    attributes: Mapping[str, str] = ...,
) -> dict[str, Any]:
    ...
```



```python
# update_placement method usage example with argument unpacking

kwargs: UpdatePlacementRequestRequestTypeDef = {  # (1)
    "placementName": ...,
    "projectName": ...,
}

parent.update_placement(**kwargs)
```

1. See [:material-code-braces: UpdatePlacementRequestRequestTypeDef](./type_defs.md#updateplacementrequestrequesttypedef) 

### update\_project

Updates a project associated with your AWS account and region.

Type annotations and code completion for `#!python session.client("iot1click-projects").update_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

```python
# update_project method definition

await def update_project(
    self,
    *,
    projectName: str,
    description: str = ...,
    placementTemplate: PlacementTemplateTypeDef = ...,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: PlacementTemplateTypeDef](./type_defs.md#placementtemplatetypedef) 


```python
# update_project method usage example with argument unpacking

kwargs: UpdateProjectRequestRequestTypeDef = {  # (1)
    "projectName": ...,
}

parent.update_project(**kwargs)
```

1. See [:material-code-braces: UpdateProjectRequestRequestTypeDef](./type_defs.md#updateprojectrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("iot1click-projects").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("iot1click-projects").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

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

Type annotations and code completion for `#!python session.client("iot1click-projects").get_paginator` method with overloads.

- `client.get_paginator("list_placements")` -> [ListPlacementsPaginator](./paginators.md#listplacementspaginator)
- `client.get_paginator("list_projects")` -> [ListProjectsPaginator](./paginators.md#listprojectspaginator)


