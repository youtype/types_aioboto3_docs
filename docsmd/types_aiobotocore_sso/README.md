# SSO module

> [Index](../README.md) > SSO


!!! note ""

    Auto-generated documentation for [SSO](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#sso)
    type annotations stubs module [types-aiobotocore-sso](https://pypi.org/project/types-aiobotocore-sso/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `SSO` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `SSO` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[sso]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[sso]'

# standalone installation
python -m pip install types-aiobotocore-sso
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-sso
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SSOClient

Type annotations and code completion for  `#!python session.client("sso")` as [SSOClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client)

```python
# SSOClient usage example

from aioboto3.session import Session

from types_aiobotocore_sso.client import SSOClient


session = Session()
async with session.client("sso") as client:
    client: SSOClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("sso").get_paginator("...")`.

```python
# ListAccountRolesPaginator usage example

from types_aiobotocore_sso.paginator import ListAccountRolesPaginator

def get_list_account_roles_paginator() -> ListAccountRolesPaginator:
    return client.get_paginator("list_account_roles"))
```

- [ListAccountRolesPaginator](./paginators.md#listaccountrolespaginator)
- [ListAccountsPaginator](./paginators.md#listaccountspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ListAccountRolesPaginatorName usage example

from types_aiobotocore_sso.literals import ListAccountRolesPaginatorName

def get_value() -> ListAccountRolesPaginatorName:
    return "list_account_roles"
```

- [ListAccountRolesPaginatorName](./literals.md#listaccountrolespaginatorname)
- [ListAccountsPaginatorName](./literals.md#listaccountspaginatorname)
- [SSOServiceName](./literals.md#ssoservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccountInfoTypeDef](./type_defs.md#accountinfotypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetRoleCredentialsRequestRequestTypeDef](./type_defs.md#getrolecredentialsrequestrequesttypedef)
- [RoleCredentialsTypeDef](./type_defs.md#rolecredentialstypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAccountRolesRequestRequestTypeDef](./type_defs.md#listaccountrolesrequestrequesttypedef)
- [RoleInfoTypeDef](./type_defs.md#roleinfotypedef)
- [ListAccountsRequestRequestTypeDef](./type_defs.md#listaccountsrequestrequesttypedef)
- [LogoutRequestRequestTypeDef](./type_defs.md#logoutrequestrequesttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListAccountsResponseTypeDef](./type_defs.md#listaccountsresponsetypedef)
- [GetRoleCredentialsResponseTypeDef](./type_defs.md#getrolecredentialsresponsetypedef)
- [ListAccountRolesRequestPaginateTypeDef](./type_defs.md#listaccountrolesrequestpaginatetypedef)
- [ListAccountsRequestPaginateTypeDef](./type_defs.md#listaccountsrequestpaginatetypedef)
- [ListAccountRolesResponseTypeDef](./type_defs.md#listaccountrolesresponsetypedef)
