# B2BI module

> [Index](../README.md) > B2BI


!!! note ""

    Auto-generated documentation for [B2BI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI)
    type annotations stubs module [types-aiobotocore-b2bi](https://pypi.org/project/types-aiobotocore-b2bi/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `B2BI` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[b2bi]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[b2bi]'


# standalone installation
python -m pip install types-aiobotocore-b2bi
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-b2bi
```

## Usage

Code samples can be found in [Examples](./usage.md).

## B2BIClient

Type annotations and code completion for  `#!python session.client("b2bi")` as [B2BIClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI.Client)

```python
# B2BIClient usage example

from aioboto3.session import Session

from types_aiobotocore_b2bi.client import B2BIClient


session = Session()
async with session.client("b2bi") as client:
    client: B2BIClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("b2bi").get_paginator("...")`.

```python
# ListCapabilitiesPaginator usage example

from types_aiobotocore_b2bi.paginator import ListCapabilitiesPaginator

def get_list_capabilities_paginator() -> ListCapabilitiesPaginator:
    return client.get_paginator("list_capabilities"))
```

- [ListCapabilitiesPaginator](./paginators.md#listcapabilitiespaginator)
- [ListPartnershipsPaginator](./paginators.md#listpartnershipspaginator)
- [ListProfilesPaginator](./paginators.md#listprofilespaginator)
- [ListTransformersPaginator](./paginators.md#listtransformerspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CapabilityTypeType usage example

from types_aiobotocore_b2bi.literals import CapabilityTypeType

def get_value() -> CapabilityTypeType:
    return "edi"
```

- [CapabilityTypeType](./literals.md#capabilitytypetype)
- [FileFormatType](./literals.md#fileformattype)
- [ListCapabilitiesPaginatorName](./literals.md#listcapabilitiespaginatorname)
- [ListPartnershipsPaginatorName](./literals.md#listpartnershipspaginatorname)
- [ListProfilesPaginatorName](./literals.md#listprofilespaginatorname)
- [ListTransformersPaginatorName](./literals.md#listtransformerspaginatorname)
- [LoggingType](./literals.md#loggingtype)
- [TransformerJobStatusType](./literals.md#transformerjobstatustype)
- [TransformerStatusType](./literals.md#transformerstatustype)
- [X12TransactionSetType](./literals.md#x12transactionsettype)
- [X12VersionType](./literals.md#x12versiontype)
- [B2BIServiceName](./literals.md#b2biservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CapabilitySummaryTypeDef](./type_defs.md#capabilitysummarytypedef)
- [S3LocationTypeDef](./type_defs.md#s3locationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteCapabilityRequestRequestTypeDef](./type_defs.md#deletecapabilityrequestrequesttypedef)
- [DeletePartnershipRequestRequestTypeDef](./type_defs.md#deletepartnershiprequestrequesttypedef)
- [DeleteProfileRequestRequestTypeDef](./type_defs.md#deleteprofilerequestrequesttypedef)
- [DeleteTransformerRequestRequestTypeDef](./type_defs.md#deletetransformerrequestrequesttypedef)
- [X12DetailsTypeDef](./type_defs.md#x12detailstypedef)
- [GetCapabilityRequestRequestTypeDef](./type_defs.md#getcapabilityrequestrequesttypedef)
- [GetPartnershipRequestRequestTypeDef](./type_defs.md#getpartnershiprequestrequesttypedef)
- [GetProfileRequestRequestTypeDef](./type_defs.md#getprofilerequestrequesttypedef)
- [GetTransformerJobRequestRequestTypeDef](./type_defs.md#gettransformerjobrequestrequesttypedef)
- [GetTransformerRequestRequestTypeDef](./type_defs.md#gettransformerrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListCapabilitiesRequestRequestTypeDef](./type_defs.md#listcapabilitiesrequestrequesttypedef)
- [ListPartnershipsRequestRequestTypeDef](./type_defs.md#listpartnershipsrequestrequesttypedef)
- [PartnershipSummaryTypeDef](./type_defs.md#partnershipsummarytypedef)
- [ListProfilesRequestRequestTypeDef](./type_defs.md#listprofilesrequestrequesttypedef)
- [ProfileSummaryTypeDef](./type_defs.md#profilesummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTransformersRequestRequestTypeDef](./type_defs.md#listtransformersrequestrequesttypedef)
- [TestMappingRequestRequestTypeDef](./type_defs.md#testmappingrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdatePartnershipRequestRequestTypeDef](./type_defs.md#updatepartnershiprequestrequesttypedef)
- [UpdateProfileRequestRequestTypeDef](./type_defs.md#updateprofilerequestrequesttypedef)
- [StartTransformerJobRequestRequestTypeDef](./type_defs.md#starttransformerjobrequestrequesttypedef)
- [CreatePartnershipRequestRequestTypeDef](./type_defs.md#createpartnershiprequestrequesttypedef)
- [CreateProfileRequestRequestTypeDef](./type_defs.md#createprofilerequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreatePartnershipResponseTypeDef](./type_defs.md#createpartnershipresponsetypedef)
- [CreateProfileResponseTypeDef](./type_defs.md#createprofileresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetPartnershipResponseTypeDef](./type_defs.md#getpartnershipresponsetypedef)
- [GetProfileResponseTypeDef](./type_defs.md#getprofileresponsetypedef)
- [GetTransformerJobResponseTypeDef](./type_defs.md#gettransformerjobresponsetypedef)
- [ListCapabilitiesResponseTypeDef](./type_defs.md#listcapabilitiesresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartTransformerJobResponseTypeDef](./type_defs.md#starttransformerjobresponsetypedef)
- [TestMappingResponseTypeDef](./type_defs.md#testmappingresponsetypedef)
- [TestParsingResponseTypeDef](./type_defs.md#testparsingresponsetypedef)
- [UpdatePartnershipResponseTypeDef](./type_defs.md#updatepartnershipresponsetypedef)
- [UpdateProfileResponseTypeDef](./type_defs.md#updateprofileresponsetypedef)
- [EdiTypeTypeDef](./type_defs.md#editypetypedef)
- [ListCapabilitiesRequestListCapabilitiesPaginateTypeDef](./type_defs.md#listcapabilitiesrequestlistcapabilitiespaginatetypedef)
- [ListPartnershipsRequestListPartnershipsPaginateTypeDef](./type_defs.md#listpartnershipsrequestlistpartnershipspaginatetypedef)
- [ListProfilesRequestListProfilesPaginateTypeDef](./type_defs.md#listprofilesrequestlistprofilespaginatetypedef)
- [ListTransformersRequestListTransformersPaginateTypeDef](./type_defs.md#listtransformersrequestlisttransformerspaginatetypedef)
- [ListPartnershipsResponseTypeDef](./type_defs.md#listpartnershipsresponsetypedef)
- [ListProfilesResponseTypeDef](./type_defs.md#listprofilesresponsetypedef)
- [CreateTransformerRequestRequestTypeDef](./type_defs.md#createtransformerrequestrequesttypedef)
- [CreateTransformerResponseTypeDef](./type_defs.md#createtransformerresponsetypedef)
- [EdiConfigurationTypeDef](./type_defs.md#ediconfigurationtypedef)
- [GetTransformerResponseTypeDef](./type_defs.md#gettransformerresponsetypedef)
- [TestParsingRequestRequestTypeDef](./type_defs.md#testparsingrequestrequesttypedef)
- [TransformerSummaryTypeDef](./type_defs.md#transformersummarytypedef)
- [UpdateTransformerRequestRequestTypeDef](./type_defs.md#updatetransformerrequestrequesttypedef)
- [UpdateTransformerResponseTypeDef](./type_defs.md#updatetransformerresponsetypedef)
- [CapabilityConfigurationTypeDef](./type_defs.md#capabilityconfigurationtypedef)
- [ListTransformersResponseTypeDef](./type_defs.md#listtransformersresponsetypedef)
- [CreateCapabilityRequestRequestTypeDef](./type_defs.md#createcapabilityrequestrequesttypedef)
- [CreateCapabilityResponseTypeDef](./type_defs.md#createcapabilityresponsetypedef)
- [GetCapabilityResponseTypeDef](./type_defs.md#getcapabilityresponsetypedef)
- [UpdateCapabilityRequestRequestTypeDef](./type_defs.md#updatecapabilityrequestrequesttypedef)
- [UpdateCapabilityResponseTypeDef](./type_defs.md#updatecapabilityresponsetypedef)

