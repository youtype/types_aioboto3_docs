# Examples

> [Index](../README.md) > [SagemakerEdgeManager](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SagemakerEdgeManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
    type annotations stubs module [types-aiobotocore-sagemaker-edge](https://pypi.org/project/types-aiobotocore-sagemaker-edge/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[sagemaker-edge]` package installed.

Write your `SagemakerEdgeManager` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("sagemaker-edge") as client:  # (1)
        result = await client.get_deployments()  # (2)
    ```

    1. client: [SagemakerEdgeManagerClient](./client.md)
    2. result: [:material-code-braces: GetDeploymentsResultTypeDef](./type_defs.md#getdeploymentsresulttypedef) 






### Explicit type annotations

With `types-aioboto3-lite[sagemaker-edge]`
or a standalone `types_aiobotocore_sagemaker_edge` package, you have to explicitly specify
`client: SagemakerEdgeManagerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_sagemaker_edge.client import SagemakerEdgeManagerClient
    from types_aiobotocore_sagemaker_edge.type_defs import GetDeploymentsResultTypeDef
    from types_aiobotocore_sagemaker_edge.type_defs import GetDeploymentsRequestRequestTypeDef


    session = Session()

    client: SagemakerEdgeManagerClient
    async with session.client("sagemaker-edge") as client:  # (1)
        kwargs: GetDeploymentsRequestRequestTypeDef = {...}  # (2)
        result: GetDeploymentsResultTypeDef = await client.get_deployments(**kwargs)  # (3)
    ```

    1. client: [SagemakerEdgeManagerClient](./client.md)
    2. kwargs: [:material-code-braces: GetDeploymentsRequestRequestTypeDef](./type_defs.md#getdeploymentsrequestrequesttypedef) 
    3. result: [:material-code-braces: GetDeploymentsResultTypeDef](./type_defs.md#getdeploymentsresulttypedef) 






