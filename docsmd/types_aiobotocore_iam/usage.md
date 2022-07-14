# Examples

> [Index](../README.md) > [IAM](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IAM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
    type annotations stubs module [types-aiobotocore-iam](https://pypi.org/project/types-aiobotocore-iam/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[iam]` package installed.

Write your `IAM` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("iam") as client:  # (1)
        result = await client.add_client_id_to_open_id_connect_provider()  # (2)
    ```

    1. client: [IAMClient](./client.md)
    2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("iam") as client:  # (1)
        paginator = client.get_paginator("get_account_authorization_details")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [IAMClient](./client.md)
    2. paginator: [GetAccountAuthorizationDetailsPaginator](./paginators.md#getaccountauthorizationdetailspaginator)
    3. item: [:material-code-braces: GetAccountAuthorizationDetailsResponseTypeDef](./type_defs.md#getaccountauthorizationdetailsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("iam") as client:  # (1)
        waiter = client.get_waiter("instance_profile_exists")  # (2)
        await waiter.wait()
    ```

    1. client: [IAMClient](./client.md)
    2. waiter: [InstanceProfileExistsWaiter](./waiters.md#instanceprofileexistswaiter)


### Explicit type annotations

With `types-aioboto3-lite[iam]`
or a standalone `types_aiobotocore_iam` package, you have to explicitly specify
`client: IAMClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_iam.client import IAMClient
    from types_aiobotocore_iam.type_defs import EmptyResponseMetadataTypeDef
    from types_aiobotocore_iam.type_defs import AddClientIDToOpenIDConnectProviderRequestRequestTypeDef


    session = Session()

    client: IAMClient
    async with session.client("iam") as client:  # (1)
        kwargs: AddClientIDToOpenIDConnectProviderRequestRequestTypeDef = {...}  # (2)
        result: EmptyResponseMetadataTypeDef = await client.add_client_id_to_open_id_connect_provider(**kwargs)  # (3)
    ```

    1. client: [IAMClient](./client.md)
    2. kwargs: [:material-code-braces: AddClientIDToOpenIDConnectProviderRequestRequestTypeDef](./type_defs.md#addclientidtoopenidconnectproviderrequestrequesttypedef) 
    3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_iam.client import IAMClient
    from types_aiobotocore_iam.paginator import GetAccountAuthorizationDetailsPaginator
    from types_aiobotocore_iam.type_defs import GetAccountAuthorizationDetailsResponseTypeDef


    session = Session()

    client: IAMClient
    async with session.client("iam") as client:  # (1)
        paginator: GetAccountAuthorizationDetailsPaginator = client.get_paginator("get_account_authorization_details")  # (2)
        async for item in paginator.paginate(...):
            item: GetAccountAuthorizationDetailsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [IAMClient](./client.md)
    2. paginator: [GetAccountAuthorizationDetailsPaginator](./paginators.md#getaccountauthorizationdetailspaginator)
    3. item: [:material-code-braces: GetAccountAuthorizationDetailsResponseTypeDef](./type_defs.md#getaccountauthorizationdetailsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_iam.client import IAMClient
    from types_aiobotocore_iam.waiter import InstanceProfileExistsWaiter


    session = Session()

    async with session.client("iam") as client:  # (1)
        waiter = client.get_waiter("instance_profile_exists")  # (2)
        await waiter.wait()
    ```

    1. client: [IAMClient](./client.md)
    2. waiter: [InstanceProfileExistsWaiter](./waiters.md#instanceprofileexistswaiter)



## Service Resource

### Implicit type annotations

Can be used with `types-aioboto3[iam]` package installed.


=== "ServiceResource"

    ```python title="ServiceResource usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.resource("iam") as resource:  # (1)
        result = resource.AccessKey()  # (2)
    ```

    1. resource: [IAMServiceResource](./service_resource.md)
    2. result: 



=== "Collections"

    ```python title="Collection usage example"
    from aioboto3.session import Session


    session = Session()
    resource = session.resource("iam")  # (1)

    collection = resource.groups  # (2)
    for item in collection:
        print(item)  # (3)
    ```

    1. resource: [IAMServiceResource](./service_resource.md)
    2. collection: [IAMServiceResource](./service_resource.md#iamserviceresourcegroups)
    3. item: Group


### Explicit type annotations

With `types-aioboto3-lite[iam]`
or a standalone `types_aiobotocore_iam` package, you have to explicitly specify
`resource: IAMServiceResource` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.



=== "ServiceResource"

    ```python title="ServiceResource usage example"
    from aioboto3.session import Session

    from types_aiobotocore_iam.service_resource import IAMServiceResource
    from types_aiobotocore_iam.service_resource import AccessKey


    session = Session()

    resource: IAMServiceResource
    async with session.resource("iam") as resource:  # (1)
        result: AccessKey = resource.AccessKey() # (2)
    ```

    1. resource: [IAMServiceResource](./service_resource.md)
    2. result: 



=== "Collections"

    ```python title="Collection usage example"
    from aioboto3.session import Session

    from types_aiobotocore_iam.service_resource import IAMServiceResource
    from types_aiobotocore_iam.service_resource import ServiceResourceGroupsCollection
    from types_aiobotocore_iam.service_resource import Group


    session = Session()

    resource: IAMServiceResource
    async with session.resource("iam") as resource:  # (1)
        collection: ServiceResourceGroupsCollection = resource.groups  # (2)
        for item in collection:
            item: Group
            print(item)  # (3)
    ```

    1. resource: [IAMServiceResource](./service_resource.md)
    2. collection: [IAMServiceResource](./service_resource.md#iamserviceresourcegroups)
    3. item: Group

