# CloudWatchRUMClient

> [Index](../README.md) > [CloudWatchRUM](./README.md) > CloudWatchRUMClient

!!! note ""

    Auto-generated documentation for [CloudWatchRUM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#cloudwatchrum)
    type annotations stubs module [types-aiobotocore-rum](https://pypi.org/project/types-aiobotocore-rum/).

## CloudWatchRUMClient

Type annotations and code completion for `#!python session.client("rum")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

```python
# CloudWatchRUMClient usage example

from aioboto3.session import Session
from types_aiobotocore_rum.client import CloudWatchRUMClient

session = Session()
async with session.client("rum") as client:
    client: CloudWatchRUMClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("rum").exceptions` structure.

```python
# CloudWatchRUMClient.exceptions usage example

async with session.client("rum") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# CloudWatchRUMClient.exceptions type checking example

from types_aiobotocore_rum.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("rum").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("rum").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

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


### batch\_create\_rum\_metric\_definitions

Specifies the extended metrics and custom metrics that you want a CloudWatch
RUM app monitor to send to a destination.

Type annotations and code completion for `#!python session.client("rum").batch_create_rum_metric_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

```python
# batch_create_rum_metric_definitions method definition

await def batch_create_rum_metric_definitions(
    self,
    *,
    AppMonitorName: str,
    Destination: MetricDestinationType,  # (1)
    MetricDefinitions: Sequence[MetricDefinitionRequestUnionTypeDef],  # (2)
    DestinationArn: str = ...,
) -> BatchCreateRumMetricDefinitionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: MetricDestinationType](./literals.md#metricdestinationtype) 
2. See [:material-code-braces: MetricDefinitionRequestTypeDef](./type_defs.md#metricdefinitionrequesttypedef) [:material-code-braces: MetricDefinitionRequestOutputTypeDef](./type_defs.md#metricdefinitionrequestoutputtypedef) 
3. See [:material-code-braces: BatchCreateRumMetricDefinitionsResponseTypeDef](./type_defs.md#batchcreaterummetricdefinitionsresponsetypedef) 


```python
# batch_create_rum_metric_definitions method usage example with argument unpacking

kwargs: BatchCreateRumMetricDefinitionsRequestRequestTypeDef = {  # (1)
    "AppMonitorName": ...,
    "Destination": ...,
    "MetricDefinitions": ...,
}

parent.batch_create_rum_metric_definitions(**kwargs)
```

1. See [:material-code-braces: BatchCreateRumMetricDefinitionsRequestRequestTypeDef](./type_defs.md#batchcreaterummetricdefinitionsrequestrequesttypedef) 

### batch\_delete\_rum\_metric\_definitions

Removes the specified metrics from being sent to an extended metrics
destination.

Type annotations and code completion for `#!python session.client("rum").batch_delete_rum_metric_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

```python
# batch_delete_rum_metric_definitions method definition

await def batch_delete_rum_metric_definitions(
    self,
    *,
    AppMonitorName: str,
    Destination: MetricDestinationType,  # (1)
    MetricDefinitionIds: Sequence[str],
    DestinationArn: str = ...,
) -> BatchDeleteRumMetricDefinitionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MetricDestinationType](./literals.md#metricdestinationtype) 
2. See [:material-code-braces: BatchDeleteRumMetricDefinitionsResponseTypeDef](./type_defs.md#batchdeleterummetricdefinitionsresponsetypedef) 


```python
# batch_delete_rum_metric_definitions method usage example with argument unpacking

kwargs: BatchDeleteRumMetricDefinitionsRequestRequestTypeDef = {  # (1)
    "AppMonitorName": ...,
    "Destination": ...,
    "MetricDefinitionIds": ...,
}

parent.batch_delete_rum_metric_definitions(**kwargs)
```

1. See [:material-code-braces: BatchDeleteRumMetricDefinitionsRequestRequestTypeDef](./type_defs.md#batchdeleterummetricdefinitionsrequestrequesttypedef) 

### batch\_get\_rum\_metric\_definitions

Retrieves the list of metrics and dimensions that a RUM app monitor is sending
to a single destination.

Type annotations and code completion for `#!python session.client("rum").batch_get_rum_metric_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

```python
# batch_get_rum_metric_definitions method definition

await def batch_get_rum_metric_definitions(
    self,
    *,
    AppMonitorName: str,
    Destination: MetricDestinationType,  # (1)
    DestinationArn: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> BatchGetRumMetricDefinitionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MetricDestinationType](./literals.md#metricdestinationtype) 
2. See [:material-code-braces: BatchGetRumMetricDefinitionsResponseTypeDef](./type_defs.md#batchgetrummetricdefinitionsresponsetypedef) 


```python
# batch_get_rum_metric_definitions method usage example with argument unpacking

kwargs: BatchGetRumMetricDefinitionsRequestRequestTypeDef = {  # (1)
    "AppMonitorName": ...,
    "Destination": ...,
}

parent.batch_get_rum_metric_definitions(**kwargs)
```

1. See [:material-code-braces: BatchGetRumMetricDefinitionsRequestRequestTypeDef](./type_defs.md#batchgetrummetricdefinitionsrequestrequesttypedef) 

### create\_app\_monitor

Creates a Amazon CloudWatch RUM app monitor, which collects telemetry data from
your application and sends that data to RUM.

Type annotations and code completion for `#!python session.client("rum").create_app_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

```python
# create_app_monitor method definition

await def create_app_monitor(
    self,
    *,
    Domain: str,
    Name: str,
    AppMonitorConfiguration: AppMonitorConfigurationTypeDef = ...,  # (1)
    CustomEvents: CustomEventsTypeDef = ...,  # (2)
    CwLogEnabled: bool = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateAppMonitorResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AppMonitorConfigurationTypeDef](./type_defs.md#appmonitorconfigurationtypedef) 
2. See [:material-code-braces: CustomEventsTypeDef](./type_defs.md#customeventstypedef) 
3. See [:material-code-braces: CreateAppMonitorResponseTypeDef](./type_defs.md#createappmonitorresponsetypedef) 


```python
# create_app_monitor method usage example with argument unpacking

kwargs: CreateAppMonitorRequestRequestTypeDef = {  # (1)
    "Domain": ...,
    "Name": ...,
}

parent.create_app_monitor(**kwargs)
```

1. See [:material-code-braces: CreateAppMonitorRequestRequestTypeDef](./type_defs.md#createappmonitorrequestrequesttypedef) 

### delete\_app\_monitor

Deletes an existing app monitor.

Type annotations and code completion for `#!python session.client("rum").delete_app_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

```python
# delete_app_monitor method definition

await def delete_app_monitor(
    self,
    *,
    Name: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_app_monitor method usage example with argument unpacking

kwargs: DeleteAppMonitorRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_app_monitor(**kwargs)
```

1. See [:material-code-braces: DeleteAppMonitorRequestRequestTypeDef](./type_defs.md#deleteappmonitorrequestrequesttypedef) 

### delete\_rum\_metrics\_destination

Deletes a destination for CloudWatch RUM extended metrics, so that the
specified app monitor stops sending extended metrics to that destination.

Type annotations and code completion for `#!python session.client("rum").delete_rum_metrics_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

```python
# delete_rum_metrics_destination method definition

await def delete_rum_metrics_destination(
    self,
    *,
    AppMonitorName: str,
    Destination: MetricDestinationType,  # (1)
    DestinationArn: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: MetricDestinationType](./literals.md#metricdestinationtype) 


```python
# delete_rum_metrics_destination method usage example with argument unpacking

kwargs: DeleteRumMetricsDestinationRequestRequestTypeDef = {  # (1)
    "AppMonitorName": ...,
    "Destination": ...,
}

parent.delete_rum_metrics_destination(**kwargs)
```

1. See [:material-code-braces: DeleteRumMetricsDestinationRequestRequestTypeDef](./type_defs.md#deleterummetricsdestinationrequestrequesttypedef) 

### get\_app\_monitor

Retrieves the complete configuration information for one app monitor.

Type annotations and code completion for `#!python session.client("rum").get_app_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

```python
# get_app_monitor method definition

await def get_app_monitor(
    self,
    *,
    Name: str,
) -> GetAppMonitorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAppMonitorResponseTypeDef](./type_defs.md#getappmonitorresponsetypedef) 


```python
# get_app_monitor method usage example with argument unpacking

kwargs: GetAppMonitorRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_app_monitor(**kwargs)
```

1. See [:material-code-braces: GetAppMonitorRequestRequestTypeDef](./type_defs.md#getappmonitorrequestrequesttypedef) 

### get\_app\_monitor\_data

Retrieves the raw performance events that RUM has collected from your web
application, so that you can do your own processing or analysis of this data.

Type annotations and code completion for `#!python session.client("rum").get_app_monitor_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

```python
# get_app_monitor_data method definition

await def get_app_monitor_data(
    self,
    *,
    Name: str,
    TimeRange: TimeRangeTypeDef,  # (1)
    Filters: Sequence[QueryFilterTypeDef] = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetAppMonitorDataResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
2. See [:material-code-braces: QueryFilterTypeDef](./type_defs.md#queryfiltertypedef) 
3. See [:material-code-braces: GetAppMonitorDataResponseTypeDef](./type_defs.md#getappmonitordataresponsetypedef) 


```python
# get_app_monitor_data method usage example with argument unpacking

kwargs: GetAppMonitorDataRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "TimeRange": ...,
}

parent.get_app_monitor_data(**kwargs)
```

1. See [:material-code-braces: GetAppMonitorDataRequestRequestTypeDef](./type_defs.md#getappmonitordatarequestrequesttypedef) 

### list\_app\_monitors

Returns a list of the Amazon CloudWatch RUM app monitors in the account.

Type annotations and code completion for `#!python session.client("rum").list_app_monitors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

```python
# list_app_monitors method definition

await def list_app_monitors(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAppMonitorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAppMonitorsResponseTypeDef](./type_defs.md#listappmonitorsresponsetypedef) 


```python
# list_app_monitors method usage example with argument unpacking

kwargs: ListAppMonitorsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_app_monitors(**kwargs)
```

1. See [:material-code-braces: ListAppMonitorsRequestRequestTypeDef](./type_defs.md#listappmonitorsrequestrequesttypedef) 

### list\_rum\_metrics\_destinations

Returns a list of destinations that you have created to receive RUM extended
metrics, for the specified app monitor.

Type annotations and code completion for `#!python session.client("rum").list_rum_metrics_destinations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

```python
# list_rum_metrics_destinations method definition

await def list_rum_metrics_destinations(
    self,
    *,
    AppMonitorName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListRumMetricsDestinationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRumMetricsDestinationsResponseTypeDef](./type_defs.md#listrummetricsdestinationsresponsetypedef) 


```python
# list_rum_metrics_destinations method usage example with argument unpacking

kwargs: ListRumMetricsDestinationsRequestRequestTypeDef = {  # (1)
    "AppMonitorName": ...,
}

parent.list_rum_metrics_destinations(**kwargs)
```

1. See [:material-code-braces: ListRumMetricsDestinationsRequestRequestTypeDef](./type_defs.md#listrummetricsdestinationsrequestrequesttypedef) 

### list\_tags\_for\_resource

Displays the tags associated with a CloudWatch RUM resource.

Type annotations and code completion for `#!python session.client("rum").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### put\_rum\_events

Sends telemetry events about your application performance and user behavior to
CloudWatch RUM.

Type annotations and code completion for `#!python session.client("rum").put_rum_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

```python
# put_rum_events method definition

await def put_rum_events(
    self,
    *,
    AppMonitorDetails: AppMonitorDetailsTypeDef,  # (1)
    BatchId: str,
    Id: str,
    RumEvents: Sequence[RumEventTypeDef],  # (2)
    UserDetails: UserDetailsTypeDef,  # (3)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: AppMonitorDetailsTypeDef](./type_defs.md#appmonitordetailstypedef) 
2. See [:material-code-braces: RumEventTypeDef](./type_defs.md#rumeventtypedef) 
3. See [:material-code-braces: UserDetailsTypeDef](./type_defs.md#userdetailstypedef) 


```python
# put_rum_events method usage example with argument unpacking

kwargs: PutRumEventsRequestRequestTypeDef = {  # (1)
    "AppMonitorDetails": ...,
    "BatchId": ...,
    "Id": ...,
    "RumEvents": ...,
    "UserDetails": ...,
}

parent.put_rum_events(**kwargs)
```

1. See [:material-code-braces: PutRumEventsRequestRequestTypeDef](./type_defs.md#putrumeventsrequestrequesttypedef) 

### put\_rum\_metrics\_destination

Creates or updates a destination to receive extended metrics from CloudWatch
RUM.

Type annotations and code completion for `#!python session.client("rum").put_rum_metrics_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

```python
# put_rum_metrics_destination method definition

await def put_rum_metrics_destination(
    self,
    *,
    AppMonitorName: str,
    Destination: MetricDestinationType,  # (1)
    DestinationArn: str = ...,
    IamRoleArn: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: MetricDestinationType](./literals.md#metricdestinationtype) 


```python
# put_rum_metrics_destination method usage example with argument unpacking

kwargs: PutRumMetricsDestinationRequestRequestTypeDef = {  # (1)
    "AppMonitorName": ...,
    "Destination": ...,
}

parent.put_rum_metrics_destination(**kwargs)
```

1. See [:material-code-braces: PutRumMetricsDestinationRequestRequestTypeDef](./type_defs.md#putrummetricsdestinationrequestrequesttypedef) 

### tag\_resource

Assigns one or more tags (key-value pairs) to the specified CloudWatch RUM
resource.

Type annotations and code completion for `#!python session.client("rum").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

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

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes one or more tags from the specified resource.

Type annotations and code completion for `#!python session.client("rum").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

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

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_app\_monitor

Updates the configuration of an existing app monitor.

Type annotations and code completion for `#!python session.client("rum").update_app_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

```python
# update_app_monitor method definition

await def update_app_monitor(
    self,
    *,
    Name: str,
    AppMonitorConfiguration: AppMonitorConfigurationTypeDef = ...,  # (1)
    CustomEvents: CustomEventsTypeDef = ...,  # (2)
    CwLogEnabled: bool = ...,
    Domain: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: AppMonitorConfigurationTypeDef](./type_defs.md#appmonitorconfigurationtypedef) 
2. See [:material-code-braces: CustomEventsTypeDef](./type_defs.md#customeventstypedef) 


```python
# update_app_monitor method usage example with argument unpacking

kwargs: UpdateAppMonitorRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.update_app_monitor(**kwargs)
```

1. See [:material-code-braces: UpdateAppMonitorRequestRequestTypeDef](./type_defs.md#updateappmonitorrequestrequesttypedef) 

### update\_rum\_metric\_definition

Modifies one existing metric definition for CloudWatch RUM extended metrics.

Type annotations and code completion for `#!python session.client("rum").update_rum_metric_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

```python
# update_rum_metric_definition method definition

await def update_rum_metric_definition(
    self,
    *,
    AppMonitorName: str,
    Destination: MetricDestinationType,  # (1)
    MetricDefinition: MetricDefinitionRequestTypeDef,  # (2)
    MetricDefinitionId: str,
    DestinationArn: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: MetricDestinationType](./literals.md#metricdestinationtype) 
2. See [:material-code-braces: MetricDefinitionRequestTypeDef](./type_defs.md#metricdefinitionrequesttypedef) 


```python
# update_rum_metric_definition method usage example with argument unpacking

kwargs: UpdateRumMetricDefinitionRequestRequestTypeDef = {  # (1)
    "AppMonitorName": ...,
    "Destination": ...,
    "MetricDefinition": ...,
    "MetricDefinitionId": ...,
}

parent.update_rum_metric_definition(**kwargs)
```

1. See [:material-code-braces: UpdateRumMetricDefinitionRequestRequestTypeDef](./type_defs.md#updaterummetricdefinitionrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("rum").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("rum").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

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

Type annotations and code completion for `#!python session.client("rum").get_paginator` method with overloads.

- `client.get_paginator("batch_get_rum_metric_definitions")` -> [BatchGetRumMetricDefinitionsPaginator](./paginators.md#batchgetrummetricdefinitionspaginator)
- `client.get_paginator("get_app_monitor_data")` -> [GetAppMonitorDataPaginator](./paginators.md#getappmonitordatapaginator)
- `client.get_paginator("list_app_monitors")` -> [ListAppMonitorsPaginator](./paginators.md#listappmonitorspaginator)
- `client.get_paginator("list_rum_metrics_destinations")` -> [ListRumMetricsDestinationsPaginator](./paginators.md#listrummetricsdestinationspaginator)


