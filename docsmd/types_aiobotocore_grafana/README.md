# ManagedGrafana module

> [Index](../README.md) > ManagedGrafana


!!! note ""

    Auto-generated documentation for [ManagedGrafana](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#managedgrafana)
    type annotations stubs module [types-aiobotocore-grafana](https://pypi.org/project/types-aiobotocore-grafana/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `ManagedGrafana` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `ManagedGrafana` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[grafana]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[grafana]'

# standalone installation
python -m pip install types-aiobotocore-grafana
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-grafana
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ManagedGrafanaClient

Type annotations and code completion for  `#!python session.client("grafana")` as [ManagedGrafanaClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client)

```python
# ManagedGrafanaClient usage example

from aioboto3.session import Session

from types_aiobotocore_grafana.client import ManagedGrafanaClient


session = Session()
async with session.client("grafana") as client:
    client: ManagedGrafanaClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("grafana").get_paginator("...")`.

```python
# ListPermissionsPaginator usage example

from types_aiobotocore_grafana.paginator import ListPermissionsPaginator

def get_list_permissions_paginator() -> ListPermissionsPaginator:
    return client.get_paginator("list_permissions"))
```

- [ListPermissionsPaginator](./paginators.md#listpermissionspaginator)
- [ListVersionsPaginator](./paginators.md#listversionspaginator)
- [ListWorkspaceServiceAccountTokensPaginator](./paginators.md#listworkspaceserviceaccounttokenspaginator)
- [ListWorkspaceServiceAccountsPaginator](./paginators.md#listworkspaceserviceaccountspaginator)
- [ListWorkspacesPaginator](./paginators.md#listworkspacespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccountAccessTypeType usage example

from types_aiobotocore_grafana.literals import AccountAccessTypeType

def get_value() -> AccountAccessTypeType:
    return "CURRENT_ACCOUNT"
```

- [AccountAccessTypeType](./literals.md#accountaccesstypetype)
- [AuthenticationProviderTypesType](./literals.md#authenticationprovidertypestype)
- [DataSourceTypeType](./literals.md#datasourcetypetype)
- [LicenseTypeType](./literals.md#licensetypetype)
- [ListPermissionsPaginatorName](./literals.md#listpermissionspaginatorname)
- [ListVersionsPaginatorName](./literals.md#listversionspaginatorname)
- [ListWorkspaceServiceAccountTokensPaginatorName](./literals.md#listworkspaceserviceaccounttokenspaginatorname)
- [ListWorkspaceServiceAccountsPaginatorName](./literals.md#listworkspaceserviceaccountspaginatorname)
- [ListWorkspacesPaginatorName](./literals.md#listworkspacespaginatorname)
- [NotificationDestinationTypeType](./literals.md#notificationdestinationtypetype)
- [PermissionTypeType](./literals.md#permissiontypetype)
- [RoleType](./literals.md#roletype)
- [SamlConfigurationStatusType](./literals.md#samlconfigurationstatustype)
- [UpdateActionType](./literals.md#updateactiontype)
- [UserTypeType](./literals.md#usertypetype)
- [WorkspaceStatusType](./literals.md#workspacestatustype)
- [ManagedGrafanaServiceName](./literals.md#managedgrafanaservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AssertionAttributesTypeDef](./type_defs.md#assertionattributestypedef)
- [AssociateLicenseRequestRequestTypeDef](./type_defs.md#associatelicenserequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AwsSsoAuthenticationTypeDef](./type_defs.md#awsssoauthenticationtypedef)
- [AuthenticationSummaryTypeDef](./type_defs.md#authenticationsummarytypedef)
- [CreateWorkspaceApiKeyRequestRequestTypeDef](./type_defs.md#createworkspaceapikeyrequestrequesttypedef)
- [NetworkAccessConfigurationTypeDef](./type_defs.md#networkaccessconfigurationtypedef)
- [VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef)
- [CreateWorkspaceServiceAccountRequestRequestTypeDef](./type_defs.md#createworkspaceserviceaccountrequestrequesttypedef)
- [CreateWorkspaceServiceAccountTokenRequestRequestTypeDef](./type_defs.md#createworkspaceserviceaccounttokenrequestrequesttypedef)
- [ServiceAccountTokenSummaryWithKeyTypeDef](./type_defs.md#serviceaccounttokensummarywithkeytypedef)
- [DeleteWorkspaceApiKeyRequestRequestTypeDef](./type_defs.md#deleteworkspaceapikeyrequestrequesttypedef)
- [DeleteWorkspaceRequestRequestTypeDef](./type_defs.md#deleteworkspacerequestrequesttypedef)
- [DeleteWorkspaceServiceAccountRequestRequestTypeDef](./type_defs.md#deleteworkspaceserviceaccountrequestrequesttypedef)
- [DeleteWorkspaceServiceAccountTokenRequestRequestTypeDef](./type_defs.md#deleteworkspaceserviceaccounttokenrequestrequesttypedef)
- [DescribeWorkspaceAuthenticationRequestRequestTypeDef](./type_defs.md#describeworkspaceauthenticationrequestrequesttypedef)
- [DescribeWorkspaceConfigurationRequestRequestTypeDef](./type_defs.md#describeworkspaceconfigurationrequestrequesttypedef)
- [DescribeWorkspaceRequestRequestTypeDef](./type_defs.md#describeworkspacerequestrequesttypedef)
- [DisassociateLicenseRequestRequestTypeDef](./type_defs.md#disassociatelicenserequestrequesttypedef)
- [IdpMetadataTypeDef](./type_defs.md#idpmetadatatypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListPermissionsRequestRequestTypeDef](./type_defs.md#listpermissionsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListVersionsRequestRequestTypeDef](./type_defs.md#listversionsrequestrequesttypedef)
- [ListWorkspaceServiceAccountTokensRequestRequestTypeDef](./type_defs.md#listworkspaceserviceaccounttokensrequestrequesttypedef)
- [ServiceAccountTokenSummaryTypeDef](./type_defs.md#serviceaccounttokensummarytypedef)
- [ListWorkspaceServiceAccountsRequestRequestTypeDef](./type_defs.md#listworkspaceserviceaccountsrequestrequesttypedef)
- [ServiceAccountSummaryTypeDef](./type_defs.md#serviceaccountsummarytypedef)
- [ListWorkspacesRequestRequestTypeDef](./type_defs.md#listworkspacesrequestrequesttypedef)
- [NetworkAccessConfigurationOutputTypeDef](./type_defs.md#networkaccessconfigurationoutputtypedef)
- [UserTypeDef](./type_defs.md#usertypedef)
- [RoleValuesOutputTypeDef](./type_defs.md#rolevaluesoutputtypedef)
- [RoleValuesTypeDef](./type_defs.md#rolevaluestypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateWorkspaceConfigurationRequestRequestTypeDef](./type_defs.md#updateworkspaceconfigurationrequestrequesttypedef)
- [VpcConfigurationOutputTypeDef](./type_defs.md#vpcconfigurationoutputtypedef)
- [CreateWorkspaceApiKeyResponseTypeDef](./type_defs.md#createworkspaceapikeyresponsetypedef)
- [CreateWorkspaceServiceAccountResponseTypeDef](./type_defs.md#createworkspaceserviceaccountresponsetypedef)
- [DeleteWorkspaceApiKeyResponseTypeDef](./type_defs.md#deleteworkspaceapikeyresponsetypedef)
- [DeleteWorkspaceServiceAccountResponseTypeDef](./type_defs.md#deleteworkspaceserviceaccountresponsetypedef)
- [DeleteWorkspaceServiceAccountTokenResponseTypeDef](./type_defs.md#deleteworkspaceserviceaccounttokenresponsetypedef)
- [DescribeWorkspaceConfigurationResponseTypeDef](./type_defs.md#describeworkspaceconfigurationresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ListVersionsResponseTypeDef](./type_defs.md#listversionsresponsetypedef)
- [WorkspaceSummaryTypeDef](./type_defs.md#workspacesummarytypedef)
- [CreateWorkspaceRequestRequestTypeDef](./type_defs.md#createworkspacerequestrequesttypedef)
- [UpdateWorkspaceRequestRequestTypeDef](./type_defs.md#updateworkspacerequestrequesttypedef)
- [CreateWorkspaceServiceAccountTokenResponseTypeDef](./type_defs.md#createworkspaceserviceaccounttokenresponsetypedef)
- [ListPermissionsRequestPaginateTypeDef](./type_defs.md#listpermissionsrequestpaginatetypedef)
- [ListVersionsRequestPaginateTypeDef](./type_defs.md#listversionsrequestpaginatetypedef)
- [ListWorkspaceServiceAccountTokensRequestPaginateTypeDef](./type_defs.md#listworkspaceserviceaccounttokensrequestpaginatetypedef)
- [ListWorkspaceServiceAccountsRequestPaginateTypeDef](./type_defs.md#listworkspaceserviceaccountsrequestpaginatetypedef)
- [ListWorkspacesRequestPaginateTypeDef](./type_defs.md#listworkspacesrequestpaginatetypedef)
- [ListWorkspaceServiceAccountTokensResponseTypeDef](./type_defs.md#listworkspaceserviceaccounttokensresponsetypedef)
- [ListWorkspaceServiceAccountsResponseTypeDef](./type_defs.md#listworkspaceserviceaccountsresponsetypedef)
- [PermissionEntryTypeDef](./type_defs.md#permissionentrytypedef)
- [UpdateInstructionOutputTypeDef](./type_defs.md#updateinstructionoutputtypedef)
- [UpdateInstructionTypeDef](./type_defs.md#updateinstructiontypedef)
- [SamlConfigurationOutputTypeDef](./type_defs.md#samlconfigurationoutputtypedef)
- [RoleValuesUnionTypeDef](./type_defs.md#rolevaluesuniontypedef)
- [WorkspaceDescriptionTypeDef](./type_defs.md#workspacedescriptiontypedef)
- [ListWorkspacesResponseTypeDef](./type_defs.md#listworkspacesresponsetypedef)
- [ListPermissionsResponseTypeDef](./type_defs.md#listpermissionsresponsetypedef)
- [UpdateErrorTypeDef](./type_defs.md#updateerrortypedef)
- [UpdateInstructionUnionTypeDef](./type_defs.md#updateinstructionuniontypedef)
- [SamlAuthenticationTypeDef](./type_defs.md#samlauthenticationtypedef)
- [SamlConfigurationTypeDef](./type_defs.md#samlconfigurationtypedef)
- [AssociateLicenseResponseTypeDef](./type_defs.md#associatelicenseresponsetypedef)
- [CreateWorkspaceResponseTypeDef](./type_defs.md#createworkspaceresponsetypedef)
- [DeleteWorkspaceResponseTypeDef](./type_defs.md#deleteworkspaceresponsetypedef)
- [DescribeWorkspaceResponseTypeDef](./type_defs.md#describeworkspaceresponsetypedef)
- [DisassociateLicenseResponseTypeDef](./type_defs.md#disassociatelicenseresponsetypedef)
- [UpdateWorkspaceResponseTypeDef](./type_defs.md#updateworkspaceresponsetypedef)
- [UpdatePermissionsResponseTypeDef](./type_defs.md#updatepermissionsresponsetypedef)
- [UpdatePermissionsRequestRequestTypeDef](./type_defs.md#updatepermissionsrequestrequesttypedef)
- [AuthenticationDescriptionTypeDef](./type_defs.md#authenticationdescriptiontypedef)
- [UpdateWorkspaceAuthenticationRequestRequestTypeDef](./type_defs.md#updateworkspaceauthenticationrequestrequesttypedef)
- [DescribeWorkspaceAuthenticationResponseTypeDef](./type_defs.md#describeworkspaceauthenticationresponsetypedef)
- [UpdateWorkspaceAuthenticationResponseTypeDef](./type_defs.md#updateworkspaceauthenticationresponsetypedef)
