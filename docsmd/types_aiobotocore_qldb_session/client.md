# QLDBSessionClient

> [Index](../README.md) > [QLDBSession](./README.md) > QLDBSessionClient

!!! note ""

    Auto-generated documentation for [QLDBSession](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#qldbsession)
    type annotations stubs module [types-aiobotocore-qldb-session](https://pypi.org/project/types-aiobotocore-qldb-session/).

## QLDBSessionClient

Type annotations and code completion for `#!python session.client("qldb-session")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client)

```python
# QLDBSessionClient usage example

from aioboto3.session import Session
from types_aiobotocore_qldb_session.client import QLDBSessionClient

session = Session()
async with session.client("qldb-session") as client:
    client: QLDBSessionClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("qldb-session").exceptions` structure.

```python
# QLDBSessionClient.exceptions usage example

async with session.client("qldb-session") as client:
    try:
        do_something(client)
    except (
            client.exceptions.BadRequestException,
        client.exceptions.CapacityExceededException,
        client.exceptions.ClientError,
        client.exceptions.InvalidSessionException,
        client.exceptions.LimitExceededException,
        client.exceptions.OccConflictException,
        client.exceptions.RateExceededException,
    ) as e:
        print(e)
```

```python
# QLDBSessionClient.exceptions type checking example

from types_aiobotocore_qldb_session.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("qldb-session").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("qldb-session").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client)

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


### send\_command

Sends a command to an Amazon QLDB ledger.

Type annotations and code completion for `#!python session.client("qldb-session").send_command` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client)

```python
# send_command method definition

await def send_command(
    self,
    *,
    SessionToken: str = ...,
    StartSession: StartSessionRequestTypeDef = ...,  # (1)
    StartTransaction: Mapping[str, Any] = ...,
    EndSession: Mapping[str, Any] = ...,
    CommitTransaction: CommitTransactionRequestTypeDef = ...,  # (2)
    AbortTransaction: Mapping[str, Any] = ...,
    ExecuteStatement: ExecuteStatementRequestTypeDef = ...,  # (3)
    FetchPage: FetchPageRequestTypeDef = ...,  # (4)
) -> SendCommandResultTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: StartSessionRequestTypeDef](./type_defs.md#startsessionrequesttypedef) 
2. See [:material-code-braces: CommitTransactionRequestTypeDef](./type_defs.md#committransactionrequesttypedef) 
3. See [:material-code-braces: ExecuteStatementRequestTypeDef](./type_defs.md#executestatementrequesttypedef) 
4. See [:material-code-braces: FetchPageRequestTypeDef](./type_defs.md#fetchpagerequesttypedef) 
5. See [:material-code-braces: SendCommandResultTypeDef](./type_defs.md#sendcommandresulttypedef) 


```python
# send_command method usage example with argument unpacking

kwargs: SendCommandRequestRequestTypeDef = {  # (1)
    "SessionToken": ...,
}

parent.send_command(**kwargs)
```

1. See [:material-code-braces: SendCommandRequestRequestTypeDef](./type_defs.md#sendcommandrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("qldb-session").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("qldb-session").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client)

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




