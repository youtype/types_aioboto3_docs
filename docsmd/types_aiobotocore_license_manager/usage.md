# Examples

> [Index](../README.md) > [LicenseManager](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LicenseManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#licensemanager)
    type annotations stubs module [types-aiobotocore-license-manager](https://pypi.org/project/types-aiobotocore-license-manager/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[license-manager]` package installed.

Write your `LicenseManager` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# LicenseManagerClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("license-manager") as client:  # (1)
    result = await client.accept_grant()  # (2)
```

1. client: [LicenseManagerClient](./client.md)
2. result: [:material-code-braces: AcceptGrantResponseTypeDef](./type_defs.md#acceptgrantresponsetypedef)



#### Paginator usage example

```python
# ListAssociationsForLicenseConfigurationPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("license-manager") as client:  # (1)
    paginator = client.get_paginator("list_associations_for_license_configuration")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [LicenseManagerClient](./client.md)
2. paginator: [ListAssociationsForLicenseConfigurationPaginator](./paginators.md#listassociationsforlicenseconfigurationpaginator)
3. item: [:material-code-braces: ListAssociationsForLicenseConfigurationResponseTypeDef](./type_defs.md#listassociationsforlicenseconfigurationresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[license-manager]`
or a standalone `types_aiobotocore_license_manager` package, you have to explicitly specify
`client: LicenseManagerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# LicenseManagerClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_license_manager.client import LicenseManagerClient
from types_aiobotocore_license_manager.type_defs import AcceptGrantResponseTypeDef
from types_aiobotocore_license_manager.type_defs import AcceptGrantRequestTypeDef


session = Session()

client: LicenseManagerClient
async with session.client("license-manager") as client:  # (1)
    kwargs: AcceptGrantRequestTypeDef = {...}  # (2)
    result: AcceptGrantResponseTypeDef = await client.accept_grant(**kwargs)  # (3)
```

1. client: [LicenseManagerClient](./client.md)
2. kwargs: [:material-code-braces: AcceptGrantRequestTypeDef](./type_defs.md#acceptgrantrequesttypedef)
3. result: [:material-code-braces: AcceptGrantResponseTypeDef](./type_defs.md#acceptgrantresponsetypedef)



#### Paginator usage example

```python
# ListAssociationsForLicenseConfigurationPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_license_manager.client import LicenseManagerClient
from types_aiobotocore_license_manager.paginator import ListAssociationsForLicenseConfigurationPaginator
from types_aiobotocore_license_manager.type_defs import ListAssociationsForLicenseConfigurationResponseTypeDef


session = Session()

client: LicenseManagerClient
async with session.client("license-manager") as client:  # (1)
    paginator: ListAssociationsForLicenseConfigurationPaginator = client.get_paginator("list_associations_for_license_configuration")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssociationsForLicenseConfigurationResponseTypeDef
        print(item)  # (3)
```

1. client: [LicenseManagerClient](./client.md)
2. paginator: [ListAssociationsForLicenseConfigurationPaginator](./paginators.md#listassociationsforlicenseconfigurationpaginator)
3. item: [:material-code-braces: ListAssociationsForLicenseConfigurationResponseTypeDef](./type_defs.md#listassociationsforlicenseconfigurationresponsetypedef)




