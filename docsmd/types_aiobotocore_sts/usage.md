# Examples

> [Index](../README.md) > [STS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [STS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#sts)
    type annotations stubs module [types-aiobotocore-sts](https://pypi.org/project/types-aiobotocore-sts/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[sts]` package installed.

Write your `STS` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# STSClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("sts") as client:  # (1)
    result = await client.assume_role()  # (2)
```

1. client: [STSClient](./client.md)
2. result: [:material-code-braces: AssumeRoleResponseTypeDef](./type_defs.md#assumeroleresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[sts]`
or a standalone `types_aiobotocore_sts` package, you have to explicitly specify
`client: STSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# STSClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_sts.client import STSClient
from types_aiobotocore_sts.type_defs import AssumeRoleResponseTypeDef
from types_aiobotocore_sts.type_defs import AssumeRoleRequestTypeDef


session = Session()

client: STSClient
async with session.client("sts") as client:  # (1)
    kwargs: AssumeRoleRequestTypeDef = {...}  # (2)
    result: AssumeRoleResponseTypeDef = await client.assume_role(**kwargs)  # (3)
```

1. client: [STSClient](./client.md)
2. kwargs: [:material-code-braces: AssumeRoleRequestTypeDef](./type_defs.md#assumerolerequesttypedef)
3. result: [:material-code-braces: AssumeRoleResponseTypeDef](./type_defs.md#assumeroleresponsetypedef)






