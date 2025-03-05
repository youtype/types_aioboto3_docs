# CodeBuild module

> [Index](../README.md) > CodeBuild


!!! note ""

    Auto-generated documentation for [CodeBuild](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#codebuild)
    type annotations stubs module [types-aiobotocore-codebuild](https://pypi.org/project/types-aiobotocore-codebuild/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==14.1.0' mypy-boto3-builder`
1. Select `aioboto3` AWS SDK.
1. Add `CodeBuild` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `CodeBuild` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[codebuild]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[codebuild]'

# standalone installation
python -m pip install types-aiobotocore-codebuild
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-codebuild
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CodeBuildClient

Type annotations and code completion for  `#!python session.client("codebuild")` as [CodeBuildClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client)

```python
# CodeBuildClient usage example

from aioboto3.session import Session

from types_aiobotocore_codebuild.client import CodeBuildClient


session = Session()
async with session.client("codebuild") as client:
    client: CodeBuildClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("codebuild").get_paginator("...")`.

```python
# DescribeCodeCoveragesPaginator usage example

from types_aiobotocore_codebuild.paginator import DescribeCodeCoveragesPaginator

def get_describe_code_coverages_paginator() -> DescribeCodeCoveragesPaginator:
    return client.get_paginator("describe_code_coverages"))
```

- [DescribeCodeCoveragesPaginator](./paginators.md#describecodecoveragespaginator)
- [DescribeTestCasesPaginator](./paginators.md#describetestcasespaginator)
- [ListBuildBatchesForProjectPaginator](./paginators.md#listbuildbatchesforprojectpaginator)
- [ListBuildBatchesPaginator](./paginators.md#listbuildbatchespaginator)
- [ListBuildsForProjectPaginator](./paginators.md#listbuildsforprojectpaginator)
- [ListBuildsPaginator](./paginators.md#listbuildspaginator)
- [ListProjectsPaginator](./paginators.md#listprojectspaginator)
- [ListReportGroupsPaginator](./paginators.md#listreportgroupspaginator)
- [ListReportsForReportGroupPaginator](./paginators.md#listreportsforreportgrouppaginator)
- [ListReportsPaginator](./paginators.md#listreportspaginator)
- [ListSharedProjectsPaginator](./paginators.md#listsharedprojectspaginator)
- [ListSharedReportGroupsPaginator](./paginators.md#listsharedreportgroupspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ArtifactNamespaceType usage example

from types_aiobotocore_codebuild.literals import ArtifactNamespaceType

def get_value() -> ArtifactNamespaceType:
    return "BUILD_ID"
```

- [ArtifactNamespaceType](./literals.md#artifactnamespacetype)
- [ArtifactPackagingType](./literals.md#artifactpackagingtype)
- [ArtifactsTypeType](./literals.md#artifactstypetype)
- [AuthTypeType](./literals.md#authtypetype)
- [BatchReportModeTypeType](./literals.md#batchreportmodetypetype)
- [BucketOwnerAccessType](./literals.md#bucketowneraccesstype)
- [BuildBatchPhaseTypeType](./literals.md#buildbatchphasetypetype)
- [BuildPhaseTypeType](./literals.md#buildphasetypetype)
- [CacheModeType](./literals.md#cachemodetype)
- [CacheTypeType](./literals.md#cachetypetype)
- [ComputeTypeType](./literals.md#computetypetype)
- [CredentialProviderTypeType](./literals.md#credentialprovidertypetype)
- [DescribeCodeCoveragesPaginatorName](./literals.md#describecodecoveragespaginatorname)
- [DescribeTestCasesPaginatorName](./literals.md#describetestcasespaginatorname)
- [EnvironmentTypeType](./literals.md#environmenttypetype)
- [EnvironmentVariableTypeType](./literals.md#environmentvariabletypetype)
- [FileSystemTypeType](./literals.md#filesystemtypetype)
- [FleetContextCodeType](./literals.md#fleetcontextcodetype)
- [FleetOverflowBehaviorType](./literals.md#fleetoverflowbehaviortype)
- [FleetProxyRuleBehaviorType](./literals.md#fleetproxyrulebehaviortype)
- [FleetProxyRuleEffectTypeType](./literals.md#fleetproxyruleeffecttypetype)
- [FleetProxyRuleTypeType](./literals.md#fleetproxyruletypetype)
- [FleetScalingMetricTypeType](./literals.md#fleetscalingmetrictypetype)
- [FleetScalingTypeType](./literals.md#fleetscalingtypetype)
- [FleetSortByTypeType](./literals.md#fleetsortbytypetype)
- [FleetStatusCodeType](./literals.md#fleetstatuscodetype)
- [ImagePullCredentialsTypeType](./literals.md#imagepullcredentialstypetype)
- [LanguageTypeType](./literals.md#languagetypetype)
- [ListBuildBatchesForProjectPaginatorName](./literals.md#listbuildbatchesforprojectpaginatorname)
- [ListBuildBatchesPaginatorName](./literals.md#listbuildbatchespaginatorname)
- [ListBuildsForProjectPaginatorName](./literals.md#listbuildsforprojectpaginatorname)
- [ListBuildsPaginatorName](./literals.md#listbuildspaginatorname)
- [ListProjectsPaginatorName](./literals.md#listprojectspaginatorname)
- [ListReportGroupsPaginatorName](./literals.md#listreportgroupspaginatorname)
- [ListReportsForReportGroupPaginatorName](./literals.md#listreportsforreportgrouppaginatorname)
- [ListReportsPaginatorName](./literals.md#listreportspaginatorname)
- [ListSharedProjectsPaginatorName](./literals.md#listsharedprojectspaginatorname)
- [ListSharedReportGroupsPaginatorName](./literals.md#listsharedreportgroupspaginatorname)
- [LogsConfigStatusTypeType](./literals.md#logsconfigstatustypetype)
- [MachineTypeType](./literals.md#machinetypetype)
- [PlatformTypeType](./literals.md#platformtypetype)
- [ProjectSortByTypeType](./literals.md#projectsortbytypetype)
- [ProjectVisibilityTypeType](./literals.md#projectvisibilitytypetype)
- [ReportCodeCoverageSortByTypeType](./literals.md#reportcodecoveragesortbytypetype)
- [ReportExportConfigTypeType](./literals.md#reportexportconfigtypetype)
- [ReportGroupSortByTypeType](./literals.md#reportgroupsortbytypetype)
- [ReportGroupStatusTypeType](./literals.md#reportgroupstatustypetype)
- [ReportGroupTrendFieldTypeType](./literals.md#reportgrouptrendfieldtypetype)
- [ReportPackagingTypeType](./literals.md#reportpackagingtypetype)
- [ReportStatusTypeType](./literals.md#reportstatustypetype)
- [ReportTypeType](./literals.md#reporttypetype)
- [RetryBuildBatchTypeType](./literals.md#retrybuildbatchtypetype)
- [ServerTypeType](./literals.md#servertypetype)
- [SharedResourceSortByTypeType](./literals.md#sharedresourcesortbytypetype)
- [SortOrderTypeType](./literals.md#sortordertypetype)
- [SourceAuthTypeType](./literals.md#sourceauthtypetype)
- [SourceTypeType](./literals.md#sourcetypetype)
- [StatusTypeType](./literals.md#statustypetype)
- [WebhookBuildTypeType](./literals.md#webhookbuildtypetype)
- [WebhookFilterTypeType](./literals.md#webhookfiltertypetype)
- [WebhookScopeTypeType](./literals.md#webhookscopetypetype)
- [WebhookStatusType](./literals.md#webhookstatustype)
- [CodeBuildServiceName](./literals.md#codebuildservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AutoRetryConfigTypeDef](./type_defs.md#autoretryconfigtypedef)
- [BatchDeleteBuildsInputTypeDef](./type_defs.md#batchdeletebuildsinputtypedef)
- [BuildNotDeletedTypeDef](./type_defs.md#buildnotdeletedtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BatchGetBuildBatchesInputTypeDef](./type_defs.md#batchgetbuildbatchesinputtypedef)
- [BatchGetBuildsInputTypeDef](./type_defs.md#batchgetbuildsinputtypedef)
- [BatchGetFleetsInputTypeDef](./type_defs.md#batchgetfleetsinputtypedef)
- [BatchGetProjectsInputTypeDef](./type_defs.md#batchgetprojectsinputtypedef)
- [BatchGetReportGroupsInputTypeDef](./type_defs.md#batchgetreportgroupsinputtypedef)
- [BatchGetReportsInputTypeDef](./type_defs.md#batchgetreportsinputtypedef)
- [BatchRestrictionsOutputTypeDef](./type_defs.md#batchrestrictionsoutputtypedef)
- [BatchRestrictionsTypeDef](./type_defs.md#batchrestrictionstypedef)
- [BuildArtifactsTypeDef](./type_defs.md#buildartifactstypedef)
- [BuildBatchFilterTypeDef](./type_defs.md#buildbatchfiltertypedef)
- [PhaseContextTypeDef](./type_defs.md#phasecontexttypedef)
- [ProjectCacheOutputTypeDef](./type_defs.md#projectcacheoutputtypedef)
- [ProjectFileSystemLocationTypeDef](./type_defs.md#projectfilesystemlocationtypedef)
- [ProjectSourceVersionTypeDef](./type_defs.md#projectsourceversiontypedef)
- [VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef)
- [BuildStatusConfigTypeDef](./type_defs.md#buildstatusconfigtypedef)
- [ResolvedArtifactTypeDef](./type_defs.md#resolvedartifacttypedef)
- [DebugSessionTypeDef](./type_defs.md#debugsessiontypedef)
- [ExportedEnvironmentVariableTypeDef](./type_defs.md#exportedenvironmentvariabletypedef)
- [NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef)
- [CloudWatchLogsConfigTypeDef](./type_defs.md#cloudwatchlogsconfigtypedef)
- [CodeCoverageReportSummaryTypeDef](./type_defs.md#codecoveragereportsummarytypedef)
- [CodeCoverageTypeDef](./type_defs.md#codecoveragetypedef)
- [ComputeConfigurationTypeDef](./type_defs.md#computeconfigurationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ProjectArtifactsTypeDef](./type_defs.md#projectartifactstypedef)
- [ScopeConfigurationTypeDef](./type_defs.md#scopeconfigurationtypedef)
- [WebhookFilterTypeDef](./type_defs.md#webhookfiltertypedef)
- [DeleteBuildBatchInputTypeDef](./type_defs.md#deletebuildbatchinputtypedef)
- [DeleteFleetInputTypeDef](./type_defs.md#deletefleetinputtypedef)
- [DeleteProjectInputTypeDef](./type_defs.md#deleteprojectinputtypedef)
- [DeleteReportGroupInputTypeDef](./type_defs.md#deletereportgroupinputtypedef)
- [DeleteReportInputTypeDef](./type_defs.md#deletereportinputtypedef)
- [DeleteResourcePolicyInputTypeDef](./type_defs.md#deleteresourcepolicyinputtypedef)
- [DeleteSourceCredentialsInputTypeDef](./type_defs.md#deletesourcecredentialsinputtypedef)
- [DeleteWebhookInputTypeDef](./type_defs.md#deletewebhookinputtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeCodeCoveragesInputTypeDef](./type_defs.md#describecodecoveragesinputtypedef)
- [TestCaseFilterTypeDef](./type_defs.md#testcasefiltertypedef)
- [TestCaseTypeDef](./type_defs.md#testcasetypedef)
- [EnvironmentImageTypeDef](./type_defs.md#environmentimagetypedef)
- [EnvironmentVariableTypeDef](./type_defs.md#environmentvariabletypedef)
- [FleetProxyRuleOutputTypeDef](./type_defs.md#fleetproxyruleoutputtypedef)
- [FleetProxyRuleTypeDef](./type_defs.md#fleetproxyruletypedef)
- [FleetStatusTypeDef](./type_defs.md#fleetstatustypedef)
- [GetReportGroupTrendInputTypeDef](./type_defs.md#getreportgrouptrendinputtypedef)
- [ReportGroupTrendStatsTypeDef](./type_defs.md#reportgrouptrendstatstypedef)
- [ReportWithRawDataTypeDef](./type_defs.md#reportwithrawdatatypedef)
- [GetResourcePolicyInputTypeDef](./type_defs.md#getresourcepolicyinputtypedef)
- [GitSubmodulesConfigTypeDef](./type_defs.md#gitsubmodulesconfigtypedef)
- [ImportSourceCredentialsInputTypeDef](./type_defs.md#importsourcecredentialsinputtypedef)
- [InvalidateProjectCacheInputTypeDef](./type_defs.md#invalidateprojectcacheinputtypedef)
- [ListBuildsForProjectInputTypeDef](./type_defs.md#listbuildsforprojectinputtypedef)
- [ListBuildsInputTypeDef](./type_defs.md#listbuildsinputtypedef)
- [ListFleetsInputTypeDef](./type_defs.md#listfleetsinputtypedef)
- [ListProjectsInputTypeDef](./type_defs.md#listprojectsinputtypedef)
- [ListReportGroupsInputTypeDef](./type_defs.md#listreportgroupsinputtypedef)
- [ReportFilterTypeDef](./type_defs.md#reportfiltertypedef)
- [ListSharedProjectsInputTypeDef](./type_defs.md#listsharedprojectsinputtypedef)
- [ListSharedReportGroupsInputTypeDef](./type_defs.md#listsharedreportgroupsinputtypedef)
- [SourceCredentialsInfoTypeDef](./type_defs.md#sourcecredentialsinfotypedef)
- [S3LogsConfigTypeDef](./type_defs.md#s3logsconfigtypedef)
- [ProjectBadgeTypeDef](./type_defs.md#projectbadgetypedef)
- [ProjectCacheTypeDef](./type_defs.md#projectcachetypedef)
- [ProjectFleetTypeDef](./type_defs.md#projectfleettypedef)
- [RegistryCredentialTypeDef](./type_defs.md#registrycredentialtypedef)
- [SourceAuthTypeDef](./type_defs.md#sourceauthtypedef)
- [PutResourcePolicyInputTypeDef](./type_defs.md#putresourcepolicyinputtypedef)
- [S3ReportExportConfigTypeDef](./type_defs.md#s3reportexportconfigtypedef)
- [TestReportSummaryTypeDef](./type_defs.md#testreportsummarytypedef)
- [RetryBuildBatchInputTypeDef](./type_defs.md#retrybuildbatchinputtypedef)
- [RetryBuildInputTypeDef](./type_defs.md#retrybuildinputtypedef)
- [TargetTrackingScalingConfigurationTypeDef](./type_defs.md#targettrackingscalingconfigurationtypedef)
- [StopBuildBatchInputTypeDef](./type_defs.md#stopbuildbatchinputtypedef)
- [StopBuildInputTypeDef](./type_defs.md#stopbuildinputtypedef)
- [UpdateProjectVisibilityInputTypeDef](./type_defs.md#updateprojectvisibilityinputtypedef)
- [VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef)
- [BatchDeleteBuildsOutputTypeDef](./type_defs.md#batchdeletebuildsoutputtypedef)
- [DeleteBuildBatchOutputTypeDef](./type_defs.md#deletebuildbatchoutputtypedef)
- [DeleteSourceCredentialsOutputTypeDef](./type_defs.md#deletesourcecredentialsoutputtypedef)
- [GetResourcePolicyOutputTypeDef](./type_defs.md#getresourcepolicyoutputtypedef)
- [ImportSourceCredentialsOutputTypeDef](./type_defs.md#importsourcecredentialsoutputtypedef)
- [ListBuildBatchesForProjectOutputTypeDef](./type_defs.md#listbuildbatchesforprojectoutputtypedef)
- [ListBuildBatchesOutputTypeDef](./type_defs.md#listbuildbatchesoutputtypedef)
- [ListBuildsForProjectOutputTypeDef](./type_defs.md#listbuildsforprojectoutputtypedef)
- [ListBuildsOutputTypeDef](./type_defs.md#listbuildsoutputtypedef)
- [ListFleetsOutputTypeDef](./type_defs.md#listfleetsoutputtypedef)
- [ListProjectsOutputTypeDef](./type_defs.md#listprojectsoutputtypedef)
- [ListReportGroupsOutputTypeDef](./type_defs.md#listreportgroupsoutputtypedef)
- [ListReportsForReportGroupOutputTypeDef](./type_defs.md#listreportsforreportgroupoutputtypedef)
- [ListReportsOutputTypeDef](./type_defs.md#listreportsoutputtypedef)
- [ListSharedProjectsOutputTypeDef](./type_defs.md#listsharedprojectsoutputtypedef)
- [ListSharedReportGroupsOutputTypeDef](./type_defs.md#listsharedreportgroupsoutputtypedef)
- [PutResourcePolicyOutputTypeDef](./type_defs.md#putresourcepolicyoutputtypedef)
- [UpdateProjectVisibilityOutputTypeDef](./type_defs.md#updateprojectvisibilityoutputtypedef)
- [ProjectBuildBatchConfigOutputTypeDef](./type_defs.md#projectbuildbatchconfigoutputtypedef)
- [ProjectBuildBatchConfigTypeDef](./type_defs.md#projectbuildbatchconfigtypedef)
- [ListBuildBatchesForProjectInputTypeDef](./type_defs.md#listbuildbatchesforprojectinputtypedef)
- [ListBuildBatchesInputTypeDef](./type_defs.md#listbuildbatchesinputtypedef)
- [BuildBatchPhaseTypeDef](./type_defs.md#buildbatchphasetypedef)
- [BuildPhaseTypeDef](./type_defs.md#buildphasetypedef)
- [BuildSummaryTypeDef](./type_defs.md#buildsummarytypedef)
- [DescribeCodeCoveragesOutputTypeDef](./type_defs.md#describecodecoveragesoutputtypedef)
- [CreateWebhookInputTypeDef](./type_defs.md#createwebhookinputtypedef)
- [UpdateWebhookInputTypeDef](./type_defs.md#updatewebhookinputtypedef)
- [WebhookTypeDef](./type_defs.md#webhooktypedef)
- [DescribeCodeCoveragesInputPaginateTypeDef](./type_defs.md#describecodecoveragesinputpaginatetypedef)
- [ListBuildBatchesForProjectInputPaginateTypeDef](./type_defs.md#listbuildbatchesforprojectinputpaginatetypedef)
- [ListBuildBatchesInputPaginateTypeDef](./type_defs.md#listbuildbatchesinputpaginatetypedef)
- [ListBuildsForProjectInputPaginateTypeDef](./type_defs.md#listbuildsforprojectinputpaginatetypedef)
- [ListBuildsInputPaginateTypeDef](./type_defs.md#listbuildsinputpaginatetypedef)
- [ListProjectsInputPaginateTypeDef](./type_defs.md#listprojectsinputpaginatetypedef)
- [ListReportGroupsInputPaginateTypeDef](./type_defs.md#listreportgroupsinputpaginatetypedef)
- [ListSharedProjectsInputPaginateTypeDef](./type_defs.md#listsharedprojectsinputpaginatetypedef)
- [ListSharedReportGroupsInputPaginateTypeDef](./type_defs.md#listsharedreportgroupsinputpaginatetypedef)
- [DescribeTestCasesInputPaginateTypeDef](./type_defs.md#describetestcasesinputpaginatetypedef)
- [DescribeTestCasesInputTypeDef](./type_defs.md#describetestcasesinputtypedef)
- [DescribeTestCasesOutputTypeDef](./type_defs.md#describetestcasesoutputtypedef)
- [EnvironmentLanguageTypeDef](./type_defs.md#environmentlanguagetypedef)
- [ProxyConfigurationOutputTypeDef](./type_defs.md#proxyconfigurationoutputtypedef)
- [ProxyConfigurationTypeDef](./type_defs.md#proxyconfigurationtypedef)
- [GetReportGroupTrendOutputTypeDef](./type_defs.md#getreportgrouptrendoutputtypedef)
- [ListReportsForReportGroupInputPaginateTypeDef](./type_defs.md#listreportsforreportgroupinputpaginatetypedef)
- [ListReportsForReportGroupInputTypeDef](./type_defs.md#listreportsforreportgroupinputtypedef)
- [ListReportsInputPaginateTypeDef](./type_defs.md#listreportsinputpaginatetypedef)
- [ListReportsInputTypeDef](./type_defs.md#listreportsinputtypedef)
- [ListSourceCredentialsOutputTypeDef](./type_defs.md#listsourcecredentialsoutputtypedef)
- [LogsConfigTypeDef](./type_defs.md#logsconfigtypedef)
- [LogsLocationTypeDef](./type_defs.md#logslocationtypedef)
- [ProjectCacheUnionTypeDef](./type_defs.md#projectcacheuniontypedef)
- [ProjectEnvironmentOutputTypeDef](./type_defs.md#projectenvironmentoutputtypedef)
- [ProjectEnvironmentTypeDef](./type_defs.md#projectenvironmenttypedef)
- [ProjectSourceTypeDef](./type_defs.md#projectsourcetypedef)
- [ReportExportConfigTypeDef](./type_defs.md#reportexportconfigtypedef)
- [ScalingConfigurationInputTypeDef](./type_defs.md#scalingconfigurationinputtypedef)
- [ScalingConfigurationOutputTypeDef](./type_defs.md#scalingconfigurationoutputtypedef)
- [VpcConfigUnionTypeDef](./type_defs.md#vpcconfiguniontypedef)
- [ProjectBuildBatchConfigUnionTypeDef](./type_defs.md#projectbuildbatchconfiguniontypedef)
- [BuildGroupTypeDef](./type_defs.md#buildgrouptypedef)
- [CreateWebhookOutputTypeDef](./type_defs.md#createwebhookoutputtypedef)
- [UpdateWebhookOutputTypeDef](./type_defs.md#updatewebhookoutputtypedef)
- [EnvironmentPlatformTypeDef](./type_defs.md#environmentplatformtypedef)
- [ProxyConfigurationUnionTypeDef](./type_defs.md#proxyconfigurationuniontypedef)
- [ProjectEnvironmentUnionTypeDef](./type_defs.md#projectenvironmentuniontypedef)
- [BuildTypeDef](./type_defs.md#buildtypedef)
- [ProjectTypeDef](./type_defs.md#projecttypedef)
- [StartBuildInputTypeDef](./type_defs.md#startbuildinputtypedef)
- [CreateReportGroupInputTypeDef](./type_defs.md#createreportgroupinputtypedef)
- [ReportGroupTypeDef](./type_defs.md#reportgrouptypedef)
- [ReportTypeDef](./type_defs.md#reporttypedef)
- [UpdateReportGroupInputTypeDef](./type_defs.md#updatereportgroupinputtypedef)
- [FleetTypeDef](./type_defs.md#fleettypedef)
- [StartBuildBatchInputTypeDef](./type_defs.md#startbuildbatchinputtypedef)
- [BuildBatchTypeDef](./type_defs.md#buildbatchtypedef)
- [ListCuratedEnvironmentImagesOutputTypeDef](./type_defs.md#listcuratedenvironmentimagesoutputtypedef)
- [CreateFleetInputTypeDef](./type_defs.md#createfleetinputtypedef)
- [UpdateFleetInputTypeDef](./type_defs.md#updatefleetinputtypedef)
- [CreateProjectInputTypeDef](./type_defs.md#createprojectinputtypedef)
- [UpdateProjectInputTypeDef](./type_defs.md#updateprojectinputtypedef)
- [BatchGetBuildsOutputTypeDef](./type_defs.md#batchgetbuildsoutputtypedef)
- [RetryBuildOutputTypeDef](./type_defs.md#retrybuildoutputtypedef)
- [StartBuildOutputTypeDef](./type_defs.md#startbuildoutputtypedef)
- [StopBuildOutputTypeDef](./type_defs.md#stopbuildoutputtypedef)
- [BatchGetProjectsOutputTypeDef](./type_defs.md#batchgetprojectsoutputtypedef)
- [CreateProjectOutputTypeDef](./type_defs.md#createprojectoutputtypedef)
- [UpdateProjectOutputTypeDef](./type_defs.md#updateprojectoutputtypedef)
- [BatchGetReportGroupsOutputTypeDef](./type_defs.md#batchgetreportgroupsoutputtypedef)
- [CreateReportGroupOutputTypeDef](./type_defs.md#createreportgroupoutputtypedef)
- [UpdateReportGroupOutputTypeDef](./type_defs.md#updatereportgroupoutputtypedef)
- [BatchGetReportsOutputTypeDef](./type_defs.md#batchgetreportsoutputtypedef)
- [BatchGetFleetsOutputTypeDef](./type_defs.md#batchgetfleetsoutputtypedef)
- [CreateFleetOutputTypeDef](./type_defs.md#createfleetoutputtypedef)
- [UpdateFleetOutputTypeDef](./type_defs.md#updatefleetoutputtypedef)
- [BatchGetBuildBatchesOutputTypeDef](./type_defs.md#batchgetbuildbatchesoutputtypedef)
- [RetryBuildBatchOutputTypeDef](./type_defs.md#retrybuildbatchoutputtypedef)
- [StartBuildBatchOutputTypeDef](./type_defs.md#startbuildbatchoutputtypedef)
- [StopBuildBatchOutputTypeDef](./type_defs.md#stopbuildbatchoutputtypedef)

