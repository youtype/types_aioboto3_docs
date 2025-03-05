# Examples

> [Index](../README.md) > [AgreementService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AgreementService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#agreementservice)
    type annotations stubs module [types-aiobotocore-marketplace-agreement](https://pypi.org/project/types-aiobotocore-marketplace-agreement/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[marketplace-agreement]` package installed.

Write your `AgreementService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# AgreementServiceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("marketplace-agreement") as client:  # (1)
    result = await client.describe_agreement()  # (2)
```

1. client: [AgreementServiceClient](./client.md)
2. result: [:material-code-braces: DescribeAgreementOutputTypeDef](./type_defs.md#describeagreementoutputtypedef)






### Explicit type annotations

With `types-aioboto3-lite[marketplace-agreement]`
or a standalone `types_aiobotocore_marketplace_agreement` package, you have to explicitly specify
`client: AgreementServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# AgreementServiceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_marketplace_agreement.client import AgreementServiceClient
from types_aiobotocore_marketplace_agreement.type_defs import DescribeAgreementOutputTypeDef
from types_aiobotocore_marketplace_agreement.type_defs import DescribeAgreementInputTypeDef


session = Session()

client: AgreementServiceClient
async with session.client("marketplace-agreement") as client:  # (1)
    kwargs: DescribeAgreementInputTypeDef = {...}  # (2)
    result: DescribeAgreementOutputTypeDef = await client.describe_agreement(**kwargs)  # (3)
```

1. client: [AgreementServiceClient](./client.md)
2. kwargs: [:material-code-braces: DescribeAgreementInputTypeDef](./type_defs.md#describeagreementinputtypedef)
3. result: [:material-code-braces: DescribeAgreementOutputTypeDef](./type_defs.md#describeagreementoutputtypedef)






