# Examples

> [Index](../README.md) > [GreengrassV2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [GreengrassV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
    type annotations stubs module [types-aiobotocore-greengrassv2](https://pypi.org/project/types-aiobotocore-greengrassv2/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[greengrassv2]` package installed.

Write your `GreengrassV2` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("greengrassv2") as client:  # (1)
        result = await client.associate_service_role_to_account()  # (2)
    ```

    1. client: [GreengrassV2Client](./client.md)
    2. result: [:material-code-braces: AssociateServiceRoleToAccountResponseTypeDef](./type_defs.md#associateserviceroletoaccountresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("greengrassv2") as client:  # (1)
        paginator = client.get_paginator("list_client_devices_associated_with_core_device")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [GreengrassV2Client](./client.md)
    2. paginator: [ListClientDevicesAssociatedWithCoreDevicePaginator](./paginators.md#listclientdevicesassociatedwithcoredevicepaginator)
    3. item: [:material-code-braces: ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef](./type_defs.md#listclientdevicesassociatedwithcoredeviceresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[greengrassv2]`
or a standalone `types_aiobotocore_greengrassv2` package, you have to explicitly specify
`client: GreengrassV2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_greengrassv2.client import GreengrassV2Client
    from types_aiobotocore_greengrassv2.type_defs import AssociateServiceRoleToAccountResponseTypeDef
    from types_aiobotocore_greengrassv2.type_defs import AssociateServiceRoleToAccountRequestRequestTypeDef


    session = Session()

    client: GreengrassV2Client
    async with session.client("greengrassv2") as client:  # (1)
        kwargs: AssociateServiceRoleToAccountRequestRequestTypeDef = {...}  # (2)
        result: AssociateServiceRoleToAccountResponseTypeDef = await client.associate_service_role_to_account(**kwargs)  # (3)
    ```

    1. client: [GreengrassV2Client](./client.md)
    2. kwargs: [:material-code-braces: AssociateServiceRoleToAccountRequestRequestTypeDef](./type_defs.md#associateserviceroletoaccountrequestrequesttypedef) 
    3. result: [:material-code-braces: AssociateServiceRoleToAccountResponseTypeDef](./type_defs.md#associateserviceroletoaccountresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_greengrassv2.client import GreengrassV2Client
    from types_aiobotocore_greengrassv2.paginator import ListClientDevicesAssociatedWithCoreDevicePaginator
    from types_aiobotocore_greengrassv2.type_defs import ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef


    session = Session()

    client: GreengrassV2Client
    async with session.client("greengrassv2") as client:  # (1)
        paginator: ListClientDevicesAssociatedWithCoreDevicePaginator = client.get_paginator("list_client_devices_associated_with_core_device")  # (2)
        async for item in paginator.paginate(...):
            item: ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [GreengrassV2Client](./client.md)
    2. paginator: [ListClientDevicesAssociatedWithCoreDevicePaginator](./paginators.md#listclientdevicesassociatedwithcoredevicepaginator)
    3. item: [:material-code-braces: ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef](./type_defs.md#listclientdevicesassociatedwithcoredeviceresponsetypedef) 




