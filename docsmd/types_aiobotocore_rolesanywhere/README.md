# IAMRolesAnywhere module

> [Index](../README.md) > IAMRolesAnywhere


!!! note ""

    Auto-generated documentation for [IAMRolesAnywhere](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
    type annotations stubs module [types-aiobotocore-rolesanywhere](https://pypi.org/project/types-aiobotocore-rolesanywhere/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `IAMRolesAnywhere` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[rolesanywhere]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[rolesanywhere]'


# standalone installation
python -m pip install types-aiobotocore-rolesanywhere
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-rolesanywhere
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IAMRolesAnywhereClient

Type annotations and code completion for  `#!python session.client("rolesanywhere")` as [IAMRolesAnywhereClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_rolesanywhere.client import IAMRolesAnywhereClient


session = Session()
async with session.client("rolesanywhere") as client:
    client: IAMRolesAnywhereClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("rolesanywhere").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_rolesanywhere.paginator import ListCrlsPaginator

def get_list_crls_paginator() -> ListCrlsPaginator:
    return client.get_paginator("list_crls"))
```

- [ListCrlsPaginator](./paginators.md#listcrlspaginator)
- [ListProfilesPaginator](./paginators.md#listprofilespaginator)
- [ListSubjectsPaginator](./paginators.md#listsubjectspaginator)
- [ListTrustAnchorsPaginator](./paginators.md#listtrustanchorspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_rolesanywhere.literals import ListCrlsPaginatorName

def get_value() -> ListCrlsPaginatorName:
    return "list_crls"
```

- [ListCrlsPaginatorName](./literals.md#listcrlspaginatorname)
- [ListProfilesPaginatorName](./literals.md#listprofilespaginatorname)
- [ListSubjectsPaginatorName](./literals.md#listsubjectspaginatorname)
- [ListTrustAnchorsPaginatorName](./literals.md#listtrustanchorspaginatorname)
- [TrustAnchorTypeType](./literals.md#trustanchortypetype)
- [IAMRolesAnywhereServiceName](./literals.md#iamrolesanywhereservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_rolesanywhere.type_defs import TagTypeDef

def get_value() -> TagTypeDef:
    return {
        "key": ...,
        "value": ...,
    }
```

- [TagTypeDef](./type_defs.md#tagtypedef)
- [CredentialSummaryTypeDef](./type_defs.md#credentialsummarytypedef)
- [CrlDetailTypeDef](./type_defs.md#crldetailtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [InstancePropertyTypeDef](./type_defs.md#instancepropertytypedef)
- [ProfileDetailTypeDef](./type_defs.md#profiledetailtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListRequestRequestTypeDef](./type_defs.md#listrequestrequesttypedef)
- [SubjectSummaryTypeDef](./type_defs.md#subjectsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ScalarCrlRequestRequestTypeDef](./type_defs.md#scalarcrlrequestrequesttypedef)
- [ScalarProfileRequestRequestTypeDef](./type_defs.md#scalarprofilerequestrequesttypedef)
- [ScalarSubjectRequestRequestTypeDef](./type_defs.md#scalarsubjectrequestrequesttypedef)
- [ScalarTrustAnchorRequestRequestTypeDef](./type_defs.md#scalartrustanchorrequestrequesttypedef)
- [SourceDataTypeDef](./type_defs.md#sourcedatatypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateCrlRequestRequestTypeDef](./type_defs.md#updatecrlrequestrequesttypedef)
- [UpdateProfileRequestRequestTypeDef](./type_defs.md#updateprofilerequestrequesttypedef)
- [CreateProfileRequestRequestTypeDef](./type_defs.md#createprofilerequestrequesttypedef)
- [ImportCrlRequestRequestTypeDef](./type_defs.md#importcrlrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CrlDetailResponseTypeDef](./type_defs.md#crldetailresponsetypedef)
- [ListCrlsResponseTypeDef](./type_defs.md#listcrlsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [SubjectDetailTypeDef](./type_defs.md#subjectdetailtypedef)
- [ListProfilesResponseTypeDef](./type_defs.md#listprofilesresponsetypedef)
- [ProfileDetailResponseTypeDef](./type_defs.md#profiledetailresponsetypedef)
- [ListRequestListCrlsPaginateTypeDef](./type_defs.md#listrequestlistcrlspaginatetypedef)
- [ListRequestListProfilesPaginateTypeDef](./type_defs.md#listrequestlistprofilespaginatetypedef)
- [ListRequestListSubjectsPaginateTypeDef](./type_defs.md#listrequestlistsubjectspaginatetypedef)
- [ListRequestListTrustAnchorsPaginateTypeDef](./type_defs.md#listrequestlisttrustanchorspaginatetypedef)
- [ListSubjectsResponseTypeDef](./type_defs.md#listsubjectsresponsetypedef)
- [SourceTypeDef](./type_defs.md#sourcetypedef)
- [SubjectDetailResponseTypeDef](./type_defs.md#subjectdetailresponsetypedef)
- [CreateTrustAnchorRequestRequestTypeDef](./type_defs.md#createtrustanchorrequestrequesttypedef)
- [TrustAnchorDetailTypeDef](./type_defs.md#trustanchordetailtypedef)
- [UpdateTrustAnchorRequestRequestTypeDef](./type_defs.md#updatetrustanchorrequestrequesttypedef)
- [ListTrustAnchorsResponseTypeDef](./type_defs.md#listtrustanchorsresponsetypedef)
- [TrustAnchorDetailResponseTypeDef](./type_defs.md#trustanchordetailresponsetypedef)

