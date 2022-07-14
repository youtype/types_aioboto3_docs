# Examples

> [Index](../README.md) > [Cloud9](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Cloud9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
    type annotations stubs module [types-aiobotocore-cloud9](https://pypi.org/project/types-aiobotocore-cloud9/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[cloud9]` package installed.

Write your `Cloud9` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cloud9") as client:  # (1)
        result = await client.create_environment_ec2()  # (2)
    ```

    1. client: [Cloud9Client](./client.md)
    2. result: [:material-code-braces: CreateEnvironmentEC2ResultTypeDef](./type_defs.md#createenvironmentec2resulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cloud9") as client:  # (1)
        paginator = client.get_paginator("describe_environment_memberships")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [Cloud9Client](./client.md)
    2. paginator: [DescribeEnvironmentMembershipsPaginator](./paginators.md#describeenvironmentmembershipspaginator)
    3. item: [:material-code-braces: DescribeEnvironmentMembershipsResultTypeDef](./type_defs.md#describeenvironmentmembershipsresulttypedef) 




### Explicit type annotations

With `types-aioboto3-lite[cloud9]`
or a standalone `types_aiobotocore_cloud9` package, you have to explicitly specify
`client: Cloud9Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloud9.client import Cloud9Client
    from types_aiobotocore_cloud9.type_defs import CreateEnvironmentEC2ResultTypeDef
    from types_aiobotocore_cloud9.type_defs import CreateEnvironmentEC2RequestRequestTypeDef


    session = Session()

    client: Cloud9Client
    async with session.client("cloud9") as client:  # (1)
        kwargs: CreateEnvironmentEC2RequestRequestTypeDef = {...}  # (2)
        result: CreateEnvironmentEC2ResultTypeDef = await client.create_environment_ec2(**kwargs)  # (3)
    ```

    1. client: [Cloud9Client](./client.md)
    2. kwargs: [:material-code-braces: CreateEnvironmentEC2RequestRequestTypeDef](./type_defs.md#createenvironmentec2requestrequesttypedef) 
    3. result: [:material-code-braces: CreateEnvironmentEC2ResultTypeDef](./type_defs.md#createenvironmentec2resulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloud9.client import Cloud9Client
    from types_aiobotocore_cloud9.paginator import DescribeEnvironmentMembershipsPaginator
    from types_aiobotocore_cloud9.type_defs import DescribeEnvironmentMembershipsResultTypeDef


    session = Session()

    client: Cloud9Client
    async with session.client("cloud9") as client:  # (1)
        paginator: DescribeEnvironmentMembershipsPaginator = client.get_paginator("describe_environment_memberships")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeEnvironmentMembershipsResultTypeDef
            print(item)  # (3)
    ```

    1. client: [Cloud9Client](./client.md)
    2. paginator: [DescribeEnvironmentMembershipsPaginator](./paginators.md#describeenvironmentmembershipspaginator)
    3. item: [:material-code-braces: DescribeEnvironmentMembershipsResultTypeDef](./type_defs.md#describeenvironmentmembershipsresulttypedef) 




