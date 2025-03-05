# Examples

> [Index](../README.md) > [PinpointSMSVoice](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PinpointSMSVoice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#pinpointsmsvoice)
    type annotations stubs module [types-aiobotocore-pinpoint-sms-voice](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[pinpoint-sms-voice]` package installed.

Write your `PinpointSMSVoice` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# PinpointSMSVoiceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("pinpoint-sms-voice") as client:  # (1)
    result = await client.get_configuration_set_event_destinations()  # (2)
```

1. client: [PinpointSMSVoiceClient](./client.md)
2. result: [:material-code-braces: GetConfigurationSetEventDestinationsResponseTypeDef](./type_defs.md#getconfigurationseteventdestinationsresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[pinpoint-sms-voice]`
or a standalone `types_aiobotocore_pinpoint_sms_voice` package, you have to explicitly specify
`client: PinpointSMSVoiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# PinpointSMSVoiceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_pinpoint_sms_voice.client import PinpointSMSVoiceClient
from types_aiobotocore_pinpoint_sms_voice.type_defs import GetConfigurationSetEventDestinationsResponseTypeDef
from types_aiobotocore_pinpoint_sms_voice.type_defs import GetConfigurationSetEventDestinationsRequestTypeDef


session = Session()

client: PinpointSMSVoiceClient
async with session.client("pinpoint-sms-voice") as client:  # (1)
    kwargs: GetConfigurationSetEventDestinationsRequestTypeDef = {...}  # (2)
    result: GetConfigurationSetEventDestinationsResponseTypeDef = await client.get_configuration_set_event_destinations(**kwargs)  # (3)
```

1. client: [PinpointSMSVoiceClient](./client.md)
2. kwargs: [:material-code-braces: GetConfigurationSetEventDestinationsRequestTypeDef](./type_defs.md#getconfigurationseteventdestinationsrequesttypedef)
3. result: [:material-code-braces: GetConfigurationSetEventDestinationsResponseTypeDef](./type_defs.md#getconfigurationseteventdestinationsresponsetypedef)






