# EventBridgePipesClient

> [Index](../README.md) > [EventBridgePipes](./README.md) > EventBridgePipesClient

!!! note ""

    Auto-generated documentation for [EventBridgePipes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#eventbridgepipes)
    type annotations stubs module [types-aiobotocore-pipes](https://pypi.org/project/types-aiobotocore-pipes/).

## EventBridgePipesClient

Type annotations and code completion for `#!python session.client("pipes")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client)

```python
# EventBridgePipesClient usage example

from aioboto3.session import Session
from types_aiobotocore_pipes.client import EventBridgePipesClient

session = Session()
async with session.client("pipes") as client:
    client: EventBridgePipesClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("pipes").exceptions` structure.

```python
# EventBridgePipesClient.exceptions usage example

async with session.client("pipes") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalException,
        client.exceptions.NotFoundException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# EventBridgePipesClient.exceptions type checking example

from types_aiobotocore_pipes.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("pipes").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("pipes").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client)

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


### create\_pipe

Create a pipe.

Type annotations and code completion for `#!python session.client("pipes").create_pipe` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client)

```python
# create_pipe method definition

await def create_pipe(
    self,
    *,
    Name: str,
    Source: str,
    Target: str,
    RoleArn: str,
    Description: str = ...,
    DesiredState: RequestedPipeStateType = ...,  # (1)
    SourceParameters: PipeSourceParametersTypeDef = ...,  # (2)
    Enrichment: str = ...,
    EnrichmentParameters: PipeEnrichmentParametersTypeDef = ...,  # (3)
    TargetParameters: PipeTargetParametersTypeDef = ...,  # (4)
    Tags: Mapping[str, str] = ...,
    LogConfiguration: PipeLogConfigurationParametersTypeDef = ...,  # (5)
    KmsKeyIdentifier: str = ...,
) -> CreatePipeResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: RequestedPipeStateType](./literals.md#requestedpipestatetype) 
2. See [:material-code-braces: PipeSourceParametersTypeDef](./type_defs.md#pipesourceparameterstypedef) 
3. See [:material-code-braces: PipeEnrichmentParametersTypeDef](./type_defs.md#pipeenrichmentparameterstypedef) 
4. See [:material-code-braces: PipeTargetParametersTypeDef](./type_defs.md#pipetargetparameterstypedef) 
5. See [:material-code-braces: PipeLogConfigurationParametersTypeDef](./type_defs.md#pipelogconfigurationparameterstypedef) 
6. See [:material-code-braces: CreatePipeResponseTypeDef](./type_defs.md#createpiperesponsetypedef) 


```python
# create_pipe method usage example with argument unpacking

kwargs: CreatePipeRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Source": ...,
    "Target": ...,
    "RoleArn": ...,
}

parent.create_pipe(**kwargs)
```

1. See [:material-code-braces: CreatePipeRequestRequestTypeDef](./type_defs.md#createpiperequestrequesttypedef) 

### delete\_pipe

Delete an existing pipe.

Type annotations and code completion for `#!python session.client("pipes").delete_pipe` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client)

```python
# delete_pipe method definition

await def delete_pipe(
    self,
    *,
    Name: str,
) -> DeletePipeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeletePipeResponseTypeDef](./type_defs.md#deletepiperesponsetypedef) 


```python
# delete_pipe method usage example with argument unpacking

kwargs: DeletePipeRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_pipe(**kwargs)
```

1. See [:material-code-braces: DeletePipeRequestRequestTypeDef](./type_defs.md#deletepiperequestrequesttypedef) 

### describe\_pipe

Get the information about an existing pipe.

Type annotations and code completion for `#!python session.client("pipes").describe_pipe` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client)

```python
# describe_pipe method definition

await def describe_pipe(
    self,
    *,
    Name: str,
) -> DescribePipeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePipeResponseTypeDef](./type_defs.md#describepiperesponsetypedef) 


```python
# describe_pipe method usage example with argument unpacking

kwargs: DescribePipeRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.describe_pipe(**kwargs)
```

1. See [:material-code-braces: DescribePipeRequestRequestTypeDef](./type_defs.md#describepiperequestrequesttypedef) 

### list\_pipes

Get the pipes associated with this account.

Type annotations and code completion for `#!python session.client("pipes").list_pipes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client)

