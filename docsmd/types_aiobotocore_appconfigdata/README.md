# AppConfigData module

> [Index](../README.md) > AppConfigData


!!! note ""

    Auto-generated documentation for [AppConfigData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#appconfigdata)
    type annotations stubs module [types-aiobotocore-appconfigdata](https://pypi.org/project/types-aiobotocore-appconfigdata/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==14.1.0' mypy-boto3-builder`
1. Select `aioboto3` AWS SDK.
1. Add `AppConfigData` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `AppConfigData` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[appconfigdata]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[appconfigdata]'

# standalone installation
python -m pip install types-aiobotocore-appconfigdata
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-appconfigdata
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AppConfigDataClient

Type annotations and code completion for  `#!python session.client("appconfigdata")` as [AppConfigDataClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData.Client)

```python
# AppConfigDataClient usage example

from aioboto3.session import Session

from types_aiobotocore_appconfigdata.client import AppConfigDataClient


session = Session()
async with session.client("appconfigdata") as client:
    client: AppConfigDataClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AppConfigDataServiceName usage example

from types_aiobotocore_appconfigdata.literals import AppConfigDataServiceName

def get_value() -> AppConfigDataServiceName:
    return "appconfigdata"
```

- [AppConfigDataServiceName](./literals.md#appconfigdataservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [GetLatestConfigurationRequestTypeDef](./type_defs.md#getlatestconfigurationrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [StartConfigurationSessionRequestTypeDef](./type_defs.md#startconfigurationsessionrequesttypedef)
- [GetLatestConfigurationResponseTypeDef](./type_defs.md#getlatestconfigurationresponsetypedef)
- [StartConfigurationSessionResponseTypeDef](./type_defs.md#startconfigurationsessionresponsetypedef)

