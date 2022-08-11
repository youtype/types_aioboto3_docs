# QLDBSession module

> [Index](../README.md) > QLDBSession


!!! note ""

    Auto-generated documentation for [QLDBSession](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession)
    type annotations stubs module [types-aiobotocore-qldb-session](https://pypi.org/project/types-aiobotocore-qldb-session/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `QLDBSession` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[qldb-session]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[qldb-session]'


# standalone installation
python -m pip install types-aiobotocore-qldb-session
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-qldb-session
```

## Usage

Code samples can be found in [Examples](./usage.md).

## QLDBSessionClient

Type annotations and code completion for  `#!python session.client("qldb-session")` as [QLDBSessionClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_qldb_session.client import QLDBSessionClient


session = Session()
async with session.client("qldb-session") as client:
    client: QLDBSessionClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_qldb_session.literals import QLDBSessionServiceName

def get_value() -> QLDBSessionServiceName:
    return "qldb-session"
```

- [QLDBSessionServiceName](./literals.md#qldbsessionservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_qldb_session.type_defs import TimingInformationTypeDef

def get_value() -> TimingInformationTypeDef:
    return {
        "ProcessingTimeMilliseconds": ...,
    }
```

- [TimingInformationTypeDef](./type_defs.md#timinginformationtypedef)
- [CommitTransactionRequestTypeDef](./type_defs.md#committransactionrequesttypedef)
- [IOUsageTypeDef](./type_defs.md#iousagetypedef)
- [ValueHolderTypeDef](./type_defs.md#valueholdertypedef)
- [FetchPageRequestTypeDef](./type_defs.md#fetchpagerequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [StartSessionRequestTypeDef](./type_defs.md#startsessionrequesttypedef)
- [AbortTransactionResultTypeDef](./type_defs.md#aborttransactionresulttypedef)
- [EndSessionResultTypeDef](./type_defs.md#endsessionresulttypedef)
- [StartSessionResultTypeDef](./type_defs.md#startsessionresulttypedef)
- [StartTransactionResultTypeDef](./type_defs.md#starttransactionresulttypedef)
- [CommitTransactionResultTypeDef](./type_defs.md#committransactionresulttypedef)
- [ExecuteStatementRequestTypeDef](./type_defs.md#executestatementrequesttypedef)
- [PageTypeDef](./type_defs.md#pagetypedef)
- [SendCommandRequestRequestTypeDef](./type_defs.md#sendcommandrequestrequesttypedef)
- [ExecuteStatementResultTypeDef](./type_defs.md#executestatementresulttypedef)
- [FetchPageResultTypeDef](./type_defs.md#fetchpageresulttypedef)
- [SendCommandResultTypeDef](./type_defs.md#sendcommandresulttypedef)

