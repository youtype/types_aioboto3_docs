# RDSDataService module

> [Index](../README.md) > RDSDataService


!!! note ""

    Auto-generated documentation for [RDSDataService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
    type annotations stubs module [types-aiobotocore-rds-data](https://pypi.org/project/types-aiobotocore-rds-data/).

## How to install



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

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_rds_data.client import RDSDataServiceClient


session = Session()
async with session.client("rds-data") as client:
    client: RDSDataServiceClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_rds_data.literals import DecimalReturnTypeType

def get_value() -> DecimalReturnTypeType:
    return "DOUBLE_OR_LONG"
```

- [DecimalReturnTypeType](./literals.md#decimalreturntypetype)
- [TypeHintType](./literals.md#typehinttype)
- [RDSDataServiceServiceName](./literals.md#rdsdataserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_rds_data.type_defs import ArrayValueTypeDef

def get_value() -> ArrayValueTypeDef:
    return {
        "arrayValues": ...,
    }
```

- [ArrayValueTypeDef](./type_defs.md#arrayvaluetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BeginTransactionRequestRequestTypeDef](./type_defs.md#begintransactionrequestrequesttypedef)
- [ColumnMetadataTypeDef](./type_defs.md#columnmetadatatypedef)
- [CommitTransactionRequestRequestTypeDef](./type_defs.md#committransactionrequestrequesttypedef)
- [ExecuteSqlRequestRequestTypeDef](./type_defs.md#executesqlrequestrequesttypedef)
- [ResultSetOptionsTypeDef](./type_defs.md#resultsetoptionstypedef)
- [FieldTypeDef](./type_defs.md#fieldtypedef)
- [RecordTypeDef](./type_defs.md#recordtypedef)
- [RollbackTransactionRequestRequestTypeDef](./type_defs.md#rollbacktransactionrequestrequesttypedef)
- [StructValueTypeDef](./type_defs.md#structvaluetypedef)
- [ValueTypeDef](./type_defs.md#valuetypedef)
- [BeginTransactionResponseTypeDef](./type_defs.md#begintransactionresponsetypedef)
- [CommitTransactionResponseTypeDef](./type_defs.md#committransactionresponsetypedef)
- [RollbackTransactionResponseTypeDef](./type_defs.md#rollbacktransactionresponsetypedef)
- [ResultSetMetadataTypeDef](./type_defs.md#resultsetmetadatatypedef)
- [ExecuteStatementResponseTypeDef](./type_defs.md#executestatementresponsetypedef)
- [SqlParameterTypeDef](./type_defs.md#sqlparametertypedef)
- [UpdateResultTypeDef](./type_defs.md#updateresulttypedef)
- [ResultFrameTypeDef](./type_defs.md#resultframetypedef)
- [BatchExecuteStatementRequestRequestTypeDef](./type_defs.md#batchexecutestatementrequestrequesttypedef)
- [ExecuteStatementRequestRequestTypeDef](./type_defs.md#executestatementrequestrequesttypedef)
- [BatchExecuteStatementResponseTypeDef](./type_defs.md#batchexecutestatementresponsetypedef)
- [SqlStatementResultTypeDef](./type_defs.md#sqlstatementresulttypedef)
- [ExecuteSqlResponseTypeDef](./type_defs.md#executesqlresponsetypedef)

