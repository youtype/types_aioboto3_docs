# EC2InstanceConnectClient

> [Index](../README.md) > [EC2InstanceConnect](./README.md) > EC2InstanceConnectClient

!!! note ""

    Auto-generated documentation for [EC2InstanceConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#ec2instanceconnect)
    type annotations stubs module [types-aiobotocore-ec2-instance-connect](https://pypi.org/project/types-aiobotocore-ec2-instance-connect/).

## EC2InstanceConnectClient

Type annotations and code completion for `#!python session.client("ec2-instance-connect")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect.Client)

```python
# EC2InstanceConnectClient usage example

from aioboto3.session import Session
from types_aiobotocore_ec2_instance_connect.client import EC2InstanceConnectClient

session = Session()
async with session.client("ec2-instance-connect") as client:
    client: EC2InstanceConnectClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("ec2-instance-connect").exceptions` structure.

```python
# EC2InstanceConnectClient.exceptions usage example

async with session.client("ec2-instance-connect") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AuthException,
        client.exceptions.ClientError,
        client.exceptions.EC2InstanceNotFoundException,
        client.exceptions.EC2InstanceStateInvalidException,
        client.exceptions.EC2InstanceTypeInvalidException,
        client.exceptions.EC2InstanceUnavailableException,
        client.exceptions.InvalidArgsException,
        client.exceptions.SerialConsoleAccessDisabledException,
        client.exceptions.SerialConsoleSessionLimitExceededException,
        client.exceptions.SerialConsoleSessionUnavailableException,
        client.exceptions.SerialConsoleSessionUnsupportedException,
        client.exceptions.ServiceException,
        client.exceptions.ThrottlingException,
    ) as e:
        print(e)
```

```python
# EC2InstanceConnectClient.exceptions type checking example

from types_aiobotocore_ec2_instance_connect.client import Exceptions

def handle_error(exc: Exceptions.AuthException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("ec2-instance-connect").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("ec2-instance-connect").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect.Client)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### send\_ssh\_public\_key

Pushes an SSH public key to the specified EC2 instance for use by the specified
user.

Type annotations and code completion for `#!python session.client("ec2-instance-connect").send_ssh_public_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect.Client)

```python
# send_ssh_public_key method definition

await def send_ssh_public_key(
    self,
    *,
    InstanceId: str,
    InstanceOSUser: str,
    SSHPublicKey: str,
    AvailabilityZone: str = ...,
) -> SendSSHPublicKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SendSSHPublicKeyResponseTypeDef](./type_defs.md#sendsshpublickeyresponsetypedef) 


```python
# send_ssh_public_key method usage example with argument unpacking

kwargs: SendSSHPublicKeyRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "InstanceOSUser": ...,
    "SSHPublicKey": ...,
}

parent.send_ssh_public_key(**kwargs)
```

1. See [:material-code-braces: SendSSHPublicKeyRequestRequestTypeDef](./type_defs.md#sendsshpublickeyrequestrequesttypedef) 

### send\_serial\_console\_ssh\_public\_key

Pushes an SSH public key to the specified EC2 instance.

Type annotations and code completion for `#!python session.client("ec2-instance-connect").send_serial_console_ssh_public_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect.Client)

```python
# send_serial_console_ssh_public_key method definition

await def send_serial_console_ssh_public_key(
    self,
    *,
    InstanceId: str,
    SSHPublicKey: str,
    SerialPort: int = ...,
) -> SendSerialConsoleSSHPublicKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SendSerialConsoleSSHPublicKeyResponseTypeDef](./type_defs.md#sendserialconsolesshpublickeyresponsetypedef) 


```python
# send_serial_console_ssh_public_key method usage example with argument unpacking

kwargs: SendSerialConsoleSSHPublicKeyRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "SSHPublicKey": ...,
}

parent.send_serial_console_ssh_public_key(**kwargs)
```

1. See [:material-code-braces: SendSerialConsoleSSHPublicKeyRequestRequestTypeDef](./type_defs.md#sendserialconsolesshpublickeyrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("ec2-instance-connect").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("ec2-instance-connect").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




