# ForecastQueryService module

> [Index](../README.md) > ForecastQueryService


!!! note ""

    Auto-generated documentation for [ForecastQueryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService)
    type annotations stubs module [types-aiobotocore-forecastquery](https://pypi.org/project/types-aiobotocore-forecastquery/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `ForecastQueryService` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[forecastquery]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[forecastquery]'


# standalone installation
python -m pip install types-aiobotocore-forecastquery
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-forecastquery
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ForecastQueryServiceClient

Type annotations and code completion for  `#!python session.client("forecastquery")` as [ForecastQueryServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_forecastquery.client import ForecastQueryServiceClient


session = Session()
async with session.client("forecastquery") as client:
    client: ForecastQueryServiceClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_forecastquery.literals import ForecastQueryServiceServiceName

def get_value() -> ForecastQueryServiceServiceName:
    return "forecastquery"
```

- [ForecastQueryServiceServiceName](./literals.md#forecastqueryserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_forecastquery.type_defs import DataPointTypeDef

def get_value() -> DataPointTypeDef:
    return {
        "Timestamp": ...,
    }
```

- [DataPointTypeDef](./type_defs.md#datapointtypedef)
- [QueryForecastRequestRequestTypeDef](./type_defs.md#queryforecastrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ForecastTypeDef](./type_defs.md#forecasttypedef)
- [QueryForecastResponseTypeDef](./type_defs.md#queryforecastresponsetypedef)

