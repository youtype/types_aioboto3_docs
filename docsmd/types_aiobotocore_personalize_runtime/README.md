# PersonalizeRuntime module

> [Index](../README.md) > PersonalizeRuntime


!!! note ""

    Auto-generated documentation for [PersonalizeRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#personalizeruntime)
    type annotations stubs module [types-aiobotocore-personalize-runtime](https://pypi.org/project/types-aiobotocore-personalize-runtime/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `PersonalizeRuntime` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `PersonalizeRuntime` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[personalize-runtime]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[personalize-runtime]'

# standalone installation
python -m pip install types-aiobotocore-personalize-runtime
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-personalize-runtime
```

## Usage

Code samples can be found in [Examples](./usage.md).

## PersonalizeRuntimeClient

Type annotations and code completion for  `#!python session.client("personalize-runtime")` as [PersonalizeRuntimeClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime.Client)

```python
# PersonalizeRuntimeClient usage example

from aioboto3.session import Session

from types_aiobotocore_personalize_runtime.client import PersonalizeRuntimeClient


session = Session()
async with session.client("personalize-runtime") as client:
    client: PersonalizeRuntimeClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# PersonalizeRuntimeServiceName usage example

from types_aiobotocore_personalize_runtime.literals import PersonalizeRuntimeServiceName

def get_value() -> PersonalizeRuntimeServiceName:
    return "personalize-runtime"
```

- [PersonalizeRuntimeServiceName](./literals.md#personalizeruntimeservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [GetActionRecommendationsRequestRequestTypeDef](./type_defs.md#getactionrecommendationsrequestrequesttypedef)
- [PredictedActionTypeDef](./type_defs.md#predictedactiontypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetPersonalizedRankingRequestRequestTypeDef](./type_defs.md#getpersonalizedrankingrequestrequesttypedef)
- [PredictedItemTypeDef](./type_defs.md#predicteditemtypedef)
- [PromotionTypeDef](./type_defs.md#promotiontypedef)
- [GetActionRecommendationsResponseTypeDef](./type_defs.md#getactionrecommendationsresponsetypedef)
- [GetPersonalizedRankingResponseTypeDef](./type_defs.md#getpersonalizedrankingresponsetypedef)
- [GetRecommendationsResponseTypeDef](./type_defs.md#getrecommendationsresponsetypedef)
- [GetRecommendationsRequestRequestTypeDef](./type_defs.md#getrecommendationsrequestrequesttypedef)
