# RuntimeforBedrockDataAutomation module

> [Index](../README.md) > RuntimeforBedrockDataAutomation


!!! note ""

    Auto-generated documentation for [RuntimeforBedrockDataAutomation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation-runtime.html#runtimeforbedrockdataautomation)
    type annotations stubs module [types-aiobotocore-bedrock-data-automation-runtime](https://pypi.org/project/types-aiobotocore-bedrock-data-automation-runtime/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `RuntimeforBedrockDataAutomation` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `RuntimeforBedrockDataAutomation` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[bedrock-data-automation-runtime]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[bedrock-data-automation-runtime]'

# standalone installation
python -m pip install types-aiobotocore-bedrock-data-automation-runtime
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-bedrock-data-automation-runtime
```

## Usage

Code samples can be found in [Examples](./usage.md).

## RuntimeforBedrockDataAutomationClient

Type annotations and code completion for  `#!python session.client("bedrock-data-automation-runtime")` as [RuntimeforBedrockDataAutomationClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation-runtime.html#RuntimeforBedrockDataAutomation.Client)

```python
# RuntimeforBedrockDataAutomationClient usage example

from aioboto3.session import Session

from types_aiobotocore_bedrock_data_automation_runtime.client import RuntimeforBedrockDataAutomationClient


session = Session()
async with session.client("bedrock-data-automation-runtime") as client:
    client: RuntimeforBedrockDataAutomationClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AutomationJobStatusType usage example

from types_aiobotocore_bedrock_data_automation_runtime.literals import AutomationJobStatusType

def get_value() -> AutomationJobStatusType:
    return "ClientError"
```

- [AutomationJobStatusType](./literals.md#automationjobstatustype)
- [BlueprintStageType](./literals.md#blueprintstagetype)
- [DataAutomationStageType](./literals.md#dataautomationstagetype)
- [RuntimeforBedrockDataAutomationServiceName](./literals.md#runtimeforbedrockdataautomationservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BlueprintTypeDef](./type_defs.md#blueprinttypedef)
- [DataAutomationConfigurationTypeDef](./type_defs.md#dataautomationconfigurationtypedef)
- [EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
- [EventBridgeConfigurationTypeDef](./type_defs.md#eventbridgeconfigurationtypedef)
- [GetDataAutomationStatusRequestRequestTypeDef](./type_defs.md#getdataautomationstatusrequestrequesttypedef)
- [OutputConfigurationTypeDef](./type_defs.md#outputconfigurationtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [InputConfigurationTypeDef](./type_defs.md#inputconfigurationtypedef)
- [NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef)
- [GetDataAutomationStatusResponseTypeDef](./type_defs.md#getdataautomationstatusresponsetypedef)
- [InvokeDataAutomationAsyncResponseTypeDef](./type_defs.md#invokedataautomationasyncresponsetypedef)
- [InvokeDataAutomationAsyncRequestRequestTypeDef](./type_defs.md#invokedataautomationasyncrequestrequesttypedef)
