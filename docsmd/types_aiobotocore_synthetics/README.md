# Synthetics module

> [Index](../README.md) > Synthetics


!!! note ""

    Auto-generated documentation for [Synthetics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
    type annotations stubs module [types-aiobotocore-synthetics](https://pypi.org/project/types-aiobotocore-synthetics/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `Synthetics`.

### From PyPI with pip

Install `types-aioboto3` for `Synthetics` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[synthetics]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[synthetics]'


# standalone installation
python -m pip install types-aiobotocore-synthetics
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-synthetics
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SyntheticsClient

Type annotations and code completion for  `#!python session.client("synthetics")` as [SyntheticsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_synthetics.client import SyntheticsClient


session = Session()
async with session.client("synthetics") as client:
    client: SyntheticsClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_synthetics.literals import CanaryRunStateReasonCodeType

def get_value() -> CanaryRunStateReasonCodeType:
    return "CANARY_FAILURE"
```

- [CanaryRunStateReasonCodeType](./literals.md#canaryrunstatereasoncodetype)
- [CanaryRunStateType](./literals.md#canaryrunstatetype)
- [CanaryStateReasonCodeType](./literals.md#canarystatereasoncodetype)
- [CanaryStateType](./literals.md#canarystatetype)
- [EncryptionModeType](./literals.md#encryptionmodetype)
- [SyntheticsServiceName](./literals.md#syntheticsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_synthetics.type_defs import S3EncryptionConfigTypeDef

def get_value() -> S3EncryptionConfigTypeDef:
    return {
        "EncryptionMode": ...,
    }
```

- [S3EncryptionConfigTypeDef](./type_defs.md#s3encryptionconfigtypedef)
- [AssociateResourceRequestRequestTypeDef](./type_defs.md#associateresourcerequestrequesttypedef)
- [BaseScreenshotTypeDef](./type_defs.md#basescreenshottypedef)
- [CanaryCodeInputTypeDef](./type_defs.md#canarycodeinputtypedef)
- [CanaryCodeOutputTypeDef](./type_defs.md#canarycodeoutputtypedef)
- [CanaryRunConfigInputTypeDef](./type_defs.md#canaryrunconfiginputtypedef)
- [CanaryRunConfigOutputTypeDef](./type_defs.md#canaryrunconfigoutputtypedef)
- [CanaryRunStatusTypeDef](./type_defs.md#canaryrunstatustypedef)
- [CanaryRunTimelineTypeDef](./type_defs.md#canaryruntimelinetypedef)
- [CanaryScheduleInputTypeDef](./type_defs.md#canaryscheduleinputtypedef)
- [CanaryScheduleOutputTypeDef](./type_defs.md#canaryscheduleoutputtypedef)
- [CanaryStatusTypeDef](./type_defs.md#canarystatustypedef)
- [CanaryTimelineTypeDef](./type_defs.md#canarytimelinetypedef)
- [VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef)
- [VpcConfigInputTypeDef](./type_defs.md#vpcconfiginputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateGroupRequestRequestTypeDef](./type_defs.md#creategrouprequestrequesttypedef)
- [GroupTypeDef](./type_defs.md#grouptypedef)
- [DeleteCanaryRequestRequestTypeDef](./type_defs.md#deletecanaryrequestrequesttypedef)
- [DeleteGroupRequestRequestTypeDef](./type_defs.md#deletegrouprequestrequesttypedef)
- [DescribeCanariesLastRunRequestRequestTypeDef](./type_defs.md#describecanarieslastrunrequestrequesttypedef)
- [DescribeCanariesRequestRequestTypeDef](./type_defs.md#describecanariesrequestrequesttypedef)
- [DescribeRuntimeVersionsRequestRequestTypeDef](./type_defs.md#describeruntimeversionsrequestrequesttypedef)
- [RuntimeVersionTypeDef](./type_defs.md#runtimeversiontypedef)
- [DisassociateResourceRequestRequestTypeDef](./type_defs.md#disassociateresourcerequestrequesttypedef)
- [GetCanaryRequestRequestTypeDef](./type_defs.md#getcanaryrequestrequesttypedef)
- [GetCanaryRunsRequestRequestTypeDef](./type_defs.md#getcanaryrunsrequestrequesttypedef)
- [GetGroupRequestRequestTypeDef](./type_defs.md#getgrouprequestrequesttypedef)
- [GroupSummaryTypeDef](./type_defs.md#groupsummarytypedef)
- [ListAssociatedGroupsRequestRequestTypeDef](./type_defs.md#listassociatedgroupsrequestrequesttypedef)
- [ListGroupResourcesRequestRequestTypeDef](./type_defs.md#listgroupresourcesrequestrequesttypedef)
- [ListGroupsRequestRequestTypeDef](./type_defs.md#listgroupsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [StartCanaryRequestRequestTypeDef](./type_defs.md#startcanaryrequestrequesttypedef)
- [StopCanaryRequestRequestTypeDef](./type_defs.md#stopcanaryrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [ArtifactConfigInputTypeDef](./type_defs.md#artifactconfiginputtypedef)
- [ArtifactConfigOutputTypeDef](./type_defs.md#artifactconfigoutputtypedef)
- [VisualReferenceInputTypeDef](./type_defs.md#visualreferenceinputtypedef)
- [VisualReferenceOutputTypeDef](./type_defs.md#visualreferenceoutputtypedef)
- [CanaryRunTypeDef](./type_defs.md#canaryruntypedef)
- [ListGroupResourcesResponseTypeDef](./type_defs.md#listgroupresourcesresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [CreateGroupResponseTypeDef](./type_defs.md#creategroupresponsetypedef)
- [GetGroupResponseTypeDef](./type_defs.md#getgroupresponsetypedef)
- [DescribeRuntimeVersionsResponseTypeDef](./type_defs.md#describeruntimeversionsresponsetypedef)
- [ListAssociatedGroupsResponseTypeDef](./type_defs.md#listassociatedgroupsresponsetypedef)
- [ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef)
- [CreateCanaryRequestRequestTypeDef](./type_defs.md#createcanaryrequestrequesttypedef)
- [UpdateCanaryRequestRequestTypeDef](./type_defs.md#updatecanaryrequestrequesttypedef)
- [CanaryTypeDef](./type_defs.md#canarytypedef)
- [CanaryLastRunTypeDef](./type_defs.md#canarylastruntypedef)
- [GetCanaryRunsResponseTypeDef](./type_defs.md#getcanaryrunsresponsetypedef)
- [CreateCanaryResponseTypeDef](./type_defs.md#createcanaryresponsetypedef)
- [DescribeCanariesResponseTypeDef](./type_defs.md#describecanariesresponsetypedef)
- [GetCanaryResponseTypeDef](./type_defs.md#getcanaryresponsetypedef)
- [DescribeCanariesLastRunResponseTypeDef](./type_defs.md#describecanarieslastrunresponsetypedef)

