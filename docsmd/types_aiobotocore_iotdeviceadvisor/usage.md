# Examples

> [Index](../README.md) > [IoTDeviceAdvisor](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTDeviceAdvisor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
    type annotations stubs module [types-aiobotocore-iotdeviceadvisor](https://pypi.org/project/types-aiobotocore-iotdeviceadvisor/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[iotdeviceadvisor]` package installed.

Write your `IoTDeviceAdvisor` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("iotdeviceadvisor") as client:  # (1)
        result = await client.create_suite_definition()  # (2)
    ```

    1. client: [IoTDeviceAdvisorClient](./client.md)
    2. result: [:material-code-braces: CreateSuiteDefinitionResponseTypeDef](./type_defs.md#createsuitedefinitionresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[iotdeviceadvisor]`
or a standalone `types_aiobotocore_iotdeviceadvisor` package, you have to explicitly specify
`client: IoTDeviceAdvisorClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_iotdeviceadvisor.client import IoTDeviceAdvisorClient
    from types_aiobotocore_iotdeviceadvisor.type_defs import CreateSuiteDefinitionResponseTypeDef
    from types_aiobotocore_iotdeviceadvisor.type_defs import CreateSuiteDefinitionRequestRequestTypeDef


    session = Session()

    client: IoTDeviceAdvisorClient
    async with session.client("iotdeviceadvisor") as client:  # (1)
        kwargs: CreateSuiteDefinitionRequestRequestTypeDef = {...}  # (2)
        result: CreateSuiteDefinitionResponseTypeDef = await client.create_suite_definition(**kwargs)  # (3)
    ```

    1. client: [IoTDeviceAdvisorClient](./client.md)
    2. kwargs: [:material-code-braces: CreateSuiteDefinitionRequestRequestTypeDef](./type_defs.md#createsuitedefinitionrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateSuiteDefinitionResponseTypeDef](./type_defs.md#createsuitedefinitionresponsetypedef) 






