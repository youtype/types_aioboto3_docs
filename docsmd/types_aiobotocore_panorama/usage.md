# Examples

> [Index](../README.md) > [Panorama](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Panorama](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#panorama)
    type annotations stubs module [types-aiobotocore-panorama](https://pypi.org/project/types-aiobotocore-panorama/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[panorama]` package installed.

Write your `Panorama` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# PanoramaClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("panorama") as client:  # (1)
    result = await client.create_application_instance()  # (2)
```

1. client: [PanoramaClient](./client.md)
2. result: [:material-code-braces: CreateApplicationInstanceResponseTypeDef](./type_defs.md#createapplicationinstanceresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[panorama]`
or a standalone `types_aiobotocore_panorama` package, you have to explicitly specify
`client: PanoramaClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# PanoramaClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_panorama.client import PanoramaClient
from types_aiobotocore_panorama.type_defs import CreateApplicationInstanceResponseTypeDef
from types_aiobotocore_panorama.type_defs import CreateApplicationInstanceRequestTypeDef


session = Session()

client: PanoramaClient
async with session.client("panorama") as client:  # (1)
    kwargs: CreateApplicationInstanceRequestTypeDef = {...}  # (2)
    result: CreateApplicationInstanceResponseTypeDef = await client.create_application_instance(**kwargs)  # (3)
```

1. client: [PanoramaClient](./client.md)
2. kwargs: [:material-code-braces: CreateApplicationInstanceRequestTypeDef](./type_defs.md#createapplicationinstancerequesttypedef)
3. result: [:material-code-braces: CreateApplicationInstanceResponseTypeDef](./type_defs.md#createapplicationinstanceresponsetypedef)






