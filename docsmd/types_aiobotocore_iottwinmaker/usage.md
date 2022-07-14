# Examples

> [Index](../README.md) > [IoTTwinMaker](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTTwinMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
    type annotations stubs module [types-aiobotocore-iottwinmaker](https://pypi.org/project/types-aiobotocore-iottwinmaker/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[iottwinmaker]` package installed.

Write your `IoTTwinMaker` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("iottwinmaker") as client:  # (1)
        result = await client.batch_put_property_values()  # (2)
    ```

    1. client: [IoTTwinMakerClient](./client.md)
    2. result: [:material-code-braces: BatchPutPropertyValuesResponseTypeDef](./type_defs.md#batchputpropertyvaluesresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[iottwinmaker]`
or a standalone `types_aiobotocore_iottwinmaker` package, you have to explicitly specify
`client: IoTTwinMakerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_iottwinmaker.client import IoTTwinMakerClient
    from types_aiobotocore_iottwinmaker.type_defs import BatchPutPropertyValuesResponseTypeDef
    from types_aiobotocore_iottwinmaker.type_defs import BatchPutPropertyValuesRequestRequestTypeDef


    session = Session()

    client: IoTTwinMakerClient
    async with session.client("iottwinmaker") as client:  # (1)
        kwargs: BatchPutPropertyValuesRequestRequestTypeDef = {...}  # (2)
        result: BatchPutPropertyValuesResponseTypeDef = await client.batch_put_property_values(**kwargs)  # (3)
    ```

    1. client: [IoTTwinMakerClient](./client.md)
    2. kwargs: [:material-code-braces: BatchPutPropertyValuesRequestRequestTypeDef](./type_defs.md#batchputpropertyvaluesrequestrequesttypedef) 
    3. result: [:material-code-braces: BatchPutPropertyValuesResponseTypeDef](./type_defs.md#batchputpropertyvaluesresponsetypedef) 






