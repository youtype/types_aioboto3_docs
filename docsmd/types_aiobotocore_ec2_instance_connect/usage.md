# Examples

> [Index](../README.md) > [EC2InstanceConnect](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EC2InstanceConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
    type annotations stubs module [types-aiobotocore-ec2-instance-connect](https://pypi.org/project/types-aiobotocore-ec2-instance-connect/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[ec2-instance-connect]` package installed.

Write your `EC2InstanceConnect` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("ec2-instance-connect") as client:  # (1)
        result = await client.send_serial_console_ssh_public_key()  # (2)
    ```

    1. client: [EC2InstanceConnectClient](./client.md)
    2. result: [:material-code-braces: SendSerialConsoleSSHPublicKeyResponseTypeDef](./type_defs.md#sendserialconsolesshpublickeyresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[ec2-instance-connect]`
or a standalone `types_aiobotocore_ec2_instance_connect` package, you have to explicitly specify
`client: EC2InstanceConnectClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_ec2_instance_connect.client import EC2InstanceConnectClient
    from types_aiobotocore_ec2_instance_connect.type_defs import SendSerialConsoleSSHPublicKeyResponseTypeDef
    from types_aiobotocore_ec2_instance_connect.type_defs import SendSerialConsoleSSHPublicKeyRequestRequestTypeDef


    session = Session()

    client: EC2InstanceConnectClient
    async with session.client("ec2-instance-connect") as client:  # (1)
        kwargs: SendSerialConsoleSSHPublicKeyRequestRequestTypeDef = {...}  # (2)
        result: SendSerialConsoleSSHPublicKeyResponseTypeDef = await client.send_serial_console_ssh_public_key(**kwargs)  # (3)
    ```

    1. client: [EC2InstanceConnectClient](./client.md)
    2. kwargs: [:material-code-braces: SendSerialConsoleSSHPublicKeyRequestRequestTypeDef](./type_defs.md#sendserialconsolesshpublickeyrequestrequesttypedef) 
    3. result: [:material-code-braces: SendSerialConsoleSSHPublicKeyResponseTypeDef](./type_defs.md#sendserialconsolesshpublickeyresponsetypedef) 






