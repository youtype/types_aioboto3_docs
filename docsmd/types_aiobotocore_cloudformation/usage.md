# Examples

> [Index](../README.md) > [CloudFormation](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudFormation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
    type annotations stubs module [types-aiobotocore-cloudformation](https://pypi.org/project/types-aiobotocore-cloudformation/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[cloudformation]` package installed.

Write your `CloudFormation` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cloudformation") as client:  # (1)
        result = await client.activate_type()  # (2)
    ```

    1. client: [CloudFormationClient](./client.md)
    2. result: [:material-code-braces: ActivateTypeOutputTypeDef](./type_defs.md#activatetypeoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cloudformation") as client:  # (1)
        paginator = client.get_paginator("describe_account_limits")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [CloudFormationClient](./client.md)
    2. paginator: [DescribeAccountLimitsPaginator](./paginators.md#describeaccountlimitspaginator)
    3. item: [:material-code-braces: DescribeAccountLimitsOutputTypeDef](./type_defs.md#describeaccountlimitsoutputtypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cloudformation") as client:  # (1)
        waiter = client.get_waiter("change_set_create_complete")  # (2)
        await waiter.wait()
    ```

    1. client: [CloudFormationClient](./client.md)
    2. waiter: [ChangeSetCreateCompleteWaiter](./waiters.md#changesetcreatecompletewaiter)


### Explicit type annotations

With `types-aioboto3-lite[cloudformation]`
or a standalone `types_aiobotocore_cloudformation` package, you have to explicitly specify
`client: CloudFormationClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudformation.client import CloudFormationClient
    from types_aiobotocore_cloudformation.type_defs import ActivateTypeOutputTypeDef
    from types_aiobotocore_cloudformation.type_defs import ActivateTypeInputRequestTypeDef


    session = Session()

    client: CloudFormationClient
    async with session.client("cloudformation") as client:  # (1)
        kwargs: ActivateTypeInputRequestTypeDef = {...}  # (2)
        result: ActivateTypeOutputTypeDef = await client.activate_type(**kwargs)  # (3)
    ```

    1. client: [CloudFormationClient](./client.md)
    2. kwargs: [:material-code-braces: ActivateTypeInputRequestTypeDef](./type_defs.md#activatetypeinputrequesttypedef) 
    3. result: [:material-code-braces: ActivateTypeOutputTypeDef](./type_defs.md#activatetypeoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudformation.client import CloudFormationClient
    from types_aiobotocore_cloudformation.paginator import DescribeAccountLimitsPaginator
    from types_aiobotocore_cloudformation.type_defs import DescribeAccountLimitsOutputTypeDef


    session = Session()

    client: CloudFormationClient
    async with session.client("cloudformation") as client:  # (1)
        paginator: DescribeAccountLimitsPaginator = client.get_paginator("describe_account_limits")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeAccountLimitsOutputTypeDef
            print(item)  # (3)
    ```

    1. client: [CloudFormationClient](./client.md)
    2. paginator: [DescribeAccountLimitsPaginator](./paginators.md#describeaccountlimitspaginator)
    3. item: [:material-code-braces: DescribeAccountLimitsOutputTypeDef](./type_defs.md#describeaccountlimitsoutputtypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudformation.client import CloudFormationClient
    from types_aiobotocore_cloudformation.waiter import ChangeSetCreateCompleteWaiter


    session = Session()

    async with session.client("cloudformation") as client:  # (1)
        waiter = client.get_waiter("change_set_create_complete")  # (2)
        await waiter.wait()
    ```

    1. client: [CloudFormationClient](./client.md)
    2. waiter: [ChangeSetCreateCompleteWaiter](./waiters.md#changesetcreatecompletewaiter)



## Service Resource

### Implicit type annotations

Can be used with `types-aioboto3[cloudformation]` package installed.


=== "ServiceResource"

    ```python title="ServiceResource usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.resource("cloudformation") as resource:  # (1)
        result = resource.Event()  # (2)
    ```

    1. resource: [CloudFormationServiceResource](./service_resource.md)
    2. result: 



=== "Collections"

    ```python title="Collection usage example"
    from aioboto3.session import Session


    session = Session()
    resource = session.resource("cloudformation")  # (1)

    collection = resource.stacks  # (2)
    for item in collection:
        print(item)  # (3)
    ```

    1. resource: [CloudFormationServiceResource](./service_resource.md)
    2. collection: [CloudFormationServiceResource](./service_resource.md#cloudformationserviceresourcestacks)
    3. item: Stack


### Explicit type annotations

With `types-aioboto3-lite[cloudformation]`
or a standalone `types_aiobotocore_cloudformation` package, you have to explicitly specify
`resource: CloudFormationServiceResource` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.



=== "ServiceResource"

    ```python title="ServiceResource usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudformation.service_resource import CloudFormationServiceResource
    from types_aiobotocore_cloudformation.service_resource import Event


    session = Session()

    resource: CloudFormationServiceResource
    async with session.resource("cloudformation") as resource:  # (1)
        result: Event = resource.Event() # (2)
    ```

    1. resource: [CloudFormationServiceResource](./service_resource.md)
    2. result: 



=== "Collections"

    ```python title="Collection usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudformation.service_resource import CloudFormationServiceResource
    from types_aiobotocore_cloudformation.service_resource import ServiceResourceStacksCollection
    from types_aiobotocore_cloudformation.service_resource import Stack


    session = Session()

    resource: CloudFormationServiceResource
    async with session.resource("cloudformation") as resource:  # (1)
        collection: ServiceResourceStacksCollection = resource.stacks  # (2)
        for item in collection:
            item: Stack
            print(item)  # (3)
    ```

    1. resource: [CloudFormationServiceResource](./service_resource.md)
    2. collection: [CloudFormationServiceResource](./service_resource.md#cloudformationserviceresourcestacks)
    3. item: Stack

