# PersonalizeEventsClient

> [Index](../README.md) > [PersonalizeEvents](./README.md) > PersonalizeEventsClient

!!! note ""

    Auto-generated documentation for [PersonalizeEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
    type annotations stubs module [types-aiobotocore-personalize-events](https://pypi.org/project/types-aiobotocore-personalize-events/).

## PersonalizeEventsClient

Type annotations and code completion for `#!python session.client("personalize-events")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client)

```python title="Usage example"
from aioboto3.session import Session
from types_aiobotocore_personalize_events.client import PersonalizeEventsClient

session = Session()
async with session.client("personalize-events") as client:
    client: PersonalizeEventsClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("personalize-events").exceptions` structure.

```python title="Usage example"
async with session.client("personalize-events") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InvalidInputException,
        client.ResourceInUseException,
        client.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_personalize_events.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.client("personalize-events").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.client("personalize-events").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client.close)

```python title="Method definition"
await def close(
    self,
) -> None:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.client("personalize-events").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client.generate_presigned_url)

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


### put\_events

Records user interaction event data.

Type annotations and code completion for `#!python session.client("personalize-events").put_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client.put_events)

```python title="Method definition"
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


```python title="Usage example with kwargs"
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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client.put_items)

```python title="Method definition"
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


```python title="Usage example with kwargs"
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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client.put_users)

```python title="Method definition"
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


```python title="Usage example with kwargs"
kwargs: PutUsersRequestRequestTypeDef = {  # (1)
    "datasetArn": ...,
    "users": ...,
}

parent.put_users(**kwargs)
```

1. See [:material-code-braces: PutUsersRequestRequestTypeDef](./type_defs.md#putusersrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("personalize-events").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> PersonalizeEventsClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("personalize-events").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





