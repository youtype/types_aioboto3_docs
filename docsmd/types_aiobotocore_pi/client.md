# PIClient

> [Index](../README.md) > [PI](./README.md) > PIClient

!!! note ""

    Auto-generated documentation for [PI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#pi)
    type annotations stubs module [types-aiobotocore-pi](https://pypi.org/project/types-aiobotocore-pi/).

## PIClient

Type annotations and code completion for `#!python session.client("pi")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

```python
# PIClient usage example

from aioboto3.session import Session
from types_aiobotocore_pi.client import PIClient

session = Session()
async with session.client("pi") as client:
    client: PIClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("pi").exceptions` structure.

```python
# PIClient.exceptions usage example

async with session.client("pi") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.InternalServiceError,
        client.exceptions.InvalidArgumentException,
        client.exceptions.NotAuthorizedException,
    ) as e:
        print(e)
```

```python
# PIClient.exceptions type checking example

from types_aiobotocore_pi.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("pi").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("pi").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

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


### create\_performance\_analysis\_report

Creates a new performance analysis report for a specific time period for the DB
instance.

Type annotations and code completion for `#!python session.client("pi").create_performance_analysis_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

```python
# create_performance_analysis_report method definition

await def create_performance_analysis_report(
    self,
    *,
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreatePerformanceAnalysisReportResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreatePerformanceAnalysisReportResponseTypeDef](./type_defs.md#createperformanceanalysisreportresponsetypedef) 


```python
# create_performance_analysis_report method usage example with argument unpacking

kwargs: CreatePerformanceAnalysisReportRequestRequestTypeDef = {  # (1)
    "ServiceType": ...,
    "Identifier": ...,
    "StartTime": ...,
    "EndTime": ...,
}

parent.create_performance_analysis_report(**kwargs)
```

1. See [:material-code-braces: CreatePerformanceAnalysisReportRequestRequestTypeDef](./type_defs.md#createperformanceanalysisreportrequestrequesttypedef) 

### delete\_performance\_analysis\_report

Deletes a performance analysis report.

Type annotations and code completion for `#!python session.client("pi").delete_performance_analysis_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

```python
# delete_performance_analysis_report method definition

await def delete_performance_analysis_report(
    self,
    *,
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    AnalysisReportId: str,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 


```python
# delete_performance_analysis_report method usage example with argument unpacking

kwargs: DeletePerformanceAnalysisReportRequestRequestTypeDef = {  # (1)
    "ServiceType": ...,
    "Identifier": ...,
    "AnalysisReportId": ...,
}

parent.delete_performance_analysis_report(**kwargs)
```

1. See [:material-code-braces: DeletePerformanceAnalysisReportRequestRequestTypeDef](./type_defs.md#deleteperformanceanalysisreportrequestrequesttypedef) 

### describe\_dimension\_keys

For a specific time period, retrieve the top <code>N</code> dimension keys for
a metric.

Type annotations and code completion for `#!python session.client("pi").describe_dimension_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

```python
# describe_dimension_keys method definition

await def describe_dimension_keys(
    self,
    *,
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    Metric: str,
    GroupBy: DimensionGroupTypeDef,  # (2)
    PeriodInSeconds: int = ...,
    AdditionalMetrics: Sequence[str] = ...,
    PartitionBy: DimensionGroupTypeDef = ...,  # (2)
    Filter: Mapping[str, str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeDimensionKeysResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-braces: DimensionGroupTypeDef](./type_defs.md#dimensiongrouptypedef) 
3. See [:material-code-braces: DimensionGroupTypeDef](./type_defs.md#dimensiongrouptypedef) 
4. See [:material-code-braces: DescribeDimensionKeysResponseTypeDef](./type_defs.md#describedimensionkeysresponsetypedef) 


```python
# describe_dimension_keys method usage example with argument unpacking

kwargs: DescribeDimensionKeysRequestRequestTypeDef = {  # (1)
    "ServiceType": ...,
    "Identifier": ...,
    "StartTime": ...,
    "EndTime": ...,
    "Metric": ...,
    "GroupBy": ...,
}

parent.describe_dimension_keys(**kwargs)
```

1. See [:material-code-braces: DescribeDimensionKeysRequestRequestTypeDef](./type_defs.md#describedimensionkeysrequestrequesttypedef) 

### get\_dimension\_key\_details

Get the attributes of the specified dimension group for a DB instance or data
source.

Type annotations and code completion for `#!python session.client("pi").get_dimension_key_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

```python
# get_dimension_key_details method definition

await def get_dimension_key_details(
    self,
    *,
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    Group: str,
    GroupIdentifier: str,
    RequestedDimensions: Sequence[str] = ...,
) -> GetDimensionKeyDetailsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-braces: GetDimensionKeyDetailsResponseTypeDef](./type_defs.md#getdimensionkeydetailsresponsetypedef) 


```python
# get_dimension_key_details method usage example with argument unpacking

kwargs: GetDimensionKeyDetailsRequestRequestTypeDef = {  # (1)
    "ServiceType": ...,
    "Identifier": ...,
    "Group": ...,
    "GroupIdentifier": ...,
}

parent.get_dimension_key_details(**kwargs)
```

1. See [:material-code-braces: GetDimensionKeyDetailsRequestRequestTypeDef](./type_defs.md#getdimensionkeydetailsrequestrequesttypedef) 

### get\_performance\_analysis\_report

Retrieves the report including the report ID, status, time details, and the
insights with recommendations.

Type annotations and code completion for `#!python session.client("pi").get_performance_analysis_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

```python
# get_performance_analysis_report method definition

await def get_performance_analysis_report(
    self,
    *,
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    AnalysisReportId: str,
    TextFormat: TextFormatType = ...,  # (2)
    AcceptLanguage: AcceptLanguageType = ...,  # (3)
) -> GetPerformanceAnalysisReportResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-brackets: TextFormatType](./literals.md#textformattype) 
3. See [:material-code-brackets: AcceptLanguageType](./literals.md#acceptlanguagetype) 
4. See [:material-code-braces: GetPerformanceAnalysisReportResponseTypeDef](./type_defs.md#getperformanceanalysisreportresponsetypedef) 


```python
# get_performance_analysis_report method usage example with argument unpacking

kwargs: GetPerformanceAnalysisReportRequestRequestTypeDef = {  # (1)
    "ServiceType": ...,
    "Identifier": ...,
    "AnalysisReportId": ...,
}

parent.get_performance_analysis_report(**kwargs)
```

1. See [:material-code-braces: GetPerformanceAnalysisReportRequestRequestTypeDef](./type_defs.md#getperformanceanalysisreportrequestrequesttypedef) 

### get\_resource\_metadata

Retrieve the metadata for different features.

Type annotations and code completion for `#!python session.client("pi").get_resource_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

```python
# get_resource_metadata method definition

await def get_resource_metadata(
    self,
    *,
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
) -> GetResourceMetadataResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-braces: GetResourceMetadataResponseTypeDef](./type_defs.md#getresourcemetadataresponsetypedef) 


```python
# get_resource_metadata method usage example with argument unpacking

kwargs: GetResourceMetadataRequestRequestTypeDef = {  # (1)
    "ServiceType": ...,
    "Identifier": ...,
}

parent.get_resource_metadata(**kwargs)
```

1. See [:material-code-braces: GetResourceMetadataRequestRequestTypeDef](./type_defs.md#getresourcemetadatarequestrequesttypedef) 

### get\_resource\_metrics

Retrieve Performance Insights metrics for a set of data sources over a time
period.

Type annotations and code completion for `#!python session.client("pi").get_resource_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

```python
# get_resource_metrics method definition

await def get_resource_metrics(
    self,
    *,
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    MetricQueries: Sequence[MetricQueryTypeDef],  # (2)
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    PeriodInSeconds: int = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    PeriodAlignment: PeriodAlignmentType = ...,  # (3)
) -> GetResourceMetricsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-braces: MetricQueryTypeDef](./type_defs.md#metricquerytypedef) 
3. See [:material-code-brackets: PeriodAlignmentType](./literals.md#periodalignmenttype) 
4. See [:material-code-braces: GetResourceMetricsResponseTypeDef](./type_defs.md#getresourcemetricsresponsetypedef) 


```python
# get_resource_metrics method usage example with argument unpacking

kwargs: GetResourceMetricsRequestRequestTypeDef = {  # (1)
    "ServiceType": ...,
    "Identifier": ...,
    "MetricQueries": ...,
    "StartTime": ...,
    "EndTime": ...,
}

parent.get_resource_metrics(**kwargs)
```

1. See [:material-code-braces: GetResourceMetricsRequestRequestTypeDef](./type_defs.md#getresourcemetricsrequestrequesttypedef) 

### list\_available\_resource\_dimensions

Retrieve the dimensions that can be queried for each specified metric type on a
specified DB instance.

Type annotations and code completion for `#!python session.client("pi").list_available_resource_dimensions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

```python
# list_available_resource_dimensions method definition

await def list_available_resource_dimensions(
    self,
    *,
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    Metrics: Sequence[str],
    MaxResults: int = ...,
    NextToken: str = ...,
    AuthorizedActions: Sequence[FineGrainedActionType] = ...,  # (2)
) -> ListAvailableResourceDimensionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-brackets: FineGrainedActionType](./literals.md#finegrainedactiontype) 
3. See [:material-code-braces: ListAvailableResourceDimensionsResponseTypeDef](./type_defs.md#listavailableresourcedimensionsresponsetypedef) 


```python
# list_available_resource_dimensions method usage example with argument unpacking

kwargs: ListAvailableResourceDimensionsRequestRequestTypeDef = {  # (1)
    "ServiceType": ...,
    "Identifier": ...,
    "Metrics": ...,
}

parent.list_available_resource_dimensions(**kwargs)
```

1. See [:material-code-braces: ListAvailableResourceDimensionsRequestRequestTypeDef](./type_defs.md#listavailableresourcedimensionsrequestrequesttypedef) 

### list\_available\_resource\_metrics

Retrieve metrics of the specified types that can be queried for a specified DB
instance.

Type annotations and code completion for `#!python session.client("pi").list_available_resource_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

```python
# list_available_resource_metrics method definition

await def list_available_resource_metrics(
    self,
    *,
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    MetricTypes: Sequence[str],
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAvailableResourceMetricsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-braces: ListAvailableResourceMetricsResponseTypeDef](./type_defs.md#listavailableresourcemetricsresponsetypedef) 


```python
# list_available_resource_metrics method usage example with argument unpacking

kwargs: ListAvailableResourceMetricsRequestRequestTypeDef = {  # (1)
    "ServiceType": ...,
    "Identifier": ...,
    "MetricTypes": ...,
}

parent.list_available_resource_metrics(**kwargs)
```

1. See [:material-code-braces: ListAvailableResourceMetricsRequestRequestTypeDef](./type_defs.md#listavailableresourcemetricsrequestrequesttypedef) 

### list\_performance\_analysis\_reports

Lists all the analysis reports created for the DB instance.

Type annotations and code completion for `#!python session.client("pi").list_performance_analysis_reports` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

```python
# list_performance_analysis_reports method definition

await def list_performance_analysis_reports(
    self,
    *,
    ServiceType: ServiceTypeType,  # (1)
    Identifier: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    ListTags: bool = ...,
) -> ListPerformanceAnalysisReportsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-braces: ListPerformanceAnalysisReportsResponseTypeDef](./type_defs.md#listperformanceanalysisreportsresponsetypedef) 


```python
# list_performance_analysis_reports method usage example with argument unpacking

kwargs: ListPerformanceAnalysisReportsRequestRequestTypeDef = {  # (1)
    "ServiceType": ...,
    "Identifier": ...,
}

parent.list_performance_analysis_reports(**kwargs)
```

1. See [:material-code-braces: ListPerformanceAnalysisReportsRequestRequestTypeDef](./type_defs.md#listperformanceanalysisreportsrequestrequesttypedef) 

### list\_tags\_for\_resource

Retrieves all the metadata tags associated with Amazon RDS Performance Insights
resource.

Type annotations and code completion for `#!python session.client("pi").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ServiceType: ServiceTypeType,  # (1)
    ResourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ServiceType": ...,
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### tag\_resource

Adds metadata tags to the Amazon RDS Performance Insights resource.

Type annotations and code completion for `#!python session.client("pi").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ServiceType: ServiceTypeType,  # (1)
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (2)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ServiceType": ...,
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Deletes the metadata tags from the Amazon RDS Performance Insights resource.

Type annotations and code completion for `#!python session.client("pi").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ServiceType: ServiceTypeType,  # (1)
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ServiceType": ...,
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("pi").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("pi").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

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




