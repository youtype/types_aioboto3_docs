# ApplicationCostProfilerClient

> [Index](../README.md) > [ApplicationCostProfiler](./README.md) > ApplicationCostProfilerClient

!!! note ""

    Auto-generated documentation for [ApplicationCostProfiler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#applicationcostprofiler)
    type annotations stubs module [types-aiobotocore-applicationcostprofiler](https://pypi.org/project/types-aiobotocore-applicationcostprofiler/).

## ApplicationCostProfilerClient

Type annotations and code completion for `#!python session.client("applicationcostprofiler")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client)

```python
# ApplicationCostProfilerClient usage example

from aioboto3.session import Session
from types_aiobotocore_applicationcostprofiler.client import ApplicationCostProfilerClient

session = Session()
async with session.client("applicationcostprofiler") as client:
    client: ApplicationCostProfilerClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("applicationcostprofiler").exceptions` structure.

```python
# ApplicationCostProfilerClient.exceptions usage example

async with session.client("applicationcostprofiler") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.InternalServerException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# ApplicationCostProfilerClient.exceptions type checking example

from types_aiobotocore_applicationcostprofiler.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("applicationcostprofiler").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("applicationcostprofiler").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client)

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

Deletes the specified report definition in AWS Application Cost Profiler.

Type annotations and code completion for `#!python session.client("applicationcostprofiler").delete_report_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client)

```python
# delete_report_definition method definition

await def delete_report_definition(
    self,
    *,
    reportId: str,
) -> DeleteReportDefinitionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteReportDefinitionResultTypeDef](./type_defs.md#deletereportdefinitionresulttypedef) 


```python
# delete_report_definition method usage example with argument unpacking

kwargs: DeleteReportDefinitionRequestRequestTypeDef = {  # (1)
    "reportId": ...,
}

parent.delete_report_definition(**kwargs)
```

1. See [:material-code-braces: DeleteReportDefinitionRequestRequestTypeDef](./type_defs.md#deletereportdefinitionrequestrequesttypedef) 

### get\_report\_definition

Retrieves the definition of a report already configured in AWS Application Cost
Profiler.

Type annotations and code completion for `#!python session.client("applicationcostprofiler").get_report_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client)

```python
# get_report_definition method definition

await def get_report_definition(
    self,
    *,
    reportId: str,
) -> GetReportDefinitionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetReportDefinitionResultTypeDef](./type_defs.md#getreportdefinitionresulttypedef) 


```python
# get_report_definition method usage example with argument unpacking

kwargs: GetReportDefinitionRequestRequestTypeDef = {  # (1)
    "reportId": ...,
}

parent.get_report_definition(**kwargs)
```

1. See [:material-code-braces: GetReportDefinitionRequestRequestTypeDef](./type_defs.md#getreportdefinitionrequestrequesttypedef) 

### import\_application\_usage

Ingests application usage data from Amazon Simple Storage Service (Amazon S3).

Type annotations and code completion for `#!python session.client("applicationcostprofiler").import_application_usage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client)

```python
# import_application_usage method definition

await def import_application_usage(
    self,
    *,
    sourceS3Location: SourceS3LocationTypeDef,  # (1)
) -> ImportApplicationUsageResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SourceS3LocationTypeDef](./type_defs.md#sources3locationtypedef) 
2. See [:material-code-braces: ImportApplicationUsageResultTypeDef](./type_defs.md#importapplicationusageresulttypedef) 


```python
# import_application_usage method usage example with argument unpacking

kwargs: ImportApplicationUsageRequestRequestTypeDef = {  # (1)
    "sourceS3Location": ...,
}

parent.import_application_usage(**kwargs)
```

1. See [:material-code-braces: ImportApplicationUsageRequestRequestTypeDef](./type_defs.md#importapplicationusagerequestrequesttypedef) 

### list\_report\_definitions

Retrieves a list of all reports and their configurations for your AWS account.

Type annotations and code completion for `#!python session.client("applicationcostprofiler").list_report_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client)

```python
# list_report_definitions method definition

await def list_report_definitions(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListReportDefinitionsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListReportDefinitionsResultTypeDef](./type_defs.md#listreportdefinitionsresulttypedef) 


```python
# list_report_definitions method usage example with argument unpacking

kwargs: ListReportDefinitionsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_report_definitions(**kwargs)
```

1. See [:material-code-braces: ListReportDefinitionsRequestRequestTypeDef](./type_defs.md#listreportdefinitionsrequestrequesttypedef) 

### put\_report\_definition

Creates the report definition for a report in Application Cost Profiler.

Type annotations and code completion for `#!python session.client("applicationcostprofiler").put_report_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client)

```python
# put_report_definition method definition

await def put_report_definition(
    self,
    *,
    reportId: str,
    reportDescription: str,
    reportFrequency: ReportFrequencyType,  # (1)
    format: FormatType,  # (2)
    destinationS3Location: S3LocationTypeDef,  # (3)
) -> PutReportDefinitionResultTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ReportFrequencyType](./literals.md#reportfrequencytype) 
2. See [:material-code-brackets: FormatType](./literals.md#formattype) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-braces: PutReportDefinitionResultTypeDef](./type_defs.md#putreportdefinitionresulttypedef) 


```python
# put_report_definition method usage example with argument unpacking

kwargs: PutReportDefinitionRequestRequestTypeDef = {  # (1)
    "reportId": ...,
    "reportDescription": ...,
    "reportFrequency": ...,
    "format": ...,
    "destinationS3Location": ...,
}

parent.put_report_definition(**kwargs)
```

1. See [:material-code-braces: PutReportDefinitionRequestRequestTypeDef](./type_defs.md#putreportdefinitionrequestrequesttypedef) 

### update\_report\_definition

Updates existing report in AWS Application Cost Profiler.

Type annotations and code completion for `#!python session.client("applicationcostprofiler").update_report_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client)

```python
# update_report_definition method definition

await def update_report_definition(
    self,
    *,
    reportId: str,
    reportDescription: str,
    reportFrequency: ReportFrequencyType,  # (1)
    format: FormatType,  # (2)
    destinationS3Location: S3LocationTypeDef,  # (3)
) -> UpdateReportDefinitionResultTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ReportFrequencyType](./literals.md#reportfrequencytype) 
2. See [:material-code-brackets: FormatType](./literals.md#formattype) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-braces: UpdateReportDefinitionResultTypeDef](./type_defs.md#updatereportdefinitionresulttypedef) 


```python
# update_report_definition method usage example with argument unpacking

kwargs: UpdateReportDefinitionRequestRequestTypeDef = {  # (1)
    "reportId": ...,
    "reportDescription": ...,
    "reportFrequency": ...,
    "format": ...,
    "destinationS3Location": ...,
}

parent.update_report_definition(**kwargs)
```

1. See [:material-code-braces: UpdateReportDefinitionRequestRequestTypeDef](./type_defs.md#updatereportdefinitionrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("applicationcostprofiler").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("applicationcostprofiler").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Client)

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

Type annotations and code completion for `#!python session.client("applicationcostprofiler").get_paginator` method with overloads.

- `client.get_paginator("list_report_definitions")` -> [ListReportDefinitionsPaginator](./paginators.md#listreportdefinitionspaginator)


