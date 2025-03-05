# WorkMailMessageFlowClient

> [Index](../README.md) > [WorkMailMessageFlow](./README.md) > WorkMailMessageFlowClient

!!! note ""

    Auto-generated documentation for [WorkMailMessageFlow](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#workmailmessageflow)
    type annotations stubs module [types-aiobotocore-workmailmessageflow](https://pypi.org/project/types-aiobotocore-workmailmessageflow/).

## WorkMailMessageFlowClient

Type annotations and code completion for `#!python session.client("workmailmessageflow")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client)

```python
# WorkMailMessageFlowClient usage example

from aioboto3.session import Session
from types_aiobotocore_workmailmessageflow.client import WorkMailMessageFlowClient

session = Session()
async with session.client("workmailmessageflow") as client:
    client: WorkMailMessageFlowClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("workmailmessageflow").exceptions` structure.

```python
# WorkMailMessageFlowClient.exceptions usage example

async with session.client("workmailmessageflow") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.InvalidContentLocation,
        client.exceptions.MessageFrozen,
        client.exceptions.MessageRejected,
        client.exceptions.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python
# WorkMailMessageFlowClient.exceptions type checking example

from types_aiobotocore_workmailmessageflow.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("workmailmessageflow").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("workmailmessageflow").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client)

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


### get\_raw\_message\_content

Retrieves the raw content of an in-transit email message, in MIME format.

Type annotations and code completion for `#!python session.client("workmailmessageflow").get_raw_message_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client)

```python
# get_raw_message_content method definition

await def get_raw_message_content(
    self,
    *,
    messageId: str,
) -> GetRawMessageContentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRawMessageContentResponseTypeDef](./type_defs.md#getrawmessagecontentresponsetypedef)


```python
# get_raw_message_content method usage example with argument unpacking

kwargs: GetRawMessageContentRequestTypeDef = {  # (1)
    "messageId": ...,
}

parent.get_raw_message_content(**kwargs)
```

1. See [:material-code-braces: GetRawMessageContentRequestTypeDef](./type_defs.md#getrawmessagecontentrequesttypedef)

### put\_raw\_message\_content

Updates the raw content of an in-transit email message, in MIME format.

Type annotations and code completion for `#!python session.client("workmailmessageflow").put_raw_message_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client)

```python
# put_raw_message_content method definition

await def put_raw_message_content(
    self,
    *,
    messageId: str,
    content: RawMessageContentTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: RawMessageContentTypeDef](./type_defs.md#rawmessagecontenttypedef)


```python
# put_raw_message_content method usage example with argument unpacking

kwargs: PutRawMessageContentRequestTypeDef = {  # (1)
    "messageId": ...,
    "content": ...,
}

parent.put_raw_message_content(**kwargs)
```

1. See [:material-code-braces: PutRawMessageContentRequestTypeDef](./type_defs.md#putrawmessagecontentrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("workmailmessageflow").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("workmailmessageflow").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```





