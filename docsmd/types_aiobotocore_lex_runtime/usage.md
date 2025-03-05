# Examples

> [Index](../README.md) > [LexRuntimeService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LexRuntimeService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#lexruntimeservice)
    type annotations stubs module [types-aiobotocore-lex-runtime](https://pypi.org/project/types-aiobotocore-lex-runtime/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[lex-runtime]` package installed.

Write your `LexRuntimeService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# LexRuntimeServiceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("lex-runtime") as client:  # (1)
    result = await client.delete_session()  # (2)
```

1. client: [LexRuntimeServiceClient](./client.md)
2. result: [:material-code-braces: DeleteSessionResponseTypeDef](./type_defs.md#deletesessionresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[lex-runtime]`
or a standalone `types_aiobotocore_lex_runtime` package, you have to explicitly specify
`client: LexRuntimeServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# LexRuntimeServiceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_lex_runtime.client import LexRuntimeServiceClient
from types_aiobotocore_lex_runtime.type_defs import DeleteSessionResponseTypeDef
from types_aiobotocore_lex_runtime.type_defs import DeleteSessionRequestTypeDef


session = Session()

client: LexRuntimeServiceClient
async with session.client("lex-runtime") as client:  # (1)
    kwargs: DeleteSessionRequestTypeDef = {...}  # (2)
    result: DeleteSessionResponseTypeDef = await client.delete_session(**kwargs)  # (3)
```

1. client: [LexRuntimeServiceClient](./client.md)
2. kwargs: [:material-code-braces: DeleteSessionRequestTypeDef](./type_defs.md#deletesessionrequesttypedef)
3. result: [:material-code-braces: DeleteSessionResponseTypeDef](./type_defs.md#deletesessionresponsetypedef)






