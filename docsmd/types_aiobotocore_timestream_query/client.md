# TimestreamQueryClient

> [Index](../README.md) > [TimestreamQuery](./README.md) > TimestreamQueryClient

!!! note ""

    Auto-generated documentation for [TimestreamQuery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#timestreamquery)
    type annotations stubs module [types-aiobotocore-timestream-query](https://pypi.org/project/types-aiobotocore-timestream-query/).

## TimestreamQueryClient

Type annotations and code completion for `#!python session.client("timestream-query")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

```python
# TimestreamQueryClient usage example

from aioboto3.session import Session
from types_aiobotocore_timestream_query.client import TimestreamQueryClient

session = Session()
async with session.client("timestream-query") as client:
    client: TimestreamQueryClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("timestream-query").exceptions` structure.

```python
# TimestreamQueryClient.exceptions usage example

async with session.client("timestream-query") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.InvalidEndpointException,
        client.exceptions.QueryExecutionException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# TimestreamQueryClient.exceptions type checking example

from types_aiobotocore_timestream_query.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("timestream-query").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("timestream-query").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

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


### cancel\_query

Cancels a query that has been issued.

Type annotations and code completion for `#!python session.client("timestream-query").cancel_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

```python
# cancel_query method definition

await def cancel_query(
    self,
    *,
    QueryId: str,
) -> CancelQueryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelQueryResponseTypeDef](./type_defs.md#cancelqueryresponsetypedef) 


```python
# cancel_query method usage example with argument unpacking

kwargs: CancelQueryRequestRequestTypeDef = {  # (1)
    "QueryId": ...,
}

parent.cancel_query(**kwargs)
```

1. See [:material-code-braces: CancelQueryRequestRequestTypeDef](./type_defs.md#cancelqueryrequestrequesttypedef) 

### create\_scheduled\_query

Create a scheduled query that will be run on your behalf at the configured
schedule.

Type annotations and code completion for `#!python session.client("timestream-query").create_scheduled_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

```python
# create_scheduled_query method definition

await def create_scheduled_query(
    self,
    *,
    Name: str,
    QueryString: str,
    ScheduleConfiguration: ScheduleConfigurationTypeDef,  # (1)
    NotificationConfiguration: NotificationConfigurationTypeDef,  # (2)
    ScheduledQueryExecutionRoleArn: str,
    ErrorReportConfiguration: ErrorReportConfigurationTypeDef,  # (3)
    TargetConfiguration: TargetConfigurationTypeDef = ...,  # (4)
    ClientToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (5)
    KmsKeyId: str = ...,
) -> CreateScheduledQueryResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
2. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
3. See [:material-code-braces: ErrorReportConfigurationTypeDef](./type_defs.md#errorreportconfigurationtypedef) 
4. See [:material-code-braces: TargetConfigurationTypeDef](./type_defs.md#targetconfigurationtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: CreateScheduledQueryResponseTypeDef](./type_defs.md#createscheduledqueryresponsetypedef) 


```python
# create_scheduled_query method usage example with argument unpacking

kwargs: CreateScheduledQueryRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "QueryString": ...,
    "ScheduleConfiguration": ...,
    "NotificationConfiguration": ...,
    "ScheduledQueryExecutionRoleArn": ...,
    "ErrorReportConfiguration": ...,
}

parent.create_scheduled_query(**kwargs)
```

1. See [:material-code-braces: CreateScheduledQueryRequestRequestTypeDef](./type_defs.md#createscheduledqueryrequestrequesttypedef) 

### delete\_scheduled\_query

Deletes a given scheduled query.

Type annotations and code completion for `#!python session.client("timestream-query").delete_scheduled_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

```python
# delete_scheduled_query method definition

await def delete_scheduled_query(
    self,
    *,
    ScheduledQueryArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_scheduled_query method usage example with argument unpacking

kwargs: DeleteScheduledQueryRequestRequestTypeDef = {  # (1)
    "ScheduledQueryArn": ...,
}

parent.delete_scheduled_query(**kwargs)
```

1. See [:material-code-braces: DeleteScheduledQueryRequestRequestTypeDef](./type_defs.md#deletescheduledqueryrequestrequesttypedef) 

### describe\_account\_settings

Describes the settings for your account that include the query pricing model
and the configured maximum TCUs the service can use for your query workload.

Type annotations and code completion for `#!python session.client("timestream-query").describe_account_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

```python
# describe_account_settings method definition

await def describe_account_settings(
    self,
) -> DescribeAccountSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAccountSettingsResponseTypeDef](./type_defs.md#describeaccountsettingsresponsetypedef) 

### describe\_endpoints

DescribeEndpoints returns a list of available endpoints to make Timestream API
calls against.

Type annotations and code completion for `#!python session.client("timestream-query").describe_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

```python
# describe_endpoints method definition

await def describe_endpoints(
    self,
) -> DescribeEndpointsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEndpointsResponseTypeDef](./type_defs.md#describeendpointsresponsetypedef) 

### describe\_scheduled\_query

Provides detailed information about a scheduled query.

Type annotations and code completion for `#!python session.client("timestream-query").describe_scheduled_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

```python
# describe_scheduled_query method definition

await def describe_scheduled_query(
    self,
    *,
    ScheduledQueryArn: str,
) -> DescribeScheduledQueryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeScheduledQueryResponseTypeDef](./type_defs.md#describescheduledqueryresponsetypedef) 


```python
# describe_scheduled_query method usage example with argument unpacking

kwargs: DescribeScheduledQueryRequestRequestTypeDef = {  # (1)
    "ScheduledQueryArn": ...,
}

parent.describe_scheduled_query(**kwargs)
```

1. See [:material-code-braces: DescribeScheduledQueryRequestRequestTypeDef](./type_defs.md#describescheduledqueryrequestrequesttypedef) 

### execute\_scheduled\_query

You can use this API to run a scheduled query manually.

Type annotations and code completion for `#!python session.client("timestream-query").execute_scheduled_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

```python
# execute_scheduled_query method definition

await def execute_scheduled_query(
    self,
    *,
    ScheduledQueryArn: str,
    InvocationTime: TimestampTypeDef,
    ClientToken: str = ...,
    QueryInsights: ScheduledQueryInsightsTypeDef = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ScheduledQueryInsightsTypeDef](./type_defs.md#scheduledqueryinsightstypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# execute_scheduled_query method usage example with argument unpacking

kwargs: ExecuteScheduledQueryRequestRequestTypeDef = {  # (1)
    "ScheduledQueryArn": ...,
    "InvocationTime": ...,
}

parent.execute_scheduled_query(**kwargs)
```

1. See [:material-code-braces: ExecuteScheduledQueryRequestRequestTypeDef](./type_defs.md#executescheduledqueryrequestrequesttypedef) 

### list\_scheduled\_queries

Gets a list of all scheduled queries in the caller's Amazon account and Region.

Type annotations and code completion for `#!python session.client("timestream-query").list_scheduled_queries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

```python
# list_scheduled_queries method definition

await def list_scheduled_queries(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListScheduledQueriesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListScheduledQueriesResponseTypeDef](./type_defs.md#listscheduledqueriesresponsetypedef) 


```python
# list_scheduled_queries method usage example with argument unpacking

kwargs: ListScheduledQueriesRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_scheduled_queries(**kwargs)
```

1. See [:material-code-braces: ListScheduledQueriesRequestRequestTypeDef](./type_defs.md#listscheduledqueriesrequestrequesttypedef) 

### list\_tags\_for\_resource

List all tags on a Timestream query resource.

Type annotations and code completion for `#!python session.client("timestream-query").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
    MaxResults: int = ...,
    NextToken: str = ...,
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

### prepare\_query

A synchronous operation that allows you to submit a query with parameters to be
stored by Timestream for later running.

Type annotations and code completion for `#!python session.client("timestream-query").prepare_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

```python
# prepare_query method definition

await def prepare_query(
    self,
    *,
    QueryString: str,
    ValidateOnly: bool = ...,
) -> PrepareQueryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PrepareQueryResponseTypeDef](./type_defs.md#preparequeryresponsetypedef) 


```python
# prepare_query method usage example with argument unpacking

kwargs: PrepareQueryRequestRequestTypeDef = {  # (1)
    "QueryString": ...,
}

parent.prepare_query(**kwargs)
```

1. See [:material-code-braces: PrepareQueryRequestRequestTypeDef](./type_defs.md#preparequeryrequestrequesttypedef) 

### query

<code>Query</code> is a synchronous operation that enables you to run a query
against your Amazon Timestream data.

Type annotations and code completion for `#!python session.client("timestream-query").query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

```python
# query method definition

await def query(
    self,
    *,
    QueryString: str,
    ClientToken: str = ...,
    NextToken: str = ...,
    MaxRows: int = ...,
    QueryInsights: QueryInsightsTypeDef = ...,  # (1)
) -> QueryResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: QueryInsightsTypeDef](./type_defs.md#queryinsightstypedef) 
2. See [:material-code-braces: QueryResponseTypeDef](./type_defs.md#queryresponsetypedef) 


```python
# query method usage example with argument unpacking

kwargs: QueryRequestRequestTypeDef = {  # (1)
    "QueryString": ...,
}

parent.query(**kwargs)
```

1. See [:material-code-braces: QueryRequestRequestTypeDef](./type_defs.md#queryrequestrequesttypedef) 

### tag\_resource

Associate a set of tags with a Timestream resource.

Type annotations and code completion for `#!python session.client("timestream-query").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

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

Removes the association of tags from a Timestream query resource.

Type annotations and code completion for `#!python session.client("timestream-query").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

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

### update\_account\_settings

Transitions your account to use TCUs for query pricing and modifies the maximum
query compute units that you've configured.

Type annotations and code completion for `#!python session.client("timestream-query").update_account_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

```python
# update_account_settings method definition

await def update_account_settings(
    self,
    *,
    MaxQueryTCU: int = ...,
    QueryPricingModel: QueryPricingModelType = ...,  # (1)
    QueryCompute: QueryComputeRequestTypeDef = ...,  # (2)
) -> UpdateAccountSettingsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: QueryPricingModelType](./literals.md#querypricingmodeltype) 
2. See [:material-code-braces: QueryComputeRequestTypeDef](./type_defs.md#querycomputerequesttypedef) 
3. See [:material-code-braces: UpdateAccountSettingsResponseTypeDef](./type_defs.md#updateaccountsettingsresponsetypedef) 


```python
# update_account_settings method usage example with argument unpacking

kwargs: UpdateAccountSettingsRequestRequestTypeDef = {  # (1)
    "MaxQueryTCU": ...,
}

parent.update_account_settings(**kwargs)
```

1. See [:material-code-braces: UpdateAccountSettingsRequestRequestTypeDef](./type_defs.md#updateaccountsettingsrequestrequesttypedef) 

### update\_scheduled\_query

Update a scheduled query.

Type annotations and code completion for `#!python session.client("timestream-query").update_scheduled_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

```python
# update_scheduled_query method definition

await def update_scheduled_query(
    self,
    *,
    ScheduledQueryArn: str,
    State: ScheduledQueryStateType,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScheduledQueryStateType](./literals.md#scheduledquerystatetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_scheduled_query method usage example with argument unpacking

kwargs: UpdateScheduledQueryRequestRequestTypeDef = {  # (1)
    "ScheduledQueryArn": ...,
    "State": ...,
}

parent.update_scheduled_query(**kwargs)
```

1. See [:material-code-braces: UpdateScheduledQueryRequestRequestTypeDef](./type_defs.md#updatescheduledqueryrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("timestream-query").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("timestream-query").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

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

Type annotations and code completion for `#!python session.client("timestream-query").get_paginator` method with overloads.

- `client.get_paginator("list_scheduled_queries")` -> [ListScheduledQueriesPaginator](./paginators.md#listscheduledqueriespaginator)
- `client.get_paginator("list_tags_for_resource")` -> [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
- `client.get_paginator("query")` -> [QueryPaginator](./paginators.md#querypaginator)


