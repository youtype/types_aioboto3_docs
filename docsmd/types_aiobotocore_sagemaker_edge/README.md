# SagemakerEdgeManager module

> [Index](../README.md) > SagemakerEdgeManager


!!! note ""

    Auto-generated documentation for [SagemakerEdgeManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#sagemakeredgemanager)
    type annotations stubs module [types-aiobotocore-sagemaker-edge](https://pypi.org/project/types-aiobotocore-sagemaker-edge/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `SagemakerEdgeManager` service.
1. Use provided commands to install generated packages.



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

```python
# SagemakerEdgeManagerClient usage example

from aioboto3.session import Session

from types_aiobotocore_sagemaker_edge.client import SagemakerEdgeManagerClient


session = Session()
async with session.client("sagemaker-edge") as client:
    client: SagemakerEdgeManagerClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ChecksumTypeType usage example

from types_aiobotocore_sagemaker_edge.literals import ChecksumTypeType

def get_value() -> ChecksumTypeType:
    return "SHA1"
```

- [ChecksumTypeType](./literals.md#checksumtypetype)
- [DeploymentStatusType](./literals.md#deploymentstatustype)
- [DeploymentTypeType](./literals.md#deploymenttypetype)
- [FailureHandlingPolicyType](./literals.md#failurehandlingpolicytype)
- [ModelStateType](./literals.md#modelstatetype)
- [SagemakerEdgeManagerServiceName](./literals.md#sagemakeredgemanagerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ChecksumTypeDef](./type_defs.md#checksumtypedef)
- [DeploymentModelTypeDef](./type_defs.md#deploymentmodeltypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetDeploymentsRequestRequestTypeDef](./type_defs.md#getdeploymentsrequestrequesttypedef)
- [GetDeviceRegistrationRequestRequestTypeDef](./type_defs.md#getdeviceregistrationrequestrequesttypedef)
- [DefinitionTypeDef](./type_defs.md#definitiontypedef)
- [DeploymentResultTypeDef](./type_defs.md#deploymentresulttypedef)
- [EdgeMetricTypeDef](./type_defs.md#edgemetrictypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetDeviceRegistrationResultTypeDef](./type_defs.md#getdeviceregistrationresulttypedef)
- [EdgeDeploymentTypeDef](./type_defs.md#edgedeploymenttypedef)
- [ModelTypeDef](./type_defs.md#modeltypedef)
- [GetDeploymentsResultTypeDef](./type_defs.md#getdeploymentsresulttypedef)
- [SendHeartbeatRequestRequestTypeDef](./type_defs.md#sendheartbeatrequestrequesttypedef)
