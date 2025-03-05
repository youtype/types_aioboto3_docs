# Examples

> [Index](../README.md) > [ConnectParticipant](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ConnectParticipant](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#connectparticipant)
    type annotations stubs module [types-aiobotocore-connectparticipant](https://pypi.org/project/types-aiobotocore-connectparticipant/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[connectparticipant]` package installed.

Write your `ConnectParticipant` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ConnectParticipantClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("connectparticipant") as client:  # (1)
    result = await client.create_participant_connection()  # (2)
```

1. client: [ConnectParticipantClient](./client.md)
2. result: [:material-code-braces: CreateParticipantConnectionResponseTypeDef](./type_defs.md#createparticipantconnectionresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[connectparticipant]`
or a standalone `types_aiobotocore_connectparticipant` package, you have to explicitly specify
`client: ConnectParticipantClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ConnectParticipantClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_connectparticipant.client import ConnectParticipantClient
from types_aiobotocore_connectparticipant.type_defs import CreateParticipantConnectionResponseTypeDef
from types_aiobotocore_connectparticipant.type_defs import CreateParticipantConnectionRequestTypeDef


session = Session()

client: ConnectParticipantClient
async with session.client("connectparticipant") as client:  # (1)
    kwargs: CreateParticipantConnectionRequestTypeDef = {...}  # (2)
    result: CreateParticipantConnectionResponseTypeDef = await client.create_participant_connection(**kwargs)  # (3)
```

1. client: [ConnectParticipantClient](./client.md)
2. kwargs: [:material-code-braces: CreateParticipantConnectionRequestTypeDef](./type_defs.md#createparticipantconnectionrequesttypedef)
3. result: [:material-code-braces: CreateParticipantConnectionResponseTypeDef](./type_defs.md#createparticipantconnectionresponsetypedef)






