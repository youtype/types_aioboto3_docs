# FinSpaceData module

> [Index](../README.md) > FinSpaceData


!!! note ""

    Auto-generated documentation for [FinSpaceData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
    type annotations stubs module [types-aiobotocore-finspace-data](https://pypi.org/project/types-aiobotocore-finspace-data/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `FinSpaceData` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[finspace-data]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[finspace-data]'


# standalone installation
python -m pip install types-aiobotocore-finspace-data
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-finspace-data
```

## Usage

Code samples can be found in [Examples](./usage.md).

## FinSpaceDataClient

Type annotations and code completion for  `#!python session.client("finspace-data")` as [FinSpaceDataClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_finspace_data.client import FinSpaceDataClient


session = Session()
async with session.client("finspace-data") as client:
    client: FinSpaceDataClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("finspace-data").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_finspace_data.paginator import ListChangesetsPaginator

def get_list_changesets_paginator() -> ListChangesetsPaginator:
    return client.get_paginator("list_changesets"))
```

- [ListChangesetsPaginator](./paginators.md#listchangesetspaginator)
- [ListDataViewsPaginator](./paginators.md#listdataviewspaginator)
- [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
- [ListPermissionGroupsPaginator](./paginators.md#listpermissiongroupspaginator)
- [ListUsersPaginator](./paginators.md#listuserspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_finspace_data.literals import ApiAccessType

def get_value() -> ApiAccessType:
    return "DISABLED"
```

- [ApiAccessType](./literals.md#apiaccesstype)
- [ApplicationPermissionType](./literals.md#applicationpermissiontype)
- [ChangeTypeType](./literals.md#changetypetype)
- [ColumnDataTypeType](./literals.md#columndatatypetype)
- [DataViewStatusType](./literals.md#dataviewstatustype)
- [DatasetKindType](./literals.md#datasetkindtype)
- [DatasetStatusType](./literals.md#datasetstatustype)
- [ErrorCategoryType](./literals.md#errorcategorytype)
- [ExportFileFormatType](./literals.md#exportfileformattype)
- [IngestionStatusType](./literals.md#ingestionstatustype)
- [ListChangesetsPaginatorName](./literals.md#listchangesetspaginatorname)
- [ListDataViewsPaginatorName](./literals.md#listdataviewspaginatorname)
- [ListDatasetsPaginatorName](./literals.md#listdatasetspaginatorname)
- [ListPermissionGroupsPaginatorName](./literals.md#listpermissiongroupspaginatorname)
- [ListUsersPaginatorName](./literals.md#listuserspaginatorname)
- [UserStatusType](./literals.md#userstatustype)
- [UserTypeType](./literals.md#usertypetype)
- [locationTypeType](./literals.md#locationtypetype)
- [FinSpaceDataServiceName](./literals.md#finspacedataservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_finspace_data.type_defs import ChangesetErrorInfoTypeDef

def get_value() -> ChangesetErrorInfoTypeDef:
    return {
        "errorMessage": ...,
    }
```

- [ChangesetErrorInfoTypeDef](./type_defs.md#changeseterrorinfotypedef)
- [ColumnDefinitionTypeDef](./type_defs.md#columndefinitiontypedef)
- [CreateChangesetRequestRequestTypeDef](./type_defs.md#createchangesetrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DataViewDestinationTypeParamsTypeDef](./type_defs.md#dataviewdestinationtypeparamstypedef)
- [DatasetOwnerInfoTypeDef](./type_defs.md#datasetownerinfotypedef)
- [CreatePermissionGroupRequestRequestTypeDef](./type_defs.md#createpermissiongrouprequestrequesttypedef)
- [CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef)
- [CredentialsTypeDef](./type_defs.md#credentialstypedef)
- [DataViewErrorInfoTypeDef](./type_defs.md#dataviewerrorinfotypedef)
- [DeleteDatasetRequestRequestTypeDef](./type_defs.md#deletedatasetrequestrequesttypedef)
- [DeletePermissionGroupRequestRequestTypeDef](./type_defs.md#deletepermissiongrouprequestrequesttypedef)
- [DisableUserRequestRequestTypeDef](./type_defs.md#disableuserrequestrequesttypedef)
- [EnableUserRequestRequestTypeDef](./type_defs.md#enableuserrequestrequesttypedef)
- [GetChangesetRequestRequestTypeDef](./type_defs.md#getchangesetrequestrequesttypedef)
- [GetDataViewRequestRequestTypeDef](./type_defs.md#getdataviewrequestrequesttypedef)
- [GetDatasetRequestRequestTypeDef](./type_defs.md#getdatasetrequestrequesttypedef)
- [GetProgrammaticAccessCredentialsRequestRequestTypeDef](./type_defs.md#getprogrammaticaccesscredentialsrequestrequesttypedef)
- [GetUserRequestRequestTypeDef](./type_defs.md#getuserrequestrequesttypedef)
- [GetWorkingLocationRequestRequestTypeDef](./type_defs.md#getworkinglocationrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListChangesetsRequestRequestTypeDef](./type_defs.md#listchangesetsrequestrequesttypedef)
- [ListDataViewsRequestRequestTypeDef](./type_defs.md#listdataviewsrequestrequesttypedef)
- [ListDatasetsRequestRequestTypeDef](./type_defs.md#listdatasetsrequestrequesttypedef)
- [ListPermissionGroupsRequestRequestTypeDef](./type_defs.md#listpermissiongroupsrequestrequesttypedef)
- [PermissionGroupTypeDef](./type_defs.md#permissiongrouptypedef)
- [ListUsersRequestRequestTypeDef](./type_defs.md#listusersrequestrequesttypedef)
- [UserTypeDef](./type_defs.md#usertypedef)
- [ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef)
- [ResetUserPasswordRequestRequestTypeDef](./type_defs.md#resetuserpasswordrequestrequesttypedef)
- [UpdateChangesetRequestRequestTypeDef](./type_defs.md#updatechangesetrequestrequesttypedef)
- [UpdatePermissionGroupRequestRequestTypeDef](./type_defs.md#updatepermissiongrouprequestrequesttypedef)
- [UpdateUserRequestRequestTypeDef](./type_defs.md#updateuserrequestrequesttypedef)
- [ChangesetSummaryTypeDef](./type_defs.md#changesetsummarytypedef)
- [SchemaDefinitionTypeDef](./type_defs.md#schemadefinitiontypedef)
- [CreateChangesetResponseTypeDef](./type_defs.md#createchangesetresponsetypedef)
- [CreateDataViewResponseTypeDef](./type_defs.md#createdataviewresponsetypedef)
- [CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef)
- [CreatePermissionGroupResponseTypeDef](./type_defs.md#createpermissiongroupresponsetypedef)
- [CreateUserResponseTypeDef](./type_defs.md#createuserresponsetypedef)
- [DeleteDatasetResponseTypeDef](./type_defs.md#deletedatasetresponsetypedef)
- [DeletePermissionGroupResponseTypeDef](./type_defs.md#deletepermissiongroupresponsetypedef)
- [DisableUserResponseTypeDef](./type_defs.md#disableuserresponsetypedef)
- [EnableUserResponseTypeDef](./type_defs.md#enableuserresponsetypedef)
- [GetChangesetResponseTypeDef](./type_defs.md#getchangesetresponsetypedef)
- [GetUserResponseTypeDef](./type_defs.md#getuserresponsetypedef)
- [GetWorkingLocationResponseTypeDef](./type_defs.md#getworkinglocationresponsetypedef)
- [ResetUserPasswordResponseTypeDef](./type_defs.md#resetuserpasswordresponsetypedef)
- [UpdateChangesetResponseTypeDef](./type_defs.md#updatechangesetresponsetypedef)
- [UpdateDatasetResponseTypeDef](./type_defs.md#updatedatasetresponsetypedef)
- [UpdatePermissionGroupResponseTypeDef](./type_defs.md#updatepermissiongroupresponsetypedef)
- [UpdateUserResponseTypeDef](./type_defs.md#updateuserresponsetypedef)
- [CreateDataViewRequestRequestTypeDef](./type_defs.md#createdataviewrequestrequesttypedef)
- [GetProgrammaticAccessCredentialsResponseTypeDef](./type_defs.md#getprogrammaticaccesscredentialsresponsetypedef)
- [DataViewSummaryTypeDef](./type_defs.md#dataviewsummarytypedef)
- [GetDataViewResponseTypeDef](./type_defs.md#getdataviewresponsetypedef)
- [ListChangesetsRequestListChangesetsPaginateTypeDef](./type_defs.md#listchangesetsrequestlistchangesetspaginatetypedef)
- [ListDataViewsRequestListDataViewsPaginateTypeDef](./type_defs.md#listdataviewsrequestlistdataviewspaginatetypedef)
- [ListDatasetsRequestListDatasetsPaginateTypeDef](./type_defs.md#listdatasetsrequestlistdatasetspaginatetypedef)
- [ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef](./type_defs.md#listpermissiongroupsrequestlistpermissiongroupspaginatetypedef)
- [ListUsersRequestListUsersPaginateTypeDef](./type_defs.md#listusersrequestlistuserspaginatetypedef)
- [ListPermissionGroupsResponseTypeDef](./type_defs.md#listpermissiongroupsresponsetypedef)
- [ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef)
- [PermissionGroupParamsTypeDef](./type_defs.md#permissiongroupparamstypedef)
- [ListChangesetsResponseTypeDef](./type_defs.md#listchangesetsresponsetypedef)
- [SchemaUnionTypeDef](./type_defs.md#schemauniontypedef)
- [ListDataViewsResponseTypeDef](./type_defs.md#listdataviewsresponsetypedef)
- [CreateDatasetRequestRequestTypeDef](./type_defs.md#createdatasetrequestrequesttypedef)
- [DatasetTypeDef](./type_defs.md#datasettypedef)
- [GetDatasetResponseTypeDef](./type_defs.md#getdatasetresponsetypedef)
- [UpdateDatasetRequestRequestTypeDef](./type_defs.md#updatedatasetrequestrequesttypedef)
- [ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef)

