# Examples

> [Index](../README.md) > [QConnect](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [QConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#qconnect)
    type annotations stubs module [types-aiobotocore-qconnect](https://pypi.org/project/types-aiobotocore-qconnect/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[qconnect]` package installed.

Write your `QConnect` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# QConnectClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("qconnect") as client:  # (1)
    result = await client.activate_message_template()  # (2)
```

1. client: [QConnectClient](./client.md)
2. result: [:material-code-braces: ActivateMessageTemplateResponseTypeDef](./type_defs.md#activatemessagetemplateresponsetypedef)



#### Paginator usage example

```python
# ListAIAgentVersionsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("qconnect") as client:  # (1)
    paginator = client.get_paginator("list_ai_agent_versions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListAIAgentVersionsPaginator](./paginators.md#listaiagentversionspaginator)
3. item: [:material-code-braces: ListAIAgentVersionsResponseTypeDef](./type_defs.md#listaiagentversionsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[qconnect]`
or a standalone `types_aiobotocore_qconnect` package, you have to explicitly specify
`client: QConnectClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# QConnectClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_qconnect.client import QConnectClient
from types_aiobotocore_qconnect.type_defs import ActivateMessageTemplateResponseTypeDef
from types_aiobotocore_qconnect.type_defs import ActivateMessageTemplateRequestTypeDef


session = Session()

client: QConnectClient
async with session.client("qconnect") as client:  # (1)
    kwargs: ActivateMessageTemplateRequestTypeDef = {...}  # (2)
    result: ActivateMessageTemplateResponseTypeDef = await client.activate_message_template(**kwargs)  # (3)
```

1. client: [QConnectClient](./client.md)
2. kwargs: [:material-code-braces: ActivateMessageTemplateRequestTypeDef](./type_defs.md#activatemessagetemplaterequesttypedef)
3. result: [:material-code-braces: ActivateMessageTemplateResponseTypeDef](./type_defs.md#activatemessagetemplateresponsetypedef)



#### Paginator usage example

```python
# ListAIAgentVersionsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_qconnect.client import QConnectClient
from types_aiobotocore_qconnect.paginator import ListAIAgentVersionsPaginator
from types_aiobotocore_qconnect.type_defs import ListAIAgentVersionsResponseTypeDef


session = Session()

client: QConnectClient
async with session.client("qconnect") as client:  # (1)
    paginator: ListAIAgentVersionsPaginator = client.get_paginator("list_ai_agent_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListAIAgentVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListAIAgentVersionsPaginator](./paginators.md#listaiagentversionspaginator)
3. item: [:material-code-braces: ListAIAgentVersionsResponseTypeDef](./type_defs.md#listaiagentversionsresponsetypedef)




