# Examples

> [Index](../README.md) > [IoTWireless](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTWireless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
    type annotations stubs module [types-aiobotocore-iotwireless](https://pypi.org/project/types-aiobotocore-iotwireless/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[iotwireless]` package installed.

Write your `IoTWireless` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("iotwireless") as client:  # (1)
        result = await client.associate_aws_account_with_partner_account()  # (2)
    ```

    1. client: [IoTWirelessClient](./client.md)
    2. result: [:material-code-braces: AssociateAwsAccountWithPartnerAccountResponseTypeDef](./type_defs.md#associateawsaccountwithpartneraccountresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[iotwireless]`
or a standalone `types_aiobotocore_iotwireless` package, you have to explicitly specify
`client: IoTWirelessClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_iotwireless.client import IoTWirelessClient
    from types_aiobotocore_iotwireless.type_defs import AssociateAwsAccountWithPartnerAccountResponseTypeDef
    from types_aiobotocore_iotwireless.type_defs import AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef


    session = Session()

    client: IoTWirelessClient
    async with session.client("iotwireless") as client:  # (1)
        kwargs: AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef = {...}  # (2)
        result: AssociateAwsAccountWithPartnerAccountResponseTypeDef = await client.associate_aws_account_with_partner_account(**kwargs)  # (3)
    ```

    1. client: [IoTWirelessClient](./client.md)
    2. kwargs: [:material-code-braces: AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef](./type_defs.md#associateawsaccountwithpartneraccountrequestrequesttypedef) 
    3. result: [:material-code-braces: AssociateAwsAccountWithPartnerAccountResponseTypeDef](./type_defs.md#associateawsaccountwithpartneraccountresponsetypedef) 






