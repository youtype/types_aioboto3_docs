# Examples

> [Index](../README.md) > [WellArchitected](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WellArchitected](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#wellarchitected)
    type annotations stubs module [types-aiobotocore-wellarchitected](https://pypi.org/project/types-aiobotocore-wellarchitected/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[wellarchitected]` package installed.

Write your `WellArchitected` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# WellArchitectedClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("wellarchitected") as client:  # (1)
    result = await client.associate_lenses()  # (2)
```

1. client: [WellArchitectedClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)






### Explicit type annotations

With `types-aioboto3-lite[wellarchitected]`
or a standalone `types_aiobotocore_wellarchitected` package, you have to explicitly specify
`client: WellArchitectedClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# WellArchitectedClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_wellarchitected.client import WellArchitectedClient
from types_aiobotocore_wellarchitected.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_wellarchitected.type_defs import AssociateLensesInputTypeDef


session = Session()

client: WellArchitectedClient
async with session.client("wellarchitected") as client:  # (1)
    kwargs: AssociateLensesInputTypeDef = {...}  # (2)
    result: EmptyResponseMetadataTypeDef = await client.associate_lenses(**kwargs)  # (3)
```

1. client: [WellArchitectedClient](./client.md)
2. kwargs: [:material-code-braces: AssociateLensesInputTypeDef](./type_defs.md#associatelensesinputtypedef)
3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)






