# ACM module

> [Index](../README.md) > ACM


!!! note ""

    Auto-generated documentation for [ACM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#acm)
    type annotations stubs module [types-aiobotocore-acm](https://pypi.org/project/types-aiobotocore-acm/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `ACM` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `ACM` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[acm]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[acm]'

# standalone installation
python -m pip install types-aiobotocore-acm
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-acm
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ACMClient

Type annotations and code completion for  `#!python session.client("acm")` as [ACMClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

```python
# ACMClient usage example

from aioboto3.session import Session

from types_aiobotocore_acm.client import ACMClient


session = Session()
async with session.client("acm") as client:
    client: ACMClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("acm").get_paginator("...")`.

```python
# ListCertificatesPaginator usage example

from types_aiobotocore_acm.paginator import ListCertificatesPaginator

def get_list_certificates_paginator() -> ListCertificatesPaginator:
    return client.get_paginator("list_certificates"))
```

- [ListCertificatesPaginator](./paginators.md#listcertificatespaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.client("acm").get_waiter("...")`.

```python
# CertificateValidatedWaiter usage example

from types_aiobotocore_acm.waiter import CertificateValidatedWaiter

def get_certificate_validated_waiter() -> CertificateValidatedWaiter:
    return Session().client("acm").get_waiter("certificate_validated")
```

- [CertificateValidatedWaiter](./waiters.md#certificatevalidatedwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CertificateStatusType usage example

from types_aiobotocore_acm.literals import CertificateStatusType

def get_value() -> CertificateStatusType:
    return "EXPIRED"
```

- [CertificateStatusType](./literals.md#certificatestatustype)
- [CertificateTransparencyLoggingPreferenceType](./literals.md#certificatetransparencyloggingpreferencetype)
- [CertificateTypeType](./literals.md#certificatetypetype)
- [CertificateValidatedWaiterName](./literals.md#certificatevalidatedwaitername)
- [DomainStatusType](./literals.md#domainstatustype)
- [ExtendedKeyUsageNameType](./literals.md#extendedkeyusagenametype)
- [FailureReasonType](./literals.md#failurereasontype)
- [KeyAlgorithmType](./literals.md#keyalgorithmtype)
- [KeyUsageNameType](./literals.md#keyusagenametype)
- [ListCertificatesPaginatorName](./literals.md#listcertificatespaginatorname)
- [RecordTypeType](./literals.md#recordtypetype)
- [RenewalEligibilityType](./literals.md#renewaleligibilitytype)
- [RenewalStatusType](./literals.md#renewalstatustype)
- [RevocationReasonType](./literals.md#revocationreasontype)
- [SortByType](./literals.md#sortbytype)
- [SortOrderType](./literals.md#sortordertype)
- [ValidationMethodType](./literals.md#validationmethodtype)
- [ACMServiceName](./literals.md#acmservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [TagTypeDef](./type_defs.md#tagtypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CertificateOptionsTypeDef](./type_defs.md#certificateoptionstypedef)
- [ExtendedKeyUsageTypeDef](./type_defs.md#extendedkeyusagetypedef)
- [KeyUsageTypeDef](./type_defs.md#keyusagetypedef)
- [CertificateSummaryTypeDef](./type_defs.md#certificatesummarytypedef)
- [DeleteCertificateRequestRequestTypeDef](./type_defs.md#deletecertificaterequestrequesttypedef)
- [DescribeCertificateRequestRequestTypeDef](./type_defs.md#describecertificaterequestrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DomainValidationOptionTypeDef](./type_defs.md#domainvalidationoptiontypedef)
- [ResourceRecordTypeDef](./type_defs.md#resourcerecordtypedef)
- [ExpiryEventsConfigurationTypeDef](./type_defs.md#expiryeventsconfigurationtypedef)
- [FiltersTypeDef](./type_defs.md#filterstypedef)
- [GetCertificateRequestRequestTypeDef](./type_defs.md#getcertificaterequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListTagsForCertificateRequestRequestTypeDef](./type_defs.md#listtagsforcertificaterequestrequesttypedef)
- [RenewCertificateRequestRequestTypeDef](./type_defs.md#renewcertificaterequestrequesttypedef)
- [ResendValidationEmailRequestRequestTypeDef](./type_defs.md#resendvalidationemailrequestrequesttypedef)
- [AddTagsToCertificateRequestRequestTypeDef](./type_defs.md#addtagstocertificaterequestrequesttypedef)
- [RemoveTagsFromCertificateRequestRequestTypeDef](./type_defs.md#removetagsfromcertificaterequestrequesttypedef)
- [ExportCertificateRequestRequestTypeDef](./type_defs.md#exportcertificaterequestrequesttypedef)
- [ImportCertificateRequestRequestTypeDef](./type_defs.md#importcertificaterequestrequesttypedef)
- [UpdateCertificateOptionsRequestRequestTypeDef](./type_defs.md#updatecertificateoptionsrequestrequesttypedef)
- [DescribeCertificateRequestWaitTypeDef](./type_defs.md#describecertificaterequestwaittypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ExportCertificateResponseTypeDef](./type_defs.md#exportcertificateresponsetypedef)
- [GetCertificateResponseTypeDef](./type_defs.md#getcertificateresponsetypedef)
- [ImportCertificateResponseTypeDef](./type_defs.md#importcertificateresponsetypedef)
- [ListCertificatesResponseTypeDef](./type_defs.md#listcertificatesresponsetypedef)
- [ListTagsForCertificateResponseTypeDef](./type_defs.md#listtagsforcertificateresponsetypedef)
- [RequestCertificateResponseTypeDef](./type_defs.md#requestcertificateresponsetypedef)
- [RequestCertificateRequestRequestTypeDef](./type_defs.md#requestcertificaterequestrequesttypedef)
- [DomainValidationTypeDef](./type_defs.md#domainvalidationtypedef)
- [GetAccountConfigurationResponseTypeDef](./type_defs.md#getaccountconfigurationresponsetypedef)
- [PutAccountConfigurationRequestRequestTypeDef](./type_defs.md#putaccountconfigurationrequestrequesttypedef)
- [ListCertificatesRequestRequestTypeDef](./type_defs.md#listcertificatesrequestrequesttypedef)
- [ListCertificatesRequestPaginateTypeDef](./type_defs.md#listcertificatesrequestpaginatetypedef)
- [RenewalSummaryTypeDef](./type_defs.md#renewalsummarytypedef)
- [CertificateDetailTypeDef](./type_defs.md#certificatedetailtypedef)
- [DescribeCertificateResponseTypeDef](./type_defs.md#describecertificateresponsetypedef)
