# Paginators

> [Index](../README.md) > [RedshiftDataAPIService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [RedshiftDataAPIService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
    type annotations stubs module [types-aiobotocore-redshift-data](https://pypi.org/project/types-aiobotocore-redshift-data/).

## DescribeTablePaginator

Type annotations and code completion for `#!python session.client("redshift-data").get_paginator("describe_table")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.DescribeTable)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift_data.paginator import DescribeTablePaginator

session = Session()

session = get_session()
async with session.client("redshift-data") as client:  # (1)
    paginator: DescribeTablePaginator = client.get_paginator("describe_table")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTableResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftDataAPIServiceClient](./client.md)
2. paginator: [DescribeTablePaginator](./paginators.md#describetablepaginator)
3. item: [:material-code-braces: DescribeTableResponseTypeDef](./type_defs.md#describetableresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTablePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Database: str,
    ClusterIdentifier: str = ...,
    ConnectedDatabase: str = ...,
    DbUser: str = ...,
    Schema: str = ...,
    SecretArn: str = ...,
    Table: str = ...,
    WorkgroupName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeTableResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeTableResponseTypeDef](./type_defs.md#describetableresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTableRequestDescribeTablePaginateTypeDef = {  # (1)
    "Database": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTableRequestDescribeTablePaginateTypeDef](./type_defs.md#describetablerequestdescribetablepaginatetypedef) 
## GetStatementResultPaginator

Type annotations and code completion for `#!python session.client("redshift-data").get_paginator("get_statement_result")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.GetStatementResult)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift_data.paginator import GetStatementResultPaginator

session = Session()

session = get_session()
async with session.client("redshift-data") as client:  # (1)
    paginator: GetStatementResultPaginator = client.get_paginator("get_statement_result")  # (2)
    async for item in paginator.paginate(...):
        item: GetStatementResultResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftDataAPIServiceClient](./client.md)
2. paginator: [GetStatementResultPaginator](./paginators.md#getstatementresultpaginator)
3. item: [:material-code-braces: GetStatementResultResponseTypeDef](./type_defs.md#getstatementresultresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetStatementResultPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Id: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetStatementResultResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetStatementResultResponseTypeDef](./type_defs.md#getstatementresultresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetStatementResultRequestGetStatementResultPaginateTypeDef = {  # (1)
    "Id": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetStatementResultRequestGetStatementResultPaginateTypeDef](./type_defs.md#getstatementresultrequestgetstatementresultpaginatetypedef) 
## ListDatabasesPaginator

Type annotations and code completion for `#!python session.client("redshift-data").get_paginator("list_databases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListDatabases)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift_data.paginator import ListDatabasesPaginator

session = Session()

session = get_session()
async with session.client("redshift-data") as client:  # (1)
    paginator: ListDatabasesPaginator = client.get_paginator("list_databases")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatabasesResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftDataAPIServiceClient](./client.md)
2. paginator: [ListDatabasesPaginator](./paginators.md#listdatabasespaginator)
3. item: [:material-code-braces: ListDatabasesResponseTypeDef](./type_defs.md#listdatabasesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDatabasesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Database: str,
    ClusterIdentifier: str = ...,
    DbUser: str = ...,
    SecretArn: str = ...,
    WorkgroupName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDatabasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatabasesResponseTypeDef](./type_defs.md#listdatabasesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDatabasesRequestListDatabasesPaginateTypeDef = {  # (1)
    "Database": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatabasesRequestListDatabasesPaginateTypeDef](./type_defs.md#listdatabasesrequestlistdatabasespaginatetypedef) 
## ListSchemasPaginator

Type annotations and code completion for `#!python session.client("redshift-data").get_paginator("list_schemas")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListSchemas)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift_data.paginator import ListSchemasPaginator

session = Session()

session = get_session()
async with session.client("redshift-data") as client:  # (1)
    paginator: ListSchemasPaginator = client.get_paginator("list_schemas")  # (2)
    async for item in paginator.paginate(...):
        item: ListSchemasResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftDataAPIServiceClient](./client.md)
2. paginator: [ListSchemasPaginator](./paginators.md#listschemaspaginator)
3. item: [:material-code-braces: ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSchemasPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Database: str,
    ClusterIdentifier: str = ...,
    ConnectedDatabase: str = ...,
    DbUser: str = ...,
    SchemaPattern: str = ...,
    SecretArn: str = ...,
    WorkgroupName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSchemasResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSchemasRequestListSchemasPaginateTypeDef = {  # (1)
    "Database": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchemasRequestListSchemasPaginateTypeDef](./type_defs.md#listschemasrequestlistschemaspaginatetypedef) 
## ListStatementsPaginator

Type annotations and code completion for `#!python session.client("redshift-data").get_paginator("list_statements")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListStatements)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift_data.paginator import ListStatementsPaginator

session = Session()

session = get_session()
async with session.client("redshift-data") as client:  # (1)
    paginator: ListStatementsPaginator = client.get_paginator("list_statements")  # (2)
    async for item in paginator.paginate(...):
        item: ListStatementsResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftDataAPIServiceClient](./client.md)
2. paginator: [ListStatementsPaginator](./paginators.md#liststatementspaginator)
3. item: [:material-code-braces: ListStatementsResponseTypeDef](./type_defs.md#liststatementsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListStatementsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    RoleLevel: bool = ...,
    StatementName: str = ...,
    Status: StatusStringType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListStatementsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: StatusStringType](./literals.md#statusstringtype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListStatementsResponseTypeDef](./type_defs.md#liststatementsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListStatementsRequestListStatementsPaginateTypeDef = {  # (1)
    "RoleLevel": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStatementsRequestListStatementsPaginateTypeDef](./type_defs.md#liststatementsrequestliststatementspaginatetypedef) 
## ListTablesPaginator

Type annotations and code completion for `#!python session.client("redshift-data").get_paginator("list_tables")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListTables)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_redshift_data.paginator import ListTablesPaginator

session = Session()

session = get_session()
async with session.client("redshift-data") as client:  # (1)
    paginator: ListTablesPaginator = client.get_paginator("list_tables")  # (2)
    async for item in paginator.paginate(...):
        item: ListTablesResponseTypeDef
        print(item)  # (3)
```

1. client: [RedshiftDataAPIServiceClient](./client.md)
2. paginator: [ListTablesPaginator](./paginators.md#listtablespaginator)
3. item: [:material-code-braces: ListTablesResponseTypeDef](./type_defs.md#listtablesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTablesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Database: str,
    ClusterIdentifier: str = ...,
    ConnectedDatabase: str = ...,
    DbUser: str = ...,
    SchemaPattern: str = ...,
    SecretArn: str = ...,
    TablePattern: str = ...,
    WorkgroupName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTablesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTablesResponseTypeDef](./type_defs.md#listtablesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTablesRequestListTablesPaginateTypeDef = {  # (1)
    "Database": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTablesRequestListTablesPaginateTypeDef](./type_defs.md#listtablesrequestlisttablespaginatetypedef) 
