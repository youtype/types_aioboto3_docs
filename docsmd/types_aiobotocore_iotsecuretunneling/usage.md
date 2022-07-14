# Examples

> [Index](../README.md) > [IoTSecureTunneling](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTSecureTunneling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
    type annotations stubs module [types-aiobotocore-iotsecuretunneling](https://pypi.org/project/types-aiobotocore-iotsecuretunneling/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[iotsecuretunneling]` package installed.

Write your `IoTSecureTunneling` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("iotsecuretunneling") as client:  # (1)
        result = await client.describe_tunnel()  # (2)
    ```

    1. client: [IoTSecureTunnelingClient](./client.md)
    2. result: [:material-code-braces: DescribeTunnelResponseTypeDef](./type_defs.md#describetunnelresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[iotsecuretunneling]`
or a standalone `types_aiobotocore_iotsecuretunneling` package, you have to explicitly specify
`client: IoTSecureTunnelingClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_iotsecuretunneling.client import IoTSecureTunnelingClient
    from types_aiobotocore_iotsecuretunneling.type_defs import DescribeTunnelResponseTypeDef
    from types_aiobotocore_iotsecuretunneling.type_defs import DescribeTunnelRequestRequestTypeDef


    session = Session()

    client: IoTSecureTunnelingClient
    async with session.client("iotsecuretunneling") as client:  # (1)
        kwargs: DescribeTunnelRequestRequestTypeDef = {...}  # (2)
        result: DescribeTunnelResponseTypeDef = await client.describe_tunnel(**kwargs)  # (3)
    ```

    1. client: [IoTSecureTunnelingClient](./client.md)
    2. kwargs: [:material-code-braces: DescribeTunnelRequestRequestTypeDef](./type_defs.md#describetunnelrequestrequesttypedef) 
    3. result: [:material-code-braces: DescribeTunnelResponseTypeDef](./type_defs.md#describetunnelresponsetypedef) 






