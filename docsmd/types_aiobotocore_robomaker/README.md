# RoboMaker module

> [Index](../README.md) > RoboMaker


!!! note ""

    Auto-generated documentation for [RoboMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#robomaker)
    type annotations stubs module [types-aiobotocore-robomaker](https://pypi.org/project/types-aiobotocore-robomaker/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `RoboMaker` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `RoboMaker` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[robomaker]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[robomaker]'

# standalone installation
python -m pip install types-aiobotocore-robomaker
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-robomaker
```

## Usage

Code samples can be found in [Examples](./usage.md).

## RoboMakerClient

Type annotations and code completion for  `#!python session.client("robomaker")` as [RoboMakerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client)

```python
# RoboMakerClient usage example

from aioboto3.session import Session

from types_aiobotocore_robomaker.client import RoboMakerClient


session = Session()
async with session.client("robomaker") as client:
    client: RoboMakerClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("robomaker").get_paginator("...")`.

```python
# ListDeploymentJobsPaginator usage example

from types_aiobotocore_robomaker.paginator import ListDeploymentJobsPaginator

def get_list_deployment_jobs_paginator() -> ListDeploymentJobsPaginator:
    return client.get_paginator("list_deployment_jobs"))
```

- [ListDeploymentJobsPaginator](./paginators.md#listdeploymentjobspaginator)
- [ListFleetsPaginator](./paginators.md#listfleetspaginator)
- [ListRobotApplicationsPaginator](./paginators.md#listrobotapplicationspaginator)
- [ListRobotsPaginator](./paginators.md#listrobotspaginator)
- [ListSimulationApplicationsPaginator](./paginators.md#listsimulationapplicationspaginator)
- [ListSimulationJobBatchesPaginator](./paginators.md#listsimulationjobbatchespaginator)
- [ListSimulationJobsPaginator](./paginators.md#listsimulationjobspaginator)
- [ListWorldExportJobsPaginator](./paginators.md#listworldexportjobspaginator)
- [ListWorldGenerationJobsPaginator](./paginators.md#listworldgenerationjobspaginator)
- [ListWorldTemplatesPaginator](./paginators.md#listworldtemplatespaginator)
- [ListWorldsPaginator](./paginators.md#listworldspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ArchitectureType usage example

from types_aiobotocore_robomaker.literals import ArchitectureType

def get_value() -> ArchitectureType:
    return "ARM64"
```

- [ArchitectureType](./literals.md#architecturetype)
- [ComputeTypeType](./literals.md#computetypetype)
- [DataSourceTypeType](./literals.md#datasourcetypetype)
- [DeploymentJobErrorCodeType](./literals.md#deploymentjoberrorcodetype)
- [DeploymentStatusType](./literals.md#deploymentstatustype)
- [ExitBehaviorType](./literals.md#exitbehaviortype)
- [FailureBehaviorType](./literals.md#failurebehaviortype)
- [ListDeploymentJobsPaginatorName](./literals.md#listdeploymentjobspaginatorname)
- [ListFleetsPaginatorName](./literals.md#listfleetspaginatorname)
- [ListRobotApplicationsPaginatorName](./literals.md#listrobotapplicationspaginatorname)
- [ListRobotsPaginatorName](./literals.md#listrobotspaginatorname)
- [ListSimulationApplicationsPaginatorName](./literals.md#listsimulationapplicationspaginatorname)
- [ListSimulationJobBatchesPaginatorName](./literals.md#listsimulationjobbatchespaginatorname)
- [ListSimulationJobsPaginatorName](./literals.md#listsimulationjobspaginatorname)
- [ListWorldExportJobsPaginatorName](./literals.md#listworldexportjobspaginatorname)
- [ListWorldGenerationJobsPaginatorName](./literals.md#listworldgenerationjobspaginatorname)
- [ListWorldTemplatesPaginatorName](./literals.md#listworldtemplatespaginatorname)
- [ListWorldsPaginatorName](./literals.md#listworldspaginatorname)
- [RenderingEngineTypeType](./literals.md#renderingenginetypetype)
- [RobotDeploymentStepType](./literals.md#robotdeploymentsteptype)
- [RobotSoftwareSuiteTypeType](./literals.md#robotsoftwaresuitetypetype)
- [RobotSoftwareSuiteVersionTypeType](./literals.md#robotsoftwaresuiteversiontypetype)
- [RobotStatusType](./literals.md#robotstatustype)
- [SimulationJobBatchErrorCodeType](./literals.md#simulationjobbatcherrorcodetype)
- [SimulationJobBatchStatusType](./literals.md#simulationjobbatchstatustype)
- [SimulationJobErrorCodeType](./literals.md#simulationjoberrorcodetype)
- [SimulationJobStatusType](./literals.md#simulationjobstatustype)
- [SimulationSoftwareSuiteTypeType](./literals.md#simulationsoftwaresuitetypetype)
- [UploadBehaviorType](./literals.md#uploadbehaviortype)
- [WorldExportJobErrorCodeType](./literals.md#worldexportjoberrorcodetype)
- [WorldExportJobStatusType](./literals.md#worldexportjobstatustype)
- [WorldGenerationJobErrorCodeType](./literals.md#worldgenerationjoberrorcodetype)
- [WorldGenerationJobStatusType](./literals.md#worldgenerationjobstatustype)
- [RoboMakerServiceName](./literals.md#robomakerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BatchDeleteWorldsRequestRequestTypeDef](./type_defs.md#batchdeleteworldsrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BatchDescribeSimulationJobRequestRequestTypeDef](./type_defs.md#batchdescribesimulationjobrequestrequesttypedef)
- [BatchPolicyTypeDef](./type_defs.md#batchpolicytypedef)
- [CancelDeploymentJobRequestRequestTypeDef](./type_defs.md#canceldeploymentjobrequestrequesttypedef)
- [CancelSimulationJobBatchRequestRequestTypeDef](./type_defs.md#cancelsimulationjobbatchrequestrequesttypedef)
- [CancelSimulationJobRequestRequestTypeDef](./type_defs.md#cancelsimulationjobrequestrequesttypedef)
- [CancelWorldExportJobRequestRequestTypeDef](./type_defs.md#cancelworldexportjobrequestrequesttypedef)
- [CancelWorldGenerationJobRequestRequestTypeDef](./type_defs.md#cancelworldgenerationjobrequestrequesttypedef)
- [ComputeResponseTypeDef](./type_defs.md#computeresponsetypedef)
- [ComputeTypeDef](./type_defs.md#computetypedef)
- [CreateFleetRequestRequestTypeDef](./type_defs.md#createfleetrequestrequesttypedef)
- [EnvironmentTypeDef](./type_defs.md#environmenttypedef)
- [RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef)
- [SourceConfigTypeDef](./type_defs.md#sourceconfigtypedef)
- [SourceTypeDef](./type_defs.md#sourcetypedef)
- [CreateRobotApplicationVersionRequestRequestTypeDef](./type_defs.md#createrobotapplicationversionrequestrequesttypedef)
- [CreateRobotRequestRequestTypeDef](./type_defs.md#createrobotrequestrequesttypedef)
- [RenderingEngineTypeDef](./type_defs.md#renderingenginetypedef)
- [SimulationSoftwareSuiteTypeDef](./type_defs.md#simulationsoftwaresuitetypedef)
- [CreateSimulationApplicationVersionRequestRequestTypeDef](./type_defs.md#createsimulationapplicationversionrequestrequesttypedef)
- [LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef)
- [OutputLocationTypeDef](./type_defs.md#outputlocationtypedef)
- [VPCConfigTypeDef](./type_defs.md#vpcconfigtypedef)
- [VPCConfigResponseTypeDef](./type_defs.md#vpcconfigresponsetypedef)
- [WorldCountTypeDef](./type_defs.md#worldcounttypedef)
- [TemplateLocationTypeDef](./type_defs.md#templatelocationtypedef)
- [DataSourceConfigOutputTypeDef](./type_defs.md#datasourceconfigoutputtypedef)
- [DataSourceConfigTypeDef](./type_defs.md#datasourceconfigtypedef)
- [S3KeyOutputTypeDef](./type_defs.md#s3keyoutputtypedef)
- [DeleteFleetRequestRequestTypeDef](./type_defs.md#deletefleetrequestrequesttypedef)
- [DeleteRobotApplicationRequestRequestTypeDef](./type_defs.md#deleterobotapplicationrequestrequesttypedef)
- [DeleteRobotRequestRequestTypeDef](./type_defs.md#deleterobotrequestrequesttypedef)
- [DeleteSimulationApplicationRequestRequestTypeDef](./type_defs.md#deletesimulationapplicationrequestrequesttypedef)
- [DeleteWorldTemplateRequestRequestTypeDef](./type_defs.md#deleteworldtemplaterequestrequesttypedef)
- [DeploymentLaunchConfigOutputTypeDef](./type_defs.md#deploymentlaunchconfigoutputtypedef)
- [S3ObjectTypeDef](./type_defs.md#s3objecttypedef)
- [DeploymentLaunchConfigTypeDef](./type_defs.md#deploymentlaunchconfigtypedef)
- [DeregisterRobotRequestRequestTypeDef](./type_defs.md#deregisterrobotrequestrequesttypedef)
- [DescribeDeploymentJobRequestRequestTypeDef](./type_defs.md#describedeploymentjobrequestrequesttypedef)
- [DescribeFleetRequestRequestTypeDef](./type_defs.md#describefleetrequestrequesttypedef)
- [RobotTypeDef](./type_defs.md#robottypedef)
- [DescribeRobotApplicationRequestRequestTypeDef](./type_defs.md#describerobotapplicationrequestrequesttypedef)
- [DescribeRobotRequestRequestTypeDef](./type_defs.md#describerobotrequestrequesttypedef)
- [DescribeSimulationApplicationRequestRequestTypeDef](./type_defs.md#describesimulationapplicationrequestrequesttypedef)
- [DescribeSimulationJobBatchRequestRequestTypeDef](./type_defs.md#describesimulationjobbatchrequestrequesttypedef)
- [SimulationJobSummaryTypeDef](./type_defs.md#simulationjobsummarytypedef)
- [DescribeSimulationJobRequestRequestTypeDef](./type_defs.md#describesimulationjobrequestrequesttypedef)
- [NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef)
- [DescribeWorldExportJobRequestRequestTypeDef](./type_defs.md#describeworldexportjobrequestrequesttypedef)
- [DescribeWorldGenerationJobRequestRequestTypeDef](./type_defs.md#describeworldgenerationjobrequestrequesttypedef)
- [DescribeWorldRequestRequestTypeDef](./type_defs.md#describeworldrequestrequesttypedef)
- [DescribeWorldTemplateRequestRequestTypeDef](./type_defs.md#describeworldtemplaterequestrequesttypedef)
- [WorldFailureTypeDef](./type_defs.md#worldfailuretypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [FleetTypeDef](./type_defs.md#fleettypedef)
- [GetWorldTemplateBodyRequestRequestTypeDef](./type_defs.md#getworldtemplatebodyrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [SimulationJobBatchSummaryTypeDef](./type_defs.md#simulationjobbatchsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListWorldTemplatesRequestRequestTypeDef](./type_defs.md#listworldtemplatesrequestrequesttypedef)
- [TemplateSummaryTypeDef](./type_defs.md#templatesummarytypedef)
- [WorldSummaryTypeDef](./type_defs.md#worldsummarytypedef)
- [PortMappingTypeDef](./type_defs.md#portmappingtypedef)
- [ProgressDetailTypeDef](./type_defs.md#progressdetailtypedef)
- [RegisterRobotRequestRequestTypeDef](./type_defs.md#registerrobotrequestrequesttypedef)
- [RestartSimulationJobRequestRequestTypeDef](./type_defs.md#restartsimulationjobrequestrequesttypedef)
- [ToolTypeDef](./type_defs.md#tooltypedef)
- [UploadConfigurationTypeDef](./type_defs.md#uploadconfigurationtypedef)
- [WorldConfigTypeDef](./type_defs.md#worldconfigtypedef)
- [VPCConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef)
- [SyncDeploymentJobRequestRequestTypeDef](./type_defs.md#syncdeploymentjobrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [BatchDeleteWorldsResponseTypeDef](./type_defs.md#batchdeleteworldsresponsetypedef)
- [CreateFleetResponseTypeDef](./type_defs.md#createfleetresponsetypedef)
- [CreateRobotResponseTypeDef](./type_defs.md#createrobotresponsetypedef)
- [CreateWorldTemplateResponseTypeDef](./type_defs.md#createworldtemplateresponsetypedef)
- [DeregisterRobotResponseTypeDef](./type_defs.md#deregisterrobotresponsetypedef)
- [DescribeRobotResponseTypeDef](./type_defs.md#describerobotresponsetypedef)
- [DescribeWorldResponseTypeDef](./type_defs.md#describeworldresponsetypedef)
- [DescribeWorldTemplateResponseTypeDef](./type_defs.md#describeworldtemplateresponsetypedef)
- [GetWorldTemplateBodyResponseTypeDef](./type_defs.md#getworldtemplatebodyresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [RegisterRobotResponseTypeDef](./type_defs.md#registerrobotresponsetypedef)
- [UpdateWorldTemplateResponseTypeDef](./type_defs.md#updateworldtemplateresponsetypedef)
- [RobotApplicationSummaryTypeDef](./type_defs.md#robotapplicationsummarytypedef)
- [CreateRobotApplicationRequestRequestTypeDef](./type_defs.md#createrobotapplicationrequestrequesttypedef)
- [UpdateRobotApplicationRequestRequestTypeDef](./type_defs.md#updaterobotapplicationrequestrequesttypedef)
- [CreateRobotApplicationResponseTypeDef](./type_defs.md#createrobotapplicationresponsetypedef)
- [CreateRobotApplicationVersionResponseTypeDef](./type_defs.md#createrobotapplicationversionresponsetypedef)
- [DescribeRobotApplicationResponseTypeDef](./type_defs.md#describerobotapplicationresponsetypedef)
- [UpdateRobotApplicationResponseTypeDef](./type_defs.md#updaterobotapplicationresponsetypedef)
- [CreateSimulationApplicationRequestRequestTypeDef](./type_defs.md#createsimulationapplicationrequestrequesttypedef)
- [CreateSimulationApplicationResponseTypeDef](./type_defs.md#createsimulationapplicationresponsetypedef)
- [CreateSimulationApplicationVersionResponseTypeDef](./type_defs.md#createsimulationapplicationversionresponsetypedef)
- [DescribeSimulationApplicationResponseTypeDef](./type_defs.md#describesimulationapplicationresponsetypedef)
- [SimulationApplicationSummaryTypeDef](./type_defs.md#simulationapplicationsummarytypedef)
- [UpdateSimulationApplicationRequestRequestTypeDef](./type_defs.md#updatesimulationapplicationrequestrequesttypedef)
- [UpdateSimulationApplicationResponseTypeDef](./type_defs.md#updatesimulationapplicationresponsetypedef)
- [CreateWorldExportJobRequestRequestTypeDef](./type_defs.md#createworldexportjobrequestrequesttypedef)
- [CreateWorldExportJobResponseTypeDef](./type_defs.md#createworldexportjobresponsetypedef)
- [DescribeWorldExportJobResponseTypeDef](./type_defs.md#describeworldexportjobresponsetypedef)
- [WorldExportJobSummaryTypeDef](./type_defs.md#worldexportjobsummarytypedef)
- [CreateWorldGenerationJobRequestRequestTypeDef](./type_defs.md#createworldgenerationjobrequestrequesttypedef)
- [CreateWorldGenerationJobResponseTypeDef](./type_defs.md#createworldgenerationjobresponsetypedef)
- [WorldGenerationJobSummaryTypeDef](./type_defs.md#worldgenerationjobsummarytypedef)
- [CreateWorldTemplateRequestRequestTypeDef](./type_defs.md#createworldtemplaterequestrequesttypedef)
- [UpdateWorldTemplateRequestRequestTypeDef](./type_defs.md#updateworldtemplaterequestrequesttypedef)
- [DataSourceConfigUnionTypeDef](./type_defs.md#datasourceconfiguniontypedef)
- [DataSourceTypeDef](./type_defs.md#datasourcetypedef)
- [DeploymentApplicationConfigOutputTypeDef](./type_defs.md#deploymentapplicationconfigoutputtypedef)
- [DeploymentConfigTypeDef](./type_defs.md#deploymentconfigtypedef)
- [DeploymentLaunchConfigUnionTypeDef](./type_defs.md#deploymentlaunchconfiguniontypedef)
- [DescribeFleetResponseTypeDef](./type_defs.md#describefleetresponsetypedef)
- [ListRobotsResponseTypeDef](./type_defs.md#listrobotsresponsetypedef)
- [ListSimulationJobsResponseTypeDef](./type_defs.md#listsimulationjobsresponsetypedef)
- [FailureSummaryTypeDef](./type_defs.md#failuresummarytypedef)
- [ListDeploymentJobsRequestRequestTypeDef](./type_defs.md#listdeploymentjobsrequestrequesttypedef)
- [ListFleetsRequestRequestTypeDef](./type_defs.md#listfleetsrequestrequesttypedef)
- [ListRobotApplicationsRequestRequestTypeDef](./type_defs.md#listrobotapplicationsrequestrequesttypedef)
- [ListRobotsRequestRequestTypeDef](./type_defs.md#listrobotsrequestrequesttypedef)
- [ListSimulationApplicationsRequestRequestTypeDef](./type_defs.md#listsimulationapplicationsrequestrequesttypedef)
- [ListSimulationJobBatchesRequestRequestTypeDef](./type_defs.md#listsimulationjobbatchesrequestrequesttypedef)
- [ListSimulationJobsRequestRequestTypeDef](./type_defs.md#listsimulationjobsrequestrequesttypedef)
- [ListWorldExportJobsRequestRequestTypeDef](./type_defs.md#listworldexportjobsrequestrequesttypedef)
- [ListWorldGenerationJobsRequestRequestTypeDef](./type_defs.md#listworldgenerationjobsrequestrequesttypedef)
- [ListWorldsRequestRequestTypeDef](./type_defs.md#listworldsrequestrequesttypedef)
- [ListFleetsResponseTypeDef](./type_defs.md#listfleetsresponsetypedef)
- [ListDeploymentJobsRequestPaginateTypeDef](./type_defs.md#listdeploymentjobsrequestpaginatetypedef)
- [ListFleetsRequestPaginateTypeDef](./type_defs.md#listfleetsrequestpaginatetypedef)
- [ListRobotApplicationsRequestPaginateTypeDef](./type_defs.md#listrobotapplicationsrequestpaginatetypedef)
- [ListRobotsRequestPaginateTypeDef](./type_defs.md#listrobotsrequestpaginatetypedef)
- [ListSimulationApplicationsRequestPaginateTypeDef](./type_defs.md#listsimulationapplicationsrequestpaginatetypedef)
- [ListSimulationJobBatchesRequestPaginateTypeDef](./type_defs.md#listsimulationjobbatchesrequestpaginatetypedef)
- [ListSimulationJobsRequestPaginateTypeDef](./type_defs.md#listsimulationjobsrequestpaginatetypedef)
- [ListWorldExportJobsRequestPaginateTypeDef](./type_defs.md#listworldexportjobsrequestpaginatetypedef)
- [ListWorldGenerationJobsRequestPaginateTypeDef](./type_defs.md#listworldgenerationjobsrequestpaginatetypedef)
- [ListWorldTemplatesRequestPaginateTypeDef](./type_defs.md#listworldtemplatesrequestpaginatetypedef)
- [ListWorldsRequestPaginateTypeDef](./type_defs.md#listworldsrequestpaginatetypedef)
- [ListSimulationJobBatchesResponseTypeDef](./type_defs.md#listsimulationjobbatchesresponsetypedef)
- [ListWorldTemplatesResponseTypeDef](./type_defs.md#listworldtemplatesresponsetypedef)
- [ListWorldsResponseTypeDef](./type_defs.md#listworldsresponsetypedef)
- [PortForwardingConfigOutputTypeDef](./type_defs.md#portforwardingconfigoutputtypedef)
- [PortForwardingConfigTypeDef](./type_defs.md#portforwardingconfigtypedef)
- [RobotDeploymentTypeDef](./type_defs.md#robotdeploymenttypedef)
- [VPCConfigUnionTypeDef](./type_defs.md#vpcconfiguniontypedef)
- [ListRobotApplicationsResponseTypeDef](./type_defs.md#listrobotapplicationsresponsetypedef)
- [ListSimulationApplicationsResponseTypeDef](./type_defs.md#listsimulationapplicationsresponsetypedef)
- [ListWorldExportJobsResponseTypeDef](./type_defs.md#listworldexportjobsresponsetypedef)
- [ListWorldGenerationJobsResponseTypeDef](./type_defs.md#listworldgenerationjobsresponsetypedef)
- [CreateDeploymentJobResponseTypeDef](./type_defs.md#createdeploymentjobresponsetypedef)
- [DeploymentJobTypeDef](./type_defs.md#deploymentjobtypedef)
- [SyncDeploymentJobResponseTypeDef](./type_defs.md#syncdeploymentjobresponsetypedef)
- [DeploymentApplicationConfigTypeDef](./type_defs.md#deploymentapplicationconfigtypedef)
- [FinishedWorldsSummaryTypeDef](./type_defs.md#finishedworldssummarytypedef)
- [LaunchConfigOutputTypeDef](./type_defs.md#launchconfigoutputtypedef)
- [PortForwardingConfigUnionTypeDef](./type_defs.md#portforwardingconfiguniontypedef)
- [DescribeDeploymentJobResponseTypeDef](./type_defs.md#describedeploymentjobresponsetypedef)
- [ListDeploymentJobsResponseTypeDef](./type_defs.md#listdeploymentjobsresponsetypedef)
- [DeploymentApplicationConfigUnionTypeDef](./type_defs.md#deploymentapplicationconfiguniontypedef)
- [DescribeWorldGenerationJobResponseTypeDef](./type_defs.md#describeworldgenerationjobresponsetypedef)
- [RobotApplicationConfigOutputTypeDef](./type_defs.md#robotapplicationconfigoutputtypedef)
- [SimulationApplicationConfigOutputTypeDef](./type_defs.md#simulationapplicationconfigoutputtypedef)
- [LaunchConfigTypeDef](./type_defs.md#launchconfigtypedef)
- [CreateDeploymentJobRequestRequestTypeDef](./type_defs.md#createdeploymentjobrequestrequesttypedef)
- [CreateSimulationJobResponseTypeDef](./type_defs.md#createsimulationjobresponsetypedef)
- [DescribeSimulationJobResponseTypeDef](./type_defs.md#describesimulationjobresponsetypedef)
- [SimulationJobRequestOutputTypeDef](./type_defs.md#simulationjobrequestoutputtypedef)
- [SimulationJobTypeDef](./type_defs.md#simulationjobtypedef)
- [LaunchConfigUnionTypeDef](./type_defs.md#launchconfiguniontypedef)
- [FailedCreateSimulationJobRequestTypeDef](./type_defs.md#failedcreatesimulationjobrequesttypedef)
- [BatchDescribeSimulationJobResponseTypeDef](./type_defs.md#batchdescribesimulationjobresponsetypedef)
- [RobotApplicationConfigTypeDef](./type_defs.md#robotapplicationconfigtypedef)
- [SimulationApplicationConfigTypeDef](./type_defs.md#simulationapplicationconfigtypedef)
- [DescribeSimulationJobBatchResponseTypeDef](./type_defs.md#describesimulationjobbatchresponsetypedef)
- [StartSimulationJobBatchResponseTypeDef](./type_defs.md#startsimulationjobbatchresponsetypedef)
- [RobotApplicationConfigUnionTypeDef](./type_defs.md#robotapplicationconfiguniontypedef)
- [SimulationApplicationConfigUnionTypeDef](./type_defs.md#simulationapplicationconfiguniontypedef)
- [CreateSimulationJobRequestRequestTypeDef](./type_defs.md#createsimulationjobrequestrequesttypedef)
- [SimulationJobRequestTypeDef](./type_defs.md#simulationjobrequesttypedef)
- [SimulationJobRequestUnionTypeDef](./type_defs.md#simulationjobrequestuniontypedef)
- [StartSimulationJobBatchRequestRequestTypeDef](./type_defs.md#startsimulationjobbatchrequestrequesttypedef)
