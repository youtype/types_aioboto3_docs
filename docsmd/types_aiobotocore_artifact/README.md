# Artifact module

> [Index](../README.md) > Artifact


!!! note ""

    Auto-generated documentation for [Artifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#artifact)
    type annotations stubs module [types-aiobotocore-artifact](https://pypi.org/project/types-aiobotocore-artifact/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `Artifact` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `Artifact` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[artifact]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[artifact]'

# standalone installation
python -m pip install types-aiobotocore-artifact
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-artifact
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ArtifactClient

Type annotations and code completion for  `#!python session.client("artifact")` as [ArtifactClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact.Client)

```python
# ArtifactClient usage example

from aioboto3.session import Session

from types_aiobotocore_artifact.client import ArtifactClient


session = Session()
async with session.client("artifact") as client:
    client: ArtifactClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("artifact").get_paginator("...")`.

```python
# ListCustomerAgreementsPaginator usage example

from types_aiobotocore_artifact.paginator import ListCustomerAgreementsPaginator

def get_list_customer_agreements_paginator() -> ListCustomerAgreementsPaginator:
    return client.get_paginator("list_customer_agreements"))
```

- [ListCustomerAgreementsPaginator](./paginators.md#listcustomeragreementspaginator)
- [ListReportsPaginator](./paginators.md#listreportspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AcceptanceTypeType usage example

from types_aiobotocore_artifact.literals import AcceptanceTypeType

def get_value() -> AcceptanceTypeType:
    return "EXPLICIT"
```

- [AcceptanceTypeType](./literals.md#acceptancetypetype)
- [AgreementTypeType](./literals.md#agreementtypetype)
- [CustomerAgreementStateType](./literals.md#customeragreementstatetype)
- [ListCustomerAgreementsPaginatorName](./literals.md#listcustomeragreementspaginatorname)
- [ListReportsPaginatorName](./literals.md#listreportspaginatorname)
- [NotificationSubscriptionStatusType](./literals.md#notificationsubscriptionstatustype)
- [PublishedStateType](./literals.md#publishedstatetype)
- [UploadStateType](./literals.md#uploadstatetype)
- [ArtifactServiceName](./literals.md#artifactservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef)
- [CustomerAgreementSummaryTypeDef](./type_defs.md#customeragreementsummarytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetReportMetadataRequestRequestTypeDef](./type_defs.md#getreportmetadatarequestrequesttypedef)
- [ReportDetailTypeDef](./type_defs.md#reportdetailtypedef)
- [GetReportRequestRequestTypeDef](./type_defs.md#getreportrequestrequesttypedef)
- [GetTermForReportRequestRequestTypeDef](./type_defs.md#gettermforreportrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListCustomerAgreementsRequestRequestTypeDef](./type_defs.md#listcustomeragreementsrequestrequesttypedef)
- [ListReportsRequestRequestTypeDef](./type_defs.md#listreportsrequestrequesttypedef)
- [ReportSummaryTypeDef](./type_defs.md#reportsummarytypedef)
- [PutAccountSettingsRequestRequestTypeDef](./type_defs.md#putaccountsettingsrequestrequesttypedef)
- [GetAccountSettingsResponseTypeDef](./type_defs.md#getaccountsettingsresponsetypedef)
- [GetReportResponseTypeDef](./type_defs.md#getreportresponsetypedef)
- [GetTermForReportResponseTypeDef](./type_defs.md#gettermforreportresponsetypedef)
- [ListCustomerAgreementsResponseTypeDef](./type_defs.md#listcustomeragreementsresponsetypedef)
- [PutAccountSettingsResponseTypeDef](./type_defs.md#putaccountsettingsresponsetypedef)
- [GetReportMetadataResponseTypeDef](./type_defs.md#getreportmetadataresponsetypedef)
- [ListCustomerAgreementsRequestPaginateTypeDef](./type_defs.md#listcustomeragreementsrequestpaginatetypedef)
- [ListReportsRequestPaginateTypeDef](./type_defs.md#listreportsrequestpaginatetypedef)
- [ListReportsResponseTypeDef](./type_defs.md#listreportsresponsetypedef)
