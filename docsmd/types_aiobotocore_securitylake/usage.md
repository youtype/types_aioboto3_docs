# Examples

> [Index](../README.md) > [SecurityLake](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SecurityLake](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#securitylake)
    type annotations stubs module [types-aiobotocore-securitylake](https://pypi.org/project/types-aiobotocore-securitylake/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[securitylake]` package installed.

Write your `SecurityLake` code as usual,
type checking and code completion should work out of the box.



```python
# SecurityLakeClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("securitylake") as client:  # (1)
    result = await client.create_aws_log_source()  # (2)
```

1. client: [SecurityLakeClient](./client.md)
2. result: [:material-code-braces: CreateAwsLogSourceResponseTypeDef](./type_defs.md#createawslogsourceresponsetypedef) 



```python
# GetDataLakeSourcesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("securitylake") as client:  # (1)
    paginator = client.get_paginator("get_data_lake_sources")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SecurityLakeClient](./client.md)
2. paginator: [GetDataLakeSourcesPaginator](./paginators.md#getdatalakesourcespaginator)
3. item: [:material-code-braces: GetDataLakeSourcesResponseTypeDef](./type_defs.md#getdatalakesourcesresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[securitylake]`
or a standalone `types_aiobotocore_securitylake` package, you have to explicitly specify
`client: SecurityLakeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SecurityLakeClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_securitylake.client import SecurityLakeClient
from types_aiobotocore_securitylake.type_defs import CreateAwsLogSourceResponseTypeDef
from types_aiobotocore_securitylake.type_defs import CreateAwsLogSourceRequestRequestTypeDef


session = Session()

client: SecurityLakeClient
async with session.client("securitylake") as client:  # (1)
    kwargs: CreateAwsLogSourceRequestRequestTypeDef = {...}  # (2)
    result: CreateAwsLogSourceResponseTypeDef = await client.create_aws_log_source(**kwargs)  # (3)
```

1. client: [SecurityLakeClient](./client.md)
2. kwargs: [:material-code-braces: CreateAwsLogSourceRequestRequestTypeDef](./type_defs.md#createawslogsourcerequestrequesttypedef) 
3. result: [:material-code-braces: CreateAwsLogSourceResponseTypeDef](./type_defs.md#createawslogsourceresponsetypedef) 



```python
# GetDataLakeSourcesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_securitylake.client import SecurityLakeClient
from types_aiobotocore_securitylake.paginator import GetDataLakeSourcesPaginator
from types_aiobotocore_securitylake.type_defs import GetDataLakeSourcesResponseTypeDef


session = Session()

client: SecurityLakeClient
async with session.client("securitylake") as client:  # (1)
    paginator: GetDataLakeSourcesPaginator = client.get_paginator("get_data_lake_sources")  # (2)
    async for item in paginator.paginate(...):
        item: GetDataLakeSourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityLakeClient](./client.md)
2. paginator: [GetDataLakeSourcesPaginator](./paginators.md#getdatalakesourcespaginator)
3. item: [:material-code-braces: GetDataLakeSourcesResponseTypeDef](./type_defs.md#getdatalakesourcesresponsetypedef) 



