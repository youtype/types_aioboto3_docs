# Examples

> [Index](../README.md) > [PersonalizeRuntime](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PersonalizeRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#personalizeruntime)
    type annotations stubs module [types-aiobotocore-personalize-runtime](https://pypi.org/project/types-aiobotocore-personalize-runtime/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[personalize-runtime]` package installed.

Write your `PersonalizeRuntime` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# PersonalizeRuntimeClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("personalize-runtime") as client:  # (1)
    result = await client.get_action_recommendations()  # (2)
```

1. client: [PersonalizeRuntimeClient](./client.md)
2. result: [:material-code-braces: GetActionRecommendationsResponseTypeDef](./type_defs.md#getactionrecommendationsresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[personalize-runtime]`
or a standalone `types_aiobotocore_personalize_runtime` package, you have to explicitly specify
`client: PersonalizeRuntimeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# PersonalizeRuntimeClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_personalize_runtime.client import PersonalizeRuntimeClient
from types_aiobotocore_personalize_runtime.type_defs import GetActionRecommendationsResponseTypeDef
from types_aiobotocore_personalize_runtime.type_defs import GetActionRecommendationsRequestTypeDef


session = Session()

client: PersonalizeRuntimeClient
async with session.client("personalize-runtime") as client:  # (1)
    kwargs: GetActionRecommendationsRequestTypeDef = {...}  # (2)
    result: GetActionRecommendationsResponseTypeDef = await client.get_action_recommendations(**kwargs)  # (3)
```

1. client: [PersonalizeRuntimeClient](./client.md)
2. kwargs: [:material-code-braces: GetActionRecommendationsRequestTypeDef](./type_defs.md#getactionrecommendationsrequesttypedef)
3. result: [:material-code-braces: GetActionRecommendationsResponseTypeDef](./type_defs.md#getactionrecommendationsresponsetypedef)






