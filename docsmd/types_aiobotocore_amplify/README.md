# Amplify module

> [Index](../README.md) > Amplify


!!! note ""

    Auto-generated documentation for [Amplify](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#amplify)
    type annotations stubs module [types-aiobotocore-amplify](https://pypi.org/project/types-aiobotocore-amplify/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `Amplify` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `Amplify` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[amplify]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[amplify]'

# standalone installation
python -m pip install types-aiobotocore-amplify
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-amplify
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AmplifyClient

Type annotations and code completion for  `#!python session.client("amplify")` as [AmplifyClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client)

```python
# AmplifyClient usage example

from aioboto3.session import Session

from types_aiobotocore_amplify.client import AmplifyClient


session = Session()
async with session.client("amplify") as client:
    client: AmplifyClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("amplify").get_paginator("...")`.

```python
# ListAppsPaginator usage example

from types_aiobotocore_amplify.paginator import ListAppsPaginator

def get_list_apps_paginator() -> ListAppsPaginator:
    return client.get_paginator("list_apps"))
```

- [ListAppsPaginator](./paginators.md#listappspaginator)
- [ListBranchesPaginator](./paginators.md#listbranchespaginator)
- [ListDomainAssociationsPaginator](./paginators.md#listdomainassociationspaginator)
- [ListJobsPaginator](./paginators.md#listjobspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CacheConfigTypeType usage example

from types_aiobotocore_amplify.literals import CacheConfigTypeType

def get_value() -> CacheConfigTypeType:
    return "AMPLIFY_MANAGED"
```

- [CacheConfigTypeType](./literals.md#cacheconfigtypetype)
- [CertificateTypeType](./literals.md#certificatetypetype)
- [DomainStatusType](./literals.md#domainstatustype)
- [JobStatusType](./literals.md#jobstatustype)
- [JobTypeType](./literals.md#jobtypetype)
- [ListAppsPaginatorName](./literals.md#listappspaginatorname)
- [ListBranchesPaginatorName](./literals.md#listbranchespaginatorname)
- [ListDomainAssociationsPaginatorName](./literals.md#listdomainassociationspaginatorname)
- [ListJobsPaginatorName](./literals.md#listjobspaginatorname)
- [PlatformType](./literals.md#platformtype)
- [RepositoryCloneMethodType](./literals.md#repositoryclonemethodtype)
- [SourceUrlTypeType](./literals.md#sourceurltypetype)
- [StageType](./literals.md#stagetype)
- [UpdateStatusType](./literals.md#updatestatustype)
- [AmplifyServiceName](./literals.md#amplifyservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AutoBranchCreationConfigOutputTypeDef](./type_defs.md#autobranchcreationconfigoutputtypedef)
- [CacheConfigTypeDef](./type_defs.md#cacheconfigtypedef)
- [CustomRuleTypeDef](./type_defs.md#customruletypedef)
- [ProductionBranchTypeDef](./type_defs.md#productionbranchtypedef)
- [ArtifactTypeDef](./type_defs.md#artifacttypedef)
- [AutoBranchCreationConfigTypeDef](./type_defs.md#autobranchcreationconfigtypedef)
- [BackendEnvironmentTypeDef](./type_defs.md#backendenvironmenttypedef)
- [BackendTypeDef](./type_defs.md#backendtypedef)
- [CertificateSettingsTypeDef](./type_defs.md#certificatesettingstypedef)
- [CertificateTypeDef](./type_defs.md#certificatetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateBackendEnvironmentRequestRequestTypeDef](./type_defs.md#createbackendenvironmentrequestrequesttypedef)
- [CreateDeploymentRequestRequestTypeDef](./type_defs.md#createdeploymentrequestrequesttypedef)
- [SubDomainSettingTypeDef](./type_defs.md#subdomainsettingtypedef)
- [CreateWebhookRequestRequestTypeDef](./type_defs.md#createwebhookrequestrequesttypedef)
- [WebhookTypeDef](./type_defs.md#webhooktypedef)
- [DeleteAppRequestRequestTypeDef](./type_defs.md#deleteapprequestrequesttypedef)
- [DeleteBackendEnvironmentRequestRequestTypeDef](./type_defs.md#deletebackendenvironmentrequestrequesttypedef)
- [DeleteBranchRequestRequestTypeDef](./type_defs.md#deletebranchrequestrequesttypedef)
- [DeleteDomainAssociationRequestRequestTypeDef](./type_defs.md#deletedomainassociationrequestrequesttypedef)
- [DeleteJobRequestRequestTypeDef](./type_defs.md#deletejobrequestrequesttypedef)
- [JobSummaryTypeDef](./type_defs.md#jobsummarytypedef)
- [DeleteWebhookRequestRequestTypeDef](./type_defs.md#deletewebhookrequestrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [GetAppRequestRequestTypeDef](./type_defs.md#getapprequestrequesttypedef)
- [GetArtifactUrlRequestRequestTypeDef](./type_defs.md#getartifacturlrequestrequesttypedef)
- [GetBackendEnvironmentRequestRequestTypeDef](./type_defs.md#getbackendenvironmentrequestrequesttypedef)
- [GetBranchRequestRequestTypeDef](./type_defs.md#getbranchrequestrequesttypedef)
- [GetDomainAssociationRequestRequestTypeDef](./type_defs.md#getdomainassociationrequestrequesttypedef)
- [GetJobRequestRequestTypeDef](./type_defs.md#getjobrequestrequesttypedef)
- [GetWebhookRequestRequestTypeDef](./type_defs.md#getwebhookrequestrequesttypedef)
- [StepTypeDef](./type_defs.md#steptypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAppsRequestRequestTypeDef](./type_defs.md#listappsrequestrequesttypedef)
- [ListArtifactsRequestRequestTypeDef](./type_defs.md#listartifactsrequestrequesttypedef)
- [ListBackendEnvironmentsRequestRequestTypeDef](./type_defs.md#listbackendenvironmentsrequestrequesttypedef)
- [ListBranchesRequestRequestTypeDef](./type_defs.md#listbranchesrequestrequesttypedef)
- [ListDomainAssociationsRequestRequestTypeDef](./type_defs.md#listdomainassociationsrequestrequesttypedef)
- [ListJobsRequestRequestTypeDef](./type_defs.md#listjobsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListWebhooksRequestRequestTypeDef](./type_defs.md#listwebhooksrequestrequesttypedef)
- [StartDeploymentRequestRequestTypeDef](./type_defs.md#startdeploymentrequestrequesttypedef)
- [StopJobRequestRequestTypeDef](./type_defs.md#stopjobrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateWebhookRequestRequestTypeDef](./type_defs.md#updatewebhookrequestrequesttypedef)
- [AppTypeDef](./type_defs.md#apptypedef)
- [CreateAppRequestRequestTypeDef](./type_defs.md#createapprequestrequesttypedef)
- [UpdateAppRequestRequestTypeDef](./type_defs.md#updateapprequestrequesttypedef)
- [BranchTypeDef](./type_defs.md#branchtypedef)
- [CreateBranchRequestRequestTypeDef](./type_defs.md#createbranchrequestrequesttypedef)
- [UpdateBranchRequestRequestTypeDef](./type_defs.md#updatebranchrequestrequesttypedef)
- [CreateBackendEnvironmentResultTypeDef](./type_defs.md#createbackendenvironmentresulttypedef)
- [CreateDeploymentResultTypeDef](./type_defs.md#createdeploymentresulttypedef)
- [DeleteBackendEnvironmentResultTypeDef](./type_defs.md#deletebackendenvironmentresulttypedef)
- [GenerateAccessLogsResultTypeDef](./type_defs.md#generateaccesslogsresulttypedef)
- [GetArtifactUrlResultTypeDef](./type_defs.md#getartifacturlresulttypedef)
- [GetBackendEnvironmentResultTypeDef](./type_defs.md#getbackendenvironmentresulttypedef)
- [ListArtifactsResultTypeDef](./type_defs.md#listartifactsresulttypedef)
- [ListBackendEnvironmentsResultTypeDef](./type_defs.md#listbackendenvironmentsresulttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [CreateDomainAssociationRequestRequestTypeDef](./type_defs.md#createdomainassociationrequestrequesttypedef)
- [SubDomainTypeDef](./type_defs.md#subdomaintypedef)
- [UpdateDomainAssociationRequestRequestTypeDef](./type_defs.md#updatedomainassociationrequestrequesttypedef)
- [CreateWebhookResultTypeDef](./type_defs.md#createwebhookresulttypedef)
- [DeleteWebhookResultTypeDef](./type_defs.md#deletewebhookresulttypedef)
- [GetWebhookResultTypeDef](./type_defs.md#getwebhookresulttypedef)
- [ListWebhooksResultTypeDef](./type_defs.md#listwebhooksresulttypedef)
- [UpdateWebhookResultTypeDef](./type_defs.md#updatewebhookresulttypedef)
- [DeleteJobResultTypeDef](./type_defs.md#deletejobresulttypedef)
- [ListJobsResultTypeDef](./type_defs.md#listjobsresulttypedef)
- [StartDeploymentResultTypeDef](./type_defs.md#startdeploymentresulttypedef)
- [StartJobResultTypeDef](./type_defs.md#startjobresulttypedef)
- [StopJobResultTypeDef](./type_defs.md#stopjobresulttypedef)
- [GenerateAccessLogsRequestRequestTypeDef](./type_defs.md#generateaccesslogsrequestrequesttypedef)
- [StartJobRequestRequestTypeDef](./type_defs.md#startjobrequestrequesttypedef)
- [JobTypeDef](./type_defs.md#jobtypedef)
- [ListAppsRequestPaginateTypeDef](./type_defs.md#listappsrequestpaginatetypedef)
- [ListBranchesRequestPaginateTypeDef](./type_defs.md#listbranchesrequestpaginatetypedef)
- [ListDomainAssociationsRequestPaginateTypeDef](./type_defs.md#listdomainassociationsrequestpaginatetypedef)
- [ListJobsRequestPaginateTypeDef](./type_defs.md#listjobsrequestpaginatetypedef)
- [CreateAppResultTypeDef](./type_defs.md#createappresulttypedef)
- [DeleteAppResultTypeDef](./type_defs.md#deleteappresulttypedef)
- [GetAppResultTypeDef](./type_defs.md#getappresulttypedef)
- [ListAppsResultTypeDef](./type_defs.md#listappsresulttypedef)
- [UpdateAppResultTypeDef](./type_defs.md#updateappresulttypedef)
- [CreateBranchResultTypeDef](./type_defs.md#createbranchresulttypedef)
- [DeleteBranchResultTypeDef](./type_defs.md#deletebranchresulttypedef)
- [GetBranchResultTypeDef](./type_defs.md#getbranchresulttypedef)
- [ListBranchesResultTypeDef](./type_defs.md#listbranchesresulttypedef)
- [UpdateBranchResultTypeDef](./type_defs.md#updatebranchresulttypedef)
- [DomainAssociationTypeDef](./type_defs.md#domainassociationtypedef)
- [GetJobResultTypeDef](./type_defs.md#getjobresulttypedef)
- [CreateDomainAssociationResultTypeDef](./type_defs.md#createdomainassociationresulttypedef)
- [DeleteDomainAssociationResultTypeDef](./type_defs.md#deletedomainassociationresulttypedef)
- [GetDomainAssociationResultTypeDef](./type_defs.md#getdomainassociationresulttypedef)
- [ListDomainAssociationsResultTypeDef](./type_defs.md#listdomainassociationsresulttypedef)
- [UpdateDomainAssociationResultTypeDef](./type_defs.md#updatedomainassociationresulttypedef)
