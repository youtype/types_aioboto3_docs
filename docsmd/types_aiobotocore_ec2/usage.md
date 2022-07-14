# Examples

> [Index](../README.md) > [EC2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EC2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
    type annotations stubs module [types-aiobotocore-ec2](https://pypi.org/project/types-aiobotocore-ec2/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[ec2]` package installed.

Write your `EC2` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("ec2") as client:  # (1)
        result = await client.accept_reserved_instances_exchange_quote()  # (2)
    ```

    1. client: [EC2Client](./client.md)
    2. result: [:material-code-braces: AcceptReservedInstancesExchangeQuoteResultTypeDef](./type_defs.md#acceptreservedinstancesexchangequoteresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("ec2") as client:  # (1)
        paginator = client.get_paginator("describe_addresses_attribute")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [EC2Client](./client.md)
    2. paginator: [DescribeAddressesAttributePaginator](./paginators.md#describeaddressesattributepaginator)
    3. item: [:material-code-braces: DescribeAddressesAttributeResultTypeDef](./type_defs.md#describeaddressesattributeresulttypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("ec2") as client:  # (1)
        waiter = client.get_waiter("bundle_task_complete")  # (2)
        await waiter.wait()
    ```

    1. client: [EC2Client](./client.md)
    2. waiter: [BundleTaskCompleteWaiter](./waiters.md#bundletaskcompletewaiter)


### Explicit type annotations

With `types-aioboto3-lite[ec2]`
or a standalone `types_aiobotocore_ec2` package, you have to explicitly specify
`client: EC2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_ec2.client import EC2Client
    from types_aiobotocore_ec2.type_defs import AcceptReservedInstancesExchangeQuoteResultTypeDef
    from types_aiobotocore_ec2.type_defs import AcceptReservedInstancesExchangeQuoteRequestRequestTypeDef


    session = Session()

    client: EC2Client
    async with session.client("ec2") as client:  # (1)
        kwargs: AcceptReservedInstancesExchangeQuoteRequestRequestTypeDef = {...}  # (2)
        result: AcceptReservedInstancesExchangeQuoteResultTypeDef = await client.accept_reserved_instances_exchange_quote(**kwargs)  # (3)
    ```

    1. client: [EC2Client](./client.md)
    2. kwargs: [:material-code-braces: AcceptReservedInstancesExchangeQuoteRequestRequestTypeDef](./type_defs.md#acceptreservedinstancesexchangequoterequestrequesttypedef) 
    3. result: [:material-code-braces: AcceptReservedInstancesExchangeQuoteResultTypeDef](./type_defs.md#acceptreservedinstancesexchangequoteresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_ec2.client import EC2Client
    from types_aiobotocore_ec2.paginator import DescribeAddressesAttributePaginator
    from types_aiobotocore_ec2.type_defs import DescribeAddressesAttributeResultTypeDef


    session = Session()

    client: EC2Client
    async with session.client("ec2") as client:  # (1)
        paginator: DescribeAddressesAttributePaginator = client.get_paginator("describe_addresses_attribute")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeAddressesAttributeResultTypeDef
            print(item)  # (3)
    ```

    1. client: [EC2Client](./client.md)
    2. paginator: [DescribeAddressesAttributePaginator](./paginators.md#describeaddressesattributepaginator)
    3. item: [:material-code-braces: DescribeAddressesAttributeResultTypeDef](./type_defs.md#describeaddressesattributeresulttypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_ec2.client import EC2Client
    from types_aiobotocore_ec2.waiter import BundleTaskCompleteWaiter


    session = Session()

    async with session.client("ec2") as client:  # (1)
        waiter = client.get_waiter("bundle_task_complete")  # (2)
        await waiter.wait()
    ```

    1. client: [EC2Client](./client.md)
    2. waiter: [BundleTaskCompleteWaiter](./waiters.md#bundletaskcompletewaiter)



## Service Resource

### Implicit type annotations

Can be used with `types-aioboto3[ec2]` package installed.


=== "ServiceResource"

    ```python title="ServiceResource usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.resource("ec2") as resource:  # (1)
        result = resource.ClassicAddress()  # (2)
    ```

    1. resource: [EC2ServiceResource](./service_resource.md)
    2. result: 



=== "Collections"

    ```python title="Collection usage example"
    from aioboto3.session import Session


    session = Session()
    resource = session.resource("ec2")  # (1)

    collection = resource.classic_addresses  # (2)
    for item in collection:
        print(item)  # (3)
    ```

    1. resource: [EC2ServiceResource](./service_resource.md)
    2. collection: [EC2ServiceResource](./service_resource.md#ec2serviceresourceclassic_addresses)
    3. item: ClassicAddress


### Explicit type annotations

With `types-aioboto3-lite[ec2]`
or a standalone `types_aiobotocore_ec2` package, you have to explicitly specify
`resource: EC2ServiceResource` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.



=== "ServiceResource"

    ```python title="ServiceResource usage example"
    from aioboto3.session import Session

    from types_aiobotocore_ec2.service_resource import EC2ServiceResource
    from types_aiobotocore_ec2.service_resource import ClassicAddress


    session = Session()

    resource: EC2ServiceResource
    async with session.resource("ec2") as resource:  # (1)
        result: ClassicAddress = resource.ClassicAddress() # (2)
    ```

    1. resource: [EC2ServiceResource](./service_resource.md)
    2. result: 



=== "Collections"

    ```python title="Collection usage example"
    from aioboto3.session import Session

    from types_aiobotocore_ec2.service_resource import EC2ServiceResource
    from types_aiobotocore_ec2.service_resource import ServiceResourceClassicAddressesCollection
    from types_aiobotocore_ec2.service_resource import ClassicAddress


    session = Session()

    resource: EC2ServiceResource
    async with session.resource("ec2") as resource:  # (1)
        collection: ServiceResourceClassicAddressesCollection = resource.classic_addresses  # (2)
        for item in collection:
            item: ClassicAddress
            print(item)  # (3)
    ```

    1. resource: [EC2ServiceResource](./service_resource.md)
    2. collection: [EC2ServiceResource](./service_resource.md#ec2serviceresourceclassic_addresses)
    3. item: ClassicAddress

