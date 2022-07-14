# SSO module

> [Index](../README.md) > SSO


!!! note ""

    Auto-generated documentation for [SSO](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
    type annotations stubs module [types-aiobotocore-sso](https://pypi.org/project/types-aiobotocore-sso/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `SSO`.

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

```python title="Usage example"
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

```python title="Usage example"
from types_aiobotocore_sso.paginator import ListAccountRolesPaginator

def get_list_account_roles_paginator() -> ListAccountRolesPaginator:
    return client.get_paginator("list_account_roles"))
```

- [ListAccountRolesPaginator](./paginators.md#listaccountrolespaginator)
- [ListAccountsPaginator](./paginators.md#listaccountspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
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




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_sso.type_defs import AccountInfoTypeDef

def get_value() -> AccountInfoTypeDef:
    return {
        "accountId": ...,
    }
```

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
- [ListAccountRolesRequestListAccountRolesPaginateTypeDef](./type_defs.md#listaccountrolesrequestlistaccountrolespaginatetypedef)
- [ListAccountsRequestListAccountsPaginateTypeDef](./type_defs.md#listaccountsrequestlistaccountspaginatetypedef)
- [ListAccountRolesResponseTypeDef](./type_defs.md#listaccountrolesresponsetypedef)

