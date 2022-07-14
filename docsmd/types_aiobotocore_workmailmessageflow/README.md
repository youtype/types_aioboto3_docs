# WorkMailMessageFlow module

> [Index](../README.md) > WorkMailMessageFlow


!!! note ""

    Auto-generated documentation for [WorkMailMessageFlow](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow)
    type annotations stubs module [types-aiobotocore-workmailmessageflow](https://pypi.org/project/types-aiobotocore-workmailmessageflow/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `WorkMailMessageFlow`.

### From PyPI with pip

Install `types-aioboto3` for `WorkMailMessageFlow` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[workmailmessageflow]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[workmailmessageflow]'


# standalone installation
python -m pip install types-aiobotocore-workmailmessageflow
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-workmailmessageflow
```

## Usage

Code samples can be found in [Examples](./usage.md).

## WorkMailMessageFlowClient

Type annotations and code completion for  `#!python session.client("workmailmessageflow")` as [WorkMailMessageFlowClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_workmailmessageflow.client import WorkMailMessageFlowClient


session = Session()
async with session.client("workmailmessageflow") as client:
    client: WorkMailMessageFlowClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_workmailmessageflow.literals import WorkMailMessageFlowServiceName

def get_value() -> WorkMailMessageFlowServiceName:
    return "workmailmessageflow"
```

- [WorkMailMessageFlowServiceName](./literals.md#workmailmessageflowservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_workmailmessageflow.type_defs import GetRawMessageContentRequestRequestTypeDef

def get_value() -> GetRawMessageContentRequestRequestTypeDef:
    return {
        "messageId": ...,
    }
```

- [GetRawMessageContentRequestRequestTypeDef](./type_defs.md#getrawmessagecontentrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [S3ReferenceTypeDef](./type_defs.md#s3referencetypedef)
- [GetRawMessageContentResponseTypeDef](./type_defs.md#getrawmessagecontentresponsetypedef)
- [RawMessageContentTypeDef](./type_defs.md#rawmessagecontenttypedef)
- [PutRawMessageContentRequestRequestTypeDef](./type_defs.md#putrawmessagecontentrequestrequesttypedef)

