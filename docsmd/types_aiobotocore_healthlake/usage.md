# Examples

> [Index](../README.md) > [HealthLake](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [HealthLake](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
    type annotations stubs module [types-aiobotocore-healthlake](https://pypi.org/project/types-aiobotocore-healthlake/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[healthlake]` package installed.

Write your `HealthLake` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("healthlake") as client:  # (1)
        result = await client.create_fhir_datastore()  # (2)
    ```

    1. client: [HealthLakeClient](./client.md)
    2. result: [:material-code-braces: CreateFHIRDatastoreResponseTypeDef](./type_defs.md#createfhirdatastoreresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[healthlake]`
or a standalone `types_aiobotocore_healthlake` package, you have to explicitly specify
`client: HealthLakeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_healthlake.client import HealthLakeClient
    from types_aiobotocore_healthlake.type_defs import CreateFHIRDatastoreResponseTypeDef
    from types_aiobotocore_healthlake.type_defs import CreateFHIRDatastoreRequestRequestTypeDef


    session = Session()

    client: HealthLakeClient
    async with session.client("healthlake") as client:  # (1)
        kwargs: CreateFHIRDatastoreRequestRequestTypeDef = {...}  # (2)
        result: CreateFHIRDatastoreResponseTypeDef = await client.create_fhir_datastore(**kwargs)  # (3)
    ```

    1. client: [HealthLakeClient](./client.md)
    2. kwargs: [:material-code-braces: CreateFHIRDatastoreRequestRequestTypeDef](./type_defs.md#createfhirdatastorerequestrequesttypedef) 
    3. result: [:material-code-braces: CreateFHIRDatastoreResponseTypeDef](./type_defs.md#createfhirdatastoreresponsetypedef) 






