# Examples

> [Index](../README.md) > [PinpointEmail](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PinpointEmail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
    type annotations stubs module [types-aiobotocore-pinpoint-email](https://pypi.org/project/types-aiobotocore-pinpoint-email/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[pinpoint-email]` package installed.

Write your `PinpointEmail` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("pinpoint-email") as client:  # (1)
        result = await client.create_deliverability_test_report()  # (2)
    ```

    1. client: [PinpointEmailClient](./client.md)
    2. result: [:material-code-braces: CreateDeliverabilityTestReportResponseTypeDef](./type_defs.md#createdeliverabilitytestreportresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("pinpoint-email") as client:  # (1)
        paginator = client.get_paginator("get_dedicated_ips")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [PinpointEmailClient](./client.md)
    2. paginator: [GetDedicatedIpsPaginator](./paginators.md#getdedicatedipspaginator)
    3. item: [:material-code-braces: GetDedicatedIpsResponseTypeDef](./type_defs.md#getdedicatedipsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[pinpoint-email]`
or a standalone `types_aiobotocore_pinpoint_email` package, you have to explicitly specify
`client: PinpointEmailClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_pinpoint_email.client import PinpointEmailClient
    from types_aiobotocore_pinpoint_email.type_defs import CreateDeliverabilityTestReportResponseTypeDef
    from types_aiobotocore_pinpoint_email.type_defs import CreateDeliverabilityTestReportRequestRequestTypeDef


    session = Session()

    client: PinpointEmailClient
    async with session.client("pinpoint-email") as client:  # (1)
        kwargs: CreateDeliverabilityTestReportRequestRequestTypeDef = {...}  # (2)
        result: CreateDeliverabilityTestReportResponseTypeDef = await client.create_deliverability_test_report(**kwargs)  # (3)
    ```

    1. client: [PinpointEmailClient](./client.md)
    2. kwargs: [:material-code-braces: CreateDeliverabilityTestReportRequestRequestTypeDef](./type_defs.md#createdeliverabilitytestreportrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateDeliverabilityTestReportResponseTypeDef](./type_defs.md#createdeliverabilitytestreportresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_pinpoint_email.client import PinpointEmailClient
    from types_aiobotocore_pinpoint_email.paginator import GetDedicatedIpsPaginator
    from types_aiobotocore_pinpoint_email.type_defs import GetDedicatedIpsResponseTypeDef


    session = Session()

    client: PinpointEmailClient
    async with session.client("pinpoint-email") as client:  # (1)
        paginator: GetDedicatedIpsPaginator = client.get_paginator("get_dedicated_ips")  # (2)
        async for item in paginator.paginate(...):
            item: GetDedicatedIpsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [PinpointEmailClient](./client.md)
    2. paginator: [GetDedicatedIpsPaginator](./paginators.md#getdedicatedipspaginator)
    3. item: [:material-code-braces: GetDedicatedIpsResponseTypeDef](./type_defs.md#getdedicatedipsresponsetypedef) 




