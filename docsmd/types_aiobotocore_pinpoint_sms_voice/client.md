# PinpointSMSVoiceClient

> [Index](../README.md) > [PinpointSMSVoice](./README.md) > PinpointSMSVoiceClient

!!! note ""

    Auto-generated documentation for [PinpointSMSVoice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#pinpointsmsvoice)
    type annotations stubs module [types-aiobotocore-pinpoint-sms-voice](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice/).

## PinpointSMSVoiceClient

Type annotations and code completion for `#!python session.client("pinpoint-sms-voice")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client)

```python
# PinpointSMSVoiceClient usage example

from aioboto3.session import Session
from types_aiobotocore_pinpoint_sms_voice.client import PinpointSMSVoiceClient

session = Session()
async with session.client("pinpoint-sms-voice") as client:
    client: PinpointSMSVoiceClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("pinpoint-sms-voice").exceptions` structure.

```python
# PinpointSMSVoiceClient.exceptions usage example

async with session.client("pinpoint-sms-voice") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AlreadyExistsException,
        client.exceptions.BadRequestException,
        client.exceptions.ClientError,
        client.exceptions.InternalServiceErrorException,
        client.exceptions.LimitExceededException,
        client.exceptions.NotFoundException,
        client.exceptions.TooManyRequestsException,
    ) as e:
        print(e)
```

```python
# PinpointSMSVoiceClient.exceptions type checking example

from types_aiobotocore_pinpoint_sms_voice.client import Exceptions

def handle_error(exc: Exceptions.AlreadyExistsException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("pinpoint-sms-voice").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("pinpoint-sms-voice").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client)

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


### create\_configuration\_set

Create a new configuration set.

Type annotations and code completion for `#!python session.client("pinpoint-sms-voice").create_configuration_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client)

```python
# create_configuration_set method definition

await def create_configuration_set(
    self,
    *,
    ConfigurationSetName: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# create_configuration_set method usage example with argument unpacking

kwargs: CreateConfigurationSetRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.create_configuration_set(**kwargs)
```

1. See [:material-code-braces: CreateConfigurationSetRequestRequestTypeDef](./type_defs.md#createconfigurationsetrequestrequesttypedef) 

### create\_configuration\_set\_event\_destination

Create a new event destination in a configuration set.

Type annotations and code completion for `#!python session.client("pinpoint-sms-voice").create_configuration_set_event_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client)

```python
# create_configuration_set_event_destination method definition

await def create_configuration_set_event_destination(
    self,
    *,
    ConfigurationSetName: str,
    EventDestination: EventDestinationDefinitionTypeDef = ...,  # (1)
    EventDestinationName: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: EventDestinationDefinitionTypeDef](./type_defs.md#eventdestinationdefinitiontypedef) 


```python
# create_configuration_set_event_destination method usage example with argument unpacking

kwargs: CreateConfigurationSetEventDestinationRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.create_configuration_set_event_destination(**kwargs)
```

1. See [:material-code-braces: CreateConfigurationSetEventDestinationRequestRequestTypeDef](./type_defs.md#createconfigurationseteventdestinationrequestrequesttypedef) 

### delete\_configuration\_set

Deletes an existing configuration set.

Type annotations and code completion for `#!python session.client("pinpoint-sms-voice").delete_configuration_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client)

```python
# delete_configuration_set method definition

await def delete_configuration_set(
    self,
    *,
    ConfigurationSetName: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_configuration_set method usage example with argument unpacking

kwargs: DeleteConfigurationSetRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.delete_configuration_set(**kwargs)
```

1. See [:material-code-braces: DeleteConfigurationSetRequestRequestTypeDef](./type_defs.md#deleteconfigurationsetrequestrequesttypedef) 

### delete\_configuration\_set\_event\_destination

Deletes an event destination in a configuration set.

Type annotations and code completion for `#!python session.client("pinpoint-sms-voice").delete_configuration_set_event_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client)

```python
# delete_configuration_set_event_destination method definition

await def delete_configuration_set_event_destination(
    self,
    *,
    ConfigurationSetName: str,
    EventDestinationName: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_configuration_set_event_destination method usage example with argument unpacking

kwargs: DeleteConfigurationSetEventDestinationRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
    "EventDestinationName": ...,
}

parent.delete_configuration_set_event_destination(**kwargs)
```

1. See [:material-code-braces: DeleteConfigurationSetEventDestinationRequestRequestTypeDef](./type_defs.md#deleteconfigurationseteventdestinationrequestrequesttypedef) 

### get\_configuration\_set\_event\_destinations

Obtain information about an event destination, including the types of events it
reports, the Amazon Resource Name (ARN) of the destination, and the name of the
event destination.

Type annotations and code completion for `#!python session.client("pinpoint-sms-voice").get_configuration_set_event_destinations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client)

```python
# get_configuration_set_event_destinations method definition

await def get_configuration_set_event_destinations(
    self,
    *,
    ConfigurationSetName: str,
) -> GetConfigurationSetEventDestinationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConfigurationSetEventDestinationsResponseTypeDef](./type_defs.md#getconfigurationseteventdestinationsresponsetypedef) 


```python
# get_configuration_set_event_destinations method usage example with argument unpacking

kwargs: GetConfigurationSetEventDestinationsRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.get_configuration_set_event_destinations(**kwargs)
```

1. See [:material-code-braces: GetConfigurationSetEventDestinationsRequestRequestTypeDef](./type_defs.md#getconfigurationseteventdestinationsrequestrequesttypedef) 

### send\_voice\_message

Create a new voice message and send it to a recipient's phone number.

Type annotations and code completion for `#!python session.client("pinpoint-sms-voice").send_voice_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client)

```python
# send_voice_message method definition

await def send_voice_message(
    self,
    *,
    CallerId: str = ...,
    ConfigurationSetName: str = ...,
    Content: VoiceMessageContentTypeDef = ...,  # (1)
    DestinationPhoneNumber: str = ...,
    OriginationPhoneNumber: str = ...,
) -> SendVoiceMessageResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VoiceMessageContentTypeDef](./type_defs.md#voicemessagecontenttypedef) 
2. See [:material-code-braces: SendVoiceMessageResponseTypeDef](./type_defs.md#sendvoicemessageresponsetypedef) 


```python
# send_voice_message method usage example with argument unpacking

kwargs: SendVoiceMessageRequestRequestTypeDef = {  # (1)
    "CallerId": ...,
}

parent.send_voice_message(**kwargs)
```

1. See [:material-code-braces: SendVoiceMessageRequestRequestTypeDef](./type_defs.md#sendvoicemessagerequestrequesttypedef) 

### update\_configuration\_set\_event\_destination

Update an event destination in a configuration set.

Type annotations and code completion for `#!python session.client("pinpoint-sms-voice").update_configuration_set_event_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client)

```python
# update_configuration_set_event_destination method definition

await def update_configuration_set_event_destination(
    self,
    *,
    ConfigurationSetName: str,
    EventDestinationName: str,
    EventDestination: EventDestinationDefinitionTypeDef = ...,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: EventDestinationDefinitionTypeDef](./type_defs.md#eventdestinationdefinitiontypedef) 


```python
# update_configuration_set_event_destination method usage example with argument unpacking

kwargs: UpdateConfigurationSetEventDestinationRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
    "EventDestinationName": ...,
}

parent.update_configuration_set_event_destination(**kwargs)
```

1. See [:material-code-braces: UpdateConfigurationSetEventDestinationRequestRequestTypeDef](./type_defs.md#updateconfigurationseteventdestinationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("pinpoint-sms-voice").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("pinpoint-sms-voice").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client)

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




