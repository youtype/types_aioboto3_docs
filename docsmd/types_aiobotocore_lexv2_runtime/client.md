# LexRuntimeV2Client

> [Index](../README.md) > [LexRuntimeV2](./README.md) > LexRuntimeV2Client

!!! note ""

    Auto-generated documentation for [LexRuntimeV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#lexruntimev2)
    type annotations stubs module [types-aiobotocore-lexv2-runtime](https://pypi.org/project/types-aiobotocore-lexv2-runtime/).

## LexRuntimeV2Client

Type annotations and code completion for `#!python session.client("lexv2-runtime")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client)

```python
# LexRuntimeV2Client usage example

from aioboto3.session import Session
from types_aiobotocore_lexv2_runtime.client import LexRuntimeV2Client

session = Session()
async with session.client("lexv2-runtime") as client:
    client: LexRuntimeV2Client
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("lexv2-runtime").exceptions` structure.

```python
# LexRuntimeV2Client.exceptions usage example

async with session.client("lexv2-runtime") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.BadGatewayException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.DependencyFailedException,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# LexRuntimeV2Client.exceptions type checking example

from types_aiobotocore_lexv2_runtime.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("lexv2-runtime").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("lexv2-runtime").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client)

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

Type annotations and code completion for `#!python session.client("lexv2-runtime").delete_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client)

```python
# delete_session method definition

await def delete_session(
    self,
    *,
    botId: str,
    botAliasId: str,
    localeId: str,
    sessionId: str,
) -> DeleteSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteSessionResponseTypeDef](./type_defs.md#deletesessionresponsetypedef) 


```python
# delete_session method usage example with argument unpacking

kwargs: DeleteSessionRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botAliasId": ...,
    "localeId": ...,
    "sessionId": ...,
}

parent.delete_session(**kwargs)
```

1. See [:material-code-braces: DeleteSessionRequestRequestTypeDef](./type_defs.md#deletesessionrequestrequesttypedef) 

### get\_session

Returns session information for a specified bot, alias, and user.

Type annotations and code completion for `#!python session.client("lexv2-runtime").get_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client)

```python
# get_session method definition

await def get_session(
    self,
    *,
    botId: str,
    botAliasId: str,
    localeId: str,
    sessionId: str,
) -> GetSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSessionResponseTypeDef](./type_defs.md#getsessionresponsetypedef) 


```python
# get_session method usage example with argument unpacking

kwargs: GetSessionRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botAliasId": ...,
    "localeId": ...,
    "sessionId": ...,
}

parent.get_session(**kwargs)
```

1. See [:material-code-braces: GetSessionRequestRequestTypeDef](./type_defs.md#getsessionrequestrequesttypedef) 

### put\_session

Creates a new session or modifies an existing session with an Amazon Lex V2 bot.

Type annotations and code completion for `#!python session.client("lexv2-runtime").put_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client)

```python
# put_session method definition

await def put_session(
    self,
    *,
    botId: str,
    botAliasId: str,
    localeId: str,
    sessionId: str,
    sessionState: SessionStateTypeDef,  # (1)
    messages: Sequence[MessageUnionTypeDef] = ...,  # (2)
    requestAttributes: Mapping[str, str] = ...,
    responseContentType: str = ...,
) -> PutSessionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SessionStateTypeDef](./type_defs.md#sessionstatetypedef) 
2. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) [:material-code-braces: MessageOutputTypeDef](./type_defs.md#messageoutputtypedef) 
3. See [:material-code-braces: PutSessionResponseTypeDef](./type_defs.md#putsessionresponsetypedef) 


```python
# put_session method usage example with argument unpacking

kwargs: PutSessionRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botAliasId": ...,
    "localeId": ...,
    "sessionId": ...,
    "sessionState": ...,
}

parent.put_session(**kwargs)
```

1. See [:material-code-braces: PutSessionRequestRequestTypeDef](./type_defs.md#putsessionrequestrequesttypedef) 

### recognize\_text

Sends user input to Amazon Lex V2.

Type annotations and code completion for `#!python session.client("lexv2-runtime").recognize_text` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client)

```python
# recognize_text method definition

await def recognize_text(
    self,
    *,
    botId: str,
    botAliasId: str,
    localeId: str,
    sessionId: str,
    text: str,
    sessionState: SessionStateTypeDef = ...,  # (1)
    requestAttributes: Mapping[str, str] = ...,
) -> RecognizeTextResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SessionStateTypeDef](./type_defs.md#sessionstatetypedef) 
2. See [:material-code-braces: RecognizeTextResponseTypeDef](./type_defs.md#recognizetextresponsetypedef) 


```python
# recognize_text method usage example with argument unpacking

kwargs: RecognizeTextRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botAliasId": ...,
    "localeId": ...,
    "sessionId": ...,
    "text": ...,
}

parent.recognize_text(**kwargs)
```

1. See [:material-code-braces: RecognizeTextRequestRequestTypeDef](./type_defs.md#recognizetextrequestrequesttypedef) 

### recognize\_utterance

Sends user input to Amazon Lex V2.

Type annotations and code completion for `#!python session.client("lexv2-runtime").recognize_utterance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client)

```python
# recognize_utterance method definition

await def recognize_utterance(
    self,
    *,
    botId: str,
    botAliasId: str,
    localeId: str,
    sessionId: str,
    requestContentType: str,
    sessionState: str = ...,
    requestAttributes: str = ...,
    responseContentType: str = ...,
    inputStream: BlobTypeDef = ...,
) -> RecognizeUtteranceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RecognizeUtteranceResponseTypeDef](./type_defs.md#recognizeutteranceresponsetypedef) 


```python
# recognize_utterance method usage example with argument unpacking

kwargs: RecognizeUtteranceRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botAliasId": ...,
    "localeId": ...,
    "sessionId": ...,
    "requestContentType": ...,
}

parent.recognize_utterance(**kwargs)
```

1. See [:material-code-braces: RecognizeUtteranceRequestRequestTypeDef](./type_defs.md#recognizeutterancerequestrequesttypedef) 

### start\_conversation

Starts an HTTP/2 bidirectional event stream that enables you to send audio,
text, or DTMF input in real time.

Type annotations and code completion for `#!python session.client("lexv2-runtime").start_conversation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client)

```python
# start_conversation method definition

await def start_conversation(
    self,
    *,
    botId: str,
    botAliasId: str,
    localeId: str,
    sessionId: str,
    requestEventStream: AioEventStream[StartConversationRequestEventStreamTypeDef],  # (1)
    conversationMode: ConversationModeType = ...,  # (2)
) -> StartConversationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: StartConversationRequestEventStreamTypeDef](./type_defs.md#startconversationrequesteventstreamtypedef) 
2. See [:material-code-brackets: ConversationModeType](./literals.md#conversationmodetype) 
3. See [:material-code-braces: StartConversationResponseTypeDef](./type_defs.md#startconversationresponsetypedef) 


```python
# start_conversation method usage example with argument unpacking

kwargs: StartConversationRequestRequestTypeDef = {  # (1)
    "botId": ...,
    "botAliasId": ...,
    "localeId": ...,
    "sessionId": ...,
    "requestEventStream": ...,
}

parent.start_conversation(**kwargs)
```

1. See [:material-code-braces: StartConversationRequestRequestTypeDef](./type_defs.md#startconversationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("lexv2-runtime").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("lexv2-runtime").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client)

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




