# Examples

> [Index](../README.md) > [ChimeSDKVoice](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ChimeSDKVoice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#chimesdkvoice)
    type annotations stubs module [types-aiobotocore-chime-sdk-voice](https://pypi.org/project/types-aiobotocore-chime-sdk-voice/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[chime-sdk-voice]` package installed.

Write your `ChimeSDKVoice` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ChimeSDKVoiceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("chime-sdk-voice") as client:  # (1)
    result = await client.associate_phone_numbers_with_voice_connector()  # (2)
```

1. client: [ChimeSDKVoiceClient](./client.md)
2. result: [:material-code-braces: AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef](./type_defs.md#associatephonenumberswithvoiceconnectorresponsetypedef)



#### Paginator usage example

```python
# ListSipMediaApplicationsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("chime-sdk-voice") as client:  # (1)
    paginator = client.get_paginator("list_sip_media_applications")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ChimeSDKVoiceClient](./client.md)
2. paginator: [ListSipMediaApplicationsPaginator](./paginators.md#listsipmediaapplicationspaginator)
3. item: [:material-code-braces: ListSipMediaApplicationsResponseTypeDef](./type_defs.md#listsipmediaapplicationsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[chime-sdk-voice]`
or a standalone `types_aiobotocore_chime_sdk_voice` package, you have to explicitly specify
`client: ChimeSDKVoiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ChimeSDKVoiceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_chime_sdk_voice.client import ChimeSDKVoiceClient
from types_aiobotocore_chime_sdk_voice.type_defs import AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef
from types_aiobotocore_chime_sdk_voice.type_defs import AssociatePhoneNumbersWithVoiceConnectorRequestTypeDef


session = Session()

client: ChimeSDKVoiceClient
async with session.client("chime-sdk-voice") as client:  # (1)
    kwargs: AssociatePhoneNumbersWithVoiceConnectorRequestTypeDef = {...}  # (2)
    result: AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef = await client.associate_phone_numbers_with_voice_connector(**kwargs)  # (3)
```

1. client: [ChimeSDKVoiceClient](./client.md)
2. kwargs: [:material-code-braces: AssociatePhoneNumbersWithVoiceConnectorRequestTypeDef](./type_defs.md#associatephonenumberswithvoiceconnectorrequesttypedef)
3. result: [:material-code-braces: AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef](./type_defs.md#associatephonenumberswithvoiceconnectorresponsetypedef)



#### Paginator usage example

```python
# ListSipMediaApplicationsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_chime_sdk_voice.client import ChimeSDKVoiceClient
from types_aiobotocore_chime_sdk_voice.paginator import ListSipMediaApplicationsPaginator
from types_aiobotocore_chime_sdk_voice.type_defs import ListSipMediaApplicationsResponseTypeDef


session = Session()

client: ChimeSDKVoiceClient
async with session.client("chime-sdk-voice") as client:  # (1)
    paginator: ListSipMediaApplicationsPaginator = client.get_paginator("list_sip_media_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListSipMediaApplicationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ChimeSDKVoiceClient](./client.md)
2. paginator: [ListSipMediaApplicationsPaginator](./paginators.md#listsipmediaapplicationspaginator)
3. item: [:material-code-braces: ListSipMediaApplicationsResponseTypeDef](./type_defs.md#listsipmediaapplicationsresponsetypedef)




