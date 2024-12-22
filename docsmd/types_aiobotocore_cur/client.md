# CostandUsageReportServiceClient

> [Index](../README.md) > [CostandUsageReportService](./README.md) > CostandUsageReportServiceClient

!!! note ""

    Auto-generated documentation for [CostandUsageReportService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#costandusagereportservice)
    type annotations stubs module [types-aiobotocore-cur](https://pypi.org/project/types-aiobotocore-cur/).

## CostandUsageReportServiceClient

Type annotations and code completion for `#!python session.client("cur")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client)

```python
# CostandUsageReportServiceClient usage example

from aioboto3.session import Session
from types_aiobotocore_cur.client import CostandUsageReportServiceClient

session = Session()
async with session.client("cur") as client:
    client: CostandUsageReportServiceClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("cur").exceptions` structure.

```python
# CostandUsageReportServiceClient.exceptions usage example

async with session.client("cur") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.DuplicateReportNameException,
        client.exceptions.InternalErrorException,
        client.exceptions.ReportLimitReachedException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# CostandUsageReportServiceClient.exceptions type checking example

from types_aiobotocore_cur.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("cur").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("cur").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client)

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


### delete\_report\_definition

Deletes the specified report.

Type annotations and code completion for `#!python session.client("cur").delete_report_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client)

```python
# delete_report_definition method definition

await def delete_report_definition(
    self,
    *,
    ReportName: str,
) -> DeleteReportDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteReportDefinitionResponseTypeDef](./type_defs.md#deletereportdefinitionresponsetypedef) 


```python
# delete_report_definition method usage example with argument unpacking

kwargs: DeleteReportDefinitionRequestRequestTypeDef = {  # (1)
    "ReportName": ...,
}

parent.delete_report_definition(**kwargs)
```

1. See [:material-code-braces: DeleteReportDefinitionRequestRequestTypeDef](./type_defs.md#deletereportdefinitionrequestrequesttypedef) 

### describe\_report\_definitions

Lists the Amazon Web Services Cost and Usage Report available to this account.

Type annotations and code completion for `#!python session.client("cur").describe_report_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client)

```python
# describe_report_definitions method definition

await def describe_report_definitions(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeReportDefinitionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeReportDefinitionsResponseTypeDef](./type_defs.md#describereportdefinitionsresponsetypedef) 


```python
# describe_report_definitions method usage example with argument unpacking

kwargs: DescribeReportDefinitionsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.describe_report_definitions(**kwargs)
```

1. See [:material-code-braces: DescribeReportDefinitionsRequestRequestTypeDef](./type_defs.md#describereportdefinitionsrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags associated with the specified report definition.

Type annotations and code completion for `#!python session.client("cur").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ReportName: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ReportName": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### modify\_report\_definition

Allows you to programmatically update your report preferences.

Type annotations and code completion for `#!python session.client("cur").modify_report_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client)

```python
# modify_report_definition method definition

await def modify_report_definition(
    self,
    *,
    ReportName: str,
    ReportDefinition: ReportDefinitionTypeDef,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: ReportDefinitionTypeDef](./type_defs.md#reportdefinitiontypedef) 


```python
# modify_report_definition method usage example with argument unpacking

kwargs: ModifyReportDefinitionRequestRequestTypeDef = {  # (1)
    "ReportName": ...,
    "ReportDefinition": ...,
}

parent.modify_report_definition(**kwargs)
```

1. See [:material-code-braces: ModifyReportDefinitionRequestRequestTypeDef](./type_defs.md#modifyreportdefinitionrequestrequesttypedef) 

### put\_report\_definition

Creates a new report using the description that you provide.

Type annotations and code completion for `#!python session.client("cur").put_report_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client)

```python
# put_report_definition method definition

await def put_report_definition(
    self,
    *,
    ReportDefinition: ReportDefinitionTypeDef,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: ReportDefinitionTypeDef](./type_defs.md#reportdefinitiontypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# put_report_definition method usage example with argument unpacking

kwargs: PutReportDefinitionRequestRequestTypeDef = {  # (1)
    "ReportDefinition": ...,
}

parent.put_report_definition(**kwargs)
```

1. See [:material-code-braces: PutReportDefinitionRequestRequestTypeDef](./type_defs.md#putreportdefinitionrequestrequesttypedef) 

### tag\_resource

Associates a set of tags with a report definition.

Type annotations and code completion for `#!python session.client("cur").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ReportName: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ReportName": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Disassociates a set of tags from a report definition.

Type annotations and code completion for `#!python session.client("cur").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ReportName: str,
    TagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ReportName": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("cur").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("cur").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client)

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

Type annotations and code completion for `#!python session.client("cur").get_paginator` method with overloads.

- `client.get_paginator("describe_report_definitions")` -> [DescribeReportDefinitionsPaginator](./paginators.md#describereportdefinitionspaginator)



