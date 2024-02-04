# inspectorscan module

> [Index](../README.md) > inspectorscan


!!! note ""

    Auto-generated documentation for [inspectorscan](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan.html#inspectorscan)
    type annotations stubs module [types-aiobotocore-inspector-scan](https://pypi.org/project/types-aiobotocore-inspector-scan/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `inspectorscan` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[inspector-scan]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[inspector-scan]'


# standalone installation
python -m pip install types-aiobotocore-inspector-scan
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-inspector-scan
```

## Usage

Code samples can be found in [Examples](./usage.md).

## inspectorscanClient

Type annotations and code completion for  `#!python session.client("inspector-scan")` as [inspectorscanClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan.html#inspectorscan.Client)

```python
# inspectorscanClient usage example

from aioboto3.session import Session

from types_aiobotocore_inspector_scan.client import inspectorscanClient


session = Session()
async with session.client("inspector-scan") as client:
    client: inspectorscanClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# OutputFormatType usage example

from types_aiobotocore_inspector_scan.literals import OutputFormatType

def get_value() -> OutputFormatType:
    return "CYCLONE_DX_1_5"
```

- [OutputFormatType](./literals.md#outputformattype)
- [inspectorscanServiceName](./literals.md#inspectorscanservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ScanSbomRequestRequestTypeDef](./type_defs.md#scansbomrequestrequesttypedef)
- [ScanSbomResponseTypeDef](./type_defs.md#scansbomresponsetypedef)

