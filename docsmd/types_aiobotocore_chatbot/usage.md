# Examples

> [Index](../README.md) > [Chatbot](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Chatbot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot)
    type annotations stubs module [types-aiobotocore-chatbot](https://pypi.org/project/types-aiobotocore-chatbot/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[chatbot]` package installed.

Write your `Chatbot` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ChatbotClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("chatbot") as client:  # (1)
    result = await client.create_chime_webhook_configuration()  # (2)
```

1. client: [ChatbotClient](./client.md)
2. result: [:material-code-braces: CreateChimeWebhookConfigurationResultTypeDef](./type_defs.md#createchimewebhookconfigurationresulttypedef)



#### Paginator usage example

```python
# DescribeChimeWebhookConfigurationsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("chatbot") as client:  # (1)
    paginator = client.get_paginator("describe_chime_webhook_configurations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ChatbotClient](./client.md)
2. paginator: [DescribeChimeWebhookConfigurationsPaginator](./paginators.md#describechimewebhookconfigurationspaginator)
3. item: [:material-code-braces: DescribeChimeWebhookConfigurationsResultTypeDef](./type_defs.md#describechimewebhookconfigurationsresulttypedef)




### Explicit type annotations

With `types-aioboto3-lite[chatbot]`
or a standalone `types_aiobotocore_chatbot` package, you have to explicitly specify
`client: ChatbotClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ChatbotClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_chatbot.client import ChatbotClient
from types_aiobotocore_chatbot.type_defs import CreateChimeWebhookConfigurationResultTypeDef
from types_aiobotocore_chatbot.type_defs import CreateChimeWebhookConfigurationRequestTypeDef


session = Session()

client: ChatbotClient
async with session.client("chatbot") as client:  # (1)
    kwargs: CreateChimeWebhookConfigurationRequestTypeDef = {...}  # (2)
    result: CreateChimeWebhookConfigurationResultTypeDef = await client.create_chime_webhook_configuration(**kwargs)  # (3)
```

1. client: [ChatbotClient](./client.md)
2. kwargs: [:material-code-braces: CreateChimeWebhookConfigurationRequestTypeDef](./type_defs.md#createchimewebhookconfigurationrequesttypedef)
3. result: [:material-code-braces: CreateChimeWebhookConfigurationResultTypeDef](./type_defs.md#createchimewebhookconfigurationresulttypedef)



#### Paginator usage example

```python
# DescribeChimeWebhookConfigurationsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_chatbot.client import ChatbotClient
from types_aiobotocore_chatbot.paginator import DescribeChimeWebhookConfigurationsPaginator
from types_aiobotocore_chatbot.type_defs import DescribeChimeWebhookConfigurationsResultTypeDef


session = Session()

client: ChatbotClient
async with session.client("chatbot") as client:  # (1)
    paginator: DescribeChimeWebhookConfigurationsPaginator = client.get_paginator("describe_chime_webhook_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeChimeWebhookConfigurationsResultTypeDef
        print(item)  # (3)
```

1. client: [ChatbotClient](./client.md)
2. paginator: [DescribeChimeWebhookConfigurationsPaginator](./paginators.md#describechimewebhookconfigurationspaginator)
3. item: [:material-code-braces: DescribeChimeWebhookConfigurationsResultTypeDef](./type_defs.md#describechimewebhookconfigurationsresulttypedef)




