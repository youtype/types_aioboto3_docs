# Examples

> [Index](../README.md) > [RedshiftDataAPIService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [RedshiftDataAPIService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#redshiftdataapiservice)
    type annotations stubs module [types-aiobotocore-redshift-data](https://pypi.org/project/types-aiobotocore-redshift-data/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[redshift-data]` package installed.

Write your `RedshiftDataAPIService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# RedshiftDataAPIServiceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("redshift-data") as client:  # (1)
    result = await client.batch_execute_statement()  # (2)
```

1. client: [RedshiftDataAPIServiceClient](./client.md)
2. result: [:material-code-braces: BatchExecuteStatementOutputTypeDef](./type_defs.md#batchexecutestatementoutputtypedef)



#### Paginator usage example

```python
# DescribeTablePaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("redshift-data") as client:  # (1)
    paginator = client.get_paginator("describe_table")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [RedshiftDataAPIServiceClient](./client.md)
2. paginator: [DescribeTablePaginator](./paginators.md#describetablepaginator)
3. item: [:material-code-braces: DescribeTableResponseTypeDef](./type_defs.md#describetableresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[redshift-data]`
or a standalone `types_aiobotocore_redshift_data` package, you have to explicitly specify
`client: RedshiftDataAPIServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# RedshiftDataAPIServiceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_redshift_data.client import RedshiftDataAPIServiceClient
from types_aiobotocore_redshift_data.type_defs import BatchExecuteStatementOutputTypeDef
from types_aiobotocore_redshift_data.type_defs import BatchExecuteStatementInputTypeDef


session = Session()

client: RedshiftDataAPIServiceClient
async with session.client("redshift-data") as client:  # (1)
    kwargs: BatchExecuteStatementInputTypeDef = {...}  # (2)
    result: BatchExecuteStatementOutputTypeDef = await client.batch_execute_statement(**kwargs)  # (3)
```

1. client: [RedshiftDataAPIServiceClient](./client.md)
2. kwargs: [:material-code-braces: BatchExecuteStatementInputTypeDef](./type_defs.md#batchexecutestatementinputtypedef)
3. result: [:material-code-braces: BatchExecuteStatementOutputTypeDef](./type_defs.md#batchexecutestatementoutputtypedef)



#### Paginator usage example

```python
# DescribeTablePaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_redshift_data.client import RedshiftDataAPIServiceClient
from types_aiobotocore_redshift_data.paginator import DescribeTablePaginator
from types_aiobotocore_redshift_data.type_defs import DescribeTableResponseTypeDef


session = Session()

client: RedshiftDataAPIServiceClient
async with session.client("redshift-data") as client:  # (1)
    paginator: DescribeTablePaginator = client.get_paginator("describe_table")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTableResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftDataAPIServiceClient](./client.md)
2. paginator: [DescribeTablePaginator](./paginators.md#describetablepaginator)
3. item: [:material-code-braces: DescribeTableResponseTypeDef](./type_defs.md#describetableresponsetypedef)




