# IoT1ClickDevicesServiceClient

> [Index](../README.md) > [IoT1ClickDevicesService](./README.md) > IoT1ClickDevicesServiceClient

!!! note ""

    Auto-generated documentation for [IoT1ClickDevicesService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#iot1clickdevicesservice)
    type annotations stubs module [types-aiobotocore-iot1click-devices](https://pypi.org/project/types-aiobotocore-iot1click-devices/).

## IoT1ClickDevicesServiceClient

Type annotations and code completion for `#!python session.client("iot1click-devices")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client)

```python
# IoT1ClickDevicesServiceClient usage example

from aioboto3.session import Session
from types_aiobotocore_iot1click_devices.client import IoT1ClickDevicesServiceClient

session = Session()
async with session.client("iot1click-devices") as client:
    client: IoT1ClickDevicesServiceClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("iot1click-devices").exceptions` structure.

```python
# IoT1ClickDevicesServiceClient.exceptions usage example

async with session.client("iot1click-devices") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.ForbiddenException,
        client.exceptions.InternalFailureException,
        client.exceptions.InvalidRequestException,
        client.exceptions.PreconditionFailedException,
        client.exceptions.RangeNotSatisfiableException,
        client.exceptions.ResourceConflictException,
        client.exceptions.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python
# IoT1ClickDevicesServiceClient.exceptions type checking example

from types_aiobotocore_iot1click_devices.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("iot1click-devices").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("iot1click-devices").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client)

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


### claim\_devices\_by\_claim\_code

Adds device(s) to your account (i.e., claim one or more devices) if and only if
you received a claim code with the device(s).

Type annotations and code completion for `#!python session.client("iot1click-devices").claim_devices_by_claim_code` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client)

```python
# claim_devices_by_claim_code method definition

await def claim_devices_by_claim_code(
    self,
    *,
    ClaimCode: str,
) -> ClaimDevicesByClaimCodeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ClaimDevicesByClaimCodeResponseTypeDef](./type_defs.md#claimdevicesbyclaimcoderesponsetypedef) 


```python
# claim_devices_by_claim_code method usage example with argument unpacking

kwargs: ClaimDevicesByClaimCodeRequestRequestTypeDef = {  # (1)
    "ClaimCode": ...,
}

parent.claim_devices_by_claim_code(**kwargs)
```

1. See [:material-code-braces: ClaimDevicesByClaimCodeRequestRequestTypeDef](./type_defs.md#claimdevicesbyclaimcoderequestrequesttypedef) 

### describe\_device

Given a device ID, returns a DescribeDeviceResponse object describing the
details of the device.

Type annotations and code completion for `#!python session.client("iot1click-devices").describe_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client)

```python
# describe_device method definition

await def describe_device(
    self,
    *,
    DeviceId: str,
) -> DescribeDeviceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDeviceResponseTypeDef](./type_defs.md#describedeviceresponsetypedef) 


```python
# describe_device method usage example with argument unpacking

kwargs: DescribeDeviceRequestRequestTypeDef = {  # (1)
    "DeviceId": ...,
}

parent.describe_device(**kwargs)
```

1. See [:material-code-braces: DescribeDeviceRequestRequestTypeDef](./type_defs.md#describedevicerequestrequesttypedef) 

### finalize\_device\_claim

Given a device ID, finalizes the claim request for the associated device.

Type annotations and code completion for `#!python session.client("iot1click-devices").finalize_device_claim` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client)

```python
# finalize_device_claim method definition

await def finalize_device_claim(
    self,
    *,
    DeviceId: str,
    Tags: Mapping[str, str] = ...,
) -> FinalizeDeviceClaimResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: FinalizeDeviceClaimResponseTypeDef](./type_defs.md#finalizedeviceclaimresponsetypedef) 


```python
# finalize_device_claim method usage example with argument unpacking

kwargs: FinalizeDeviceClaimRequestRequestTypeDef = {  # (1)
    "DeviceId": ...,
}

parent.finalize_device_claim(**kwargs)
```

1. See [:material-code-braces: FinalizeDeviceClaimRequestRequestTypeDef](./type_defs.md#finalizedeviceclaimrequestrequesttypedef) 

### get\_device\_methods

Given a device ID, returns the invokable methods associated with the device.

Type annotations and code completion for `#!python session.client("iot1click-devices").get_device_methods` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client)

```python
# get_device_methods method definition

await def get_device_methods(
    self,
    *,
    DeviceId: str,
) -> GetDeviceMethodsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeviceMethodsResponseTypeDef](./type_defs.md#getdevicemethodsresponsetypedef) 


```python
# get_device_methods method usage example with argument unpacking

kwargs: GetDeviceMethodsRequestRequestTypeDef = {  # (1)
    "DeviceId": ...,
}

parent.get_device_methods(**kwargs)
```

1. See [:material-code-braces: GetDeviceMethodsRequestRequestTypeDef](./type_defs.md#getdevicemethodsrequestrequesttypedef) 

### initiate\_device\_claim

Given a device ID, initiates a claim request for the associated device.

Type annotations and code completion for `#!python session.client("iot1click-devices").initiate_device_claim` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client)

```python
# initiate_device_claim method definition

await def initiate_device_claim(
    self,
    *,
    DeviceId: str,
) -> InitiateDeviceClaimResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: InitiateDeviceClaimResponseTypeDef](./type_defs.md#initiatedeviceclaimresponsetypedef) 


```python
# initiate_device_claim method usage example with argument unpacking

