# Examples

> [Index](../README.md) > [CloudWatch](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudWatch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
    type annotations stubs module [types-aiobotocore-cloudwatch](https://pypi.org/project/types-aiobotocore-cloudwatch/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[cloudwatch]` package installed.

Write your `CloudWatch` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cloudwatch") as client:  # (1)
        result = await client.delete_alarms()  # (2)
    ```

    1. client: [CloudWatchClient](./client.md)
    2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cloudwatch") as client:  # (1)
        paginator = client.get_paginator("describe_alarm_history")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [CloudWatchClient](./client.md)
    2. paginator: [DescribeAlarmHistoryPaginator](./paginators.md#describealarmhistorypaginator)
    3. item: [:material-code-braces: DescribeAlarmHistoryOutputTypeDef](./type_defs.md#describealarmhistoryoutputtypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cloudwatch") as client:  # (1)
        waiter = client.get_waiter("alarm_exists")  # (2)
        await waiter.wait()
    ```

    1. client: [CloudWatchClient](./client.md)
    2. waiter: [AlarmExistsWaiter](./waiters.md#alarmexistswaiter)


### Explicit type annotations

With `types-aioboto3-lite[cloudwatch]`
or a standalone `types_aiobotocore_cloudwatch` package, you have to explicitly specify
`client: CloudWatchClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudwatch.client import CloudWatchClient
    from types_aiobotocore_cloudwatch.type_defs import EmptyResponseMetadataTypeDef
    from types_aiobotocore_cloudwatch.type_defs import DeleteAlarmsInputRequestTypeDef


    session = Session()

    client: CloudWatchClient
    async with session.client("cloudwatch") as client:  # (1)
        kwargs: DeleteAlarmsInputRequestTypeDef = {...}  # (2)
        result: EmptyResponseMetadataTypeDef = await client.delete_alarms(**kwargs)  # (3)
    ```

    1. client: [CloudWatchClient](./client.md)
    2. kwargs: [:material-code-braces: DeleteAlarmsInputRequestTypeDef](./type_defs.md#deletealarmsinputrequesttypedef) 
    3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudwatch.client import CloudWatchClient
    from types_aiobotocore_cloudwatch.paginator import DescribeAlarmHistoryPaginator
    from types_aiobotocore_cloudwatch.type_defs import DescribeAlarmHistoryOutputTypeDef


    session = Session()

    client: CloudWatchClient
    async with session.client("cloudwatch") as client:  # (1)
        paginator: DescribeAlarmHistoryPaginator = client.get_paginator("describe_alarm_history")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeAlarmHistoryOutputTypeDef
            print(item)  # (3)
    ```

    1. client: [CloudWatchClient](./client.md)
    2. paginator: [DescribeAlarmHistoryPaginator](./paginators.md#describealarmhistorypaginator)
    3. item: [:material-code-braces: DescribeAlarmHistoryOutputTypeDef](./type_defs.md#describealarmhistoryoutputtypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudwatch.client import CloudWatchClient
    from types_aiobotocore_cloudwatch.waiter import AlarmExistsWaiter


    session = Session()

    async with session.client("cloudwatch") as client:  # (1)
        waiter = client.get_waiter("alarm_exists")  # (2)
        await waiter.wait()
    ```

    1. client: [CloudWatchClient](./client.md)
    2. waiter: [AlarmExistsWaiter](./waiters.md#alarmexistswaiter)



## Service Resource

### Implicit type annotations

Can be used with `types-aioboto3[cloudwatch]` package installed.


=== "ServiceResource"

    ```python title="ServiceResource usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.resource("cloudwatch") as resource:  # (1)
        result = resource.Alarm()  # (2)
    ```

    1. resource: [CloudWatchServiceResource](./service_resource.md)
    2. result: 



=== "Collections"

    ```python title="Collection usage example"
    from aioboto3.session import Session


    session = Session()
    resource = session.resource("cloudwatch")  # (1)

    collection = resource.alarms  # (2)
    for item in collection:
        print(item)  # (3)
    ```

    1. resource: [CloudWatchServiceResource](./service_resource.md)
    2. collection: [CloudWatchServiceResource](./service_resource.md#cloudwatchserviceresourcealarms)
    3. item: Alarm


### Explicit type annotations

With `types-aioboto3-lite[cloudwatch]`
or a standalone `types_aiobotocore_cloudwatch` package, you have to explicitly specify
`resource: CloudWatchServiceResource` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.



=== "ServiceResource"

    ```python title="ServiceResource usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudwatch.service_resource import CloudWatchServiceResource
    from types_aiobotocore_cloudwatch.service_resource import Alarm


    session = Session()

    resource: CloudWatchServiceResource
    async with session.resource("cloudwatch") as resource:  # (1)
        result: Alarm = resource.Alarm() # (2)
    ```

    1. resource: [CloudWatchServiceResource](./service_resource.md)
    2. result: 



=== "Collections"

    ```python title="Collection usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudwatch.service_resource import CloudWatchServiceResource
    from types_aiobotocore_cloudwatch.service_resource import ServiceResourceAlarmsCollection
    from types_aiobotocore_cloudwatch.service_resource import Alarm


    session = Session()

    resource: CloudWatchServiceResource
    async with session.resource("cloudwatch") as resource:  # (1)
        collection: ServiceResourceAlarmsCollection = resource.alarms  # (2)
        for item in collection:
            item: Alarm
            print(item)  # (3)
    ```

    1. resource: [CloudWatchServiceResource](./service_resource.md)
    2. collection: [CloudWatchServiceResource](./service_resource.md#cloudwatchserviceresourcealarms)
    3. item: Alarm

