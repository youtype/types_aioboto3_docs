# CloudWatchNetworkMonitorClient

> [Index](../README.md) > [CloudWatchNetworkMonitor](./README.md) > CloudWatchNetworkMonitorClient

!!! note ""

    Auto-generated documentation for [CloudWatchNetworkMonitor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#cloudwatchnetworkmonitor)
    type annotations stubs module [types-aiobotocore-networkmonitor](https://pypi.org/project/types-aiobotocore-networkmonitor/).

## CloudWatchNetworkMonitorClient

Type annotations and code completion for `#!python session.client("networkmonitor")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client)

```python
# CloudWatchNetworkMonitorClient usage example

from aioboto3.session import Session
from types_aiobotocore_networkmonitor.client import CloudWatchNetworkMonitorClient

session = Session()
async with session.client("networkmonitor") as client:
    client: CloudWatchNetworkMonitorClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("networkmonitor").exceptions` structure.

```python
# CloudWatchNetworkMonitorClient.exceptions usage example

async with session.client("networkmonitor") as client:
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
# CloudWatchNetworkMonitorClient.exceptions type checking example

from types_aiobotocore_networkmonitor.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("networkmonitor").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("networkmonitor").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client)

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

Creates a monitor between a source subnet and destination IP address.

Type annotations and code completion for `#!python session.client("networkmonitor").create_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client)

```python
# create_monitor method definition

await def create_monitor(
    self,
    *,
    monitorName: str,
    probes: Sequence[CreateMonitorProbeInputTypeDef] = ...,  # (1)
    aggregationPeriod: int = ...,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateMonitorOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CreateMonitorProbeInputTypeDef](./type_defs.md#createmonitorprobeinputtypedef) 
2. See [:material-code-braces: CreateMonitorOutputTypeDef](./type_defs.md#createmonitoroutputtypedef) 


```python
# create_monitor method usage example with argument unpacking

kwargs: CreateMonitorInputRequestTypeDef = {  # (1)
    "monitorName": ...,
}

parent.create_monitor(**kwargs)
```

1. See [:material-code-braces: CreateMonitorInputRequestTypeDef](./type_defs.md#createmonitorinputrequesttypedef) 

### create\_probe

Create a probe within a monitor.

Type annotations and code completion for `#!python session.client("networkmonitor").create_probe` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client)

```python
# create_probe method definition

await def create_probe(
    self,
    *,
    monitorName: str,
    probe: ProbeInputTypeDef,  # (1)
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateProbeOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ProbeInputTypeDef](./type_defs.md#probeinputtypedef) 
2. See [:material-code-braces: CreateProbeOutputTypeDef](./type_defs.md#createprobeoutputtypedef) 


```python
# create_probe method usage example with argument unpacking

kwargs: CreateProbeInputRequestTypeDef = {  # (1)
    "monitorName": ...,
    "probe": ...,
}

parent.create_probe(**kwargs)
```

1. See [:material-code-braces: CreateProbeInputRequestTypeDef](./type_defs.md#createprobeinputrequesttypedef) 

### delete\_monitor

Deletes a specified monitor.

Type annotations and code completion for `#!python session.client("networkmonitor").delete_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client)

```python
# delete_monitor method definition

await def delete_monitor(
    self,
    *,
    monitorName: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_monitor method usage example with argument unpacking

kwargs: DeleteMonitorInputRequestTypeDef = {  # (1)
    "monitorName": ...,
}

parent.delete_monitor(**kwargs)
```

1. See [:material-code-braces: DeleteMonitorInputRequestTypeDef](./type_defs.md#deletemonitorinputrequesttypedef) 

### delete\_probe

Deletes the specified probe.

Type annotations and code completion for `#!python session.client("networkmonitor").delete_probe` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client)

```python
# delete_probe method definition

await def delete_probe(
    self,
    *,
    monitorName: str,
    probeId: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_probe method usage example with argument unpacking

kwargs: DeleteProbeInputRequestTypeDef = {  # (1)
    "monitorName": ...,
    "probeId": ...,
}

parent.delete_probe(**kwargs)
```

1. See [:material-code-braces: DeleteProbeInputRequestTypeDef](./type_defs.md#deleteprobeinputrequesttypedef) 

### get\_monitor

Returns details about a specific monitor.

Type annotations and code completion for `#!python session.client("networkmonitor").get_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client)

```python
# get_monitor method definition

await def get_monitor(
    self,
    *,
    monitorName: str,
) -> GetMonitorOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMonitorOutputTypeDef](./type_defs.md#getmonitoroutputtypedef) 


```python
# get_monitor method usage example with argument unpacking

kwargs: GetMonitorInputRequestTypeDef = {  # (1)
    "monitorName": ...,
}

parent.get_monitor(**kwargs)
```

1. See [:material-code-braces: GetMonitorInputRequestTypeDef](./type_defs.md#getmonitorinputrequesttypedef) 

### get\_probe

Returns the details about a probe.

Type annotations and code completion for `#!python session.client("networkmonitor").get_probe` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client)

```python
# get_probe method definition

await def get_probe(
    self,
    *,
    monitorName: str,
    probeId: str,
) -> GetProbeOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetProbeOutputTypeDef](./type_defs.md#getprobeoutputtypedef) 


```python
# get_probe method usage example with argument unpacking

kwargs: GetProbeInputRequestTypeDef = {  # (1)
    "monitorName": ...,
    "probeId": ...,
}

parent.get_probe(**kwargs)
```

1. See [:material-code-braces: GetProbeInputRequestTypeDef](./type_defs.md#getprobeinputrequesttypedef) 

### list\_monitors

Returns a list of all of your monitors.

Type annotations and code completion for `#!python session.client("networkmonitor").list_monitors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client)

```python
# list_monitors method definition

await def list_monitors(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    state: str = ...,
) -> ListMonitorsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMonitorsOutputTypeDef](./type_defs.md#listmonitorsoutputtypedef) 


```python
# list_monitors method usage example with argument unpacking

kwargs: ListMonitorsInputRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_monitors(**kwargs)
```

1. See [:material-code-braces: ListMonitorsInputRequestTypeDef](./type_defs.md#listmonitorsinputrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags assigned to this resource.

Type annotations and code completion for `#!python session.client("networkmonitor").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef) 

### tag\_resource

Adds key-value pairs to a monitor or probe.

Type annotations and code completion for `#!python session.client("networkmonitor").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client)

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

kwargs: TagResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef) 

### untag\_resource

Removes a key-value pair from a monitor or probe.

Type annotations and code completion for `#!python session.client("networkmonitor").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client)

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

kwargs: UntagResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef) 

### update\_monitor

Updates the <code>aggregationPeriod</code> for a monitor.

Type annotations and code completion for `#!python session.client("networkmonitor").update_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client)

```python
# update_monitor method definition

await def update_monitor(
    self,
    *,
    monitorName: str,
    aggregationPeriod: int,
) -> UpdateMonitorOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateMonitorOutputTypeDef](./type_defs.md#updatemonitoroutputtypedef) 


```python
# update_monitor method usage example with argument unpacking

kwargs: UpdateMonitorInputRequestTypeDef = {  # (1)
    "monitorName": ...,
    "aggregationPeriod": ...,
}

parent.update_monitor(**kwargs)
```

1. See [:material-code-braces: UpdateMonitorInputRequestTypeDef](./type_defs.md#updatemonitorinputrequesttypedef) 

### update\_probe

Updates a monitor probe.

Type annotations and code completion for `#!python session.client("networkmonitor").update_probe` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client)

```python
# update_probe method definition

await def update_probe(
    self,
    *,
    monitorName: str,
    probeId: str,
    state: ProbeStateType = ...,  # (1)
    destination: str = ...,
    destinationPort: int = ...,
    protocol: ProtocolType = ...,  # (2)
    packetSize: int = ...,
) -> UpdateProbeOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ProbeStateType](./literals.md#probestatetype) 
2. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
3. See [:material-code-braces: UpdateProbeOutputTypeDef](./type_defs.md#updateprobeoutputtypedef) 


```python
# update_probe method usage example with argument unpacking

kwargs: UpdateProbeInputRequestTypeDef = {  # (1)
    "monitorName": ...,
    "probeId": ...,
}

parent.update_probe(**kwargs)
```

1. See [:material-code-braces: UpdateProbeInputRequestTypeDef](./type_defs.md#updateprobeinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("networkmonitor").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("networkmonitor").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#CloudWatchNetworkMonitor.Client)

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

Type annotations and code completion for `#!python session.client("networkmonitor").get_paginator` method with overloads.

- `client.get_paginator("list_monitors")` -> [ListMonitorsPaginator](./paginators.md#listmonitorspaginator)


