# RDSDataService module

> [Index](../README.md) > RDSDataService


!!! note ""

    Auto-generated documentation for [RDSDataService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#rdsdataservice)
    type annotations stubs module [types-aiobotocore-rds-data](https://pypi.org/project/types-aiobotocore-rds-data/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `RDSDataService` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `RDSDataService` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[rds-data]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[rds-data]'

# standalone installation
python -m pip install types-aiobotocore-rds-data
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-rds-data
```

## Usage

Code samples can be found in [Examples](./usage.md).

## RDSDataServiceClient

Type annotations and code completion for  `#!python session.client("rds-data")` as [RDSDataServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client)

```python
# RDSDataServiceClient usage example

from aioboto3.session import Session

from types_aiobotocore_rds_data.client import RDSDataServiceClient


session = Session()
async with session.client("rds-data") as client:
    client: RDSDataServiceClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DecimalReturnTypeType usage example

from types_aiobotocore_rds_data.literals import DecimalReturnTypeType

def get_value() -> DecimalReturnTypeType:
    return "DOUBLE_OR_LONG"
```

- [DecimalReturnTypeType](./literals.md#decimalreturntypetype)
- [LongReturnTypeType](./literals.md#longreturntypetype)
- [RecordsFormatTypeType](./literals.md#recordsformattypetype)
- [TypeHintType](./literals.md#typehinttype)
- [RDSDataServiceServiceName](./literals.md#rdsdataserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ArrayValueOutputTypeDef](./type_defs.md#arrayvalueoutputtypedef)
- [ArrayValueTypeDef](./type_defs.md#arrayvaluetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BeginTransactionRequestRequestTypeDef](./type_defs.md#begintransactionrequestrequesttypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [ColumnMetadataTypeDef](./type_defs.md#columnmetadatatypedef)
- [CommitTransactionRequestRequestTypeDef](./type_defs.md#committransactionrequestrequesttypedef)
- [ExecuteSqlRequestRequestTypeDef](./type_defs.md#executesqlrequestrequesttypedef)
- [ResultSetOptionsTypeDef](./type_defs.md#resultsetoptionstypedef)
- [RollbackTransactionRequestRequestTypeDef](./type_defs.md#rollbacktransactionrequestrequesttypedef)
- [StructValueTypeDef](./type_defs.md#structvaluetypedef)
- [FieldOutputTypeDef](./type_defs.md#fieldoutputtypedef)
- [ArrayValueUnionTypeDef](./type_defs.md#arrayvalueuniontypedef)
- [BeginTransactionResponseTypeDef](./type_defs.md#begintransactionresponsetypedef)
- [CommitTransactionResponseTypeDef](./type_defs.md#committransactionresponsetypedef)
- [RollbackTransactionResponseTypeDef](./type_defs.md#rollbacktransactionresponsetypedef)
- [ResultSetMetadataTypeDef](./type_defs.md#resultsetmetadatatypedef)
- [ValueTypeDef](./type_defs.md#valuetypedef)
- [ExecuteStatementResponseTypeDef](./type_defs.md#executestatementresponsetypedef)
- [UpdateResultTypeDef](./type_defs.md#updateresulttypedef)
- [FieldTypeDef](./type_defs.md#fieldtypedef)
- [RecordTypeDef](./type_defs.md#recordtypedef)
- [BatchExecuteStatementResponseTypeDef](./type_defs.md#batchexecutestatementresponsetypedef)
- [FieldUnionTypeDef](./type_defs.md#fielduniontypedef)
- [ResultFrameTypeDef](./type_defs.md#resultframetypedef)
- [SqlParameterTypeDef](./type_defs.md#sqlparametertypedef)
- [SqlStatementResultTypeDef](./type_defs.md#sqlstatementresulttypedef)
- [BatchExecuteStatementRequestRequestTypeDef](./type_defs.md#batchexecutestatementrequestrequesttypedef)
- [ExecuteStatementRequestRequestTypeDef](./type_defs.md#executestatementrequestrequesttypedef)
- [ExecuteSqlResponseTypeDef](./type_defs.md#executesqlresponsetypedef)
