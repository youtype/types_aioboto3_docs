# PersonalizeEventsClient

> [Index](../README.md) > [PersonalizeEvents](./README.md) > PersonalizeEventsClient

!!! note ""

    Auto-generated documentation for [PersonalizeEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#personalizeevents)
    type annotations stubs module [types-aiobotocore-personalize-events](https://pypi.org/project/types-aiobotocore-personalize-events/).

## PersonalizeEventsClient

Type annotations and code completion for `#!python session.client("personalize-events")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client)

```python
# PersonalizeEventsClient usage example

from aioboto3.session import Session
from types_aiobotocore_personalize_events.client import PersonalizeEventsClient

session = Session()
async with session.client("personalize-events") as client:
    client: PersonalizeEventsClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("personalize-events").exceptions` structure.

```python
# PersonalizeEventsClient.exceptions usage example

async with session.client("personalize-events") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.InvalidInputException,
        client.exceptions.ResourceInUseException,
        client.exceptions.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python
# PersonalizeEventsClient.exceptions type checking example

from types_aiobotocore_personalize_events.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("personalize-events").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("personalize-events").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client)

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


### put\_action\_interactions

Records action interaction event data.

Type annotations and code completion for `#!python session.client("personalize-events").put_action_interactions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client)

```python
# put_action_interactions method definition

await def put_action_interactions(
    self,
    *,
    trackingId: str,
    actionInteractions: Sequence[ActionInteractionTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ActionInteractionTypeDef](./type_defs.md#actioninteractiontypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_action_interactions method usage example with argument unpacking

kwargs: PutActionInteractionsRequestRequestTypeDef = {  # (1)
    "trackingId": ...,
    "actionInteractions": ...,
}

parent.put_action_interactions(**kwargs)
```

1. See [:material-code-braces: PutActionInteractionsRequestRequestTypeDef](./type_defs.md#putactioninteractionsrequestrequesttypedef) 

### put\_actions

Adds one or more actions to an Actions dataset.

Type annotations and code completion for `#!python session.client("personalize-events").put_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client)

```python
# put_actions method definition

await def put_actions(
    self,
    *,
    datasetArn: str,
    actions: Sequence[ActionTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_actions method usage example with argument unpacking

kwargs: PutActionsRequestRequestTypeDef = {  # (1)
    "datasetArn": ...,
    "actions": ...,
}

parent.put_actions(**kwargs)
```

1. See [:material-code-braces: PutActionsRequestRequestTypeDef](./type_defs.md#putactionsrequestrequesttypedef) 

### put\_events

Records item interaction event data.

Type annotations and code completion for `#!python session.client("personalize-events").put_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client)

```python
# put_events method definition

await def put_events(
    self,
    *,
    trackingId: str,
    sessionId: str,
    eventList: Sequence[EventTypeDef],  # (1)
    userId: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_events method usage example with argument unpacking

kwargs: PutEventsRequestRequestTypeDef = {  # (1)
    "trackingId": ...,
    "sessionId": ...,
    "eventList": ...,
}

parent.put_events(**kwargs)
```

1. See [:material-code-braces: PutEventsRequestRequestTypeDef](./type_defs.md#puteventsrequestrequesttypedef) 

### put\_items

Adds one or more items to an Items dataset.

Type annotations and code completion for `#!python session.client("personalize-events").put_items` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client)

```python
# put_items method definition

await def put_items(
    self,
    *,
    datasetArn: str,
    items: Sequence[ItemTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ItemTypeDef](./type_defs.md#itemtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_items method usage example with argument unpacking

kwargs: PutItemsRequestRequestTypeDef = {  # (1)
    "datasetArn": ...,
    "items": ...,
}

parent.put_items(**kwargs)
```

1. See [:material-code-braces: PutItemsRequestRequestTypeDef](./type_defs.md#putitemsrequestrequesttypedef) 

### put\_users

Adds one or more users to a Users dataset.

Type annotations and code completion for `#!python session.client("personalize-events").put_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client)

```python
# put_users method definition

await def put_users(
    self,
    *,
    datasetArn: str,
    users: Sequence[UserTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_users method usage example with argument unpacking

kwargs: PutUsersRequestRequestTypeDef = {  # (1)
    "datasetArn": ...,
    "users": ...,
}

parent.put_users(**kwargs)
```

1. See [:material-code-braces: PutUsersRequestRequestTypeDef](./type_defs.md#putusersrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("personalize-events").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("personalize-events").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client)

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




