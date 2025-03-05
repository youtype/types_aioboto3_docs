# Examples

> [Index](../README.md) > [Invoicing](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Invoicing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing.html#invoicing)
    type annotations stubs module [types-aiobotocore-invoicing](https://pypi.org/project/types-aiobotocore-invoicing/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[invoicing]` package installed.

Write your `Invoicing` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# InvoicingClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("invoicing") as client:  # (1)
    result = await client.batch_get_invoice_profile()  # (2)
```

1. client: [InvoicingClient](./client.md)
2. result: [:material-code-braces: BatchGetInvoiceProfileResponseTypeDef](./type_defs.md#batchgetinvoiceprofileresponsetypedef)



#### Paginator usage example

```python
# ListInvoiceUnitsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("invoicing") as client:  # (1)
    paginator = client.get_paginator("list_invoice_units")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [InvoicingClient](./client.md)
2. paginator: [ListInvoiceUnitsPaginator](./paginators.md#listinvoiceunitspaginator)
3. item: [:material-code-braces: ListInvoiceUnitsResponseTypeDef](./type_defs.md#listinvoiceunitsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[invoicing]`
or a standalone `types_aiobotocore_invoicing` package, you have to explicitly specify
`client: InvoicingClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# InvoicingClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_invoicing.client import InvoicingClient
from types_aiobotocore_invoicing.type_defs import BatchGetInvoiceProfileResponseTypeDef
from types_aiobotocore_invoicing.type_defs import BatchGetInvoiceProfileRequestTypeDef


session = Session()

client: InvoicingClient
async with session.client("invoicing") as client:  # (1)
    kwargs: BatchGetInvoiceProfileRequestTypeDef = {...}  # (2)
    result: BatchGetInvoiceProfileResponseTypeDef = await client.batch_get_invoice_profile(**kwargs)  # (3)
```

1. client: [InvoicingClient](./client.md)
2. kwargs: [:material-code-braces: BatchGetInvoiceProfileRequestTypeDef](./type_defs.md#batchgetinvoiceprofilerequesttypedef)
3. result: [:material-code-braces: BatchGetInvoiceProfileResponseTypeDef](./type_defs.md#batchgetinvoiceprofileresponsetypedef)



#### Paginator usage example

```python
# ListInvoiceUnitsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_invoicing.client import InvoicingClient
from types_aiobotocore_invoicing.paginator import ListInvoiceUnitsPaginator
from types_aiobotocore_invoicing.type_defs import ListInvoiceUnitsResponseTypeDef


session = Session()

client: InvoicingClient
async with session.client("invoicing") as client:  # (1)
    paginator: ListInvoiceUnitsPaginator = client.get_paginator("list_invoice_units")  # (2)
    async for item in paginator.paginate(...):
        item: ListInvoiceUnitsResponseTypeDef
        print(item)  # (3)
```

1. client: [InvoicingClient](./client.md)
2. paginator: [ListInvoiceUnitsPaginator](./paginators.md#listinvoiceunitspaginator)
3. item: [:material-code-braces: ListInvoiceUnitsResponseTypeDef](./type_defs.md#listinvoiceunitsresponsetypedef)




