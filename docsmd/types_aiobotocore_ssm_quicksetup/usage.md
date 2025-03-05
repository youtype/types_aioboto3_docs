# Examples

> [Index](../README.md) > [SystemsManagerQuickSetup](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SystemsManagerQuickSetup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#systemsmanagerquicksetup)
    type annotations stubs module [types-aiobotocore-ssm-quicksetup](https://pypi.org/project/types-aiobotocore-ssm-quicksetup/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[ssm-quicksetup]` package installed.

Write your `SystemsManagerQuickSetup` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SystemsManagerQuickSetupClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("ssm-quicksetup") as client:  # (1)
    result = await client.create_configuration_manager()  # (2)
```

1. client: [SystemsManagerQuickSetupClient](./client.md)
2. result: [:material-code-braces: CreateConfigurationManagerOutputTypeDef](./type_defs.md#createconfigurationmanageroutputtypedef)



#### Paginator usage example

```python
# ListConfigurationManagersPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("ssm-quicksetup") as client:  # (1)
    paginator = client.get_paginator("list_configuration_managers")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SystemsManagerQuickSetupClient](./client.md)
2. paginator: [ListConfigurationManagersPaginator](./paginators.md#listconfigurationmanagerspaginator)
3. item: [:material-code-braces: ListConfigurationManagersOutputTypeDef](./type_defs.md#listconfigurationmanagersoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[ssm-quicksetup]`
or a standalone `types_aiobotocore_ssm_quicksetup` package, you have to explicitly specify
`client: SystemsManagerQuickSetupClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SystemsManagerQuickSetupClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ssm_quicksetup.client import SystemsManagerQuickSetupClient
from types_aiobotocore_ssm_quicksetup.type_defs import CreateConfigurationManagerOutputTypeDef
from types_aiobotocore_ssm_quicksetup.type_defs import CreateConfigurationManagerInputTypeDef


session = Session()

client: SystemsManagerQuickSetupClient
async with session.client("ssm-quicksetup") as client:  # (1)
    kwargs: CreateConfigurationManagerInputTypeDef = {...}  # (2)
    result: CreateConfigurationManagerOutputTypeDef = await client.create_configuration_manager(**kwargs)  # (3)
```

1. client: [SystemsManagerQuickSetupClient](./client.md)
2. kwargs: [:material-code-braces: CreateConfigurationManagerInputTypeDef](./type_defs.md#createconfigurationmanagerinputtypedef)
3. result: [:material-code-braces: CreateConfigurationManagerOutputTypeDef](./type_defs.md#createconfigurationmanageroutputtypedef)



#### Paginator usage example

```python
# ListConfigurationManagersPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ssm_quicksetup.client import SystemsManagerQuickSetupClient
from types_aiobotocore_ssm_quicksetup.paginator import ListConfigurationManagersPaginator
from types_aiobotocore_ssm_quicksetup.type_defs import ListConfigurationManagersOutputTypeDef


session = Session()

client: SystemsManagerQuickSetupClient
async with session.client("ssm-quicksetup") as client:  # (1)
    paginator: ListConfigurationManagersPaginator = client.get_paginator("list_configuration_managers")  # (2)
    async for item in paginator.paginate(...):
        item: ListConfigurationManagersOutputTypeDef
        print(item)  # (3)
```

1. client: [SystemsManagerQuickSetupClient](./client.md)
2. paginator: [ListConfigurationManagersPaginator](./paginators.md#listconfigurationmanagerspaginator)
3. item: [:material-code-braces: ListConfigurationManagersOutputTypeDef](./type_defs.md#listconfigurationmanagersoutputtypedef)




