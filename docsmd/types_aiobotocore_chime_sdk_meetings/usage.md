# Examples

> [Index](../README.md) > [ChimeSDKMeetings](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ChimeSDKMeetings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#chimesdkmeetings)
    type annotations stubs module [types-aiobotocore-chime-sdk-meetings](https://pypi.org/project/types-aiobotocore-chime-sdk-meetings/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[chime-sdk-meetings]` package installed.

Write your `ChimeSDKMeetings` code as usual,
type checking and code completion should work out of the box.



```python
# ChimeSDKMeetingsClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("chime-sdk-meetings") as client:  # (1)
    result = await client.batch_create_attendee()  # (2)
```

1. client: [ChimeSDKMeetingsClient](./client.md)
2. result: [:material-code-braces: BatchCreateAttendeeResponseTypeDef](./type_defs.md#batchcreateattendeeresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[chime-sdk-meetings]`
or a standalone `types_aiobotocore_chime_sdk_meetings` package, you have to explicitly specify
`client: ChimeSDKMeetingsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ChimeSDKMeetingsClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_chime_sdk_meetings.client import ChimeSDKMeetingsClient
from types_aiobotocore_chime_sdk_meetings.type_defs import BatchCreateAttendeeResponseTypeDef
from types_aiobotocore_chime_sdk_meetings.type_defs import BatchCreateAttendeeRequestRequestTypeDef


session = Session()

client: ChimeSDKMeetingsClient
async with session.client("chime-sdk-meetings") as client:  # (1)
    kwargs: BatchCreateAttendeeRequestRequestTypeDef = {...}  # (2)
    result: BatchCreateAttendeeResponseTypeDef = await client.batch_create_attendee(**kwargs)  # (3)
```

1. client: [ChimeSDKMeetingsClient](./client.md)
2. kwargs: [:material-code-braces: BatchCreateAttendeeRequestRequestTypeDef](./type_defs.md#batchcreateattendeerequestrequesttypedef) 
3. result: [:material-code-braces: BatchCreateAttendeeResponseTypeDef](./type_defs.md#batchcreateattendeeresponsetypedef) 





