# Examples

> [Index](../README.md) > [VoiceID](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [VoiceID](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#voiceid)
    type annotations stubs module [types-aiobotocore-voice-id](https://pypi.org/project/types-aiobotocore-voice-id/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[voice-id]` package installed.

Write your `VoiceID` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# VoiceIDClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("voice-id") as client:  # (1)
    result = await client.associate_fraudster()  # (2)
```

1. client: [VoiceIDClient](./client.md)
2. result: [:material-code-braces: AssociateFraudsterResponseTypeDef](./type_defs.md#associatefraudsterresponsetypedef)



#### Paginator usage example

```python
# ListDomainsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("voice-id") as client:  # (1)
    paginator = client.get_paginator("list_domains")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [VoiceIDClient](./client.md)
2. paginator: [ListDomainsPaginator](./paginators.md#listdomainspaginator)
3. item: [:material-code-braces: ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[voice-id]`
or a standalone `types_aiobotocore_voice_id` package, you have to explicitly specify
`client: VoiceIDClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# VoiceIDClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_voice_id.client import VoiceIDClient
from types_aiobotocore_voice_id.type_defs import AssociateFraudsterResponseTypeDef
from types_aiobotocore_voice_id.type_defs import AssociateFraudsterRequestTypeDef


session = Session()

client: VoiceIDClient
async with session.client("voice-id") as client:  # (1)
    kwargs: AssociateFraudsterRequestTypeDef = {...}  # (2)
    result: AssociateFraudsterResponseTypeDef = await client.associate_fraudster(**kwargs)  # (3)
```

1. client: [VoiceIDClient](./client.md)
2. kwargs: [:material-code-braces: AssociateFraudsterRequestTypeDef](./type_defs.md#associatefraudsterrequesttypedef)
3. result: [:material-code-braces: AssociateFraudsterResponseTypeDef](./type_defs.md#associatefraudsterresponsetypedef)



#### Paginator usage example

```python
# ListDomainsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_voice_id.client import VoiceIDClient
from types_aiobotocore_voice_id.paginator import ListDomainsPaginator
from types_aiobotocore_voice_id.type_defs import ListDomainsResponseTypeDef


session = Session()

client: VoiceIDClient
async with session.client("voice-id") as client:  # (1)
    paginator: ListDomainsPaginator = client.get_paginator("list_domains")  # (2)
    async for item in paginator.paginate(...):
        item: ListDomainsResponseTypeDef
        print(item)  # (3)
```

1. client: [VoiceIDClient](./client.md)
2. paginator: [ListDomainsPaginator](./paginators.md#listdomainspaginator)
3. item: [:material-code-braces: ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef)




