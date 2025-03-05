# Examples

> [Index](../README.md) > [ChimeSDKIdentity](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ChimeSDKIdentity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#chimesdkidentity)
    type annotations stubs module [types-aiobotocore-chime-sdk-identity](https://pypi.org/project/types-aiobotocore-chime-sdk-identity/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[chime-sdk-identity]` package installed.

Write your `ChimeSDKIdentity` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ChimeSDKIdentityClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("chime-sdk-identity") as client:  # (1)
    result = await client.create_app_instance()  # (2)
```

1. client: [ChimeSDKIdentityClient](./client.md)
2. result: [:material-code-braces: CreateAppInstanceResponseTypeDef](./type_defs.md#createappinstanceresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[chime-sdk-identity]`
or a standalone `types_aiobotocore_chime_sdk_identity` package, you have to explicitly specify
`client: ChimeSDKIdentityClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ChimeSDKIdentityClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_chime_sdk_identity.client import ChimeSDKIdentityClient
from types_aiobotocore_chime_sdk_identity.type_defs import CreateAppInstanceResponseTypeDef
from types_aiobotocore_chime_sdk_identity.type_defs import CreateAppInstanceRequestTypeDef


session = Session()

client: ChimeSDKIdentityClient
async with session.client("chime-sdk-identity") as client:  # (1)
    kwargs: CreateAppInstanceRequestTypeDef = {...}  # (2)
    result: CreateAppInstanceResponseTypeDef = await client.create_app_instance(**kwargs)  # (3)
```

1. client: [ChimeSDKIdentityClient](./client.md)
2. kwargs: [:material-code-braces: CreateAppInstanceRequestTypeDef](./type_defs.md#createappinstancerequesttypedef)
3. result: [:material-code-braces: CreateAppInstanceResponseTypeDef](./type_defs.md#createappinstanceresponsetypedef)






