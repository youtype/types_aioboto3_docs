# KendraRankingClient

> [Index](../README.md) > [KendraRanking](./README.md) > KendraRankingClient

!!! note ""

    Auto-generated documentation for [KendraRanking](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#kendraranking)
    type annotations stubs module [types-aiobotocore-kendra-ranking](https://pypi.org/project/types-aiobotocore-kendra-ranking/).

## KendraRankingClient

Type annotations and code completion for `#!python session.client("kendra-ranking")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking.Client)

```python
# KendraRankingClient usage example

from aioboto3.session import Session
from types_aiobotocore_kendra_ranking.client import KendraRankingClient

session = Session()
async with session.client("kendra-ranking") as client:
    client: KendraRankingClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("kendra-ranking").exceptions` structure.

```python
# KendraRankingClient.exceptions usage example

async with session.client("kendra-ranking") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ResourceUnavailableException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# KendraRankingClient.exceptions type checking example

from types_aiobotocore_kendra_ranking.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("kendra-ranking").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("kendra-ranking").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking.Client)

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


### create\_rescore\_execution\_plan

Creates a rescore execution plan.

Type annotations and code completion for `#!python session.client("kendra-ranking").create_rescore_execution_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking.Client)

```python
# create_rescore_execution_plan method definition

await def create_rescore_execution_plan(
    self,
    *,
    Name: str,
    Description: str = ...,
    CapacityUnits: CapacityUnitsConfigurationTypeDef = ...,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    ClientToken: str = ...,
) -> CreateRescoreExecutionPlanResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: CapacityUnitsConfigurationTypeDef](./type_defs.md#capacityunitsconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateRescoreExecutionPlanResponseTypeDef](./type_defs.md#createrescoreexecutionplanresponsetypedef) 


```python
# create_rescore_execution_plan method usage example with argument unpacking

kwargs: CreateRescoreExecutionPlanRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_rescore_execution_plan(**kwargs)
```

1. See [:material-code-braces: CreateRescoreExecutionPlanRequestRequestTypeDef](./type_defs.md#createrescoreexecutionplanrequestrequesttypedef) 

### delete\_rescore\_execution\_plan

Deletes a rescore execution plan.

Type annotations and code completion for `#!python session.client("kendra-ranking").delete_rescore_execution_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking.Client)

```python
# delete_rescore_execution_plan method definition

await def delete_rescore_execution_plan(
    self,
    *,
    Id: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_rescore_execution_plan method usage example with argument unpacking

kwargs: DeleteRescoreExecutionPlanRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_rescore_execution_plan(**kwargs)
```

1. See [:material-code-braces: DeleteRescoreExecutionPlanRequestRequestTypeDef](./type_defs.md#deleterescoreexecutionplanrequestrequesttypedef) 

### describe\_rescore\_execution\_plan

Gets information about a rescore execution plan.

Type annotations and code completion for `#!python session.client("kendra-ranking").describe_rescore_execution_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking.Client)

```python
# describe_rescore_execution_plan method definition

await def describe_rescore_execution_plan(
    self,
    *,
    Id: str,
) -> DescribeRescoreExecutionPlanResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRescoreExecutionPlanResponseTypeDef](./type_defs.md#describerescoreexecutionplanresponsetypedef) 


```python
# describe_rescore_execution_plan method usage example with argument unpacking

kwargs: DescribeRescoreExecutionPlanRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.describe_rescore_execution_plan(**kwargs)
```

1. See [:material-code-braces: DescribeRescoreExecutionPlanRequestRequestTypeDef](./type_defs.md#describerescoreexecutionplanrequestrequesttypedef) 

### list\_rescore\_execution\_plans

Lists your rescore execution plans.

Type annotations and code completion for `#!python session.client("kendra-ranking").list_rescore_execution_plans` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking.Client)

```python
# list_rescore_execution_plans method definition

await def list_rescore_execution_plans(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListRescoreExecutionPlansResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRescoreExecutionPlansResponseTypeDef](./type_defs.md#listrescoreexecutionplansresponsetypedef) 


```python
# list_rescore_execution_plans method usage example with argument unpacking

kwargs: ListRescoreExecutionPlansRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_rescore_execution_plans(**kwargs)
```

1. See [:material-code-braces: ListRescoreExecutionPlansRequestRequestTypeDef](./type_defs.md#listrescoreexecutionplansrequestrequesttypedef) 

### list\_tags\_for\_resource

Gets a list of tags associated with a specified resource.

Type annotations and code completion for `#!python session.client("kendra-ranking").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### rescore

Rescores or re-ranks search results from a search service such as OpenSearch
(self managed).

Type annotations and code completion for `#!python session.client("kendra-ranking").rescore` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking.Client)

```python
# rescore method definition

await def rescore(
    self,
    *,
    RescoreExecutionPlanId: str,
    SearchQuery: str,
    Documents: Sequence[DocumentTypeDef],  # (1)
) -> RescoreResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
2. See [:material-code-braces: RescoreResultTypeDef](./type_defs.md#rescoreresulttypedef) 


```python
# rescore method usage example with argument unpacking

kwargs: RescoreRequestRequestTypeDef = {  # (1)
    "RescoreExecutionPlanId": ...,
    "SearchQuery": ...,
    "Documents": ...,
}

parent.rescore(**kwargs)
```

1. See [:material-code-braces: RescoreRequestRequestTypeDef](./type_defs.md#rescorerequestrequesttypedef) 

### tag\_resource

Adds a specified tag to a specified rescore execution plan.

Type annotations and code completion for `#!python session.client("kendra-ranking").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes a tag from a rescore execution plan.

Type annotations and code completion for `#!python session.client("kendra-ranking").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_rescore\_execution\_plan

Updates a rescore execution plan.

Type annotations and code completion for `#!python session.client("kendra-ranking").update_rescore_execution_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking.Client)

```python
# update_rescore_execution_plan method definition

await def update_rescore_execution_plan(
    self,
    *,
    Id: str,
    Name: str = ...,
    Description: str = ...,
    CapacityUnits: CapacityUnitsConfigurationTypeDef = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CapacityUnitsConfigurationTypeDef](./type_defs.md#capacityunitsconfigurationtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_rescore_execution_plan method usage example with argument unpacking

kwargs: UpdateRescoreExecutionPlanRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.update_rescore_execution_plan(**kwargs)
```

1. See [:material-code-braces: UpdateRescoreExecutionPlanRequestRequestTypeDef](./type_defs.md#updaterescoreexecutionplanrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("kendra-ranking").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("kendra-ranking").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking.Client)

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




