# Examples

> [Index](../README.md) > [EKS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EKS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
    type annotations stubs module [types-aiobotocore-eks](https://pypi.org/project/types-aiobotocore-eks/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[eks]` package installed.

Write your `EKS` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("eks") as client:  # (1)
        result = await client.associate_encryption_config()  # (2)
    ```

    1. client: [EKSClient](./client.md)
    2. result: [:material-code-braces: AssociateEncryptionConfigResponseTypeDef](./type_defs.md#associateencryptionconfigresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("eks") as client:  # (1)
        paginator = client.get_paginator("describe_addon_versions")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [EKSClient](./client.md)
    2. paginator: [DescribeAddonVersionsPaginator](./paginators.md#describeaddonversionspaginator)
    3. item: [:material-code-braces: DescribeAddonVersionsResponseTypeDef](./type_defs.md#describeaddonversionsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("eks") as client:  # (1)
        waiter = client.get_waiter("addon_active")  # (2)
        await waiter.wait()
    ```

    1. client: [EKSClient](./client.md)
    2. waiter: [AddonActiveWaiter](./waiters.md#addonactivewaiter)


### Explicit type annotations

With `types-aioboto3-lite[eks]`
or a standalone `types_aiobotocore_eks` package, you have to explicitly specify
`client: EKSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_eks.client import EKSClient
    from types_aiobotocore_eks.type_defs import AssociateEncryptionConfigResponseTypeDef
    from types_aiobotocore_eks.type_defs import AssociateEncryptionConfigRequestRequestTypeDef


    session = Session()

    client: EKSClient
    async with session.client("eks") as client:  # (1)
        kwargs: AssociateEncryptionConfigRequestRequestTypeDef = {...}  # (2)
        result: AssociateEncryptionConfigResponseTypeDef = await client.associate_encryption_config(**kwargs)  # (3)
    ```

    1. client: [EKSClient](./client.md)
    2. kwargs: [:material-code-braces: AssociateEncryptionConfigRequestRequestTypeDef](./type_defs.md#associateencryptionconfigrequestrequesttypedef) 
    3. result: [:material-code-braces: AssociateEncryptionConfigResponseTypeDef](./type_defs.md#associateencryptionconfigresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_eks.client import EKSClient
    from types_aiobotocore_eks.paginator import DescribeAddonVersionsPaginator
    from types_aiobotocore_eks.type_defs import DescribeAddonVersionsResponseTypeDef


    session = Session()

    client: EKSClient
    async with session.client("eks") as client:  # (1)
        paginator: DescribeAddonVersionsPaginator = client.get_paginator("describe_addon_versions")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeAddonVersionsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [EKSClient](./client.md)
    2. paginator: [DescribeAddonVersionsPaginator](./paginators.md#describeaddonversionspaginator)
    3. item: [:material-code-braces: DescribeAddonVersionsResponseTypeDef](./type_defs.md#describeaddonversionsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_eks.client import EKSClient
    from types_aiobotocore_eks.waiter import AddonActiveWaiter


    session = Session()

    async with session.client("eks") as client:  # (1)
        waiter = client.get_waiter("addon_active")  # (2)
        await waiter.wait()
    ```

    1. client: [EKSClient](./client.md)
    2. waiter: [AddonActiveWaiter](./waiters.md#addonactivewaiter)


