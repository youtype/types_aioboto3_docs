# Examples

> [Index](../README.md) > [CognitoSync](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CognitoSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#cognitosync)
    type annotations stubs module [types-aiobotocore-cognito-sync](https://pypi.org/project/types-aiobotocore-cognito-sync/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[cognito-sync]` package installed.

Write your `CognitoSync` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# CognitoSyncClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("cognito-sync") as client:  # (1)
    result = await client.bulk_publish()  # (2)
```

1. client: [CognitoSyncClient](./client.md)
2. result: [:material-code-braces: BulkPublishResponseTypeDef](./type_defs.md#bulkpublishresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[cognito-sync]`
or a standalone `types_aiobotocore_cognito_sync` package, you have to explicitly specify
`client: CognitoSyncClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# CognitoSyncClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_cognito_sync.client import CognitoSyncClient
from types_aiobotocore_cognito_sync.type_defs import BulkPublishResponseTypeDef
from types_aiobotocore_cognito_sync.type_defs import BulkPublishRequestTypeDef


session = Session()

client: CognitoSyncClient
async with session.client("cognito-sync") as client:  # (1)
    kwargs: BulkPublishRequestTypeDef = {...}  # (2)
    result: BulkPublishResponseTypeDef = await client.bulk_publish(**kwargs)  # (3)
```

1. client: [CognitoSyncClient](./client.md)
2. kwargs: [:material-code-braces: BulkPublishRequestTypeDef](./type_defs.md#bulkpublishrequesttypedef)
3. result: [:material-code-braces: BulkPublishResponseTypeDef](./type_defs.md#bulkpublishresponsetypedef)