kwargs: InitiateDeviceClaimRequestRequestTypeDef = {  # (1)
    "DeviceId": ...,
}

parent.initiate_device_claim(**kwargs)
```

1. See [:material-code-braces: InitiateDeviceClaimRequestRequestTypeDef](./type_defs.md#initiatedeviceclaimrequestrequesttypedef) 

### invoke\_device\_method

Given a device ID, issues a request to invoke a named device method (with
possible parameters).

Type annotations and code completion for `#!python session.client("iot1click-devices").invoke_device_method` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client)

```python
# invoke_device_method method definition

await def invoke_device_method(
    self,
    *,
    DeviceId: str,
    DeviceMethod: DeviceMethodTypeDef = ...,  # (1)
    DeviceMethodParameters: str = ...,
) -> InvokeDeviceMethodResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DeviceMethodTypeDef](./type_defs.md#devicemethodtypedef) 
2. See [:material-code-braces: InvokeDeviceMethodResponseTypeDef](./type_defs.md#invokedevicemethodresponsetypedef) 


```python
# invoke_device_method method usage example with argument unpacking

kwargs: InvokeDeviceMethodRequestRequestTypeDef = {  # (1)
    "DeviceId": ...,
}

parent.invoke_device_method(**kwargs)
```

1. See [:material-code-braces: InvokeDeviceMethodRequestRequestTypeDef](./type_defs.md#invokedevicemethodrequestrequesttypedef) 

### list\_device\_events

Using a device ID, returns a DeviceEventsResponse object containing an array of
events for the device.

Type annotations and code completion for `#!python session.client("iot1click-devices").list_device_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client)

```python
# list_device_events method definition

await def list_device_events(
    self,
    *,
    DeviceId: str,
    FromTimeStamp: TimestampTypeDef,
    ToTimeStamp: TimestampTypeDef,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListDeviceEventsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDeviceEventsResponseTypeDef](./type_defs.md#listdeviceeventsresponsetypedef) 


```python
# list_device_events method usage example with argument unpacking

kwargs: ListDeviceEventsRequestRequestTypeDef = {  # (1)
    "DeviceId": ...,
    "FromTimeStamp": ...,
    "ToTimeStamp": ...,
}

parent.list_device_events(**kwargs)
```

1. See [:material-code-braces: ListDeviceEventsRequestRequestTypeDef](./type_defs.md#listdeviceeventsrequestrequesttypedef) 

### list\_devices

Lists the 1-Click compatible devices associated with your AWS account.

Type annotations and code completion for `#!python session.client("iot1click-devices").list_devices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client)

```python
# list_devices method definition

await def list_devices(
    self,
    *,
    DeviceType: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListDevicesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef) 


```python
# list_devices method usage example with argument unpacking

kwargs: ListDevicesRequestRequestTypeDef = {  # (1)
    "DeviceType": ...,
}

parent.list_devices(**kwargs)
```

1. See [:material-code-braces: ListDevicesRequestRequestTypeDef](./type_defs.md#listdevicesrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags associated with the specified resource ARN.

Type annotations and code completion for `#!python session.client("iot1click-devices").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client)

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

### tag\_resource

Adds or updates the tags associated with the resource ARN.

Type annotations and code completion for `#!python session.client("iot1click-devices").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### unclaim\_device

Disassociates a device from your AWS account using its device ID.

Type annotations and code completion for `#!python session.client("iot1click-devices").unclaim_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client)

```python
# unclaim_device method definition

await def unclaim_device(
    self,
    *,
    DeviceId: str,
) -> UnclaimDeviceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UnclaimDeviceResponseTypeDef](./type_defs.md#unclaimdeviceresponsetypedef) 


```python
# unclaim_device method usage example with argument unpacking

kwargs: UnclaimDeviceRequestRequestTypeDef = {  # (1)
    "DeviceId": ...,
}

parent.unclaim_device(**kwargs)
```

1. See [:material-code-braces: UnclaimDeviceRequestRequestTypeDef](./type_defs.md#unclaimdevicerequestrequesttypedef) 

### untag\_resource

Using tag keys, deletes the tags (key/value pairs) associated with the
specified resource ARN.

Type annotations and code completion for `#!python session.client("iot1click-devices").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_device\_state

Using a Boolean value (true or false), this operation enables or disables the
device given a device ID.

Type annotations and code completion for `#!python session.client("iot1click-devices").update_device_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client)

```python
# update_device_state method definition

await def update_device_state(
    self,
    *,
    DeviceId: str,
    Enabled: bool = ...,
) -> dict[str, Any]:
    ...
```



```python
# update_device_state method usage example with argument unpacking

kwargs: UpdateDeviceStateRequestRequestTypeDef = {  # (1)
    "DeviceId": ...,
}

parent.update_device_state(**kwargs)
```

1. See [:material-code-braces: UpdateDeviceStateRequestRequestTypeDef](./type_defs.md#updatedevicestaterequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("iot1click-devices").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("iot1click-devices").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client)

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

Type annotations and code completion for `#!python session.client("iot1click-devices").get_paginator` method with overloads.

- `client.get_paginator("list_device_events")` -> [ListDeviceEventsPaginator](./paginators.md#listdeviceeventspaginator)
- `client.get_paginator("list_devices")` -> [ListDevicesPaginator](./paginators.md#listdevicespaginator)


