# Examples

> [Index](../README.md) > [Pinpoint](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Pinpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#pinpoint)
    type annotations stubs module [types-aiobotocore-pinpoint](https://pypi.org/project/types-aiobotocore-pinpoint/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[pinpoint]` package installed.

Write your `Pinpoint` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# PinpointClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("pinpoint") as client:  # (1)
    result = await client.create_app()  # (2)
```

1. client: [PinpointClient](./client.md)
2. result: [:material-code-braces: CreateAppResponseTypeDef](./type_defs.md#createappresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[pinpoint]`
or a standalone `types_aiobotocore_pinpoint` package, you have to explicitly specify
`client: PinpointClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# PinpointClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_pinpoint.client import PinpointClient
from types_aiobotocore_pinpoint.type_defs import CreateAppResponseTypeDef
from types_aiobotocore_pinpoint.type_defs import CreateAppRequestTypeDef


session = Session()

client: PinpointClient
async with session.client("pinpoint") as client:  # (1)
    kwargs: CreateAppRequestTypeDef = {...}  # (2)
    result: CreateAppResponseTypeDef = await client.create_app(**kwargs)  # (3)
```

1. client: [PinpointClient](./client.md)
2. kwargs: [:material-code-braces: CreateAppRequestTypeDef](./type_defs.md#createapprequesttypedef)
3. result: [:material-code-braces: CreateAppResponseTypeDef](./type_defs.md#createappresponsetypedef)






