# PollyClient

> [Index](../README.md) > [Polly](./README.md) > PollyClient

!!! note ""

    Auto-generated documentation for [Polly](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#polly)
    type annotations stubs module [types-aiobotocore-polly](https://pypi.org/project/types-aiobotocore-polly/).

## PollyClient

Type annotations and code completion for `#!python session.client("polly")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client)

```python
# PollyClient usage example

from aioboto3.session import Session
from types_aiobotocore_polly.client import PollyClient

session = Session()
async with session.client("polly") as client:
    client: PollyClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("polly").exceptions` structure.

```python
# PollyClient.exceptions usage example

async with session.client("polly") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.EngineNotSupportedException,
        client.exceptions.InvalidLexiconException,
        client.exceptions.InvalidNextTokenException,
        client.exceptions.InvalidS3BucketException,
        client.exceptions.InvalidS3KeyException,
        client.exceptions.InvalidSampleRateException,
        client.exceptions.InvalidSnsTopicArnException,
        client.exceptions.InvalidSsmlException,
        client.exceptions.InvalidTaskIdException,
        client.exceptions.LanguageNotSupportedException,
        client.exceptions.LexiconNotFoundException,
        client.exceptions.LexiconSizeExceededException,
        client.exceptions.MarksNotSupportedForFormatException,
        client.exceptions.MaxLexemeLengthExceededException,
        client.exceptions.MaxLexiconsNumberExceededException,
        client.exceptions.ServiceFailureException,
        client.exceptions.SsmlMarksNotSupportedForTextTypeException,
        client.exceptions.SynthesisTaskNotFoundException,
        client.exceptions.TextLengthExceededException,
        client.exceptions.UnsupportedPlsAlphabetException,
        client.exceptions.UnsupportedPlsLanguageException,
    ) as e:
        print(e)
```

```python
# PollyClient.exceptions type checking example

from types_aiobotocore_polly.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("polly").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("polly").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client)

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


### delete\_lexicon

Deletes the specified pronunciation lexicon stored in an Amazon Web Services
Region.

Type annotations and code completion for `#!python session.client("polly").delete_lexicon` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client)

```python
# delete_lexicon method definition

await def delete_lexicon(
    self,
    *,
    Name: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_lexicon method usage example with argument unpacking

kwargs: DeleteLexiconInputRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_lexicon(**kwargs)
```

