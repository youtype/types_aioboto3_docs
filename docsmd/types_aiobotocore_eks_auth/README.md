# EKSAuth module

> [Index](../README.md) > EKSAuth


!!! note ""

    Auto-generated documentation for [EKSAuth](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks-auth.html#eksauth)
    type annotations stubs module [types-aiobotocore-eks-auth](https://pypi.org/project/types-aiobotocore-eks-auth/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `EKSAuth` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `EKSAuth` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[eks-auth]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[eks-auth]'

# standalone installation
python -m pip install types-aiobotocore-eks-auth
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-eks-auth
```

## Usage

Code samples can be found in [Examples](./usage.md).

## EKSAuthClient

Type annotations and code completion for  `#!python session.client("eks-auth")` as [EKSAuthClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks-auth.html#EKSAuth.Client)

```python
# EKSAuthClient usage example

from aioboto3.session import Session

from types_aiobotocore_eks_auth.client import EKSAuthClient


session = Session()
async with session.client("eks-auth") as client:
    client: EKSAuthClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# EKSAuthServiceName usage example

from types_aiobotocore_eks_auth.literals import EKSAuthServiceName

def get_value() -> EKSAuthServiceName:
    return "eks-auth"
```

- [EKSAuthServiceName](./literals.md#eksauthservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AssumeRoleForPodIdentityRequestRequestTypeDef](./type_defs.md#assumeroleforpodidentityrequestrequesttypedef)
- [AssumedRoleUserTypeDef](./type_defs.md#assumedroleusertypedef)
- [CredentialsTypeDef](./type_defs.md#credentialstypedef)
- [PodIdentityAssociationTypeDef](./type_defs.md#podidentityassociationtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [SubjectTypeDef](./type_defs.md#subjecttypedef)
- [AssumeRoleForPodIdentityResponseTypeDef](./type_defs.md#assumeroleforpodidentityresponsetypedef)
