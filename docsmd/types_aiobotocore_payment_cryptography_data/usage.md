# Examples

> [Index](../README.md) > [PaymentCryptographyDataPlane](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PaymentCryptographyDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#paymentcryptographydataplane)
    type annotations stubs module [types-aiobotocore-payment-cryptography-data](https://pypi.org/project/types-aiobotocore-payment-cryptography-data/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[payment-cryptography-data]` package installed.

Write your `PaymentCryptographyDataPlane` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# PaymentCryptographyDataPlaneClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("payment-cryptography-data") as client:  # (1)
    result = await client.decrypt_data()  # (2)
```

1. client: [PaymentCryptographyDataPlaneClient](./client.md)
2. result: [:material-code-braces: DecryptDataOutputTypeDef](./type_defs.md#decryptdataoutputtypedef)






### Explicit type annotations

With `types-aioboto3-lite[payment-cryptography-data]`
or a standalone `types_aiobotocore_payment_cryptography_data` package, you have to explicitly specify
`client: PaymentCryptographyDataPlaneClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# PaymentCryptographyDataPlaneClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_payment_cryptography_data.client import PaymentCryptographyDataPlaneClient
from types_aiobotocore_payment_cryptography_data.type_defs import DecryptDataOutputTypeDef
from types_aiobotocore_payment_cryptography_data.type_defs import DecryptDataInputTypeDef


session = Session()

client: PaymentCryptographyDataPlaneClient
async with session.client("payment-cryptography-data") as client:  # (1)
    kwargs: DecryptDataInputTypeDef = {...}  # (2)
    result: DecryptDataOutputTypeDef = await client.decrypt_data(**kwargs)  # (3)
```

1. client: [PaymentCryptographyDataPlaneClient](./client.md)
2. kwargs: [:material-code-braces: DecryptDataInputTypeDef](./type_defs.md#decryptdatainputtypedef)
3. result: [:material-code-braces: DecryptDataOutputTypeDef](./type_defs.md#decryptdataoutputtypedef)






