# Examples

> [Index](../README.md) > [CostExplorer](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CostExplorer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
    type annotations stubs module [types-aiobotocore-ce](https://pypi.org/project/types-aiobotocore-ce/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[ce]` package installed.

Write your `CostExplorer` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("ce") as client:  # (1)
        result = await client.create_anomaly_monitor()  # (2)
    ```

    1. client: [CostExplorerClient](./client.md)
    2. result: [:material-code-braces: CreateAnomalyMonitorResponseTypeDef](./type_defs.md#createanomalymonitorresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[ce]`
or a standalone `types_aiobotocore_ce` package, you have to explicitly specify
`client: CostExplorerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_ce.client import CostExplorerClient
    from types_aiobotocore_ce.type_defs import CreateAnomalyMonitorResponseTypeDef
    from types_aiobotocore_ce.type_defs import CreateAnomalyMonitorRequestRequestTypeDef


    session = Session()

    client: CostExplorerClient
    async with session.client("ce") as client:  # (1)
        kwargs: CreateAnomalyMonitorRequestRequestTypeDef = {...}  # (2)
        result: CreateAnomalyMonitorResponseTypeDef = await client.create_anomaly_monitor(**kwargs)  # (3)
    ```

    1. client: [CostExplorerClient](./client.md)
    2. kwargs: [:material-code-braces: CreateAnomalyMonitorRequestRequestTypeDef](./type_defs.md#createanomalymonitorrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateAnomalyMonitorResponseTypeDef](./type_defs.md#createanomalymonitorresponsetypedef) 






