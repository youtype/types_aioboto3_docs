# SagemakerEdgeManager module

> [Index](../README.md) > SagemakerEdgeManager


!!! note ""

    Auto-generated documentation for [SagemakerEdgeManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
    type annotations stubs module [types-aiobotocore-sagemaker-edge](https://pypi.org/project/types-aiobotocore-sagemaker-edge/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `SagemakerEdgeManager`.

### From PyPI with pip

Install `types-aioboto3` for `SagemakerEdgeManager` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[sagemaker-edge]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[sagemaker-edge]'


# standalone installation
python -m pip install types-aiobotocore-sagemaker-edge
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-sagemaker-edge
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SagemakerEdgeManagerClient

Type annotations and code completion for  `#!python session.client("sagemaker-edge")` as [SagemakerEdgeManagerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sagemaker_edge.client import SagemakerEdgeManagerClient


session = Session()
async with session.client("sagemaker-edge") as client:
    client: SagemakerEdgeManagerClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_sagemaker_edge.literals import SagemakerEdgeManagerServiceName

def get_value() -> SagemakerEdgeManagerServiceName:
    return "sagemaker-edge"
```

- [SagemakerEdgeManagerServiceName](./literals.md#sagemakeredgemanagerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_sagemaker_edge.type_defs import EdgeMetricTypeDef

def get_value() -> EdgeMetricTypeDef:
    return {
        "Dimension": ...,
    }
```

- [EdgeMetricTypeDef](./type_defs.md#edgemetrictypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetDeviceRegistrationRequestRequestTypeDef](./type_defs.md#getdeviceregistrationrequestrequesttypedef)
- [ModelTypeDef](./type_defs.md#modeltypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetDeviceRegistrationResultTypeDef](./type_defs.md#getdeviceregistrationresulttypedef)
- [SendHeartbeatRequestRequestTypeDef](./type_defs.md#sendheartbeatrequestrequesttypedef)

