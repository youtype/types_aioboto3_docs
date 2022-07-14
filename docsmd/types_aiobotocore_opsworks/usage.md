# Examples

> [Index](../README.md) > [OpsWorks](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [OpsWorks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
    type annotations stubs module [types-aiobotocore-opsworks](https://pypi.org/project/types-aiobotocore-opsworks/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[opsworks]` package installed.

Write your `OpsWorks` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("opsworks") as client:  # (1)
        result = await client.assign_instance()  # (2)
    ```

    1. client: [OpsWorksClient](./client.md)
    2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
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



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("opsworks") as client:  # (1)
        waiter = client.get_waiter("app_exists")  # (2)
        await waiter.wait()
    ```

    1. client: [OpsWorksClient](./client.md)
    2. waiter: [AppExistsWaiter](./waiters.md#appexistswaiter)


### Explicit type annotations

With `types-aioboto3-lite[opsworks]`
or a standalone `types_aiobotocore_opsworks` package, you have to explicitly specify
`client: OpsWorksClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_opsworks.client import OpsWorksClient
    from types_aiobotocore_opsworks.type_defs import EmptyResponseMetadataTypeDef
    from types_aiobotocore_opsworks.type_defs import AssignInstanceRequestRequestTypeDef


    session = Session()

    client: OpsWorksClient
    async with session.client("opsworks") as client:  # (1)
        kwargs: AssignInstanceRequestRequestTypeDef = {...}  # (2)
        result: EmptyResponseMetadataTypeDef = await client.assign_instance(**kwargs)  # (3)
    ```

    1. client: [OpsWorksClient](./client.md)
    2. kwargs: [:material-code-braces: AssignInstanceRequestRequestTypeDef](./type_defs.md#assigninstancerequestrequesttypedef) 
    3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
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



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_opsworks.client import OpsWorksClient
    from types_aiobotocore_opsworks.waiter import AppExistsWaiter


    session = Session()

    async with session.client("opsworks") as client:  # (1)
        waiter = client.get_waiter("app_exists")  # (2)
        await waiter.wait()
    ```

    1. client: [OpsWorksClient](./client.md)
    2. waiter: [AppExistsWaiter](./waiters.md#appexistswaiter)



## Service Resource

### Implicit type annotations

Can be used with `types-aioboto3[opsworks]` package installed.


=== "ServiceResource"

    ```python title="ServiceResource usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.resource("opsworks") as resource:  # (1)
        result = resource.Layer()  # (2)
    ```

    1. resource: [OpsWorksServiceResource](./service_resource.md)
    2. result: 



=== "Collections"

    ```python title="Collection usage example"
    from aioboto3.session import Session


    session = Session()
    resource = session.resource("opsworks")  # (1)

    collection = resource.stacks  # (2)
    for item in collection:
        print(item)  # (3)
    ```

    1. resource: [OpsWorksServiceResource](./service_resource.md)
    2. collection: [OpsWorksServiceResource](./service_resource.md#opsworksserviceresourcestacks)
    3. item: Stack


### Explicit type annotations

With `types-aioboto3-lite[opsworks]`
or a standalone `types_aiobotocore_opsworks` package, you have to explicitly specify
`resource: OpsWorksServiceResource` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.



=== "ServiceResource"

    ```python title="ServiceResource usage example"
    from aioboto3.session import Session

    from types_aiobotocore_opsworks.service_resource import OpsWorksServiceResource
    from types_aiobotocore_opsworks.service_resource import Layer


    session = Session()

    resource: OpsWorksServiceResource
    async with session.resource("opsworks") as resource:  # (1)
        result: Layer = resource.Layer() # (2)
    ```

    1. resource: [OpsWorksServiceResource](./service_resource.md)
    2. result: 



=== "Collections"

    ```python title="Collection usage example"
    from aioboto3.session import Session

    from types_aiobotocore_opsworks.service_resource import OpsWorksServiceResource
    from types_aiobotocore_opsworks.service_resource import ServiceResourceStacksCollection
    from types_aiobotocore_opsworks.service_resource import Stack


    session = Session()

    resource: OpsWorksServiceResource
    async with session.resource("opsworks") as resource:  # (1)
        collection: ServiceResourceStacksCollection = resource.stacks  # (2)
        for item in collection:
            item: Stack
            print(item)  # (3)
    ```

    1. resource: [OpsWorksServiceResource](./service_resource.md)
    2. collection: [OpsWorksServiceResource](./service_resource.md#opsworksserviceresourcestacks)
    3. item: Stack

