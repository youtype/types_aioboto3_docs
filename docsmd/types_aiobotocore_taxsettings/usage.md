# Examples

> [Index](../README.md) > [TaxSettings](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [TaxSettings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#taxsettings)
    type annotations stubs module [types-aiobotocore-taxsettings](https://pypi.org/project/types-aiobotocore-taxsettings/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[taxsettings]` package installed.

Write your `TaxSettings` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# TaxSettingsClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("taxsettings") as client:  # (1)
    result = await client.batch_delete_tax_registration()  # (2)
```

1. client: [TaxSettingsClient](./client.md)
2. result: [:material-code-braces: BatchDeleteTaxRegistrationResponseTypeDef](./type_defs.md#batchdeletetaxregistrationresponsetypedef)



#### Paginator usage example

```python
# ListSupplementalTaxRegistrationsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("taxsettings") as client:  # (1)
    paginator = client.get_paginator("list_supplemental_tax_registrations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [TaxSettingsClient](./client.md)
2. paginator: [ListSupplementalTaxRegistrationsPaginator](./paginators.md#listsupplementaltaxregistrationspaginator)
3. item: [:material-code-braces: ListSupplementalTaxRegistrationsResponseTypeDef](./type_defs.md#listsupplementaltaxregistrationsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[taxsettings]`
or a standalone `types_aiobotocore_taxsettings` package, you have to explicitly specify
`client: TaxSettingsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# TaxSettingsClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_taxsettings.client import TaxSettingsClient
from types_aiobotocore_taxsettings.type_defs import BatchDeleteTaxRegistrationResponseTypeDef
from types_aiobotocore_taxsettings.type_defs import BatchDeleteTaxRegistrationRequestTypeDef


session = Session()

client: TaxSettingsClient
async with session.client("taxsettings") as client:  # (1)
    kwargs: BatchDeleteTaxRegistrationRequestTypeDef = {...}  # (2)
    result: BatchDeleteTaxRegistrationResponseTypeDef = await client.batch_delete_tax_registration(**kwargs)  # (3)
```

1. client: [TaxSettingsClient](./client.md)
2. kwargs: [:material-code-braces: BatchDeleteTaxRegistrationRequestTypeDef](./type_defs.md#batchdeletetaxregistrationrequesttypedef)
3. result: [:material-code-braces: BatchDeleteTaxRegistrationResponseTypeDef](./type_defs.md#batchdeletetaxregistrationresponsetypedef)



#### Paginator usage example

```python
# ListSupplementalTaxRegistrationsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_taxsettings.client import TaxSettingsClient
from types_aiobotocore_taxsettings.paginator import ListSupplementalTaxRegistrationsPaginator
from types_aiobotocore_taxsettings.type_defs import ListSupplementalTaxRegistrationsResponseTypeDef


session = Session()

client: TaxSettingsClient
async with session.client("taxsettings") as client:  # (1)
    paginator: ListSupplementalTaxRegistrationsPaginator = client.get_paginator("list_supplemental_tax_registrations")  # (2)
    async for item in paginator.paginate(...):
        item: ListSupplementalTaxRegistrationsResponseTypeDef
        print(item)  # (3)
```

1. client: [TaxSettingsClient](./client.md)
2. paginator: [ListSupplementalTaxRegistrationsPaginator](./paginators.md#listsupplementaltaxregistrationspaginator)
3. item: [:material-code-braces: ListSupplementalTaxRegistrationsResponseTypeDef](./type_defs.md#listsupplementaltaxregistrationsresponsetypedef)




