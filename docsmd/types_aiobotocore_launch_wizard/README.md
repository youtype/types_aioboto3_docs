# LaunchWizard module

> [Index](../README.md) > LaunchWizard


!!! note ""

    Auto-generated documentation for [LaunchWizard](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#launchwizard)
    type annotations stubs module [types-aiobotocore-launch-wizard](https://pypi.org/project/types-aiobotocore-launch-wizard/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `LaunchWizard` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `LaunchWizard` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[launch-wizard]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[launch-wizard]'

# standalone installation
python -m pip install types-aiobotocore-launch-wizard
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-launch-wizard
```

## Usage

Code samples can be found in [Examples](./usage.md).

## LaunchWizardClient

Type annotations and code completion for  `#!python session.client("launch-wizard")` as [LaunchWizardClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client)

```python
# LaunchWizardClient usage example

from aioboto3.session import Session

from types_aiobotocore_launch_wizard.client import LaunchWizardClient


session = Session()
async with session.client("launch-wizard") as client:
    client: LaunchWizardClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("launch-wizard").get_paginator("...")`.

```python
# ListDeploymentEventsPaginator usage example

from types_aiobotocore_launch_wizard.paginator import ListDeploymentEventsPaginator

def get_list_deployment_events_paginator() -> ListDeploymentEventsPaginator:
    return client.get_paginator("list_deployment_events"))
```

- [ListDeploymentEventsPaginator](./paginators.md#listdeploymenteventspaginator)
- [ListDeploymentsPaginator](./paginators.md#listdeploymentspaginator)
- [ListWorkloadDeploymentPatternsPaginator](./paginators.md#listworkloaddeploymentpatternspaginator)
- [ListWorkloadsPaginator](./paginators.md#listworkloadspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DeploymentFilterKeyType usage example

from types_aiobotocore_launch_wizard.literals import DeploymentFilterKeyType

def get_value() -> DeploymentFilterKeyType:
    return "DEPLOYMENT_STATUS"
```

- [DeploymentFilterKeyType](./literals.md#deploymentfilterkeytype)
- [DeploymentStatusType](./literals.md#deploymentstatustype)
- [EventStatusType](./literals.md#eventstatustype)
- [ListDeploymentEventsPaginatorName](./literals.md#listdeploymenteventspaginatorname)
- [ListDeploymentsPaginatorName](./literals.md#listdeploymentspaginatorname)
- [ListWorkloadDeploymentPatternsPaginatorName](./literals.md#listworkloaddeploymentpatternspaginatorname)
- [ListWorkloadsPaginatorName](./literals.md#listworkloadspaginatorname)
- [WorkloadDeploymentPatternStatusType](./literals.md#workloaddeploymentpatternstatustype)
- [WorkloadStatusType](./literals.md#workloadstatustype)
- [LaunchWizardServiceName](./literals.md#launchwizardservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CreateDeploymentInputRequestTypeDef](./type_defs.md#createdeploymentinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteDeploymentInputRequestTypeDef](./type_defs.md#deletedeploymentinputrequesttypedef)
- [DeploymentConditionalFieldTypeDef](./type_defs.md#deploymentconditionalfieldtypedef)
- [DeploymentDataSummaryTypeDef](./type_defs.md#deploymentdatasummarytypedef)
- [DeploymentDataTypeDef](./type_defs.md#deploymentdatatypedef)
- [DeploymentEventDataSummaryTypeDef](./type_defs.md#deploymenteventdatasummarytypedef)
- [DeploymentFilterTypeDef](./type_defs.md#deploymentfiltertypedef)
- [GetDeploymentInputRequestTypeDef](./type_defs.md#getdeploymentinputrequesttypedef)
- [GetWorkloadDeploymentPatternInputRequestTypeDef](./type_defs.md#getworkloaddeploymentpatterninputrequesttypedef)
- [GetWorkloadInputRequestTypeDef](./type_defs.md#getworkloadinputrequesttypedef)
- [WorkloadDataTypeDef](./type_defs.md#workloaddatatypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListDeploymentEventsInputRequestTypeDef](./type_defs.md#listdeploymenteventsinputrequesttypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [ListWorkloadDeploymentPatternsInputRequestTypeDef](./type_defs.md#listworkloaddeploymentpatternsinputrequesttypedef)
- [WorkloadDeploymentPatternDataSummaryTypeDef](./type_defs.md#workloaddeploymentpatterndatasummarytypedef)
- [ListWorkloadsInputRequestTypeDef](./type_defs.md#listworkloadsinputrequesttypedef)
- [WorkloadDataSummaryTypeDef](./type_defs.md#workloaddatasummarytypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [CreateDeploymentOutputTypeDef](./type_defs.md#createdeploymentoutputtypedef)
- [DeleteDeploymentOutputTypeDef](./type_defs.md#deletedeploymentoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [DeploymentSpecificationsFieldTypeDef](./type_defs.md#deploymentspecificationsfieldtypedef)
- [ListDeploymentsOutputTypeDef](./type_defs.md#listdeploymentsoutputtypedef)
- [GetDeploymentOutputTypeDef](./type_defs.md#getdeploymentoutputtypedef)
- [ListDeploymentEventsOutputTypeDef](./type_defs.md#listdeploymenteventsoutputtypedef)
- [ListDeploymentsInputRequestTypeDef](./type_defs.md#listdeploymentsinputrequesttypedef)
- [GetWorkloadOutputTypeDef](./type_defs.md#getworkloadoutputtypedef)
- [ListDeploymentEventsInputPaginateTypeDef](./type_defs.md#listdeploymenteventsinputpaginatetypedef)
- [ListDeploymentsInputPaginateTypeDef](./type_defs.md#listdeploymentsinputpaginatetypedef)
- [ListWorkloadDeploymentPatternsInputPaginateTypeDef](./type_defs.md#listworkloaddeploymentpatternsinputpaginatetypedef)
- [ListWorkloadsInputPaginateTypeDef](./type_defs.md#listworkloadsinputpaginatetypedef)
- [ListWorkloadDeploymentPatternsOutputTypeDef](./type_defs.md#listworkloaddeploymentpatternsoutputtypedef)
- [ListWorkloadsOutputTypeDef](./type_defs.md#listworkloadsoutputtypedef)
- [WorkloadDeploymentPatternDataTypeDef](./type_defs.md#workloaddeploymentpatterndatatypedef)
- [GetWorkloadDeploymentPatternOutputTypeDef](./type_defs.md#getworkloaddeploymentpatternoutputtypedef)
