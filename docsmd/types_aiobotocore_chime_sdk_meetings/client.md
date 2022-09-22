# ChimeSDKMeetingsClient

> [Index](../README.md) > [ChimeSDKMeetings](./README.md) > ChimeSDKMeetingsClient

!!! note ""

    Auto-generated documentation for [ChimeSDKMeetings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
    type annotations stubs module [types-aiobotocore-chime-sdk-meetings](https://pypi.org/project/types-aiobotocore-chime-sdk-meetings/).

## ChimeSDKMeetingsClient

Type annotations and code completion for `#!python session.client("chime-sdk-meetings")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client)

```python title="Usage example"
from aioboto3.session import Session
from types_aiobotocore_chime_sdk_meetings.client import ChimeSDKMeetingsClient

session = Session()
async with session.client("chime-sdk-meetings") as client:
    client: ChimeSDKMeetingsClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("chime-sdk-meetings").exceptions` structure.

```python title="Usage example"
async with session.client("chime-sdk-meetings") as client:
    try:
        do_something(client)
    except (
            client.BadRequestException,
        client.ClientError,
        client.ConflictException,
        client.ForbiddenException,
        client.LimitExceededException,
        client.NotFoundException,
        client.ResourceNotFoundException,
        client.ServiceFailureException,
        client.ServiceUnavailableException,
        client.ThrottlingException,
        client.TooManyTagsException,
        client.UnauthorizedException,
        client.UnprocessableEntityException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_chime_sdk_meetings.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```


## Methods


### batch\_create\_attendee

Creates up to 100 attendees for an active Amazon Chime SDK meeting.

Type annotations and code completion for `#!python session.client("chime-sdk-meetings").batch_create_attendee` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.batch_create_attendee)

```python title="Method definition"
await def batch_create_attendee(
    self,
    *,
    MeetingId: str,
    Attendees: Sequence[CreateAttendeeRequestItemTypeDef],  # (1)
) -> BatchCreateAttendeeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CreateAttendeeRequestItemTypeDef](./type_defs.md#createattendeerequestitemtypedef) 
2. See [:material-code-braces: BatchCreateAttendeeResponseTypeDef](./type_defs.md#batchcreateattendeeresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: BatchCreateAttendeeRequestRequestTypeDef = {  # (1)
    "MeetingId": ...,
    "Attendees": ...,
}

parent.batch_create_attendee(**kwargs)
```

1. See [:material-code-braces: BatchCreateAttendeeRequestRequestTypeDef](./type_defs.md#batchcreateattendeerequestrequesttypedef) 

### batch\_update\_attendee\_capabilities\_except

Updates `AttendeeCapabilities` except the capabilities listed in an
`ExcludedAttendeeIds` table.

Type annotations and code completion for `#!python session.client("chime-sdk-meetings").batch_update_attendee_capabilities_except` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.batch_update_attendee_capabilities_except)

```python title="Method definition"
await def batch_update_attendee_capabilities_except(
    self,
    *,
    MeetingId: str,
    ExcludedAttendeeIds: Sequence[AttendeeIdItemTypeDef],  # (1)
    Capabilities: AttendeeCapabilitiesTypeDef,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AttendeeIdItemTypeDef](./type_defs.md#attendeeiditemtypedef) 
2. See [:material-code-braces: AttendeeCapabilitiesTypeDef](./type_defs.md#attendeecapabilitiestypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python title="Usage example with kwargs"
kwargs: BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef = {  # (1)
    "MeetingId": ...,
    "ExcludedAttendeeIds": ...,
    "Capabilities": ...,
}

parent.batch_update_attendee_capabilities_except(**kwargs)
```

1. See [:material-code-braces: BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef](./type_defs.md#batchupdateattendeecapabilitiesexceptrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.client("chime-sdk-meetings").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.client("chime-sdk-meetings").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.close)

```python title="Method definition"
await def close(
    self,
) -> None:
    ...
```


### create\_attendee

Creates a new attendee for an active Amazon Chime SDK meeting.

Type annotations and code completion for `#!python session.client("chime-sdk-meetings").create_attendee` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.create_attendee)

```python title="Method definition"
await def create_attendee(
    self,
    *,
    MeetingId: str,
    ExternalUserId: str,
    Capabilities: AttendeeCapabilitiesTypeDef = ...,  # (1)
) -> CreateAttendeeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AttendeeCapabilitiesTypeDef](./type_defs.md#attendeecapabilitiestypedef) 
2. See [:material-code-braces: CreateAttendeeResponseTypeDef](./type_defs.md#createattendeeresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: CreateAttendeeRequestRequestTypeDef = {  # (1)
    "MeetingId": ...,
    "ExternalUserId": ...,
}

parent.create_attendee(**kwargs)
```

1. See [:material-code-braces: CreateAttendeeRequestRequestTypeDef](./type_defs.md#createattendeerequestrequesttypedef) 

### create\_meeting

Creates a new Amazon Chime SDK meeting in the specified media Region with no
initial attendees.

Type annotations and code completion for `#!python session.client("chime-sdk-meetings").create_meeting` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.create_meeting)

```python title="Method definition"
await def create_meeting(
    self,
    *,
    ClientRequestToken: str,
    MediaRegion: str,
    ExternalMeetingId: str,
    MeetingHostId: str = ...,
    NotificationsConfiguration: NotificationsConfigurationTypeDef = ...,  # (1)
    MeetingFeatures: MeetingFeaturesConfigurationTypeDef = ...,  # (2)
    PrimaryMeetingId: str = ...,
    TenantIds: Sequence[str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateMeetingResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: NotificationsConfigurationTypeDef](./type_defs.md#notificationsconfigurationtypedef) 
2. See [:material-code-braces: MeetingFeaturesConfigurationTypeDef](./type_defs.md#meetingfeaturesconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateMeetingResponseTypeDef](./type_defs.md#createmeetingresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: CreateMeetingRequestRequestTypeDef = {  # (1)
    "ClientRequestToken": ...,
    "MediaRegion": ...,
    "ExternalMeetingId": ...,
}

parent.create_meeting(**kwargs)
```

1. See [:material-code-braces: CreateMeetingRequestRequestTypeDef](./type_defs.md#createmeetingrequestrequesttypedef) 

### create\_meeting\_with\_attendees

Creates a new Amazon Chime SDK meeting in the specified media Region, with
attendees.

Type annotations and code completion for `#!python session.client("chime-sdk-meetings").create_meeting_with_attendees` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.create_meeting_with_attendees)

```python title="Method definition"
await def create_meeting_with_attendees(
    self,
    *,
    ClientRequestToken: str,
    MediaRegion: str,
    ExternalMeetingId: str,
    Attendees: Sequence[CreateAttendeeRequestItemTypeDef],  # (1)
    MeetingHostId: str = ...,
    MeetingFeatures: MeetingFeaturesConfigurationTypeDef = ...,  # (2)
    NotificationsConfiguration: NotificationsConfigurationTypeDef = ...,  # (3)
    PrimaryMeetingId: str = ...,
    TenantIds: Sequence[str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateMeetingWithAttendeesResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: CreateAttendeeRequestItemTypeDef](./type_defs.md#createattendeerequestitemtypedef) 
2. See [:material-code-braces: MeetingFeaturesConfigurationTypeDef](./type_defs.md#meetingfeaturesconfigurationtypedef) 
3. See [:material-code-braces: NotificationsConfigurationTypeDef](./type_defs.md#notificationsconfigurationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateMeetingWithAttendeesResponseTypeDef](./type_defs.md#createmeetingwithattendeesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: CreateMeetingWithAttendeesRequestRequestTypeDef = {  # (1)
    "ClientRequestToken": ...,
    "MediaRegion": ...,
    "ExternalMeetingId": ...,
    "Attendees": ...,
}

parent.create_meeting_with_attendees(**kwargs)
```

1. See [:material-code-braces: CreateMeetingWithAttendeesRequestRequestTypeDef](./type_defs.md#createmeetingwithattendeesrequestrequesttypedef) 

### delete\_attendee

Deletes an attendee from the specified Amazon Chime SDK meeting and deletes
their `JoinToken`.

Type annotations and code completion for `#!python session.client("chime-sdk-meetings").delete_attendee` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.delete_attendee)

```python title="Method definition"
await def delete_attendee(
    self,
    *,
    MeetingId: str,
    AttendeeId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python title="Usage example with kwargs"
kwargs: DeleteAttendeeRequestRequestTypeDef = {  # (1)
    "MeetingId": ...,
    "AttendeeId": ...,
}

parent.delete_attendee(**kwargs)
```

1. See [:material-code-braces: DeleteAttendeeRequestRequestTypeDef](./type_defs.md#deleteattendeerequestrequesttypedef) 

### delete\_meeting

Deletes the specified Amazon Chime SDK meeting.

Type annotations and code completion for `#!python session.client("chime-sdk-meetings").delete_meeting` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.delete_meeting)

```python title="Method definition"
await def delete_meeting(
    self,
    *,
    MeetingId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python title="Usage example with kwargs"
kwargs: DeleteMeetingRequestRequestTypeDef = {  # (1)
    "MeetingId": ...,
}

parent.delete_meeting(**kwargs)
```

1. See [:material-code-braces: DeleteMeetingRequestRequestTypeDef](./type_defs.md#deletemeetingrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.client("chime-sdk-meetings").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.generate_presigned_url)

```python title="Method definition"
await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_attendee

Gets the Amazon Chime SDK attendee details for a specified meeting ID and
attendee ID.

Type annotations and code completion for `#!python session.client("chime-sdk-meetings").get_attendee` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.get_attendee)

```python title="Method definition"
await def get_attendee(
    self,
    *,
    MeetingId: str,
    AttendeeId: str,
) -> GetAttendeeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAttendeeResponseTypeDef](./type_defs.md#getattendeeresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetAttendeeRequestRequestTypeDef = {  # (1)
    "MeetingId": ...,
    "AttendeeId": ...,
}

parent.get_attendee(**kwargs)
```

1. See [:material-code-braces: GetAttendeeRequestRequestTypeDef](./type_defs.md#getattendeerequestrequesttypedef) 

### get\_meeting

Gets the Amazon Chime SDK meeting details for the specified meeting ID.

Type annotations and code completion for `#!python session.client("chime-sdk-meetings").get_meeting` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.get_meeting)

```python title="Method definition"
await def get_meeting(
    self,
    *,
    MeetingId: str,
) -> GetMeetingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMeetingResponseTypeDef](./type_defs.md#getmeetingresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetMeetingRequestRequestTypeDef = {  # (1)
    "MeetingId": ...,
}

parent.get_meeting(**kwargs)
```

1. See [:material-code-braces: GetMeetingRequestRequestTypeDef](./type_defs.md#getmeetingrequestrequesttypedef) 

### list\_attendees

Lists the attendees for the specified Amazon Chime SDK meeting.

Type annotations and code completion for `#!python session.client("chime-sdk-meetings").list_attendees` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.list_attendees)

```python title="Method definition"
await def list_attendees(
    self,
    *,
    MeetingId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAttendeesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAttendeesResponseTypeDef](./type_defs.md#listattendeesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAttendeesRequestRequestTypeDef = {  # (1)
    "MeetingId": ...,
}

parent.list_attendees(**kwargs)
```

1. See [:material-code-braces: ListAttendeesRequestRequestTypeDef](./type_defs.md#listattendeesrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of the tags available for the specified resource.

Type annotations and code completion for `#!python session.client("chime-sdk-meetings").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.list_tags_for_resource)

```python title="Method definition"
await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### start\_meeting\_transcription

Starts transcription for the specified `meetingId` .

Type annotations and code completion for `#!python session.client("chime-sdk-meetings").start_meeting_transcription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.start_meeting_transcription)

```python title="Method definition"
await def start_meeting_transcription(
    self,
    *,
    MeetingId: str,
    TranscriptionConfiguration: TranscriptionConfigurationTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TranscriptionConfigurationTypeDef](./type_defs.md#transcriptionconfigurationtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python title="Usage example with kwargs"
kwargs: StartMeetingTranscriptionRequestRequestTypeDef = {  # (1)
    "MeetingId": ...,
    "TranscriptionConfiguration": ...,
}

parent.start_meeting_transcription(**kwargs)
```

1. See [:material-code-braces: StartMeetingTranscriptionRequestRequestTypeDef](./type_defs.md#startmeetingtranscriptionrequestrequesttypedef) 

### stop\_meeting\_transcription

Stops transcription for the specified `meetingId` .

Type annotations and code completion for `#!python session.client("chime-sdk-meetings").stop_meeting_transcription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.stop_meeting_transcription)

```python title="Method definition"
await def stop_meeting_transcription(
    self,
    *,
    MeetingId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python title="Usage example with kwargs"
kwargs: StopMeetingTranscriptionRequestRequestTypeDef = {  # (1)
    "MeetingId": ...,
}

parent.stop_meeting_transcription(**kwargs)
```

1. See [:material-code-braces: StopMeetingTranscriptionRequestRequestTypeDef](./type_defs.md#stopmeetingtranscriptionrequestrequesttypedef) 

### tag\_resource

The resource that supports tags.

Type annotations and code completion for `#!python session.client("chime-sdk-meetings").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.tag_resource)

```python title="Method definition"
await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python title="Usage example with kwargs"
kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes the specified tags from the specified resources.

Type annotations and code completion for `#!python session.client("chime-sdk-meetings").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.untag_resource)

```python title="Method definition"
await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python title="Usage example with kwargs"
kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_attendee\_capabilities

The capabilties that you want to update.

Type annotations and code completion for `#!python session.client("chime-sdk-meetings").update_attendee_capabilities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.update_attendee_capabilities)

```python title="Method definition"
await def update_attendee_capabilities(
    self,
    *,
    MeetingId: str,
    AttendeeId: str,
    Capabilities: AttendeeCapabilitiesTypeDef,  # (1)
) -> UpdateAttendeeCapabilitiesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AttendeeCapabilitiesTypeDef](./type_defs.md#attendeecapabilitiestypedef) 
2. See [:material-code-braces: UpdateAttendeeCapabilitiesResponseTypeDef](./type_defs.md#updateattendeecapabilitiesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: UpdateAttendeeCapabilitiesRequestRequestTypeDef = {  # (1)
    "MeetingId": ...,
    "AttendeeId": ...,
    "Capabilities": ...,
}

parent.update_attendee_capabilities(**kwargs)
```

1. See [:material-code-braces: UpdateAttendeeCapabilitiesRequestRequestTypeDef](./type_defs.md#updateattendeecapabilitiesrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("chime-sdk-meetings").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> ChimeSDKMeetingsClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("chime-sdk-meetings").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





