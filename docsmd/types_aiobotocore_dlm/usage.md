# Examples

> [Index](../README.md) > [DLM](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DLM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#dlm)
    type annotations stubs module [types-aiobotocore-dlm](https://pypi.org/project/types-aiobotocore-dlm/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[dlm]` package installed.

Write your `DLM` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# DLMClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("dlm") as client:  # (1)
    result = await client.create_lifecycle_policy()  # (2)
```

1. client: [DLMClient](./client.md)
2. result: [:material-code-braces: CreateLifecyclePolicyResponseTypeDef](./type_defs.md#createlifecyclepolicyresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[dlm]`
or a standalone `types_aiobotocore_dlm` package, you have to explicitly specify
`client: DLMClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# DLMClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_dlm.client import DLMClient
from types_aiobotocore_dlm.type_defs import CreateLifecyclePolicyResponseTypeDef
from types_aiobotocore_dlm.type_defs import CreateLifecyclePolicyRequestTypeDef


session = Session()

client: DLMClient
async with session.client("dlm") as client:  # (1)
    kwargs: CreateLifecyclePolicyRequestTypeDef = {...}  # (2)
    result: CreateLifecyclePolicyResponseTypeDef = await client.create_lifecycle_policy(**kwargs)  # (3)
```

1. client: [DLMClient](./client.md)
2. kwargs: [:material-code-braces: CreateLifecyclePolicyRequestTypeDef](./type_defs.md#createlifecyclepolicyrequesttypedef)
3. result: [:material-code-braces: CreateLifecyclePolicyResponseTypeDef](./type_defs.md#createlifecyclepolicyresponsetypedef)






