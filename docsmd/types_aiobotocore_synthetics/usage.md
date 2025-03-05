# Examples

> [Index](../README.md) > [Synthetics](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Synthetics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#synthetics)
    type annotations stubs module [types-aiobotocore-synthetics](https://pypi.org/project/types-aiobotocore-synthetics/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[synthetics]` package installed.

Write your `Synthetics` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SyntheticsClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("synthetics") as client:  # (1)
    result = await client.create_canary()  # (2)
```

1. client: [SyntheticsClient](./client.md)
2. result: [:material-code-braces: CreateCanaryResponseTypeDef](./type_defs.md#createcanaryresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[synthetics]`
or a standalone `types_aiobotocore_synthetics` package, you have to explicitly specify
`client: SyntheticsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SyntheticsClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_synthetics.client import SyntheticsClient
from types_aiobotocore_synthetics.type_defs import CreateCanaryResponseTypeDef
from types_aiobotocore_synthetics.type_defs import CreateCanaryRequestTypeDef


session = Session()

client: SyntheticsClient
async with session.client("synthetics") as client:  # (1)
    kwargs: CreateCanaryRequestTypeDef = {...}  # (2)
    result: CreateCanaryResponseTypeDef = await client.create_canary(**kwargs)  # (3)
```

1. client: [SyntheticsClient](./client.md)
2. kwargs: [:material-code-braces: CreateCanaryRequestTypeDef](./type_defs.md#createcanaryrequesttypedef)
3. result: [:material-code-braces: CreateCanaryResponseTypeDef](./type_defs.md#createcanaryresponsetypedef)






