# Examples

> [Index](../README.md) > [SupplyChain](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SupplyChain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain)
    type annotations stubs module [types-aiobotocore-supplychain](https://pypi.org/project/types-aiobotocore-supplychain/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[supplychain]` package installed.

Write your `SupplyChain` code as usual,
type checking and code completion should work out of the box.



```python
# SupplyChainClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("supplychain") as client:  # (1)
    result = await client.create_bill_of_materials_import_job()  # (2)
```

1. client: [SupplyChainClient](./client.md)
2. result: [:material-code-braces: CreateBillOfMaterialsImportJobResponseTypeDef](./type_defs.md#createbillofmaterialsimportjobresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[supplychain]`
or a standalone `types_aiobotocore_supplychain` package, you have to explicitly specify
`client: SupplyChainClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SupplyChainClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_supplychain.client import SupplyChainClient
from types_aiobotocore_supplychain.type_defs import CreateBillOfMaterialsImportJobResponseTypeDef
from types_aiobotocore_supplychain.type_defs import CreateBillOfMaterialsImportJobRequestRequestTypeDef


session = Session()

client: SupplyChainClient
async with session.client("supplychain") as client:  # (1)
    kwargs: CreateBillOfMaterialsImportJobRequestRequestTypeDef = {...}  # (2)
    result: CreateBillOfMaterialsImportJobResponseTypeDef = await client.create_bill_of_materials_import_job(**kwargs)  # (3)
```

1. client: [SupplyChainClient](./client.md)
2. kwargs: [:material-code-braces: CreateBillOfMaterialsImportJobRequestRequestTypeDef](./type_defs.md#createbillofmaterialsimportjobrequestrequesttypedef) 
3. result: [:material-code-braces: CreateBillOfMaterialsImportJobResponseTypeDef](./type_defs.md#createbillofmaterialsimportjobresponsetypedef) 






