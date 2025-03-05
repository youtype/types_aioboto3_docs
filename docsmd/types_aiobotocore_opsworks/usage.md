# Examples

> [Index](../README.md) > [OpsWorks](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [OpsWorks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#opsworks)
    type annotations stubs module [types-aiobotocore-opsworks](https://pypi.org/project/types-aiobotocore-opsworks/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[opsworks]` package installed.

Write your `OpsWorks` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# OpsWorksClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("opsworks") as client:  # (1)
    result = await client.assign_instance()  # (2)
```

1. client: [OpsWorksClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# DescribeEcsClustersPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("opsworks") as client:  # (1)
    paginator = client.get_paginator("describe_ecs_clusters")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [OpsWorksClient](./client.md)
2. paginator: [DescribeEcsClustersPaginator](./paginators.md#describeecsclusterspaginator)
3. item: [:material-code-braces: DescribeEcsClustersResultTypeDef](./type_defs.md#describeecsclustersresulttypedef)



#### Waiter usage example

```python
# AppExistsWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("opsworks") as client:  # (1)
    waiter = client.get_waiter("app_exists")  # (2)
    await waiter.wait(...)
```

1. client: [OpsWorksClient](./client.md)
2. waiter: [AppExistsWaiter](./waiters.md#appexistswaiter)


### Explicit type annotations

With `types-aioboto3-lite[opsworks]`
or a standalone `types_aiobotocore_opsworks` package, you have to explicitly specify
`client: OpsWorksClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# OpsWorksClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_opsworks.client import OpsWorksClient
from types_aiobotocore_opsworks.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_opsworks.type_defs import AssignInstanceRequestTypeDef


session = Session()

client: OpsWorksClient
async with session.client("opsworks") as client:  # (1)
    kwargs: AssignInstanceRequestTypeDef = {...}  # (2)
    result: EmptyResponseMetadataTypeDef = await client.assign_instance(**kwargs)  # (3)
```

1. client: [OpsWorksClient](./client.md)
2. kwargs: [:material-code-braces: AssignInstanceRequestTypeDef](./type_defs.md#assigninstancerequesttypedef)
3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# DescribeEcsClustersPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_opsworks.client import OpsWorksClient
from types_aiobotocore_opsworks.paginator import DescribeEcsClustersPaginator
from types_aiobotocore_opsworks.type_defs import DescribeEcsClustersResultTypeDef


session = Session()

client: OpsWorksClient
async with session.client("opsworks") as client:  # (1)
    paginator: DescribeEcsClustersPaginator = client.get_paginator("describe_ecs_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEcsClustersResultTypeDef
        print(item)  # (3)
```

1. client: [OpsWorksClient](./client.md)
2. paginator: [DescribeEcsClustersPaginator](./paginators.md#describeecsclusterspaginator)
3. item: [:material-code-braces: DescribeEcsClustersResultTypeDef](./type_defs.md#describeecsclustersresulttypedef)



#### Waiter usage example

```python
# AppExistsWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_opsworks.client import OpsWorksClient
from types_aiobotocore_opsworks.waiter import AppExistsWaiter


session = Session()

async with session.client("opsworks") as client:  # (1)
    waiter = client.get_waiter("app_exists")  # (2)
    await waiter.wait(...)
```

1. client: [OpsWorksClient](./client.md)
2. waiter: [AppExistsWaiter](./waiters.md#appexistswaiter)



## Service Resource

### Implicit type annotations

Can be used with `types-aioboto3[opsworks]` package installed.


#### ServiceResource method usage example

```python
# OpsWorksServiceResource usage example

from aioboto3.session import Session


session = Session()

async with session.resource("opsworks") as resource:  # (1)
    result = await resource.create_stack(...)  # (2)
```

1. resource: [OpsWorksServiceResource](./service_resource.md)
2. result: [Stack](./service_resource.md#stack)



#### Collection usage example

```python
# ServiceResourceStacksCollection usage example

from aioboto3.session import Session


session = Session()

async with session.resource("opsworks") as resource:  # (1)
    collection = resource.stacks  # (2)
    async for item in collection:
        print(item)  # (3)
```

1. resource: [OpsWorksServiceResource](./service_resource.md)
2. collection: [ServiceResourceStacksCollection](./service_resource.md#serviceresourcestackscollection)
3. item: [Stack](./service_resource.md#stack)


### Explicit type annotations

With `types-aioboto3-lite[opsworks]`
or a standalone `types_aiobotocore_opsworks` package, you have to explicitly specify
`resource: OpsWorksServiceResource` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.



#### ServiceResource method usage example

```python
# OpsWorksServiceResource usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_opsworks.service_resource import OpsWorksServiceResource
from types_aiobotocore_opsworks.service_resource import Stack
from types_aiobotocore_opsworks.type_defs import CreateStackRequestServiceResourceCreateStackTypeDef


session = Session()

resource: OpsWorksServiceResource
async with session.resource("opsworks") as resource:  # (1)
    kwargs: CreateStackRequestServiceResourceCreateStackTypeDef = {...}  # (2)
    result: Stack = await resource.create_stack(...) # (3)
```

1. resource: [OpsWorksServiceResource](./service_resource.md)
2. kwargs: [:material-code-braces: CreateStackRequestServiceResourceCreateStackTypeDef](./type_defs.md#createstackrequestserviceresourcecreatestacktypedef)
3. result: [Stack](./service_resource.md#stack)



#### Collection usage example

```python
# ServiceResourceStacksCollection usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_opsworks.service_resource import OpsWorksServiceResource
from types_aiobotocore_opsworks.service_resource import ServiceResourceStacksCollection
from types_aiobotocore_opsworks.service_resource import Stack


session = Session()

resource: OpsWorksServiceResource
async with session.resource("opsworks") as resource:  # (1)
    collection: ServiceResourceStacksCollection = resource.stacks  # (2)
    async for item in collection:
        item: Stack
        print(item)  # (3)
```

1. resource: [OpsWorksServiceResource](./service_resource.md)
2. collection: [OpsWorksServiceResource](./service_resource.md#serviceresourcestackscollection)
3. item: Stack

