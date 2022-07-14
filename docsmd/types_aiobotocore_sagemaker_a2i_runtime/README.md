# AugmentedAIRuntime module

> [Index](../README.md) > AugmentedAIRuntime


!!! note ""

    Auto-generated documentation for [AugmentedAIRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
    type annotations stubs module [types-aiobotocore-sagemaker-a2i-runtime](https://pypi.org/project/types-aiobotocore-sagemaker-a2i-runtime/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `AugmentedAIRuntime`.

### From PyPI with pip

Install `types-aioboto3` for `AugmentedAIRuntime` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[sagemaker-a2i-runtime]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[sagemaker-a2i-runtime]'


# standalone installation
python -m pip install types-aiobotocore-sagemaker-a2i-runtime
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-sagemaker-a2i-runtime
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AugmentedAIRuntimeClient

Type annotations and code completion for  `#!python session.client("sagemaker-a2i-runtime")` as [AugmentedAIRuntimeClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sagemaker_a2i_runtime.client import AugmentedAIRuntimeClient


session = Session()
async with session.client("sagemaker-a2i-runtime") as client:
    client: AugmentedAIRuntimeClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("sagemaker-a2i-runtime").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_sagemaker_a2i_runtime.paginator import ListHumanLoopsPaginator

def get_list_human_loops_paginator() -> ListHumanLoopsPaginator:
    return client.get_paginator("list_human_loops"))
```

- [ListHumanLoopsPaginator](./paginators.md#listhumanloopspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_sagemaker_a2i_runtime.literals import ContentClassifierType

def get_value() -> ContentClassifierType:
    return "FreeOfAdultContent"
```

- [ContentClassifierType](./literals.md#contentclassifiertype)
- [HumanLoopStatusType](./literals.md#humanloopstatustype)
- [ListHumanLoopsPaginatorName](./literals.md#listhumanloopspaginatorname)
- [SortOrderType](./literals.md#sortordertype)
- [AugmentedAIRuntimeServiceName](./literals.md#augmentedairuntimeservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_sagemaker_a2i_runtime.type_defs import DeleteHumanLoopRequestRequestTypeDef

def get_value() -> DeleteHumanLoopRequestRequestTypeDef:
    return {
        "HumanLoopName": ...,
    }
```

- [DeleteHumanLoopRequestRequestTypeDef](./type_defs.md#deletehumanlooprequestrequesttypedef)
- [DescribeHumanLoopRequestRequestTypeDef](./type_defs.md#describehumanlooprequestrequesttypedef)
- [HumanLoopOutputTypeDef](./type_defs.md#humanloopoutputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [HumanLoopDataAttributesTypeDef](./type_defs.md#humanloopdataattributestypedef)
- [HumanLoopInputTypeDef](./type_defs.md#humanloopinputtypedef)
- [HumanLoopSummaryTypeDef](./type_defs.md#humanloopsummarytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListHumanLoopsRequestRequestTypeDef](./type_defs.md#listhumanloopsrequestrequesttypedef)
- [StopHumanLoopRequestRequestTypeDef](./type_defs.md#stophumanlooprequestrequesttypedef)
- [DescribeHumanLoopResponseTypeDef](./type_defs.md#describehumanloopresponsetypedef)
- [StartHumanLoopResponseTypeDef](./type_defs.md#starthumanloopresponsetypedef)
- [StartHumanLoopRequestRequestTypeDef](./type_defs.md#starthumanlooprequestrequesttypedef)
- [ListHumanLoopsResponseTypeDef](./type_defs.md#listhumanloopsresponsetypedef)
- [ListHumanLoopsRequestListHumanLoopsPaginateTypeDef](./type_defs.md#listhumanloopsrequestlisthumanloopspaginatetypedef)

