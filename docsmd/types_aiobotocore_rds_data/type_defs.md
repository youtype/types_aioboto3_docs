# Type definitions

> [Index](../README.md) > [RDSDataService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [RDSDataService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#rdsdataservice)
    type annotations stubs module [types-aiobotocore-rds-data](https://pypi.org/project/types-aiobotocore-rds-data/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## ArrayValueUnionTypeDef

```python
# ArrayValueUnionTypeDef definition

ArrayValueUnionTypeDef = Union[
    ArrayValueTypeDef,  # (1)
    ArrayValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ArrayValueTypeDef](./type_defs.md#arrayvaluetypedef) 
2. See [:material-code-braces: ArrayValueOutputTypeDef](./type_defs.md#arrayvalueoutputtypedef) 

## FieldUnionTypeDef

```python
# FieldUnionTypeDef definition

FieldUnionTypeDef = Union[
    FieldTypeDef,  # (1)
    FieldOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) 
2. See [:material-code-braces: FieldOutputTypeDef](./type_defs.md#fieldoutputtypedef) 



## ArrayValueOutputTypeDef

```python
# ArrayValueOutputTypeDef definition

class ArrayValueOutputTypeDef(TypedDict):
    booleanValues: NotRequired[list[bool]],
    longValues: NotRequired[list[int]],
    doubleValues: NotRequired[list[float]],
    stringValues: NotRequired[list[str]],
    arrayValues: NotRequired[list[dict[str, Any]]],
```

## ArrayValueTypeDef

```python
# ArrayValueTypeDef definition

class ArrayValueTypeDef(TypedDict):
    booleanValues: NotRequired[Sequence[bool]],
    longValues: NotRequired[Sequence[int]],
    doubleValues: NotRequired[Sequence[float]],
    stringValues: NotRequired[Sequence[str]],
    arrayValues: NotRequired[Sequence[Mapping[str, Any]]],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## BeginTransactionRequestRequestTypeDef

```python
# BeginTransactionRequestRequestTypeDef definition

class BeginTransactionRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    secretArn: str,
    database: NotRequired[str],
    schema: NotRequired[str],
```

## ColumnMetadataTypeDef

```python
# ColumnMetadataTypeDef definition

class ColumnMetadataTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[int],
    typeName: NotRequired[str],
    label: NotRequired[str],
    schemaName: NotRequired[str],
    tableName: NotRequired[str],
    isAutoIncrement: NotRequired[bool],
    isSigned: NotRequired[bool],
    isCurrency: NotRequired[bool],
    isCaseSensitive: NotRequired[bool],
    nullable: NotRequired[int],
    precision: NotRequired[int],
    scale: NotRequired[int],
    arrayBaseColumnType: NotRequired[int],
```

## CommitTransactionRequestRequestTypeDef

```python
# CommitTransactionRequestRequestTypeDef definition

class CommitTransactionRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    secretArn: str,
    transactionId: str,
```

## ExecuteSqlRequestRequestTypeDef

```python
# ExecuteSqlRequestRequestTypeDef definition

class ExecuteSqlRequestRequestTypeDef(TypedDict):
    dbClusterOrInstanceArn: str,
    awsSecretStoreArn: str,
    sqlStatements: str,
    database: NotRequired[str],
    schema: NotRequired[str],
```

## ResultSetOptionsTypeDef

```python
# ResultSetOptionsTypeDef definition

class ResultSetOptionsTypeDef(TypedDict):
    decimalReturnType: NotRequired[DecimalReturnTypeType],  # (1)
    longReturnType: NotRequired[LongReturnTypeType],  # (2)
```

1. See [:material-code-brackets: DecimalReturnTypeType](./literals.md#decimalreturntypetype) 
2. See [:material-code-brackets: LongReturnTypeType](./literals.md#longreturntypetype) 
## RollbackTransactionRequestRequestTypeDef

```python
# RollbackTransactionRequestRequestTypeDef definition

class RollbackTransactionRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    secretArn: str,
    transactionId: str,
```

## StructValueTypeDef

```python
# StructValueTypeDef definition

class StructValueTypeDef(TypedDict):
    attributes: NotRequired[list[dict[str, Any]]],
```

## FieldOutputTypeDef

```python
# FieldOutputTypeDef definition

class FieldOutputTypeDef(TypedDict):
    isNull: NotRequired[bool],
    booleanValue: NotRequired[bool],
    longValue: NotRequired[int],
    doubleValue: NotRequired[float],
    stringValue: NotRequired[str],
    blobValue: NotRequired[bytes],
    arrayValue: NotRequired[ArrayValueOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ArrayValueOutputTypeDef](./type_defs.md#arrayvalueoutputtypedef) 
## BeginTransactionResponseTypeDef

```python
# BeginTransactionResponseTypeDef definition

class BeginTransactionResponseTypeDef(TypedDict):
    transactionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CommitTransactionResponseTypeDef

```python
# CommitTransactionResponseTypeDef definition

class CommitTransactionResponseTypeDef(TypedDict):
    transactionStatus: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RollbackTransactionResponseTypeDef

```python
# RollbackTransactionResponseTypeDef definition

class RollbackTransactionResponseTypeDef(TypedDict):
    transactionStatus: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResultSetMetadataTypeDef

```python
# ResultSetMetadataTypeDef definition

class ResultSetMetadataTypeDef(TypedDict):
    columnCount: NotRequired[int],
    columnMetadata: NotRequired[list[ColumnMetadataTypeDef]],  # (1)
```

1. See [:material-code-braces: ColumnMetadataTypeDef](./type_defs.md#columnmetadatatypedef) 
## ValueTypeDef

```python
# ValueTypeDef definition

class ValueTypeDef(TypedDict):
    isNull: NotRequired[bool],
    bitValue: NotRequired[bool],
    bigIntValue: NotRequired[int],
    intValue: NotRequired[int],
    doubleValue: NotRequired[float],
    realValue: NotRequired[float],
    stringValue: NotRequired[str],
    blobValue: NotRequired[bytes],
    arrayValues: NotRequired[list[dict[str, Any]]],
    structValue: NotRequired[StructValueTypeDef],  # (1)
```

1. See [:material-code-braces: StructValueTypeDef](./type_defs.md#structvaluetypedef) 
## ExecuteStatementResponseTypeDef

```python
# ExecuteStatementResponseTypeDef definition

class ExecuteStatementResponseTypeDef(TypedDict):
    records: list[list[FieldOutputTypeDef]],  # (1)
    columnMetadata: list[ColumnMetadataTypeDef],  # (2)
    numberOfRecordsUpdated: int,
    generatedFields: list[FieldOutputTypeDef],  # (3)
    formattedRecords: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: FieldOutputTypeDef](./type_defs.md#fieldoutputtypedef) 
2. See [:material-code-braces: ColumnMetadataTypeDef](./type_defs.md#columnmetadatatypedef) 
3. See [:material-code-braces: FieldOutputTypeDef](./type_defs.md#fieldoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateResultTypeDef

```python
# UpdateResultTypeDef definition

class UpdateResultTypeDef(TypedDict):
    generatedFields: NotRequired[list[FieldOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: FieldOutputTypeDef](./type_defs.md#fieldoutputtypedef) 
## FieldTypeDef

```python
# FieldTypeDef definition

class FieldTypeDef(TypedDict):
    isNull: NotRequired[bool],
    booleanValue: NotRequired[bool],
    longValue: NotRequired[int],
    doubleValue: NotRequired[float],
    stringValue: NotRequired[str],
    blobValue: NotRequired[BlobTypeDef],
    arrayValue: NotRequired[ArrayValueUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ArrayValueTypeDef](./type_defs.md#arrayvaluetypedef) [:material-code-braces: ArrayValueOutputTypeDef](./type_defs.md#arrayvalueoutputtypedef) 
## RecordTypeDef

```python
# RecordTypeDef definition

class RecordTypeDef(TypedDict):
    values: NotRequired[list[ValueTypeDef]],  # (1)
```

1. See [:material-code-braces: ValueTypeDef](./type_defs.md#valuetypedef) 
## BatchExecuteStatementResponseTypeDef

```python
# BatchExecuteStatementResponseTypeDef definition

class BatchExecuteStatementResponseTypeDef(TypedDict):
    updateResults: list[UpdateResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateResultTypeDef](./type_defs.md#updateresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResultFrameTypeDef

```python
# ResultFrameTypeDef definition

class ResultFrameTypeDef(TypedDict):
    resultSetMetadata: NotRequired[ResultSetMetadataTypeDef],  # (1)
    records: NotRequired[list[RecordTypeDef]],  # (2)
```

1. See [:material-code-braces: ResultSetMetadataTypeDef](./type_defs.md#resultsetmetadatatypedef) 
2. See [:material-code-braces: RecordTypeDef](./type_defs.md#recordtypedef) 
## SqlParameterTypeDef

```python
# SqlParameterTypeDef definition

class SqlParameterTypeDef(TypedDict):
    name: NotRequired[str],
    value: NotRequired[FieldUnionTypeDef],  # (1)
    typeHint: NotRequired[TypeHintType],  # (2)
```

1. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) [:material-code-braces: FieldOutputTypeDef](./type_defs.md#fieldoutputtypedef) 
2. See [:material-code-brackets: TypeHintType](./literals.md#typehinttype) 
## SqlStatementResultTypeDef

```python
# SqlStatementResultTypeDef definition

class SqlStatementResultTypeDef(TypedDict):
    resultFrame: NotRequired[ResultFrameTypeDef],  # (1)
    numberOfRecordsUpdated: NotRequired[int],
```

1. See [:material-code-braces: ResultFrameTypeDef](./type_defs.md#resultframetypedef) 
## BatchExecuteStatementRequestRequestTypeDef

```python
# BatchExecuteStatementRequestRequestTypeDef definition

class BatchExecuteStatementRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    secretArn: str,
    sql: str,
    database: NotRequired[str],
    schema: NotRequired[str],
    parameterSets: NotRequired[Sequence[Sequence[SqlParameterTypeDef]]],  # (1)
    transactionId: NotRequired[str],
```

1. See [:material-code-braces: SqlParameterTypeDef](./type_defs.md#sqlparametertypedef) 
## ExecuteStatementRequestRequestTypeDef

```python
# ExecuteStatementRequestRequestTypeDef definition

class ExecuteStatementRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    secretArn: str,
    sql: str,
    database: NotRequired[str],
    schema: NotRequired[str],
    parameters: NotRequired[Sequence[SqlParameterTypeDef]],  # (1)
    transactionId: NotRequired[str],
    includeResultMetadata: NotRequired[bool],
    continueAfterTimeout: NotRequired[bool],
    resultSetOptions: NotRequired[ResultSetOptionsTypeDef],  # (2)
    formatRecordsAs: NotRequired[RecordsFormatTypeType],  # (3)
```

1. See [:material-code-braces: SqlParameterTypeDef](./type_defs.md#sqlparametertypedef) 
2. See [:material-code-braces: ResultSetOptionsTypeDef](./type_defs.md#resultsetoptionstypedef) 
3. See [:material-code-brackets: RecordsFormatTypeType](./literals.md#recordsformattypetype) 
## ExecuteSqlResponseTypeDef

```python
# ExecuteSqlResponseTypeDef definition

class ExecuteSqlResponseTypeDef(TypedDict):
    sqlStatementResults: list[SqlStatementResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SqlStatementResultTypeDef](./type_defs.md#sqlstatementresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 