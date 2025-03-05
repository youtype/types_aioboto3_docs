# Examples

> [Index](../README.md) > [MigrationHub](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MigrationHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#migrationhub)
    type annotations stubs module [types-aiobotocore-mgh](https://pypi.org/project/types-aiobotocore-mgh/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[mgh]` package installed.

Write your `MigrationHub` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# MigrationHubClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("mgh") as client:  # (1)
    result = await client.describe_application_state()  # (2)
```

1. client: [MigrationHubClient](./client.md)
2. result: [:material-code-braces: DescribeApplicationStateResultTypeDef](./type_defs.md#describeapplicationstateresulttypedef)



#### Paginator usage example

```python
# ListApplicationStatesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("mgh") as client:  # (1)
    paginator = client.get_paginator("list_application_states")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MigrationHubClient](./client.md)
2. paginator: [ListApplicationStatesPaginator](./paginators.md#listapplicationstatespaginator)
3. item: [:material-code-braces: ListApplicationStatesResultTypeDef](./type_defs.md#listapplicationstatesresulttypedef)




### Explicit type annotations

With `types-aioboto3-lite[mgh]`
or a standalone `types_aiobotocore_mgh` package, you have to explicitly specify
`client: MigrationHubClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# MigrationHubClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_mgh.client import MigrationHubClient
from types_aiobotocore_mgh.type_defs import DescribeApplicationStateResultTypeDef
from types_aiobotocore_mgh.type_defs import DescribeApplicationStateRequestTypeDef


session = Session()

client: MigrationHubClient
async with session.client("mgh") as client:  # (1)
    kwargs: DescribeApplicationStateRequestTypeDef = {...}  # (2)
    result: DescribeApplicationStateResultTypeDef = await client.describe_application_state(**kwargs)  # (3)
```

1. client: [MigrationHubClient](./client.md)
2. kwargs: [:material-code-braces: DescribeApplicationStateRequestTypeDef](./type_defs.md#describeapplicationstaterequesttypedef)
3. result: [:material-code-braces: DescribeApplicationStateResultTypeDef](./type_defs.md#describeapplicationstateresulttypedef)



#### Paginator usage example

```python
# ListApplicationStatesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_mgh.client import MigrationHubClient
from types_aiobotocore_mgh.paginator import ListApplicationStatesPaginator
from types_aiobotocore_mgh.type_defs import ListApplicationStatesResultTypeDef


session = Session()

client: MigrationHubClient
async with session.client("mgh") as client:  # (1)
    paginator: ListApplicationStatesPaginator = client.get_paginator("list_application_states")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationStatesResultTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubClient](./client.md)
2. paginator: [ListApplicationStatesPaginator](./paginators.md#listapplicationstatespaginator)
3. item: [:material-code-braces: ListApplicationStatesResultTypeDef](./type_defs.md#listapplicationstatesresulttypedef)




