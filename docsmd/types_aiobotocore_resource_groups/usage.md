# Examples

> [Index](../README.md) > [ResourceGroups](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ResourceGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
    type annotations stubs module [types-aiobotocore-resource-groups](https://pypi.org/project/types-aiobotocore-resource-groups/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[resource-groups]` package installed.

Write your `ResourceGroups` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("resource-groups") as client:  # (1)
        result = await client.create_group()  # (2)
    ```

    1. client: [ResourceGroupsClient](./client.md)
    2. result: [:material-code-braces: CreateGroupOutputTypeDef](./type_defs.md#creategroupoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("resource-groups") as client:  # (1)
        paginator = client.get_paginator("list_group_resources")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [ResourceGroupsClient](./client.md)
    2. paginator: [ListGroupResourcesPaginator](./paginators.md#listgroupresourcespaginator)
    3. item: [:material-code-braces: ListGroupResourcesOutputTypeDef](./type_defs.md#listgroupresourcesoutputtypedef) 




### Explicit type annotations

With `types-aioboto3-lite[resource-groups]`
or a standalone `types_aiobotocore_resource_groups` package, you have to explicitly specify
`client: ResourceGroupsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_resource_groups.client import ResourceGroupsClient
    from types_aiobotocore_resource_groups.type_defs import CreateGroupOutputTypeDef
    from types_aiobotocore_resource_groups.type_defs import CreateGroupInputRequestTypeDef


    session = Session()

    client: ResourceGroupsClient
    async with session.client("resource-groups") as client:  # (1)
        kwargs: CreateGroupInputRequestTypeDef = {...}  # (2)
        result: CreateGroupOutputTypeDef = await client.create_group(**kwargs)  # (3)
    ```

    1. client: [ResourceGroupsClient](./client.md)
    2. kwargs: [:material-code-braces: CreateGroupInputRequestTypeDef](./type_defs.md#creategroupinputrequesttypedef) 
    3. result: [:material-code-braces: CreateGroupOutputTypeDef](./type_defs.md#creategroupoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_resource_groups.client import ResourceGroupsClient
    from types_aiobotocore_resource_groups.paginator import ListGroupResourcesPaginator
    from types_aiobotocore_resource_groups.type_defs import ListGroupResourcesOutputTypeDef


    session = Session()

    client: ResourceGroupsClient
    async with session.client("resource-groups") as client:  # (1)
        paginator: ListGroupResourcesPaginator = client.get_paginator("list_group_resources")  # (2)
        async for item in paginator.paginate(...):
            item: ListGroupResourcesOutputTypeDef
            print(item)  # (3)
    ```

    1. client: [ResourceGroupsClient](./client.md)
    2. paginator: [ListGroupResourcesPaginator](./paginators.md#listgroupresourcespaginator)
    3. item: [:material-code-braces: ListGroupResourcesOutputTypeDef](./type_defs.md#listgroupresourcesoutputtypedef) 




