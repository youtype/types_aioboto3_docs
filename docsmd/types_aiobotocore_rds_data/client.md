# RDSDataServiceClient

> [Index](../README.md) > [RDSDataService](./README.md) > RDSDataServiceClient

!!! note ""

    Auto-generated documentation for [RDSDataService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
    type annotations stubs module [types-aiobotocore-rds-data](https://pypi.org/project/types-aiobotocore-rds-data/).

## RDSDataServiceClient

Type annotations and code completion for `#!python session.client("rds-data")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client)

```python title="Usage example"
from aioboto3.session import Session
from types_aiobotocore_rds_data.client import RDSDataServiceClient

session = Session()
async with session.client("rds-data") as client:
    client: RDSDataServiceClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("rds-data").exceptions` structure.

```python title="Usage example"
async with session.client("rds-data") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.BadRequestException,
        client.ClientError,
        client.ForbiddenException,
        client.InternalServerErrorException,
        client.NotFoundException,
        client.ServiceUnavailableError,
        client.StatementTimeoutException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_rds_data.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### batch\_execute\_statement

Runs a batch SQL statement over an array of data.

Type annotations and code completion for `#!python session.client("rds-data").batch_execute_statement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.batch_execute_statement)

```python title="Method definition"
await def batch_execute_statement(
    self,
    *,
    resourceArn: str,
    secretArn: str,
    sql: str,
    database: str = ...,
    parameterSets: Sequence[Sequence[SqlParameterTypeDef]] = ...,  # (1)
    schema: str = ...,
    transactionId: str = ...,
) -> BatchExecuteStatementResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SqlParameterTypeDef](./type_defs.md#sqlparametertypedef) 
2. See [:material-code-braces: BatchExecuteStatementResponseTypeDef](./type_defs.md#batchexecutestatementresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: BatchExecuteStatementRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "secretArn": ...,
    "sql": ...,
}

parent.batch_execute_statement(**kwargs)
```

1. See [:material-code-braces: BatchExecuteStatementRequestRequestTypeDef](./type_defs.md#batchexecutestatementrequestrequesttypedef) 

### begin\_transaction

Starts a SQL transaction.

Type annotations and code completion for `#!python session.client("rds-data").begin_transaction` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.begin_transaction)

```python title="Method definition"
await def begin_transaction(
    self,
    *,
    resourceArn: str,
    secretArn: str,
    database: str = ...,
    schema: str = ...,
) -> BeginTransactionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BeginTransactionResponseTypeDef](./type_defs.md#begintransactionresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: BeginTransactionRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "secretArn": ...,
}

parent.begin_transaction(**kwargs)
```

1. See [:material-code-braces: BeginTransactionRequestRequestTypeDef](./type_defs.md#begintransactionrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.client("rds-data").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.client("rds-data").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.close)

```python title="Method definition"
await def close(
    self,
) -> None:
    ...
```


### commit\_transaction

Ends a SQL transaction started with the `BeginTransaction` operation and commits
the changes.

Type annotations and code completion for `#!python session.client("rds-data").commit_transaction` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.commit_transaction)

```python title="Method definition"
await def commit_transaction(
    self,
    *,
    resourceArn: str,
    secretArn: str,
    transactionId: str,
) -> CommitTransactionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CommitTransactionResponseTypeDef](./type_defs.md#committransactionresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: CommitTransactionRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "secretArn": ...,
    "transactionId": ...,
}

parent.commit_transaction(**kwargs)
```

1. See [:material-code-braces: CommitTransactionRequestRequestTypeDef](./type_defs.md#committransactionrequestrequesttypedef) 

### execute\_sql

Runs one or more SQL statements.

Type annotations and code completion for `#!python session.client("rds-data").execute_sql` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.execute_sql)

```python title="Method definition"
await def execute_sql(
    self,
    *,
    awsSecretStoreArn: str,
    dbClusterOrInstanceArn: str,
    sqlStatements: str,
    database: str = ...,
    schema: str = ...,
) -> ExecuteSqlResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExecuteSqlResponseTypeDef](./type_defs.md#executesqlresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ExecuteSqlRequestRequestTypeDef = {  # (1)
    "awsSecretStoreArn": ...,
    "dbClusterOrInstanceArn": ...,
    "sqlStatements": ...,
}

parent.execute_sql(**kwargs)
```

1. See [:material-code-braces: ExecuteSqlRequestRequestTypeDef](./type_defs.md#executesqlrequestrequesttypedef) 

### execute\_statement

Runs a SQL statement against a database.

Type annotations and code completion for `#!python session.client("rds-data").execute_statement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.execute_statement)

```python title="Method definition"
await def execute_statement(
    self,
    *,
    resourceArn: str,
    secretArn: str,
    sql: str,
    continueAfterTimeout: bool = ...,
    database: str = ...,
    formatRecordsAs: RecordsFormatTypeType = ...,  # (1)
    includeResultMetadata: bool = ...,
    parameters: Sequence[SqlParameterTypeDef] = ...,  # (2)
    resultSetOptions: ResultSetOptionsTypeDef = ...,  # (3)
    schema: str = ...,
    transactionId: str = ...,
) -> ExecuteStatementResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: RecordsFormatTypeType](./literals.md#recordsformattypetype) 
2. See [:material-code-braces: SqlParameterTypeDef](./type_defs.md#sqlparametertypedef) 
3. See [:material-code-braces: ResultSetOptionsTypeDef](./type_defs.md#resultsetoptionstypedef) 
4. See [:material-code-braces: ExecuteStatementResponseTypeDef](./type_defs.md#executestatementresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ExecuteStatementRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "secretArn": ...,
    "sql": ...,
}

parent.execute_statement(**kwargs)
```

1. See [:material-code-braces: ExecuteStatementRequestRequestTypeDef](./type_defs.md#executestatementrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.client("rds-data").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.generate_presigned_url)

```python title="Method definition"
await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### rollback\_transaction

Performs a rollback of a transaction.

Type annotations and code completion for `#!python session.client("rds-data").rollback_transaction` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.rollback_transaction)

```python title="Method definition"
await def rollback_transaction(
    self,
    *,
    resourceArn: str,
    secretArn: str,
    transactionId: str,
) -> RollbackTransactionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RollbackTransactionResponseTypeDef](./type_defs.md#rollbacktransactionresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: RollbackTransactionRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "secretArn": ...,
    "transactionId": ...,
}

parent.rollback_transaction(**kwargs)
```

1. See [:material-code-braces: RollbackTransactionRequestRequestTypeDef](./type_defs.md#rollbacktransactionrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("rds-data").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> RDSDataServiceClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("rds-data").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





