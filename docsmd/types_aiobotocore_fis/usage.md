# Examples

> [Index](../README.md) > [FIS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [FIS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
    type annotations stubs module [types-aiobotocore-fis](https://pypi.org/project/types-aiobotocore-fis/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[fis]` package installed.

Write your `FIS` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("fis") as client:  # (1)
        result = await client.create_experiment_template()  # (2)
    ```

    1. client: [FISClient](./client.md)
    2. result: [:material-code-braces: CreateExperimentTemplateResponseTypeDef](./type_defs.md#createexperimenttemplateresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[fis]`
or a standalone `types_aiobotocore_fis` package, you have to explicitly specify
`client: FISClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_fis.client import FISClient
    from types_aiobotocore_fis.type_defs import CreateExperimentTemplateResponseTypeDef
    from types_aiobotocore_fis.type_defs import CreateExperimentTemplateRequestRequestTypeDef


    session = Session()

    client: FISClient
    async with session.client("fis") as client:  # (1)
        kwargs: CreateExperimentTemplateRequestRequestTypeDef = {...}  # (2)
        result: CreateExperimentTemplateResponseTypeDef = await client.create_experiment_template(**kwargs)  # (3)
    ```

    1. client: [FISClient](./client.md)
    2. kwargs: [:material-code-braces: CreateExperimentTemplateRequestRequestTypeDef](./type_defs.md#createexperimenttemplaterequestrequesttypedef) 
    3. result: [:material-code-braces: CreateExperimentTemplateResponseTypeDef](./type_defs.md#createexperimenttemplateresponsetypedef) 






