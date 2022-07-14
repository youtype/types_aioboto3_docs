# Examples

> [Index](../README.md) > [ElasticBeanstalk](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ElasticBeanstalk](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
    type annotations stubs module [types-aiobotocore-elasticbeanstalk](https://pypi.org/project/types-aiobotocore-elasticbeanstalk/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[elasticbeanstalk]` package installed.

Write your `ElasticBeanstalk` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("elasticbeanstalk") as client:  # (1)
        result = await client.abort_environment_update()  # (2)
    ```

    1. client: [ElasticBeanstalkClient](./client.md)
    2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("elasticbeanstalk") as client:  # (1)
        paginator = client.get_paginator("describe_application_versions")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [ElasticBeanstalkClient](./client.md)
    2. paginator: [DescribeApplicationVersionsPaginator](./paginators.md#describeapplicationversionspaginator)
    3. item: [:material-code-braces: ApplicationVersionDescriptionsMessageTypeDef](./type_defs.md#applicationversiondescriptionsmessagetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("elasticbeanstalk") as client:  # (1)
        waiter = client.get_waiter("environment_exists")  # (2)
        await waiter.wait()
    ```

    1. client: [ElasticBeanstalkClient](./client.md)
    2. waiter: [EnvironmentExistsWaiter](./waiters.md#environmentexistswaiter)


### Explicit type annotations

With `types-aioboto3-lite[elasticbeanstalk]`
or a standalone `types_aiobotocore_elasticbeanstalk` package, you have to explicitly specify
`client: ElasticBeanstalkClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_elasticbeanstalk.client import ElasticBeanstalkClient
    from types_aiobotocore_elasticbeanstalk.type_defs import EmptyResponseMetadataTypeDef
    from types_aiobotocore_elasticbeanstalk.type_defs import AbortEnvironmentUpdateMessageRequestTypeDef


    session = Session()

    client: ElasticBeanstalkClient
    async with session.client("elasticbeanstalk") as client:  # (1)
        kwargs: AbortEnvironmentUpdateMessageRequestTypeDef = {...}  # (2)
        result: EmptyResponseMetadataTypeDef = await client.abort_environment_update(**kwargs)  # (3)
    ```

    1. client: [ElasticBeanstalkClient](./client.md)
    2. kwargs: [:material-code-braces: AbortEnvironmentUpdateMessageRequestTypeDef](./type_defs.md#abortenvironmentupdatemessagerequesttypedef) 
    3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_elasticbeanstalk.client import ElasticBeanstalkClient
    from types_aiobotocore_elasticbeanstalk.paginator import DescribeApplicationVersionsPaginator
    from types_aiobotocore_elasticbeanstalk.type_defs import ApplicationVersionDescriptionsMessageTypeDef


    session = Session()

    client: ElasticBeanstalkClient
    async with session.client("elasticbeanstalk") as client:  # (1)
        paginator: DescribeApplicationVersionsPaginator = client.get_paginator("describe_application_versions")  # (2)
        async for item in paginator.paginate(...):
            item: ApplicationVersionDescriptionsMessageTypeDef
            print(item)  # (3)
    ```

    1. client: [ElasticBeanstalkClient](./client.md)
    2. paginator: [DescribeApplicationVersionsPaginator](./paginators.md#describeapplicationversionspaginator)
    3. item: [:material-code-braces: ApplicationVersionDescriptionsMessageTypeDef](./type_defs.md#applicationversiondescriptionsmessagetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_elasticbeanstalk.client import ElasticBeanstalkClient
    from types_aiobotocore_elasticbeanstalk.waiter import EnvironmentExistsWaiter


    session = Session()

    async with session.client("elasticbeanstalk") as client:  # (1)
        waiter = client.get_waiter("environment_exists")  # (2)
        await waiter.wait()
    ```

    1. client: [ElasticBeanstalkClient](./client.md)
    2. waiter: [EnvironmentExistsWaiter](./waiters.md#environmentexistswaiter)


