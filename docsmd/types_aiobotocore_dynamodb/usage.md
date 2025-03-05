# Examples

> [Index](../README.md) > [DynamoDB](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DynamoDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#dynamodb)
    type annotations stubs module [types-aiobotocore-dynamodb](https://pypi.org/project/types-aiobotocore-dynamodb/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[dynamodb]` package installed.

Write your `DynamoDB` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# DynamoDBClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("dynamodb") as client:  # (1)
    result = await client.batch_execute_statement()  # (2)
```

1. client: [DynamoDBClient](./client.md)
2. result: [:material-code-braces: BatchExecuteStatementOutputTypeDef](./type_defs.md#batchexecutestatementoutputtypedef)



#### Paginator usage example

```python
# ListBackupsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("dynamodb") as client:  # (1)
    paginator = client.get_paginator("list_backups")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DynamoDBClient](./client.md)
2. paginator: [ListBackupsPaginator](./paginators.md#listbackupspaginator)
3. item: [:material-code-braces: ListBackupsOutputTypeDef](./type_defs.md#listbackupsoutputtypedef)



#### Waiter usage example

```python
# TableExistsWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("dynamodb") as client:  # (1)
    waiter = client.get_waiter("table_exists")  # (2)
    await waiter.wait(...)
```

1. client: [DynamoDBClient](./client.md)
2. waiter: [TableExistsWaiter](./waiters.md#tableexistswaiter)


### Explicit type annotations

With `types-aioboto3-lite[dynamodb]`
or a standalone `types_aiobotocore_dynamodb` package, you have to explicitly specify
`client: DynamoDBClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# DynamoDBClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_dynamodb.client import DynamoDBClient
from types_aiobotocore_dynamodb.type_defs import BatchExecuteStatementOutputTypeDef
from types_aiobotocore_dynamodb.type_defs import BatchExecuteStatementInputTypeDef


session = Session()

client: DynamoDBClient
async with session.client("dynamodb") as client:  # (1)
    kwargs: BatchExecuteStatementInputTypeDef = {...}  # (2)
    result: BatchExecuteStatementOutputTypeDef = await client.batch_execute_statement(**kwargs)  # (3)
```

1. client: [DynamoDBClient](./client.md)
2. kwargs: [:material-code-braces: BatchExecuteStatementInputTypeDef](./type_defs.md#batchexecutestatementinputtypedef)
3. result: [:material-code-braces: BatchExecuteStatementOutputTypeDef](./type_defs.md#batchexecutestatementoutputtypedef)



#### Paginator usage example

```python
# ListBackupsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_dynamodb.client import DynamoDBClient
from types_aiobotocore_dynamodb.paginator import ListBackupsPaginator
from types_aiobotocore_dynamodb.type_defs import ListBackupsOutputTypeDef


session = Session()

client: DynamoDBClient
async with session.client("dynamodb") as client:  # (1)
    paginator: ListBackupsPaginator = client.get_paginator("list_backups")  # (2)
    async for item in paginator.paginate(...):
        item: ListBackupsOutputTypeDef
        print(item)  # (3)
```

1. client: [DynamoDBClient](./client.md)
2. paginator: [ListBackupsPaginator](./paginators.md#listbackupspaginator)
3. item: [:material-code-braces: ListBackupsOutputTypeDef](./type_defs.md#listbackupsoutputtypedef)



#### Waiter usage example

```python
# TableExistsWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_dynamodb.client import DynamoDBClient
from types_aiobotocore_dynamodb.waiter import TableExistsWaiter


session = Session()

async with session.client("dynamodb") as client:  # (1)
    waiter = client.get_waiter("table_exists")  # (2)
    await waiter.wait(...)
```

1. client: [DynamoDBClient](./client.md)
2. waiter: [TableExistsWaiter](./waiters.md#tableexistswaiter)



## Service Resource

### Implicit type annotations

Can be used with `types-aioboto3[dynamodb]` package installed.


#### ServiceResource method usage example

```python
# DynamoDBServiceResource usage example

from aioboto3.session import Session


session = Session()

async with session.resource("dynamodb") as resource:  # (1)
    result = await resource.create_table(...)  # (2)
```

1. resource: [DynamoDBServiceResource](./service_resource.md)
2. result: [Table](./service_resource.md#table)



#### Collection usage example

```python
# ServiceResourceTablesCollection usage example

from aioboto3.session import Session


session = Session()

async with session.resource("dynamodb") as resource:  # (1)
    collection = resource.tables  # (2)
    async for item in collection:
        print(item)  # (3)
```

1. resource: [DynamoDBServiceResource](./service_resource.md)
2. collection: [ServiceResourceTablesCollection](./service_resource.md#serviceresourcetablescollection)
3. item: [Table](./service_resource.md#table)


### Explicit type annotations

With `types-aioboto3-lite[dynamodb]`
or a standalone `types_aiobotocore_dynamodb` package, you have to explicitly specify
`resource: DynamoDBServiceResource` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.



#### ServiceResource method usage example

```python
# DynamoDBServiceResource usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_dynamodb.service_resource import DynamoDBServiceResource
from types_aiobotocore_dynamodb.service_resource import Table
from types_aiobotocore_dynamodb.type_defs import CreateTableInputServiceResourceCreateTableTypeDef


session = Session()

resource: DynamoDBServiceResource
async with session.resource("dynamodb") as resource:  # (1)
    kwargs: CreateTableInputServiceResourceCreateTableTypeDef = {...}  # (2)
    result: Table = await resource.create_table(...) # (3)
```

1. resource: [DynamoDBServiceResource](./service_resource.md)
2. kwargs: [:material-code-braces: CreateTableInputServiceResourceCreateTableTypeDef](./type_defs.md#createtableinputserviceresourcecreatetabletypedef)
3. result: [Table](./service_resource.md#table)



#### Collection usage example

```python
# ServiceResourceTablesCollection usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_dynamodb.service_resource import DynamoDBServiceResource
from types_aiobotocore_dynamodb.service_resource import ServiceResourceTablesCollection
from types_aiobotocore_dynamodb.service_resource import Table


session = Session()

resource: DynamoDBServiceResource
async with session.resource("dynamodb") as resource:  # (1)
    collection: ServiceResourceTablesCollection = resource.tables  # (2)
    async for item in collection:
        item: Table
        print(item)  # (3)
```

1. resource: [DynamoDBServiceResource](./service_resource.md)
2. collection: [DynamoDBServiceResource](./service_resource.md#serviceresourcetablescollection)
3. item: Table

