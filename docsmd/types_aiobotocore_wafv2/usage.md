# Examples

> [Index](../README.md) > [WAFV2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WAFV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
    type annotations stubs module [types-aiobotocore-wafv2](https://pypi.org/project/types-aiobotocore-wafv2/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[wafv2]` package installed.

Write your `WAFV2` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("wafv2") as client:  # (1)
        result = await client.check_capacity()  # (2)
    ```

    1. client: [WAFV2Client](./client.md)
    2. result: [:material-code-braces: CheckCapacityResponseTypeDef](./type_defs.md#checkcapacityresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[wafv2]`
or a standalone `types_aiobotocore_wafv2` package, you have to explicitly specify
`client: WAFV2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_wafv2.client import WAFV2Client
    from types_aiobotocore_wafv2.type_defs import CheckCapacityResponseTypeDef
    from types_aiobotocore_wafv2.type_defs import CheckCapacityRequestRequestTypeDef


    session = Session()

    client: WAFV2Client
    async with session.client("wafv2") as client:  # (1)
        kwargs: CheckCapacityRequestRequestTypeDef = {...}  # (2)
        result: CheckCapacityResponseTypeDef = await client.check_capacity(**kwargs)  # (3)
    ```

    1. client: [WAFV2Client](./client.md)
    2. kwargs: [:material-code-braces: CheckCapacityRequestRequestTypeDef](./type_defs.md#checkcapacityrequestrequesttypedef) 
    3. result: [:material-code-braces: CheckCapacityResponseTypeDef](./type_defs.md#checkcapacityresponsetypedef) 






