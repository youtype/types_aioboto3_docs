# Examples

> [Index](../README.md) > [Greengrass](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Greengrass](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
    type annotations stubs module [types-aiobotocore-greengrass](https://pypi.org/project/types-aiobotocore-greengrass/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[greengrass]` package installed.

Write your `Greengrass` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("greengrass") as client:  # (1)
        result = await client.associate_role_to_group()  # (2)
    ```

    1. client: [GreengrassClient](./client.md)
    2. result: [:material-code-braces: AssociateRoleToGroupResponseTypeDef](./type_defs.md#associateroletogroupresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("greengrass") as client:  # (1)
        paginator = client.get_paginator("list_bulk_deployment_detailed_reports")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [GreengrassClient](./client.md)
    2. paginator: [ListBulkDeploymentDetailedReportsPaginator](./paginators.md#listbulkdeploymentdetailedreportspaginator)
    3. item: [:material-code-braces: ListBulkDeploymentDetailedReportsResponseTypeDef](./type_defs.md#listbulkdeploymentdetailedreportsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[greengrass]`
or a standalone `types_aiobotocore_greengrass` package, you have to explicitly specify
`client: GreengrassClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_greengrass.client import GreengrassClient
    from types_aiobotocore_greengrass.type_defs import AssociateRoleToGroupResponseTypeDef
    from types_aiobotocore_greengrass.type_defs import AssociateRoleToGroupRequestRequestTypeDef


    session = Session()

    client: GreengrassClient
    async with session.client("greengrass") as client:  # (1)
        kwargs: AssociateRoleToGroupRequestRequestTypeDef = {...}  # (2)
        result: AssociateRoleToGroupResponseTypeDef = await client.associate_role_to_group(**kwargs)  # (3)
    ```

    1. client: [GreengrassClient](./client.md)
    2. kwargs: [:material-code-braces: AssociateRoleToGroupRequestRequestTypeDef](./type_defs.md#associateroletogrouprequestrequesttypedef) 
    3. result: [:material-code-braces: AssociateRoleToGroupResponseTypeDef](./type_defs.md#associateroletogroupresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_greengrass.client import GreengrassClient
    from types_aiobotocore_greengrass.paginator import ListBulkDeploymentDetailedReportsPaginator
    from types_aiobotocore_greengrass.type_defs import ListBulkDeploymentDetailedReportsResponseTypeDef


    session = Session()

    client: GreengrassClient
    async with session.client("greengrass") as client:  # (1)
        paginator: ListBulkDeploymentDetailedReportsPaginator = client.get_paginator("list_bulk_deployment_detailed_reports")  # (2)
        async for item in paginator.paginate(...):
            item: ListBulkDeploymentDetailedReportsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [GreengrassClient](./client.md)
    2. paginator: [ListBulkDeploymentDetailedReportsPaginator](./paginators.md#listbulkdeploymentdetailedreportspaginator)
    3. item: [:material-code-braces: ListBulkDeploymentDetailedReportsResponseTypeDef](./type_defs.md#listbulkdeploymentdetailedreportsresponsetypedef) 




