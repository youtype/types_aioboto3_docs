# MigrationHubConfig module

> [Index](../README.md) > MigrationHubConfig


!!! note ""

    Auto-generated documentation for [MigrationHubConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
    type annotations stubs module [types-aiobotocore-migrationhub-config](https://pypi.org/project/types-aiobotocore-migrationhub-config/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `MigrationHubConfig` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[migrationhub-config]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[migrationhub-config]'


# standalone installation
python -m pip install types-aiobotocore-migrationhub-config
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-migrationhub-config
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MigrationHubConfigClient

Type annotations and code completion for  `#!python session.client("migrationhub-config")` as [MigrationHubConfigClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_migrationhub_config.client import MigrationHubConfigClient


session = Session()
async with session.client("migrationhub-config") as client:
    client: MigrationHubConfigClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_migrationhub_config.literals import TargetTypeType

def get_value() -> TargetTypeType:
    return "ACCOUNT"
```

- [TargetTypeType](./literals.md#targettypetype)
- [MigrationHubConfigServiceName](./literals.md#migrationhubconfigservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_migrationhub_config.type_defs import TargetTypeDef

def get_value() -> TargetTypeDef:
    return {
        "Type": ...,
    }
```

- [TargetTypeDef](./type_defs.md#targettypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateHomeRegionControlRequestRequestTypeDef](./type_defs.md#createhomeregioncontrolrequestrequesttypedef)
- [DescribeHomeRegionControlsRequestRequestTypeDef](./type_defs.md#describehomeregioncontrolsrequestrequesttypedef)
- [HomeRegionControlTypeDef](./type_defs.md#homeregioncontroltypedef)
- [GetHomeRegionResultTypeDef](./type_defs.md#gethomeregionresulttypedef)
- [CreateHomeRegionControlResultTypeDef](./type_defs.md#createhomeregioncontrolresulttypedef)
- [DescribeHomeRegionControlsResultTypeDef](./type_defs.md#describehomeregioncontrolsresulttypedef)

