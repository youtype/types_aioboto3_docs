# Examples

> [Index](../README.md) > [LaunchWizard](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LaunchWizard](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#launchwizard)
    type annotations stubs module [types-aiobotocore-launch-wizard](https://pypi.org/project/types-aiobotocore-launch-wizard/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[launch-wizard]` package installed.

Write your `LaunchWizard` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# LaunchWizardClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("launch-wizard") as client:  # (1)
    result = await client.create_deployment()  # (2)
```

1. client: [LaunchWizardClient](./client.md)
2. result: [:material-code-braces: CreateDeploymentOutputTypeDef](./type_defs.md#createdeploymentoutputtypedef)



#### Paginator usage example

```python
# ListDeploymentEventsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("launch-wizard") as client:  # (1)
    paginator = client.get_paginator("list_deployment_events")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [LaunchWizardClient](./client.md)
2. paginator: [ListDeploymentEventsPaginator](./paginators.md#listdeploymenteventspaginator)
3. item: [:material-code-braces: ListDeploymentEventsOutputTypeDef](./type_defs.md#listdeploymenteventsoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[launch-wizard]`
or a standalone `types_aiobotocore_launch_wizard` package, you have to explicitly specify
`client: LaunchWizardClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# LaunchWizardClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_launch_wizard.client import LaunchWizardClient
from types_aiobotocore_launch_wizard.type_defs import CreateDeploymentOutputTypeDef
from types_aiobotocore_launch_wizard.type_defs import CreateDeploymentInputTypeDef


session = Session()

client: LaunchWizardClient
async with session.client("launch-wizard") as client:  # (1)
    kwargs: CreateDeploymentInputTypeDef = {...}  # (2)
    result: CreateDeploymentOutputTypeDef = await client.create_deployment(**kwargs)  # (3)
```

1. client: [LaunchWizardClient](./client.md)
2. kwargs: [:material-code-braces: CreateDeploymentInputTypeDef](./type_defs.md#createdeploymentinputtypedef)
3. result: [:material-code-braces: CreateDeploymentOutputTypeDef](./type_defs.md#createdeploymentoutputtypedef)



#### Paginator usage example

```python
# ListDeploymentEventsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_launch_wizard.client import LaunchWizardClient
from types_aiobotocore_launch_wizard.paginator import ListDeploymentEventsPaginator
from types_aiobotocore_launch_wizard.type_defs import ListDeploymentEventsOutputTypeDef


session = Session()

client: LaunchWizardClient
async with session.client("launch-wizard") as client:  # (1)
    paginator: ListDeploymentEventsPaginator = client.get_paginator("list_deployment_events")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeploymentEventsOutputTypeDef
        print(item)  # (3)
```

1. client: [LaunchWizardClient](./client.md)
2. paginator: [ListDeploymentEventsPaginator](./paginators.md#listdeploymenteventspaginator)
3. item: [:material-code-braces: ListDeploymentEventsOutputTypeDef](./type_defs.md#listdeploymenteventsoutputtypedef)




