# Inspectorscan module

> [Index](../README.md) > Inspectorscan


!!! note ""

    Auto-generated documentation for [Inspectorscan](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan.html#inspectorscan)
    type annotations stubs module [types-aiobotocore-inspector-scan](https://pypi.org/project/types-aiobotocore-inspector-scan/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `Inspectorscan` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `Inspectorscan` service.

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

## InspectorscanClient

Type annotations and code completion for  `#!python session.client("inspector-scan")` as [InspectorscanClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan.html#Inspectorscan.Client)

```python
# InspectorscanClient usage example

from aioboto3.session import Session

from types_aiobotocore_inspector_scan.client import InspectorscanClient


session = Session()
async with session.client("inspector-scan") as client:
    client: InspectorscanClient
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
- [InspectorscanServiceName](./literals.md#inspectorscanservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ScanSbomRequestRequestTypeDef](./type_defs.md#scansbomrequestrequesttypedef)
- [ScanSbomResponseTypeDef](./type_defs.md#scansbomresponsetypedef)
