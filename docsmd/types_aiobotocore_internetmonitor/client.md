# CloudWatchInternetMonitorClient

> [Index](../README.md) > [CloudWatchInternetMonitor](./README.md) > CloudWatchInternetMonitorClient

!!! note ""

    Auto-generated documentation for [CloudWatchInternetMonitor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#cloudwatchinternetmonitor)
    type annotations stubs module [types-aiobotocore-internetmonitor](https://pypi.org/project/types-aiobotocore-internetmonitor/).

## CloudWatchInternetMonitorClient

Type annotations and code completion for `#!python session.client("internetmonitor")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# CloudWatchInternetMonitorClient usage example

from aioboto3.session import Session
from types_aiobotocore_internetmonitor.client import CloudWatchInternetMonitorClient

session = Session()
async with session.client("internetmonitor") as client:
    client: CloudWatchInternetMonitorClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("internetmonitor").exceptions` structure.

```python
# CloudWatchInternetMonitorClient.exceptions usage example

async with session.client("internetmonitor") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.BadRequestException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerErrorException,
        client.exceptions.InternalServerException,
        client.exceptions.LimitExceededException,
        client.exceptions.NotFoundException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ThrottlingException,
        client.exceptions.TooManyRequestsException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# CloudWatchInternetMonitorClient.exceptions type checking example

from types_aiobotocore_internetmonitor.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("internetmonitor").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("internetmonitor").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

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


### create\_monitor

Creates a monitor in Amazon CloudWatch Internet Monitor.

Type annotations and code completion for `#!python session.client("internetmonitor").create_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# create_monitor method definition

await def create_monitor(
    self,
    *,
    MonitorName: str,
    Resources: Sequence[str] = ...,
    ClientToken: str = ...,
    Tags: Mapping[str, str] = ...,
    MaxCityNetworksToMonitor: int = ...,
    InternetMeasurementsLogDelivery: InternetMeasurementsLogDeliveryTypeDef = ...,  # (1)
    TrafficPercentageToMonitor: int = ...,
    HealthEventsConfig: HealthEventsConfigTypeDef = ...,  # (2)
) -> CreateMonitorOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: InternetMeasurementsLogDeliveryTypeDef](./type_defs.md#internetmeasurementslogdeliverytypedef) 
2. See [:material-code-braces: HealthEventsConfigTypeDef](./type_defs.md#healtheventsconfigtypedef) 
3. See [:material-code-braces: CreateMonitorOutputTypeDef](./type_defs.md#createmonitoroutputtypedef) 


```python
# create_monitor method usage example with argument unpacking

kwargs: CreateMonitorInputRequestTypeDef = {  # (1)
    "MonitorName": ...,
}

parent.create_monitor(**kwargs)
```

1. See [:material-code-braces: CreateMonitorInputRequestTypeDef](./type_defs.md#createmonitorinputrequesttypedef) 

### delete\_monitor

Deletes a monitor in Amazon CloudWatch Internet Monitor.

Type annotations and code completion for `#!python session.client("internetmonitor").delete_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# delete_monitor method definition

await def delete_monitor(
    self,
    *,
    MonitorName: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_monitor method usage example with argument unpacking

kwargs: DeleteMonitorInputRequestTypeDef = {  # (1)
    "MonitorName": ...,
}

parent.delete_monitor(**kwargs)
```

1. See [:material-code-braces: DeleteMonitorInputRequestTypeDef](./type_defs.md#deletemonitorinputrequesttypedef) 

### get\_health\_event

Gets information that Amazon CloudWatch Internet Monitor has created and stored
about a health event for a specified monitor.

Type annotations and code completion for `#!python session.client("internetmonitor").get_health_event` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# get_health_event method definition

await def get_health_event(
    self,
    *,
    MonitorName: str,
    EventId: str,
    LinkedAccountId: str = ...,
) -> GetHealthEventOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetHealthEventOutputTypeDef](./type_defs.md#gethealtheventoutputtypedef) 


```python
# get_health_event method usage example with argument unpacking

kwargs: GetHealthEventInputRequestTypeDef = {  # (1)
    "MonitorName": ...,
    "EventId": ...,
}

parent.get_health_event(**kwargs)
```

1. See [:material-code-braces: GetHealthEventInputRequestTypeDef](./type_defs.md#gethealtheventinputrequesttypedef) 

### get\_internet\_event

Gets information that Amazon CloudWatch Internet Monitor has generated about an
internet event.

Type annotations and code completion for `#!python session.client("internetmonitor").get_internet_event` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# get_internet_event method definition

await def get_internet_event(
    self,
    *,
    EventId: str,
) -> GetInternetEventOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInternetEventOutputTypeDef](./type_defs.md#getinterneteventoutputtypedef) 


```python
# get_internet_event method usage example with argument unpacking

kwargs: GetInternetEventInputRequestTypeDef = {  # (1)
    "EventId": ...,
}

parent.get_internet_event(**kwargs)
```

1. See [:material-code-braces: GetInternetEventInputRequestTypeDef](./type_defs.md#getinterneteventinputrequesttypedef) 

### get\_monitor

Gets information about a monitor in Amazon CloudWatch Internet Monitor based on
a monitor name.

Type annotations and code completion for `#!python session.client("internetmonitor").get_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# get_monitor method definition

await def get_monitor(
    self,
    *,
    MonitorName: str,
    LinkedAccountId: str = ...,
) -> GetMonitorOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMonitorOutputTypeDef](./type_defs.md#getmonitoroutputtypedef) 


```python
# get_monitor method usage example with argument unpacking

kwargs: GetMonitorInputRequestTypeDef = {  # (1)
    "MonitorName": ...,
}

parent.get_monitor(**kwargs)
```

1. See [:material-code-braces: GetMonitorInputRequestTypeDef](./type_defs.md#getmonitorinputrequesttypedef) 

### get\_query\_results

Return the data for a query with the Amazon CloudWatch Internet Monitor query
interface.

Type annotations and code completion for `#!python session.client("internetmonitor").get_query_results` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# get_query_results method definition

await def get_query_results(
    self,
    *,
    MonitorName: str,
    QueryId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetQueryResultsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQueryResultsOutputTypeDef](./type_defs.md#getqueryresultsoutputtypedef) 


```python
# get_query_results method usage example with argument unpacking

kwargs: GetQueryResultsInputRequestTypeDef = {  # (1)
    "MonitorName": ...,
    "QueryId": ...,
}

parent.get_query_results(**kwargs)
```

1. See [:material-code-braces: GetQueryResultsInputRequestTypeDef](./type_defs.md#getqueryresultsinputrequesttypedef) 

### get\_query\_status

Returns the current status of a query for the Amazon CloudWatch Internet
Monitor query interface, for a specified query ID and monitor.

Type annotations and code completion for `#!python session.client("internetmonitor").get_query_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# get_query_status method definition

await def get_query_status(
    self,
    *,
    MonitorName: str,
    QueryId: str,
) -> GetQueryStatusOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQueryStatusOutputTypeDef](./type_defs.md#getquerystatusoutputtypedef) 


```python
# get_query_status method usage example with argument unpacking

kwargs: GetQueryStatusInputRequestTypeDef = {  # (1)
    "MonitorName": ...,
    "QueryId": ...,
}

parent.get_query_status(**kwargs)
```

1. See [:material-code-braces: GetQueryStatusInputRequestTypeDef](./type_defs.md#getquerystatusinputrequesttypedef) 

### list\_health\_events

Lists all health events for a monitor in Amazon CloudWatch Internet Monitor.

Type annotations and code completion for `#!python session.client("internetmonitor").list_health_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# list_health_events method definition

await def list_health_events(
    self,
    *,
    MonitorName: str,
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    EventStatus: HealthEventStatusType = ...,  # (1)
    LinkedAccountId: str = ...,
) -> ListHealthEventsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: HealthEventStatusType](./literals.md#healtheventstatustype) 
2. See [:material-code-braces: ListHealthEventsOutputTypeDef](./type_defs.md#listhealtheventsoutputtypedef) 


```python
# list_health_events method usage example with argument unpacking

kwargs: ListHealthEventsInputRequestTypeDef = {  # (1)
    "MonitorName": ...,
}

parent.list_health_events(**kwargs)
```

1. See [:material-code-braces: ListHealthEventsInputRequestTypeDef](./type_defs.md#listhealtheventsinputrequesttypedef) 

### list\_internet\_events

Lists internet events that cause performance or availability issues for client
locations.

Type annotations and code completion for `#!python session.client("internetmonitor").list_internet_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# list_internet_events method definition

await def list_internet_events(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    EventStatus: str = ...,
    EventType: str = ...,
) -> ListInternetEventsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListInternetEventsOutputTypeDef](./type_defs.md#listinterneteventsoutputtypedef) 


```python
# list_internet_events method usage example with argument unpacking

kwargs: ListInternetEventsInputRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_internet_events(**kwargs)
```

1. See [:material-code-braces: ListInternetEventsInputRequestTypeDef](./type_defs.md#listinterneteventsinputrequesttypedef) 

### list\_monitors

Lists all of your monitors for Amazon CloudWatch Internet Monitor and their
statuses, along with the Amazon Resource Name (ARN) and name of each monitor.

Type annotations and code completion for `#!python session.client("internetmonitor").list_monitors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# list_monitors method definition

await def list_monitors(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    MonitorStatus: str = ...,
    IncludeLinkedAccounts: bool = ...,
) -> ListMonitorsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMonitorsOutputTypeDef](./type_defs.md#listmonitorsoutputtypedef) 


```python
# list_monitors method usage example with argument unpacking

kwargs: ListMonitorsInputRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_monitors(**kwargs)
```

1. See [:material-code-braces: ListMonitorsInputRequestTypeDef](./type_defs.md#listmonitorsinputrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags for a resource.

Type annotations and code completion for `#!python session.client("internetmonitor").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef) 

### start\_query

Start a query to return data for a specific query type for the Amazon
CloudWatch Internet Monitor query interface.

Type annotations and code completion for `#!python session.client("internetmonitor").start_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# start_query method definition

await def start_query(
    self,
    *,
    MonitorName: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    QueryType: QueryTypeType,  # (1)
    FilterParameters: Sequence[FilterParameterTypeDef] = ...,  # (2)
    LinkedAccountId: str = ...,
) -> StartQueryOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: QueryTypeType](./literals.md#querytypetype) 
2. See [:material-code-braces: FilterParameterTypeDef](./type_defs.md#filterparametertypedef) 
3. See [:material-code-braces: StartQueryOutputTypeDef](./type_defs.md#startqueryoutputtypedef) 


```python
# start_query method usage example with argument unpacking

kwargs: StartQueryInputRequestTypeDef = {  # (1)
    "MonitorName": ...,
    "StartTime": ...,
    "EndTime": ...,
    "QueryType": ...,
}

parent.start_query(**kwargs)
```

1. See [:material-code-braces: StartQueryInputRequestTypeDef](./type_defs.md#startqueryinputrequesttypedef) 

### stop\_query

Stop a query that is progress for a specific monitor.

Type annotations and code completion for `#!python session.client("internetmonitor").stop_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# stop_query method definition

await def stop_query(
    self,
    *,
    MonitorName: str,
    QueryId: str,
) -> dict[str, Any]:
    ...
```



```python
# stop_query method usage example with argument unpacking

kwargs: StopQueryInputRequestTypeDef = {  # (1)
    "MonitorName": ...,
    "QueryId": ...,
}

parent.stop_query(**kwargs)
```

1. See [:material-code-braces: StopQueryInputRequestTypeDef](./type_defs.md#stopqueryinputrequesttypedef) 

### tag\_resource

Adds a tag to a resource.

Type annotations and code completion for `#!python session.client("internetmonitor").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef) 

### untag\_resource

Removes a tag from a resource.

Type annotations and code completion for `#!python session.client("internetmonitor").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceInputRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef) 

### update\_monitor

Updates a monitor.

Type annotations and code completion for `#!python session.client("internetmonitor").update_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# update_monitor method definition

await def update_monitor(
    self,
    *,
    MonitorName: str,
    ResourcesToAdd: Sequence[str] = ...,
    ResourcesToRemove: Sequence[str] = ...,
    Status: MonitorConfigStateType = ...,  # (1)
    ClientToken: str = ...,
    MaxCityNetworksToMonitor: int = ...,
    InternetMeasurementsLogDelivery: InternetMeasurementsLogDeliveryTypeDef = ...,  # (2)
    TrafficPercentageToMonitor: int = ...,
    HealthEventsConfig: HealthEventsConfigTypeDef = ...,  # (3)
) -> UpdateMonitorOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: MonitorConfigStateType](./literals.md#monitorconfigstatetype) 
2. See [:material-code-braces: InternetMeasurementsLogDeliveryTypeDef](./type_defs.md#internetmeasurementslogdeliverytypedef) 
3. See [:material-code-braces: HealthEventsConfigTypeDef](./type_defs.md#healtheventsconfigtypedef) 
4. See [:material-code-braces: UpdateMonitorOutputTypeDef](./type_defs.md#updatemonitoroutputtypedef) 


```python
# update_monitor method usage example with argument unpacking

kwargs: UpdateMonitorInputRequestTypeDef = {  # (1)
    "MonitorName": ...,
}

parent.update_monitor(**kwargs)
```

1. See [:material-code-braces: UpdateMonitorInputRequestTypeDef](./type_defs.md#updatemonitorinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("internetmonitor").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("internetmonitor").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

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

Type annotations and code completion for `#!python session.client("internetmonitor").get_paginator` method with overloads.

- `client.get_paginator("list_health_events")` -> [ListHealthEventsPaginator](./paginators.md#listhealtheventspaginator)
- `client.get_paginator("list_internet_events")` -> [ListInternetEventsPaginator](./paginators.md#listinterneteventspaginator)
- `client.get_paginator("list_monitors")` -> [ListMonitorsPaginator](./paginators.md#listmonitorspaginator)


