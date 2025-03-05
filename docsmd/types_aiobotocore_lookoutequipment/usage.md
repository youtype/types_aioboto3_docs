# Examples

> [Index](../README.md) > [LookoutEquipment](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LookoutEquipment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#lookoutequipment)
    type annotations stubs module [types-aiobotocore-lookoutequipment](https://pypi.org/project/types-aiobotocore-lookoutequipment/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[lookoutequipment]` package installed.

Write your `LookoutEquipment` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# LookoutEquipmentClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("lookoutequipment") as client:  # (1)
    result = await client.create_dataset()  # (2)
```

1. client: [LookoutEquipmentClient](./client.md)
2. result: [:material-code-braces: CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[lookoutequipment]`
or a standalone `types_aiobotocore_lookoutequipment` package, you have to explicitly specify
`client: LookoutEquipmentClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# LookoutEquipmentClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_lookoutequipment.client import LookoutEquipmentClient
from types_aiobotocore_lookoutequipment.type_defs import CreateDatasetResponseTypeDef
from types_aiobotocore_lookoutequipment.type_defs import CreateDatasetRequestTypeDef


session = Session()

client: LookoutEquipmentClient
async with session.client("lookoutequipment") as client:  # (1)
    kwargs: CreateDatasetRequestTypeDef = {...}  # (2)
    result: CreateDatasetResponseTypeDef = await client.create_dataset(**kwargs)  # (3)
```

1. client: [LookoutEquipmentClient](./client.md)
2. kwargs: [:material-code-braces: CreateDatasetRequestTypeDef](./type_defs.md#createdatasetrequesttypedef)
3. result: [:material-code-braces: CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef)