```python
# list_pipes method definition

await def list_pipes(
    self,
    *,
    NamePrefix: str = ...,
    DesiredState: RequestedPipeStateType = ...,  # (1)
    CurrentState: PipeStateType = ...,  # (2)
    SourcePrefix: str = ...,
    TargetPrefix: str = ...,
    NextToken: str = ...,
    Limit: int = ...,
) -> ListPipesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RequestedPipeStateType](./literals.md#requestedpipestatetype) 
2. See [:material-code-brackets: PipeStateType](./literals.md#pipestatetype) 
3. See [:material-code-braces: ListPipesResponseTypeDef](./type_defs.md#listpipesresponsetypedef) 


```python
# list_pipes method usage example with argument unpacking

kwargs: ListPipesRequestRequestTypeDef = {  # (1)
    "NamePrefix": ...,
}

parent.list_pipes(**kwargs)
```

1. See [:material-code-braces: ListPipesRequestRequestTypeDef](./type_defs.md#listpipesrequestrequesttypedef) 

### list\_tags\_for\_resource

Displays the tags associated with a pipe.

Type annotations and code completion for `#!python session.client("pipes").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client)

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

### start\_pipe

Start an existing pipe.

Type annotations and code completion for `#!python session.client("pipes").start_pipe` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client)

```python
# start_pipe method definition

await def start_pipe(
    self,
    *,
    Name: str,
) -> StartPipeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartPipeResponseTypeDef](./type_defs.md#startpiperesponsetypedef) 


```python
# start_pipe method usage example with argument unpacking

kwargs: StartPipeRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.start_pipe(**kwargs)
```

1. See [:material-code-braces: StartPipeRequestRequestTypeDef](./type_defs.md#startpiperequestrequesttypedef) 

### stop\_pipe

Stop an existing pipe.

Type annotations and code completion for `#!python session.client("pipes").stop_pipe` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client)

```python
# stop_pipe method definition

await def stop_pipe(
    self,
    *,
    Name: str,
) -> StopPipeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopPipeResponseTypeDef](./type_defs.md#stoppiperesponsetypedef) 


```python
# stop_pipe method usage example with argument unpacking

kwargs: StopPipeRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.stop_pipe(**kwargs)
```

1. See [:material-code-braces: StopPipeRequestRequestTypeDef](./type_defs.md#stoppiperequestrequesttypedef) 

### tag\_resource

Assigns one or more tags (key-value pairs) to the specified pipe.

Type annotations and code completion for `#!python session.client("pipes").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client)

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

Removes one or more tags from the specified pipes.

Type annotations and code completion for `#!python session.client("pipes").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client)

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

### update\_pipe

Update an existing pipe.

Type annotations and code completion for `#!python session.client("pipes").update_pipe` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client)

```python
# update_pipe method definition

await def update_pipe(
    self,
    *,
    Name: str,
    RoleArn: str,
    Description: str = ...,
    DesiredState: RequestedPipeStateType = ...,  # (1)
    SourceParameters: UpdatePipeSourceParametersTypeDef = ...,  # (2)
    Enrichment: str = ...,
    EnrichmentParameters: PipeEnrichmentParametersTypeDef = ...,  # (3)
    Target: str = ...,
    TargetParameters: PipeTargetParametersTypeDef = ...,  # (4)
    LogConfiguration: PipeLogConfigurationParametersTypeDef = ...,  # (5)
    KmsKeyIdentifier: str = ...,
) -> UpdatePipeResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: RequestedPipeStateType](./literals.md#requestedpipestatetype) 
2. See [:material-code-braces: UpdatePipeSourceParametersTypeDef](./type_defs.md#updatepipesourceparameterstypedef) 
3. See [:material-code-braces: PipeEnrichmentParametersTypeDef](./type_defs.md#pipeenrichmentparameterstypedef) 
4. See [:material-code-braces: PipeTargetParametersTypeDef](./type_defs.md#pipetargetparameterstypedef) 
5. See [:material-code-braces: PipeLogConfigurationParametersTypeDef](./type_defs.md#pipelogconfigurationparameterstypedef) 
6. See [:material-code-braces: UpdatePipeResponseTypeDef](./type_defs.md#updatepiperesponsetypedef) 


```python
# update_pipe method usage example with argument unpacking

kwargs: UpdatePipeRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "RoleArn": ...,
}

parent.update_pipe(**kwargs)
```

1. See [:material-code-braces: UpdatePipeRequestRequestTypeDef](./type_defs.md#updatepiperequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("pipes").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("pipes").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client)

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

Type annotations and code completion for `#!python session.client("pipes").get_paginator` method with overloads.

- `client.get_paginator("list_pipes")` -> [ListPipesPaginator](./paginators.md#listpipespaginator)


