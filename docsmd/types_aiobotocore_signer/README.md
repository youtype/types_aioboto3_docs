# Signer module

> [Index](../README.md) > Signer


!!! note ""

    Auto-generated documentation for [Signer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
    type annotations stubs module [types-aiobotocore-signer](https://pypi.org/project/types-aiobotocore-signer/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `Signer` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `Signer` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[signer]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[signer]'

# standalone installation
python -m pip install types-aiobotocore-signer
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-signer
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SignerClient

Type annotations and code completion for  `#!python session.client("signer")` as [SignerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#Signer.Client)

```python
# SignerClient usage example

from aioboto3.session import Session

from types_aiobotocore_signer.client import SignerClient


session = Session()
async with session.client("signer") as client:
    client: SignerClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("signer").get_paginator("...")`.

```python
# ListSigningJobsPaginator usage example

from types_aiobotocore_signer.paginator import ListSigningJobsPaginator

def get_list_signing_jobs_paginator() -> ListSigningJobsPaginator:
    return client.get_paginator("list_signing_jobs"))
```

- [ListSigningJobsPaginator](./paginators.md#listsigningjobspaginator)
- [ListSigningPlatformsPaginator](./paginators.md#listsigningplatformspaginator)
- [ListSigningProfilesPaginator](./paginators.md#listsigningprofilespaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.client("signer").get_waiter("...")`.

```python
# SuccessfulSigningJobWaiter usage example

from types_aiobotocore_signer.waiter import SuccessfulSigningJobWaiter

def get_successful_signing_job_waiter() -> SuccessfulSigningJobWaiter:
    return Session().client("signer").get_waiter("successful_signing_job")
```

- [SuccessfulSigningJobWaiter](./waiters.md#successfulsigningjobwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CategoryType usage example

from types_aiobotocore_signer.literals import CategoryType

def get_value() -> CategoryType:
    return "AWSIoT"
```

- [CategoryType](./literals.md#categorytype)
- [EncryptionAlgorithmType](./literals.md#encryptionalgorithmtype)
- [HashAlgorithmType](./literals.md#hashalgorithmtype)
- [ImageFormatType](./literals.md#imageformattype)
- [ListSigningJobsPaginatorName](./literals.md#listsigningjobspaginatorname)
- [ListSigningPlatformsPaginatorName](./literals.md#listsigningplatformspaginatorname)
- [ListSigningProfilesPaginatorName](./literals.md#listsigningprofilespaginatorname)
- [SigningProfileStatusType](./literals.md#signingprofilestatustype)
- [SigningStatusType](./literals.md#signingstatustype)
- [SuccessfulSigningJobWaiterName](./literals.md#successfulsigningjobwaitername)
- [ValidityTypeType](./literals.md#validitytypetype)
- [SignerServiceName](./literals.md#signerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AddProfilePermissionRequestRequestTypeDef](./type_defs.md#addprofilepermissionrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CancelSigningProfileRequestRequestTypeDef](./type_defs.md#cancelsigningprofilerequestrequesttypedef)
- [DescribeSigningJobRequestRequestTypeDef](./type_defs.md#describesigningjobrequestrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [SigningJobRevocationRecordTypeDef](./type_defs.md#signingjobrevocationrecordtypedef)
- [SigningMaterialTypeDef](./type_defs.md#signingmaterialtypedef)
- [S3DestinationTypeDef](./type_defs.md#s3destinationtypedef)
- [EncryptionAlgorithmOptionsTypeDef](./type_defs.md#encryptionalgorithmoptionstypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [GetSigningPlatformRequestRequestTypeDef](./type_defs.md#getsigningplatformrequestrequesttypedef)
- [SigningImageFormatTypeDef](./type_defs.md#signingimageformattypedef)
- [GetSigningProfileRequestRequestTypeDef](./type_defs.md#getsigningprofilerequestrequesttypedef)
- [SignatureValidityPeriodTypeDef](./type_defs.md#signaturevalidityperiodtypedef)
- [SigningProfileRevocationRecordTypeDef](./type_defs.md#signingprofilerevocationrecordtypedef)
- [HashAlgorithmOptionsTypeDef](./type_defs.md#hashalgorithmoptionstypedef)
- [ListProfilePermissionsRequestRequestTypeDef](./type_defs.md#listprofilepermissionsrequestrequesttypedef)
- [PermissionTypeDef](./type_defs.md#permissiontypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListSigningPlatformsRequestRequestTypeDef](./type_defs.md#listsigningplatformsrequestrequesttypedef)
- [ListSigningProfilesRequestRequestTypeDef](./type_defs.md#listsigningprofilesrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [RemoveProfilePermissionRequestRequestTypeDef](./type_defs.md#removeprofilepermissionrequestrequesttypedef)
- [RevokeSignatureRequestRequestTypeDef](./type_defs.md#revokesignaturerequestrequesttypedef)
- [S3SignedObjectTypeDef](./type_defs.md#s3signedobjecttypedef)
- [S3SourceTypeDef](./type_defs.md#s3sourcetypedef)
- [SigningConfigurationOverridesTypeDef](./type_defs.md#signingconfigurationoverridestypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [AddProfilePermissionResponseTypeDef](./type_defs.md#addprofilepermissionresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetRevocationStatusResponseTypeDef](./type_defs.md#getrevocationstatusresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PutSigningProfileResponseTypeDef](./type_defs.md#putsigningprofileresponsetypedef)
- [RemoveProfilePermissionResponseTypeDef](./type_defs.md#removeprofilepermissionresponsetypedef)
- [SignPayloadResponseTypeDef](./type_defs.md#signpayloadresponsetypedef)
- [StartSigningJobResponseTypeDef](./type_defs.md#startsigningjobresponsetypedef)
- [SignPayloadRequestRequestTypeDef](./type_defs.md#signpayloadrequestrequesttypedef)
- [DescribeSigningJobRequestWaitTypeDef](./type_defs.md#describesigningjobrequestwaittypedef)
- [DestinationTypeDef](./type_defs.md#destinationtypedef)
- [GetRevocationStatusRequestRequestTypeDef](./type_defs.md#getrevocationstatusrequestrequesttypedef)
- [ListSigningJobsRequestRequestTypeDef](./type_defs.md#listsigningjobsrequestrequesttypedef)
- [RevokeSigningProfileRequestRequestTypeDef](./type_defs.md#revokesigningprofilerequestrequesttypedef)
- [SigningProfileTypeDef](./type_defs.md#signingprofiletypedef)
- [SigningConfigurationTypeDef](./type_defs.md#signingconfigurationtypedef)
- [ListProfilePermissionsResponseTypeDef](./type_defs.md#listprofilepermissionsresponsetypedef)
- [ListSigningJobsRequestPaginateTypeDef](./type_defs.md#listsigningjobsrequestpaginatetypedef)
- [ListSigningPlatformsRequestPaginateTypeDef](./type_defs.md#listsigningplatformsrequestpaginatetypedef)
- [ListSigningProfilesRequestPaginateTypeDef](./type_defs.md#listsigningprofilesrequestpaginatetypedef)
- [SignedObjectTypeDef](./type_defs.md#signedobjecttypedef)
- [SourceTypeDef](./type_defs.md#sourcetypedef)
- [SigningPlatformOverridesTypeDef](./type_defs.md#signingplatformoverridestypedef)
- [ListSigningProfilesResponseTypeDef](./type_defs.md#listsigningprofilesresponsetypedef)
- [GetSigningPlatformResponseTypeDef](./type_defs.md#getsigningplatformresponsetypedef)
- [SigningPlatformTypeDef](./type_defs.md#signingplatformtypedef)
- [SigningJobTypeDef](./type_defs.md#signingjobtypedef)
- [StartSigningJobRequestRequestTypeDef](./type_defs.md#startsigningjobrequestrequesttypedef)
- [DescribeSigningJobResponseTypeDef](./type_defs.md#describesigningjobresponsetypedef)
- [GetSigningProfileResponseTypeDef](./type_defs.md#getsigningprofileresponsetypedef)
- [PutSigningProfileRequestRequestTypeDef](./type_defs.md#putsigningprofilerequestrequesttypedef)
- [ListSigningPlatformsResponseTypeDef](./type_defs.md#listsigningplatformsresponsetypedef)
- [ListSigningJobsResponseTypeDef](./type_defs.md#listsigningjobsresponsetypedef)