1. See [:material-code-braces: DeleteLexiconInputRequestTypeDef](./type_defs.md#deletelexiconinputrequesttypedef) 

### describe\_voices

Returns the list of voices that are available for use when requesting speech
synthesis.

Type annotations and code completion for `#!python session.client("polly").describe_voices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client)

```python
# describe_voices method definition

await def describe_voices(
    self,
    *,
    Engine: EngineType = ...,  # (1)
    LanguageCode: LanguageCodeType = ...,  # (2)
    IncludeAdditionalLanguageCodes: bool = ...,
    NextToken: str = ...,
) -> DescribeVoicesOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: EngineType](./literals.md#enginetype) 
2. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
3. See [:material-code-braces: DescribeVoicesOutputTypeDef](./type_defs.md#describevoicesoutputtypedef) 


```python
# describe_voices method usage example with argument unpacking

kwargs: DescribeVoicesInputRequestTypeDef = {  # (1)
    "Engine": ...,
}

parent.describe_voices(**kwargs)
```

1. See [:material-code-braces: DescribeVoicesInputRequestTypeDef](./type_defs.md#describevoicesinputrequesttypedef) 

### get\_lexicon

Returns the content of the specified pronunciation lexicon stored in an Amazon
Web Services Region.

Type annotations and code completion for `#!python session.client("polly").get_lexicon` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client)

```python
# get_lexicon method definition

await def get_lexicon(
    self,
    *,
    Name: str,
) -> GetLexiconOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLexiconOutputTypeDef](./type_defs.md#getlexiconoutputtypedef) 


```python
# get_lexicon method usage example with argument unpacking

kwargs: GetLexiconInputRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_lexicon(**kwargs)
```

1. See [:material-code-braces: GetLexiconInputRequestTypeDef](./type_defs.md#getlexiconinputrequesttypedef) 

### get\_speech\_synthesis\_task

Retrieves a specific SpeechSynthesisTask object based on its TaskID.

Type annotations and code completion for `#!python session.client("polly").get_speech_synthesis_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client)

```python
# get_speech_synthesis_task method definition

await def get_speech_synthesis_task(
    self,
    *,
    TaskId: str,
) -> GetSpeechSynthesisTaskOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSpeechSynthesisTaskOutputTypeDef](./type_defs.md#getspeechsynthesistaskoutputtypedef) 


```python
# get_speech_synthesis_task method usage example with argument unpacking

kwargs: GetSpeechSynthesisTaskInputRequestTypeDef = {  # (1)
    "TaskId": ...,
}

parent.get_speech_synthesis_task(**kwargs)
```

1. See [:material-code-braces: GetSpeechSynthesisTaskInputRequestTypeDef](./type_defs.md#getspeechsynthesistaskinputrequesttypedef) 

### list\_lexicons

Returns a list of pronunciation lexicons stored in an Amazon Web Services
Region.

Type annotations and code completion for `#!python session.client("polly").list_lexicons` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client)

```python
# list_lexicons method definition

await def list_lexicons(
    self,
    *,
    NextToken: str = ...,
) -> ListLexiconsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLexiconsOutputTypeDef](./type_defs.md#listlexiconsoutputtypedef) 


```python
# list_lexicons method usage example with argument unpacking

kwargs: ListLexiconsInputRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_lexicons(**kwargs)
```

1. See [:material-code-braces: ListLexiconsInputRequestTypeDef](./type_defs.md#listlexiconsinputrequesttypedef) 

### list\_speech\_synthesis\_tasks

Returns a list of SpeechSynthesisTask objects ordered by their creation date.

Type annotations and code completion for `#!python session.client("polly").list_speech_synthesis_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client)

```python
# list_speech_synthesis_tasks method definition

await def list_speech_synthesis_tasks(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    Status: TaskStatusType = ...,  # (1)
) -> ListSpeechSynthesisTasksOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
2. See [:material-code-braces: ListSpeechSynthesisTasksOutputTypeDef](./type_defs.md#listspeechsynthesistasksoutputtypedef) 


```python
# list_speech_synthesis_tasks method usage example with argument unpacking

kwargs: ListSpeechSynthesisTasksInputRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_speech_synthesis_tasks(**kwargs)
```

1. See [:material-code-braces: ListSpeechSynthesisTasksInputRequestTypeDef](./type_defs.md#listspeechsynthesistasksinputrequesttypedef) 

### put\_lexicon

Stores a pronunciation lexicon in an Amazon Web Services Region.

Type annotations and code completion for `#!python session.client("polly").put_lexicon` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client)

```python
# put_lexicon method definition

await def put_lexicon(
    self,
    *,
    Name: str,
    Content: str,
) -> dict[str, Any]:
    ...
```



```python
# put_lexicon method usage example with argument unpacking

kwargs: PutLexiconInputRequestTypeDef = {  # (1)
    "Name": ...,
    "Content": ...,
}

parent.put_lexicon(**kwargs)
```

1. See [:material-code-braces: PutLexiconInputRequestTypeDef](./type_defs.md#putlexiconinputrequesttypedef) 

### start\_speech\_synthesis\_task

Allows the creation of an asynchronous synthesis task, by starting a new
<code>SpeechSynthesisTask</code>.

Type annotations and code completion for `#!python session.client("polly").start_speech_synthesis_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client)

```python
# start_speech_synthesis_task method definition

await def start_speech_synthesis_task(
    self,
    *,
    OutputFormat: OutputFormatType,  # (1)
    OutputS3BucketName: str,
    Text: str,
    VoiceId: VoiceIdType,  # (2)
    Engine: EngineType = ...,  # (3)
    LanguageCode: LanguageCodeType = ...,  # (4)
    LexiconNames: Sequence[str] = ...,
    OutputS3KeyPrefix: str = ...,
    SampleRate: str = ...,
    SnsTopicArn: str = ...,
    SpeechMarkTypes: Sequence[SpeechMarkTypeType] = ...,  # (5)
    TextType: TextTypeType = ...,  # (6)
) -> StartSpeechSynthesisTaskOutputTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
2. See [:material-code-brackets: VoiceIdType](./literals.md#voiceidtype) 
3. See [:material-code-brackets: EngineType](./literals.md#enginetype) 
4. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
5. See [:material-code-brackets: SpeechMarkTypeType](./literals.md#speechmarktypetype) 
6. See [:material-code-brackets: TextTypeType](./literals.md#texttypetype) 
7. See [:material-code-braces: StartSpeechSynthesisTaskOutputTypeDef](./type_defs.md#startspeechsynthesistaskoutputtypedef) 


```python
# start_speech_synthesis_task method usage example with argument unpacking

kwargs: StartSpeechSynthesisTaskInputRequestTypeDef = {  # (1)
    "OutputFormat": ...,
    "OutputS3BucketName": ...,
    "Text": ...,
    "VoiceId": ...,
}

parent.start_speech_synthesis_task(**kwargs)
```

1. See [:material-code-braces: StartSpeechSynthesisTaskInputRequestTypeDef](./type_defs.md#startspeechsynthesistaskinputrequesttypedef) 

### synthesize\_speech

Synthesizes UTF-8 input, plain text or SSML, to a stream of bytes.

Type annotations and code completion for `#!python session.client("polly").synthesize_speech` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client)

```python
# synthesize_speech method definition

await def synthesize_speech(
    self,
    *,
    OutputFormat: OutputFormatType,  # (1)
    Text: str,
    VoiceId: VoiceIdType,  # (2)
    Engine: EngineType = ...,  # (3)
    LanguageCode: LanguageCodeType = ...,  # (4)
    LexiconNames: Sequence[str] = ...,
    SampleRate: str = ...,
    SpeechMarkTypes: Sequence[SpeechMarkTypeType] = ...,  # (5)
    TextType: TextTypeType = ...,  # (6)
) -> SynthesizeSpeechOutputTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
2. See [:material-code-brackets: VoiceIdType](./literals.md#voiceidtype) 
3. See [:material-code-brackets: EngineType](./literals.md#enginetype) 
4. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
5. See [:material-code-brackets: SpeechMarkTypeType](./literals.md#speechmarktypetype) 
6. See [:material-code-brackets: TextTypeType](./literals.md#texttypetype) 
7. See [:material-code-braces: SynthesizeSpeechOutputTypeDef](./type_defs.md#synthesizespeechoutputtypedef) 


```python
# synthesize_speech method usage example with argument unpacking

kwargs: SynthesizeSpeechInputRequestTypeDef = {  # (1)
    "OutputFormat": ...,
    "Text": ...,
    "VoiceId": ...,
}

parent.synthesize_speech(**kwargs)
```

1. See [:material-code-braces: SynthesizeSpeechInputRequestTypeDef](./type_defs.md#synthesizespeechinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("polly").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("polly").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client)

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

Type annotations and code completion for `#!python session.client("polly").get_paginator` method with overloads.

- `client.get_paginator("describe_voices")` -> [DescribeVoicesPaginator](./paginators.md#describevoicespaginator)
- `client.get_paginator("list_lexicons")` -> [ListLexiconsPaginator](./paginators.md#listlexiconspaginator)
- `client.get_paginator("list_speech_synthesis_tasks")` -> [ListSpeechSynthesisTasksPaginator](./paginators.md#listspeechsynthesistaskspaginator)


