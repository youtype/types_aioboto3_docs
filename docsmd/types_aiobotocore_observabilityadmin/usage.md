# Examples

> [Index](../README.md) > [CloudWatchObservabilityAdminService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudWatchObservabilityAdminService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin.html#cloudwatchobservabilityadminservice)
    type annotations stubs module [types-aiobotocore-observabilityadmin](https://pypi.org/project/types-aiobotocore-observabilityadmin/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[observabilityadmin]` package installed.

Write your `CloudWatchObservabilityAdminService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# CloudWatchObservabilityAdminServiceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("observabilityadmin") as client:  # (1)
    result = await client.list_resource_telemetry()  # (2)
```

1. client: [CloudWatchObservabilityAdminServiceClient](./client.md)
2. result: [:material-code-braces: ListResourceTelemetryOutputTypeDef](./type_defs.md#listresourcetelemetryoutputtypedef)



#### Paginator usage example

```python
# ListResourceTelemetryForOrganizationPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("observabilityadmin") as client:  # (1)
    paginator = client.get_paginator("list_resource_telemetry_for_organization")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudWatchObservabilityAdminServiceClient](./client.md)
2. paginator: [ListResourceTelemetryForOrganizationPaginator](./paginators.md#listresourcetelemetryfororganizationpaginator)
3. item: [:material-code-braces: ListResourceTelemetryForOrganizationOutputTypeDef](./type_defs.md#listresourcetelemetryfororganizationoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[observabilityadmin]`
or a standalone `types_aiobotocore_observabilityadmin` package, you have to explicitly specify
`client: CloudWatchObservabilityAdminServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# CloudWatchObservabilityAdminServiceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_observabilityadmin.client import CloudWatchObservabilityAdminServiceClient
from types_aiobotocore_observabilityadmin.type_defs import ListResourceTelemetryOutputTypeDef
from types_aiobotocore_observabilityadmin.type_defs import ListResourceTelemetryInputTypeDef


session = Session()

client: CloudWatchObservabilityAdminServiceClient
async with session.client("observabilityadmin") as client:  # (1)
    kwargs: ListResourceTelemetryInputTypeDef = {...}  # (2)
    result: ListResourceTelemetryOutputTypeDef = await client.list_resource_telemetry(**kwargs)  # (3)
```

1. client: [CloudWatchObservabilityAdminServiceClient](./client.md)
2. kwargs: [:material-code-braces: ListResourceTelemetryInputTypeDef](./type_defs.md#listresourcetelemetryinputtypedef)
3. result: [:material-code-braces: ListResourceTelemetryOutputTypeDef](./type_defs.md#listresourcetelemetryoutputtypedef)



#### Paginator usage example

```python
# ListResourceTelemetryForOrganizationPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_observabilityadmin.client import CloudWatchObservabilityAdminServiceClient
from types_aiobotocore_observabilityadmin.paginator import ListResourceTelemetryForOrganizationPaginator
from types_aiobotocore_observabilityadmin.type_defs import ListResourceTelemetryForOrganizationOutputTypeDef


session = Session()

client: CloudWatchObservabilityAdminServiceClient
async with session.client("observabilityadmin") as client:  # (1)
    paginator: ListResourceTelemetryForOrganizationPaginator = client.get_paginator("list_resource_telemetry_for_organization")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceTelemetryForOrganizationOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchObservabilityAdminServiceClient](./client.md)
2. paginator: [ListResourceTelemetryForOrganizationPaginator](./paginators.md#listresourcetelemetryfororganizationpaginator)
3. item: [:material-code-braces: ListResourceTelemetryForOrganizationOutputTypeDef](./type_defs.md#listresourcetelemetryfororganizationoutputtypedef)




