# Examples

> [Index](../README.md) > [SupportApp](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SupportApp](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#supportapp)
    type annotations stubs module [types-aiobotocore-support-app](https://pypi.org/project/types-aiobotocore-support-app/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[support-app]` package installed.

Write your `SupportApp` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SupportAppClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("support-app") as client:  # (1)
    result = await client.list_slack_channel_configurations()  # (2)
```

1. client: [SupportAppClient](./client.md)
2. result: [:material-code-braces: ListSlackChannelConfigurationsResultTypeDef](./type_defs.md#listslackchannelconfigurationsresulttypedef)






### Explicit type annotations

With `types-aioboto3-lite[support-app]`
or a standalone `types_aiobotocore_support_app` package, you have to explicitly specify
`client: SupportAppClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SupportAppClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_support_app.client import SupportAppClient
from types_aiobotocore_support_app.type_defs import ListSlackChannelConfigurationsResultTypeDef
from types_aiobotocore_support_app.type_defs import ListSlackChannelConfigurationsRequestTypeDef


session = Session()

client: SupportAppClient
async with session.client("support-app") as client:  # (1)
    kwargs: ListSlackChannelConfigurationsRequestTypeDef = {...}  # (2)
    result: ListSlackChannelConfigurationsResultTypeDef = await client.list_slack_channel_configurations(**kwargs)  # (3)
```

1. client: [SupportAppClient](./client.md)
2. kwargs: [:material-code-braces: ListSlackChannelConfigurationsRequestTypeDef](./type_defs.md#listslackchannelconfigurationsrequesttypedef)
3. result: [:material-code-braces: ListSlackChannelConfigurationsResultTypeDef](./type_defs.md#listslackchannelconfigurationsresulttypedef)






