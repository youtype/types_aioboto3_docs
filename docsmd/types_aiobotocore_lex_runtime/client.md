# LexRuntimeServiceClient

> [Index](../README.md) > [LexRuntimeService](./README.md) > LexRuntimeServiceClient

!!! note ""

    Auto-generated documentation for [LexRuntimeService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#lexruntimeservice)
    type annotations stubs module [types-aiobotocore-lex-runtime](https://pypi.org/project/types-aiobotocore-lex-runtime/).

## LexRuntimeServiceClient

Type annotations and code completion for `#!python session.client("lex-runtime")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client)

```python
# LexRuntimeServiceClient usage example

from aioboto3.session import Session
from types_aiobotocore_lex_runtime.client import LexRuntimeServiceClient

session = Session()
async with session.client("lex-runtime") as client:
    client: LexRuntimeServiceClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("lex-runtime").exceptions` structure.

```python
# LexRuntimeServiceClient.exceptions usage example

async with session.client("lex-runtime") as client:
    try:
        do_something(client)
    except (
            client.exceptions.BadGatewayException,
        client.exceptions.BadRequestException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.DependencyFailedException,
        client.exceptions.InternalFailureException,
        client.exceptions.LimitExceededException,
        client.exceptions.LoopDetectedException,
        client.exceptions.NotAcceptableException,
        client.exceptions.NotFoundException,
        client.exceptions.RequestTimeoutException,
        client.exceptions.UnsupportedMediaTypeException,
    ) as e:
        print(e)
```

```python
# LexRuntimeServiceClient.exceptions type checking example

from types_aiobotocore_lex_runtime.client import Exceptions

def handle_error(exc: Exceptions.BadGatewayException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("lex-runtime").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("lex-runtime").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client)

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


### delete\_session

Removes session information for a specified bot, alias, and user ID.

Type annotations and code completion for `#!python session.client("lex-runtime").delete_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client)

```python
# delete_session method definition

await def delete_session(
    self,
    *,
    botName: str,
    botAlias: str,
    userId: str,
) -> DeleteSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteSessionResponseTypeDef](./type_defs.md#deletesessionresponsetypedef)


```python
# delete_session method usage example with argument unpacking

kwargs: DeleteSessionRequestTypeDef = {  # (1)
    "botName": ...,
    "botAlias": ...,
    "userId": ...,
}

parent.delete_session(**kwargs)
```

1. See [:material-code-braces: DeleteSessionRequestTypeDef](./type_defs.md#deletesessionrequesttypedef)

### get\_session

Returns session information for a specified bot, alias, and user ID.

Type annotations and code completion for `#!python session.client("lex-runtime").get_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client)

```python
# get_session method definition

await def get_session(
    self,
    *,
    botName: str,
    botAlias: str,
    userId: str,
    checkpointLabelFilter: str = ...,
) -> GetSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSessionResponseTypeDef](./type_defs.md#getsessionresponsetypedef)


```python
# get_session method usage example with argument unpacking

kwargs: GetSessionRequestTypeDef = {  # (1)
    "botName": ...,
    "botAlias": ...,
    "userId": ...,
}

parent.get_session(**kwargs)
```

1. See [:material-code-braces: GetSessionRequestTypeDef](./type_defs.md#getsessionrequesttypedef)

### post\_content

Sends user input (text or speech) to Amazon Lex.

Type annotations and code completion for `#!python session.client("lex-runtime").post_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client)

```python
# post_content method definition

await def post_content(
    self,
    *,
    botName: str,
    botAlias: str,
    userId: str,
    contentType: str,
    inputStream: BlobTypeDef,
    sessionAttributes: str = ...,
    requestAttributes: str = ...,
    accept: str = ...,
    activeContexts: str = ...,
) -> PostContentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PostContentResponseTypeDef](./type_defs.md#postcontentresponsetypedef)


```python
# post_content method usage example with argument unpacking

kwargs: PostContentRequestTypeDef = {  # (1)
    "botName": ...,
    "botAlias": ...,
    "userId": ...,
    "contentType": ...,
    "inputStream": ...,
}

parent.post_content(**kwargs)
```

1. See [:material-code-braces: PostContentRequestTypeDef](./type_defs.md#postcontentrequesttypedef)

### post\_text

Sends user input to Amazon Lex.

Type annotations and code completion for `#!python session.client("lex-runtime").post_text` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client)

```python
# post_text method definition

await def post_text(
    self,
    *,
    botName: str,
    botAlias: str,
    userId: str,
    inputText: str,
    sessionAttributes: Mapping[str, str] = ...,
    requestAttributes: Mapping[str, str] = ...,
    activeContexts: Sequence[ActiveContextUnionTypeDef] = ...,  # (1)
) -> PostTextResponseTypeDef:  # (2)
    ...
```

1. See `Sequence[ActiveContextUnionTypeDef]`
2. See [:material-code-braces: PostTextResponseTypeDef](./type_defs.md#posttextresponsetypedef)


```python
# post_text method usage example with argument unpacking

kwargs: PostTextRequestTypeDef = {  # (1)
    "botName": ...,
    "botAlias": ...,
    "userId": ...,
    "inputText": ...,
}

parent.post_text(**kwargs)
```

1. See [:material-code-braces: PostTextRequestTypeDef](./type_defs.md#posttextrequesttypedef)

### put\_session

Creates a new session or modifies an existing session with an Amazon Lex bot.

Type annotations and code completion for `#!python session.client("lex-runtime").put_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client)

```python
# put_session method definition

await def put_session(
    self,
    *,
    botName: str,
    botAlias: str,
    userId: str,
    sessionAttributes: Mapping[str, str] = ...,
    dialogAction: DialogActionUnionTypeDef = ...,  # (1)
    recentIntentSummaryView: Sequence[IntentSummaryUnionTypeDef] = ...,  # (2)
    accept: str = ...,
    activeContexts: Sequence[ActiveContextUnionTypeDef] = ...,  # (3)
) -> PutSessionResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DialogActionUnionTypeDef](#dialogactionuniontypedef)
2. See `Sequence[IntentSummaryUnionTypeDef]`
3. See `Sequence[ActiveContextUnionTypeDef]`
4. See [:material-code-braces: PutSessionResponseTypeDef](./type_defs.md#putsessionresponsetypedef)


```python
# put_session method usage example with argument unpacking

kwargs: PutSessionRequestTypeDef = {  # (1)
    "botName": ...,
    "botAlias": ...,
    "userId": ...,
}

parent.put_session(**kwargs)
```

1. See [:material-code-braces: PutSessionRequestTypeDef](./type_defs.md#putsessionrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("lex-runtime").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("lex-runtime").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client)

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





