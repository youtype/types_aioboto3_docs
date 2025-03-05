# Examples

> [Index](../README.md) > [Imagebuilder](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Imagebuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
    type annotations stubs module [types-aiobotocore-imagebuilder](https://pypi.org/project/types-aiobotocore-imagebuilder/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[imagebuilder]` package installed.

Write your `Imagebuilder` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ImagebuilderClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("imagebuilder") as client:  # (1)
    result = await client.cancel_image_creation()  # (2)
```

1. client: [ImagebuilderClient](./client.md)
2. result: [:material-code-braces: CancelImageCreationResponseTypeDef](./type_defs.md#cancelimagecreationresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[imagebuilder]`
or a standalone `types_aiobotocore_imagebuilder` package, you have to explicitly specify
`client: ImagebuilderClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ImagebuilderClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_imagebuilder.client import ImagebuilderClient
from types_aiobotocore_imagebuilder.type_defs import CancelImageCreationResponseTypeDef
from types_aiobotocore_imagebuilder.type_defs import CancelImageCreationRequestTypeDef


session = Session()

client: ImagebuilderClient
async with session.client("imagebuilder") as client:  # (1)
    kwargs: CancelImageCreationRequestTypeDef = {...}  # (2)
    result: CancelImageCreationResponseTypeDef = await client.cancel_image_creation(**kwargs)  # (3)
```

1. client: [ImagebuilderClient](./client.md)
2. kwargs: [:material-code-braces: CancelImageCreationRequestTypeDef](./type_defs.md#cancelimagecreationrequesttypedef)
3. result: [:material-code-braces: CancelImageCreationResponseTypeDef](./type_defs.md#cancelimagecreationresponsetypedef)






