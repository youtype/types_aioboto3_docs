# ECSClient

> [Index](../README.md) > [ECS](./README.md) > ECSClient

!!! note ""

    Auto-generated documentation for [ECS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ecs)
    type annotations stubs module [types-aiobotocore-ecs](https://pypi.org/project/types-aiobotocore-ecs/).

## ECSClient

Type annotations and code completion for `#!python session.client("ecs")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# ECSClient usage example

from aioboto3.session import Session
from types_aiobotocore_ecs.client import ECSClient

session = Session()
async with session.client("ecs") as client:
    client: ECSClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("ecs").exceptions` structure.

```python
# ECSClient.exceptions usage example

async with session.client("ecs") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.AttributeLimitExceededException,
        client.exceptions.BlockedException,
        client.exceptions.ClientError,
        client.exceptions.ClientException,
        client.exceptions.ClusterContainsContainerInstancesException,
        client.exceptions.ClusterContainsServicesException,
        client.exceptions.ClusterContainsTasksException,
        client.exceptions.ClusterNotFoundException,
        client.exceptions.ConflictException,
        client.exceptions.InvalidParameterException,
        client.exceptions.LimitExceededException,
        client.exceptions.MissingVersionException,
        client.exceptions.NamespaceNotFoundException,
        client.exceptions.NoUpdateAvailableException,
        client.exceptions.PlatformTaskDefinitionIncompatibilityException,
        client.exceptions.PlatformUnknownException,
        client.exceptions.ResourceInUseException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServerException,
        client.exceptions.ServiceNotActiveException,
        client.exceptions.ServiceNotFoundException,
        client.exceptions.TargetNotConnectedException,
        client.exceptions.TargetNotFoundException,
        client.exceptions.TaskSetNotFoundException,
        client.exceptions.UnsupportedFeatureException,
        client.exceptions.UpdateInProgressException,
    ) as e:
        print(e)
```

```python
# ECSClient.exceptions type checking example

from types_aiobotocore_ecs.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("ecs").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("ecs").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### create\_capacity\_provider

Creates a new capacity provider.

Type annotations and code completion for `#!python session.client("ecs").create_capacity_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# create_capacity_provider method definition

await def create_capacity_provider(
    self,
    *,
    name: str,
    autoScalingGroupProvider: AutoScalingGroupProviderTypeDef,  # (1)
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateCapacityProviderResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AutoScalingGroupProviderTypeDef](./type_defs.md#autoscalinggroupprovidertypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateCapacityProviderResponseTypeDef](./type_defs.md#createcapacityproviderresponsetypedef) 


```python
# create_capacity_provider method usage example with argument unpacking

kwargs: CreateCapacityProviderRequestRequestTypeDef = {  # (1)
    "name": ...,
    "autoScalingGroupProvider": ...,
}

parent.create_capacity_provider(**kwargs)
```

1. See [:material-code-braces: CreateCapacityProviderRequestRequestTypeDef](./type_defs.md#createcapacityproviderrequestrequesttypedef) 

### create\_cluster

Creates a new Amazon ECS cluster.

Type annotations and code completion for `#!python session.client("ecs").create_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# create_cluster method definition

await def create_cluster(
    self,
    *,
    clusterName: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (1)
    settings: Sequence[ClusterSettingTypeDef] = ...,  # (2)
    configuration: ClusterConfigurationTypeDef = ...,  # (3)
    capacityProviders: Sequence[str] = ...,
    defaultCapacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,  # (4)
    serviceConnectDefaults: ClusterServiceConnectDefaultsRequestTypeDef = ...,  # (5)
) -> CreateClusterResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ClusterSettingTypeDef](./type_defs.md#clustersettingtypedef) 
3. See [:material-code-braces: ClusterConfigurationTypeDef](./type_defs.md#clusterconfigurationtypedef) 
4. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
5. See [:material-code-braces: ClusterServiceConnectDefaultsRequestTypeDef](./type_defs.md#clusterserviceconnectdefaultsrequesttypedef) 
6. See [:material-code-braces: CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef) 


```python
# create_cluster method usage example with argument unpacking

kwargs: CreateClusterRequestRequestTypeDef = {  # (1)
    "clusterName": ...,
}

parent.create_cluster(**kwargs)
```

1. See [:material-code-braces: CreateClusterRequestRequestTypeDef](./type_defs.md#createclusterrequestrequesttypedef) 

### create\_service

Runs and maintains your desired number of tasks from a specified task
definition.

Type annotations and code completion for `#!python session.client("ecs").create_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# create_service method definition

await def create_service(
    self,
    *,
    serviceName: str,
    cluster: str = ...,
    taskDefinition: str = ...,
    availabilityZoneRebalancing: AvailabilityZoneRebalancingType = ...,  # (1)
    loadBalancers: Sequence[LoadBalancerTypeDef] = ...,  # (2)
    serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,  # (3)
    desiredCount: int = ...,
    clientToken: str = ...,
    launchType: LaunchTypeType = ...,  # (4)
    capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,  # (5)
    platformVersion: str = ...,
    role: str = ...,
    deploymentConfiguration: DeploymentConfigurationTypeDef = ...,  # (6)
    placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,  # (7)
    placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,  # (8)
    networkConfiguration: NetworkConfigurationTypeDef = ...,  # (9)
    healthCheckGracePeriodSeconds: int = ...,
    schedulingStrategy: SchedulingStrategyType = ...,  # (10)
    deploymentController: DeploymentControllerTypeDef = ...,  # (11)
    tags: Sequence[TagTypeDef] = ...,  # (12)
    enableECSManagedTags: bool = ...,
    propagateTags: PropagateTagsType = ...,  # (13)
    enableExecuteCommand: bool = ...,
    serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...,  # (14)
    volumeConfigurations: Sequence[ServiceVolumeConfigurationUnionTypeDef] = ...,  # (15)
    vpcLatticeConfigurations: Sequence[VpcLatticeConfigurationTypeDef] = ...,  # (16)
) -> CreateServiceResponseTypeDef:  # (17)
    ...
```

1. See [:material-code-brackets: AvailabilityZoneRebalancingType](./literals.md#availabilityzonerebalancingtype) 
2. See [:material-code-braces: LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef) 
3. See [:material-code-braces: ServiceRegistryTypeDef](./type_defs.md#serviceregistrytypedef) 
4. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
5. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
6. See [:material-code-braces: DeploymentConfigurationTypeDef](./type_defs.md#deploymentconfigurationtypedef) 
7. See [:material-code-braces: PlacementConstraintTypeDef](./type_defs.md#placementconstrainttypedef) 
8. See [:material-code-braces: PlacementStrategyTypeDef](./type_defs.md#placementstrategytypedef) 
9. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
10. See [:material-code-brackets: SchedulingStrategyType](./literals.md#schedulingstrategytype) 
11. See [:material-code-braces: DeploymentControllerTypeDef](./type_defs.md#deploymentcontrollertypedef) 
12. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
13. See [:material-code-brackets: PropagateTagsType](./literals.md#propagatetagstype) 
14. See [:material-code-braces: ServiceConnectConfigurationTypeDef](./type_defs.md#serviceconnectconfigurationtypedef) 
15. See [:material-code-braces: ServiceVolumeConfigurationTypeDef](./type_defs.md#servicevolumeconfigurationtypedef) [:material-code-braces: ServiceVolumeConfigurationOutputTypeDef](./type_defs.md#servicevolumeconfigurationoutputtypedef) 
16. See [:material-code-braces: VpcLatticeConfigurationTypeDef](./type_defs.md#vpclatticeconfigurationtypedef) 
17. See [:material-code-braces: CreateServiceResponseTypeDef](./type_defs.md#createserviceresponsetypedef) 


```python
# create_service method usage example with argument unpacking

kwargs: CreateServiceRequestRequestTypeDef = {  # (1)
    "serviceName": ...,
}

parent.create_service(**kwargs)
```

1. See [:material-code-braces: CreateServiceRequestRequestTypeDef](./type_defs.md#createservicerequestrequesttypedef) 

### create\_task\_set

Create a task set in the specified cluster and service.

Type annotations and code completion for `#!python session.client("ecs").create_task_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# create_task_set method definition

await def create_task_set(
    self,
    *,
    service: str,
    cluster: str,
    taskDefinition: str,
    externalId: str = ...,
    networkConfiguration: NetworkConfigurationTypeDef = ...,  # (1)
    loadBalancers: Sequence[LoadBalancerTypeDef] = ...,  # (2)
    serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,  # (3)
    launchType: LaunchTypeType = ...,  # (4)
    capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,  # (5)
    platformVersion: str = ...,
    scale: ScaleTypeDef = ...,  # (6)
    clientToken: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (7)
) -> CreateTaskSetResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
2. See [:material-code-braces: LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef) 
3. See [:material-code-braces: ServiceRegistryTypeDef](./type_defs.md#serviceregistrytypedef) 
4. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
5. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
6. See [:material-code-braces: ScaleTypeDef](./type_defs.md#scaletypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
8. See [:material-code-braces: CreateTaskSetResponseTypeDef](./type_defs.md#createtasksetresponsetypedef) 


```python
# create_task_set method usage example with argument unpacking

kwargs: CreateTaskSetRequestRequestTypeDef = {  # (1)
    "service": ...,
    "cluster": ...,
    "taskDefinition": ...,
}

parent.create_task_set(**kwargs)
```

1. See [:material-code-braces: CreateTaskSetRequestRequestTypeDef](./type_defs.md#createtasksetrequestrequesttypedef) 

### delete\_account\_setting

Disables an account setting for a specified user, role, or the root user for an
account.

Type annotations and code completion for `#!python session.client("ecs").delete_account_setting` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# delete_account_setting method definition

await def delete_account_setting(
    self,
    *,
    name: SettingNameType,  # (1)
    principalArn: str = ...,
) -> DeleteAccountSettingResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SettingNameType](./literals.md#settingnametype) 
2. See [:material-code-braces: DeleteAccountSettingResponseTypeDef](./type_defs.md#deleteaccountsettingresponsetypedef) 


```python
# delete_account_setting method usage example with argument unpacking

kwargs: DeleteAccountSettingRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.delete_account_setting(**kwargs)
```

1. See [:material-code-braces: DeleteAccountSettingRequestRequestTypeDef](./type_defs.md#deleteaccountsettingrequestrequesttypedef) 

### delete\_attributes

Deletes one or more custom attributes from an Amazon ECS resource.

Type annotations and code completion for `#!python session.client("ecs").delete_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# delete_attributes method definition

await def delete_attributes(
    self,
    *,
    attributes: Sequence[AttributeTypeDef],  # (1)
    cluster: str = ...,
) -> DeleteAttributesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
2. See [:material-code-braces: DeleteAttributesResponseTypeDef](./type_defs.md#deleteattributesresponsetypedef) 


```python
# delete_attributes method usage example with argument unpacking

kwargs: DeleteAttributesRequestRequestTypeDef = {  # (1)
    "attributes": ...,
}

parent.delete_attributes(**kwargs)
```

1. See [:material-code-braces: DeleteAttributesRequestRequestTypeDef](./type_defs.md#deleteattributesrequestrequesttypedef) 

### delete\_capacity\_provider

Deletes the specified capacity provider.

Type annotations and code completion for `#!python session.client("ecs").delete_capacity_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# delete_capacity_provider method definition

await def delete_capacity_provider(
    self,
    *,
    capacityProvider: str,
) -> DeleteCapacityProviderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteCapacityProviderResponseTypeDef](./type_defs.md#deletecapacityproviderresponsetypedef) 


```python
# delete_capacity_provider method usage example with argument unpacking

kwargs: DeleteCapacityProviderRequestRequestTypeDef = {  # (1)
    "capacityProvider": ...,
}

parent.delete_capacity_provider(**kwargs)
```

1. See [:material-code-braces: DeleteCapacityProviderRequestRequestTypeDef](./type_defs.md#deletecapacityproviderrequestrequesttypedef) 

### delete\_cluster

Deletes the specified cluster.

Type annotations and code completion for `#!python session.client("ecs").delete_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# delete_cluster method definition

await def delete_cluster(
    self,
    *,
    cluster: str,
) -> DeleteClusterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteClusterResponseTypeDef](./type_defs.md#deleteclusterresponsetypedef) 


```python
# delete_cluster method usage example with argument unpacking

kwargs: DeleteClusterRequestRequestTypeDef = {  # (1)
    "cluster": ...,
}

parent.delete_cluster(**kwargs)
```

1. See [:material-code-braces: DeleteClusterRequestRequestTypeDef](./type_defs.md#deleteclusterrequestrequesttypedef) 

### delete\_service

Deletes a specified service within a cluster.

Type annotations and code completion for `#!python session.client("ecs").delete_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# delete_service method definition

await def delete_service(
    self,
    *,
    service: str,
    cluster: str = ...,
    force: bool = ...,
) -> DeleteServiceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteServiceResponseTypeDef](./type_defs.md#deleteserviceresponsetypedef) 


```python
# delete_service method usage example with argument unpacking

kwargs: DeleteServiceRequestRequestTypeDef = {  # (1)
    "service": ...,
}

parent.delete_service(**kwargs)
```

1. See [:material-code-braces: DeleteServiceRequestRequestTypeDef](./type_defs.md#deleteservicerequestrequesttypedef) 

### delete\_task\_definitions

Deletes one or more task definitions.

Type annotations and code completion for `#!python session.client("ecs").delete_task_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# delete_task_definitions method definition

await def delete_task_definitions(
    self,
    *,
    taskDefinitions: Sequence[str],
) -> DeleteTaskDefinitionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteTaskDefinitionsResponseTypeDef](./type_defs.md#deletetaskdefinitionsresponsetypedef) 


```python
# delete_task_definitions method usage example with argument unpacking

kwargs: DeleteTaskDefinitionsRequestRequestTypeDef = {  # (1)
    "taskDefinitions": ...,
}

parent.delete_task_definitions(**kwargs)
```

1. See [:material-code-braces: DeleteTaskDefinitionsRequestRequestTypeDef](./type_defs.md#deletetaskdefinitionsrequestrequesttypedef) 

### delete\_task\_set

Deletes a specified task set within a service.

Type annotations and code completion for `#!python session.client("ecs").delete_task_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# delete_task_set method definition

await def delete_task_set(
    self,
    *,
    cluster: str,
    service: str,
    taskSet: str,
    force: bool = ...,
) -> DeleteTaskSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteTaskSetResponseTypeDef](./type_defs.md#deletetasksetresponsetypedef) 


```python
# delete_task_set method usage example with argument unpacking

kwargs: DeleteTaskSetRequestRequestTypeDef = {  # (1)
    "cluster": ...,
    "service": ...,
    "taskSet": ...,
}

parent.delete_task_set(**kwargs)
```

1. See [:material-code-braces: DeleteTaskSetRequestRequestTypeDef](./type_defs.md#deletetasksetrequestrequesttypedef) 

### deregister\_container\_instance

Deregisters an Amazon ECS container instance from the specified cluster.

Type annotations and code completion for `#!python session.client("ecs").deregister_container_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# deregister_container_instance method definition

await def deregister_container_instance(
    self,
    *,
    containerInstance: str,
    cluster: str = ...,
    force: bool = ...,
) -> DeregisterContainerInstanceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeregisterContainerInstanceResponseTypeDef](./type_defs.md#deregistercontainerinstanceresponsetypedef) 


```python
# deregister_container_instance method usage example with argument unpacking

kwargs: DeregisterContainerInstanceRequestRequestTypeDef = {  # (1)
    "containerInstance": ...,
}

parent.deregister_container_instance(**kwargs)
```

1. See [:material-code-braces: DeregisterContainerInstanceRequestRequestTypeDef](./type_defs.md#deregistercontainerinstancerequestrequesttypedef) 

### deregister\_task\_definition

Deregisters the specified task definition by family and revision.

Type annotations and code completion for `#!python session.client("ecs").deregister_task_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# deregister_task_definition method definition

await def deregister_task_definition(
    self,
    *,
    taskDefinition: str,
) -> DeregisterTaskDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeregisterTaskDefinitionResponseTypeDef](./type_defs.md#deregistertaskdefinitionresponsetypedef) 


```python
# deregister_task_definition method usage example with argument unpacking

kwargs: DeregisterTaskDefinitionRequestRequestTypeDef = {  # (1)
    "taskDefinition": ...,
}

parent.deregister_task_definition(**kwargs)
```

1. See [:material-code-braces: DeregisterTaskDefinitionRequestRequestTypeDef](./type_defs.md#deregistertaskdefinitionrequestrequesttypedef) 

### describe\_capacity\_providers

Describes one or more of your capacity providers.

Type annotations and code completion for `#!python session.client("ecs").describe_capacity_providers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# describe_capacity_providers method definition

await def describe_capacity_providers(
    self,
    *,
    capacityProviders: Sequence[str] = ...,
    include: Sequence[CapacityProviderFieldType] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeCapacityProvidersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: CapacityProviderFieldType](./literals.md#capacityproviderfieldtype) 
2. See [:material-code-braces: DescribeCapacityProvidersResponseTypeDef](./type_defs.md#describecapacityprovidersresponsetypedef) 


```python
# describe_capacity_providers method usage example with argument unpacking

kwargs: DescribeCapacityProvidersRequestRequestTypeDef = {  # (1)
    "capacityProviders": ...,
}

parent.describe_capacity_providers(**kwargs)
```

1. See [:material-code-braces: DescribeCapacityProvidersRequestRequestTypeDef](./type_defs.md#describecapacityprovidersrequestrequesttypedef) 

### describe\_clusters

Describes one or more of your clusters.

Type annotations and code completion for `#!python session.client("ecs").describe_clusters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# describe_clusters method definition

await def describe_clusters(
    self,
    *,
    clusters: Sequence[str] = ...,
    include: Sequence[ClusterFieldType] = ...,  # (1)
) -> DescribeClustersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ClusterFieldType](./literals.md#clusterfieldtype) 
2. See [:material-code-braces: DescribeClustersResponseTypeDef](./type_defs.md#describeclustersresponsetypedef) 


```python
# describe_clusters method usage example with argument unpacking

kwargs: DescribeClustersRequestRequestTypeDef = {  # (1)
    "clusters": ...,
}

parent.describe_clusters(**kwargs)
```

1. See [:material-code-braces: DescribeClustersRequestRequestTypeDef](./type_defs.md#describeclustersrequestrequesttypedef) 

### describe\_container\_instances

Describes one or more container instances.

Type annotations and code completion for `#!python session.client("ecs").describe_container_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# describe_container_instances method definition

await def describe_container_instances(
    self,
    *,
    containerInstances: Sequence[str],
    cluster: str = ...,
    include: Sequence[ContainerInstanceFieldType] = ...,  # (1)
) -> DescribeContainerInstancesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ContainerInstanceFieldType](./literals.md#containerinstancefieldtype) 
2. See [:material-code-braces: DescribeContainerInstancesResponseTypeDef](./type_defs.md#describecontainerinstancesresponsetypedef) 


```python
# describe_container_instances method usage example with argument unpacking

kwargs: DescribeContainerInstancesRequestRequestTypeDef = {  # (1)
    "containerInstances": ...,
}

parent.describe_container_instances(**kwargs)
```

1. See [:material-code-braces: DescribeContainerInstancesRequestRequestTypeDef](./type_defs.md#describecontainerinstancesrequestrequesttypedef) 

### describe\_service\_deployments

Describes one or more of your service deployments.

Type annotations and code completion for `#!python session.client("ecs").describe_service_deployments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# describe_service_deployments method definition

await def describe_service_deployments(
    self,
    *,
    serviceDeploymentArns: Sequence[str],
) -> DescribeServiceDeploymentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeServiceDeploymentsResponseTypeDef](./type_defs.md#describeservicedeploymentsresponsetypedef) 


```python
# describe_service_deployments method usage example with argument unpacking

kwargs: DescribeServiceDeploymentsRequestRequestTypeDef = {  # (1)
    "serviceDeploymentArns": ...,
}

parent.describe_service_deployments(**kwargs)
```

1. See [:material-code-braces: DescribeServiceDeploymentsRequestRequestTypeDef](./type_defs.md#describeservicedeploymentsrequestrequesttypedef) 

### describe\_service\_revisions

Describes one or more service revisions.

Type annotations and code completion for `#!python session.client("ecs").describe_service_revisions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# describe_service_revisions method definition

await def describe_service_revisions(
    self,
    *,
    serviceRevisionArns: Sequence[str],
) -> DescribeServiceRevisionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeServiceRevisionsResponseTypeDef](./type_defs.md#describeservicerevisionsresponsetypedef) 


```python
# describe_service_revisions method usage example with argument unpacking

kwargs: DescribeServiceRevisionsRequestRequestTypeDef = {  # (1)
    "serviceRevisionArns": ...,
}

parent.describe_service_revisions(**kwargs)
```

1. See [:material-code-braces: DescribeServiceRevisionsRequestRequestTypeDef](./type_defs.md#describeservicerevisionsrequestrequesttypedef) 

### describe\_services

Describes the specified services running in your cluster.

Type annotations and code completion for `#!python session.client("ecs").describe_services` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# describe_services method definition

await def describe_services(
    self,
    *,
    services: Sequence[str],
    cluster: str = ...,
    include: Sequence[ServiceFieldType] = ...,  # (1)
) -> DescribeServicesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ServiceFieldType](./literals.md#servicefieldtype) 
2. See [:material-code-braces: DescribeServicesResponseTypeDef](./type_defs.md#describeservicesresponsetypedef) 


```python
# describe_services method usage example with argument unpacking

kwargs: DescribeServicesRequestRequestTypeDef = {  # (1)
    "services": ...,
}

parent.describe_services(**kwargs)
```

1. See [:material-code-braces: DescribeServicesRequestRequestTypeDef](./type_defs.md#describeservicesrequestrequesttypedef) 

### describe\_task\_definition

Describes a task definition.

Type annotations and code completion for `#!python session.client("ecs").describe_task_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# describe_task_definition method definition

await def describe_task_definition(
    self,
    *,
    taskDefinition: str,
    include: Sequence[TaskDefinitionFieldType] = ...,  # (1)
) -> DescribeTaskDefinitionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TaskDefinitionFieldType](./literals.md#taskdefinitionfieldtype) 
2. See [:material-code-braces: DescribeTaskDefinitionResponseTypeDef](./type_defs.md#describetaskdefinitionresponsetypedef) 


```python
# describe_task_definition method usage example with argument unpacking

kwargs: DescribeTaskDefinitionRequestRequestTypeDef = {  # (1)
    "taskDefinition": ...,
}

parent.describe_task_definition(**kwargs)
```

1. See [:material-code-braces: DescribeTaskDefinitionRequestRequestTypeDef](./type_defs.md#describetaskdefinitionrequestrequesttypedef) 

### describe\_task\_sets

Describes the task sets in the specified cluster and service.

Type annotations and code completion for `#!python session.client("ecs").describe_task_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# describe_task_sets method definition

await def describe_task_sets(
    self,
    *,
    cluster: str,
    service: str,
    taskSets: Sequence[str] = ...,
    include: Sequence[TaskSetFieldType] = ...,  # (1)
) -> DescribeTaskSetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TaskSetFieldType](./literals.md#tasksetfieldtype) 
2. See [:material-code-braces: DescribeTaskSetsResponseTypeDef](./type_defs.md#describetasksetsresponsetypedef) 


```python
# describe_task_sets method usage example with argument unpacking

kwargs: DescribeTaskSetsRequestRequestTypeDef = {  # (1)
    "cluster": ...,
    "service": ...,
}

parent.describe_task_sets(**kwargs)
```

1. See [:material-code-braces: DescribeTaskSetsRequestRequestTypeDef](./type_defs.md#describetasksetsrequestrequesttypedef) 

### describe\_tasks

Describes a specified task or tasks.

Type annotations and code completion for `#!python session.client("ecs").describe_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# describe_tasks method definition

await def describe_tasks(
    self,
    *,
    tasks: Sequence[str],
    cluster: str = ...,
    include: Sequence[TaskFieldType] = ...,  # (1)
) -> DescribeTasksResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TaskFieldType](./literals.md#taskfieldtype) 
2. See [:material-code-braces: DescribeTasksResponseTypeDef](./type_defs.md#describetasksresponsetypedef) 


```python
# describe_tasks method usage example with argument unpacking

kwargs: DescribeTasksRequestRequestTypeDef = {  # (1)
    "tasks": ...,
}

parent.describe_tasks(**kwargs)
```

1. See [:material-code-braces: DescribeTasksRequestRequestTypeDef](./type_defs.md#describetasksrequestrequesttypedef) 

### discover\_poll\_endpoint

This action is only used by the Amazon ECS agent, and it is not intended for
use outside of the agent.

Type annotations and code completion for `#!python session.client("ecs").discover_poll_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# discover_poll_endpoint method definition

await def discover_poll_endpoint(
    self,
    *,
    containerInstance: str = ...,
    cluster: str = ...,
) -> DiscoverPollEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DiscoverPollEndpointResponseTypeDef](./type_defs.md#discoverpollendpointresponsetypedef) 


```python
# discover_poll_endpoint method usage example with argument unpacking

kwargs: DiscoverPollEndpointRequestRequestTypeDef = {  # (1)
    "containerInstance": ...,
}

parent.discover_poll_endpoint(**kwargs)
```

1. See [:material-code-braces: DiscoverPollEndpointRequestRequestTypeDef](./type_defs.md#discoverpollendpointrequestrequesttypedef) 

### execute\_command

Runs a command remotely on a container within a task.

Type annotations and code completion for `#!python session.client("ecs").execute_command` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# execute_command method definition

await def execute_command(
    self,
    *,
    command: str,
    interactive: bool,
    task: str,
    cluster: str = ...,
    container: str = ...,
) -> ExecuteCommandResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExecuteCommandResponseTypeDef](./type_defs.md#executecommandresponsetypedef) 


```python
# execute_command method usage example with argument unpacking

kwargs: ExecuteCommandRequestRequestTypeDef = {  # (1)
    "command": ...,
    "interactive": ...,
    "task": ...,
}

parent.execute_command(**kwargs)
```

1. See [:material-code-braces: ExecuteCommandRequestRequestTypeDef](./type_defs.md#executecommandrequestrequesttypedef) 

### get\_task\_protection

Retrieves the protection status of tasks in an Amazon ECS service.

Type annotations and code completion for `#!python session.client("ecs").get_task_protection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# get_task_protection method definition

await def get_task_protection(
    self,
    *,
    cluster: str,
    tasks: Sequence[str] = ...,
) -> GetTaskProtectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTaskProtectionResponseTypeDef](./type_defs.md#gettaskprotectionresponsetypedef) 


```python
# get_task_protection method usage example with argument unpacking

kwargs: GetTaskProtectionRequestRequestTypeDef = {  # (1)
    "cluster": ...,
}

parent.get_task_protection(**kwargs)
```

1. See [:material-code-braces: GetTaskProtectionRequestRequestTypeDef](./type_defs.md#gettaskprotectionrequestrequesttypedef) 

### list\_account\_settings

Lists the account settings for a specified principal.

Type annotations and code completion for `#!python session.client("ecs").list_account_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# list_account_settings method definition

await def list_account_settings(
    self,
    *,
    name: SettingNameType = ...,  # (1)
    value: str = ...,
    principalArn: str = ...,
    effectiveSettings: bool = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAccountSettingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SettingNameType](./literals.md#settingnametype) 
2. See [:material-code-braces: ListAccountSettingsResponseTypeDef](./type_defs.md#listaccountsettingsresponsetypedef) 


```python
# list_account_settings method usage example with argument unpacking

kwargs: ListAccountSettingsRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.list_account_settings(**kwargs)
```

1. See [:material-code-braces: ListAccountSettingsRequestRequestTypeDef](./type_defs.md#listaccountsettingsrequestrequesttypedef) 

### list\_attributes

Lists the attributes for Amazon ECS resources within a specified target type
and cluster.

Type annotations and code completion for `#!python session.client("ecs").list_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# list_attributes method definition

await def list_attributes(
    self,
    *,
    targetType: TargetTypeType,  # (1)
    cluster: str = ...,
    attributeName: str = ...,
    attributeValue: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAttributesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
2. See [:material-code-braces: ListAttributesResponseTypeDef](./type_defs.md#listattributesresponsetypedef) 


```python
# list_attributes method usage example with argument unpacking

kwargs: ListAttributesRequestRequestTypeDef = {  # (1)
    "targetType": ...,
}

parent.list_attributes(**kwargs)
```

1. See [:material-code-braces: ListAttributesRequestRequestTypeDef](./type_defs.md#listattributesrequestrequesttypedef) 

### list\_clusters

Returns a list of existing clusters.

Type annotations and code completion for `#!python session.client("ecs").list_clusters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# list_clusters method definition

await def list_clusters(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListClustersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef) 


```python
# list_clusters method usage example with argument unpacking

kwargs: ListClustersRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_clusters(**kwargs)
```

1. See [:material-code-braces: ListClustersRequestRequestTypeDef](./type_defs.md#listclustersrequestrequesttypedef) 

### list\_container\_instances

Returns a list of container instances in a specified cluster.

Type annotations and code completion for `#!python session.client("ecs").list_container_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# list_container_instances method definition

await def list_container_instances(
    self,
    *,
    cluster: str = ...,
    filter: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
    status: ContainerInstanceStatusType = ...,  # (1)
) -> ListContainerInstancesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ContainerInstanceStatusType](./literals.md#containerinstancestatustype) 
2. See [:material-code-braces: ListContainerInstancesResponseTypeDef](./type_defs.md#listcontainerinstancesresponsetypedef) 


```python
# list_container_instances method usage example with argument unpacking

kwargs: ListContainerInstancesRequestRequestTypeDef = {  # (1)
    "cluster": ...,
}

parent.list_container_instances(**kwargs)
```

1. See [:material-code-braces: ListContainerInstancesRequestRequestTypeDef](./type_defs.md#listcontainerinstancesrequestrequesttypedef) 

### list\_service\_deployments

This operation lists all the service deployments that meet the specified filter
criteria.

Type annotations and code completion for `#!python session.client("ecs").list_service_deployments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# list_service_deployments method definition

await def list_service_deployments(
    self,
    *,
    service: str,
    cluster: str = ...,
    status: Sequence[ServiceDeploymentStatusType] = ...,  # (1)
    createdAt: CreatedAtTypeDef = ...,  # (2)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListServiceDeploymentsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ServiceDeploymentStatusType](./literals.md#servicedeploymentstatustype) 
2. See [:material-code-braces: CreatedAtTypeDef](./type_defs.md#createdattypedef) 
3. See [:material-code-braces: ListServiceDeploymentsResponseTypeDef](./type_defs.md#listservicedeploymentsresponsetypedef) 


```python
# list_service_deployments method usage example with argument unpacking

kwargs: ListServiceDeploymentsRequestRequestTypeDef = {  # (1)
    "service": ...,
}

parent.list_service_deployments(**kwargs)
```

1. See [:material-code-braces: ListServiceDeploymentsRequestRequestTypeDef](./type_defs.md#listservicedeploymentsrequestrequesttypedef) 

### list\_services

Returns a list of services.

Type annotations and code completion for `#!python session.client("ecs").list_services` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# list_services method definition

await def list_services(
    self,
    *,
    cluster: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
    launchType: LaunchTypeType = ...,  # (1)
    schedulingStrategy: SchedulingStrategyType = ...,  # (2)
) -> ListServicesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
2. See [:material-code-brackets: SchedulingStrategyType](./literals.md#schedulingstrategytype) 
3. See [:material-code-braces: ListServicesResponseTypeDef](./type_defs.md#listservicesresponsetypedef) 


```python
# list_services method usage example with argument unpacking

kwargs: ListServicesRequestRequestTypeDef = {  # (1)
    "cluster": ...,
}

parent.list_services(**kwargs)
```

1. See [:material-code-braces: ListServicesRequestRequestTypeDef](./type_defs.md#listservicesrequestrequesttypedef) 

### list\_services\_by\_namespace

This operation lists all of the services that are associated with a Cloud Map
namespace.

Type annotations and code completion for `#!python session.client("ecs").list_services_by_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# list_services_by_namespace method definition

await def list_services_by_namespace(
    self,
    *,
    namespace: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListServicesByNamespaceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServicesByNamespaceResponseTypeDef](./type_defs.md#listservicesbynamespaceresponsetypedef) 


```python
# list_services_by_namespace method usage example with argument unpacking

kwargs: ListServicesByNamespaceRequestRequestTypeDef = {  # (1)
    "namespace": ...,
}

parent.list_services_by_namespace(**kwargs)
```

1. See [:material-code-braces: ListServicesByNamespaceRequestRequestTypeDef](./type_defs.md#listservicesbynamespacerequestrequesttypedef) 

### list\_tags\_for\_resource

List the tags for an Amazon ECS resource.

Type annotations and code completion for `#!python session.client("ecs").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_task\_definition\_families

Returns a list of task definition families that are registered to your account.

Type annotations and code completion for `#!python session.client("ecs").list_task_definition_families` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# list_task_definition_families method definition

await def list_task_definition_families(
    self,
    *,
    familyPrefix: str = ...,
    status: TaskDefinitionFamilyStatusType = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTaskDefinitionFamiliesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TaskDefinitionFamilyStatusType](./literals.md#taskdefinitionfamilystatustype) 
2. See [:material-code-braces: ListTaskDefinitionFamiliesResponseTypeDef](./type_defs.md#listtaskdefinitionfamiliesresponsetypedef) 


```python
# list_task_definition_families method usage example with argument unpacking

kwargs: ListTaskDefinitionFamiliesRequestRequestTypeDef = {  # (1)
    "familyPrefix": ...,
}

parent.list_task_definition_families(**kwargs)
```

1. See [:material-code-braces: ListTaskDefinitionFamiliesRequestRequestTypeDef](./type_defs.md#listtaskdefinitionfamiliesrequestrequesttypedef) 

### list\_task\_definitions

Returns a list of task definitions that are registered to your account.

Type annotations and code completion for `#!python session.client("ecs").list_task_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# list_task_definitions method definition

await def list_task_definitions(
    self,
    *,
    familyPrefix: str = ...,
    status: TaskDefinitionStatusType = ...,  # (1)
    sort: SortOrderType = ...,  # (2)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTaskDefinitionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: TaskDefinitionStatusType](./literals.md#taskdefinitionstatustype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListTaskDefinitionsResponseTypeDef](./type_defs.md#listtaskdefinitionsresponsetypedef) 


```python
# list_task_definitions method usage example with argument unpacking

kwargs: ListTaskDefinitionsRequestRequestTypeDef = {  # (1)
    "familyPrefix": ...,
}

parent.list_task_definitions(**kwargs)
```

1. See [:material-code-braces: ListTaskDefinitionsRequestRequestTypeDef](./type_defs.md#listtaskdefinitionsrequestrequesttypedef) 

### list\_tasks

Returns a list of tasks.

Type annotations and code completion for `#!python session.client("ecs").list_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# list_tasks method definition

await def list_tasks(
    self,
    *,
    cluster: str = ...,
    containerInstance: str = ...,
    family: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
    startedBy: str = ...,
    serviceName: str = ...,
    desiredStatus: DesiredStatusType = ...,  # (1)
    launchType: LaunchTypeType = ...,  # (2)
) -> ListTasksResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: DesiredStatusType](./literals.md#desiredstatustype) 
2. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
3. See [:material-code-braces: ListTasksResponseTypeDef](./type_defs.md#listtasksresponsetypedef) 


```python
# list_tasks method usage example with argument unpacking

kwargs: ListTasksRequestRequestTypeDef = {  # (1)
    "cluster": ...,
}

parent.list_tasks(**kwargs)
```

1. See [:material-code-braces: ListTasksRequestRequestTypeDef](./type_defs.md#listtasksrequestrequesttypedef) 

### put\_account\_setting

Modifies an account setting.

Type annotations and code completion for `#!python session.client("ecs").put_account_setting` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# put_account_setting method definition

await def put_account_setting(
    self,
    *,
    name: SettingNameType,  # (1)
    value: str,
    principalArn: str = ...,
) -> PutAccountSettingResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SettingNameType](./literals.md#settingnametype) 
2. See [:material-code-braces: PutAccountSettingResponseTypeDef](./type_defs.md#putaccountsettingresponsetypedef) 


```python
# put_account_setting method usage example with argument unpacking

kwargs: PutAccountSettingRequestRequestTypeDef = {  # (1)
    "name": ...,
    "value": ...,
}

parent.put_account_setting(**kwargs)
```

1. See [:material-code-braces: PutAccountSettingRequestRequestTypeDef](./type_defs.md#putaccountsettingrequestrequesttypedef) 

### put\_account\_setting\_default

Modifies an account setting for all users on an account for whom no individual
account setting has been specified.

Type annotations and code completion for `#!python session.client("ecs").put_account_setting_default` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# put_account_setting_default method definition

await def put_account_setting_default(
    self,
    *,
    name: SettingNameType,  # (1)
    value: str,
) -> PutAccountSettingDefaultResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SettingNameType](./literals.md#settingnametype) 
2. See [:material-code-braces: PutAccountSettingDefaultResponseTypeDef](./type_defs.md#putaccountsettingdefaultresponsetypedef) 


```python
# put_account_setting_default method usage example with argument unpacking

kwargs: PutAccountSettingDefaultRequestRequestTypeDef = {  # (1)
    "name": ...,
    "value": ...,
}

parent.put_account_setting_default(**kwargs)
```

1. See [:material-code-braces: PutAccountSettingDefaultRequestRequestTypeDef](./type_defs.md#putaccountsettingdefaultrequestrequesttypedef) 

### put\_attributes

Create or update an attribute on an Amazon ECS resource.

Type annotations and code completion for `#!python session.client("ecs").put_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# put_attributes method definition

await def put_attributes(
    self,
    *,
    attributes: Sequence[AttributeTypeDef],  # (1)
    cluster: str = ...,
) -> PutAttributesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
2. See [:material-code-braces: PutAttributesResponseTypeDef](./type_defs.md#putattributesresponsetypedef) 


```python
# put_attributes method usage example with argument unpacking

kwargs: PutAttributesRequestRequestTypeDef = {  # (1)
    "attributes": ...,
}

parent.put_attributes(**kwargs)
```

1. See [:material-code-braces: PutAttributesRequestRequestTypeDef](./type_defs.md#putattributesrequestrequesttypedef) 

### put\_cluster\_capacity\_providers

Modifies the available capacity providers and the default capacity provider
strategy for a cluster.

Type annotations and code completion for `#!python session.client("ecs").put_cluster_capacity_providers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# put_cluster_capacity_providers method definition

await def put_cluster_capacity_providers(
    self,
    *,
    cluster: str,
    capacityProviders: Sequence[str],
    defaultCapacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef],  # (1)
) -> PutClusterCapacityProvidersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
2. See [:material-code-braces: PutClusterCapacityProvidersResponseTypeDef](./type_defs.md#putclustercapacityprovidersresponsetypedef) 


```python
# put_cluster_capacity_providers method usage example with argument unpacking

kwargs: PutClusterCapacityProvidersRequestRequestTypeDef = {  # (1)
    "cluster": ...,
    "capacityProviders": ...,
    "defaultCapacityProviderStrategy": ...,
}

parent.put_cluster_capacity_providers(**kwargs)
```

1. See [:material-code-braces: PutClusterCapacityProvidersRequestRequestTypeDef](./type_defs.md#putclustercapacityprovidersrequestrequesttypedef) 

### register\_container\_instance

This action is only used by the Amazon ECS agent, and it is not intended for
use outside of the agent.

Type annotations and code completion for `#!python session.client("ecs").register_container_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# register_container_instance method definition

await def register_container_instance(
    self,
    *,
    cluster: str = ...,
    instanceIdentityDocument: str = ...,
    instanceIdentityDocumentSignature: str = ...,
    totalResources: Sequence[ResourceUnionTypeDef] = ...,  # (1)
    versionInfo: VersionInfoTypeDef = ...,  # (2)
    containerInstanceArn: str = ...,
    attributes: Sequence[AttributeTypeDef] = ...,  # (3)
    platformDevices: Sequence[PlatformDeviceTypeDef] = ...,  # (4)
    tags: Sequence[TagTypeDef] = ...,  # (5)
) -> RegisterContainerInstanceResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 
2. See [:material-code-braces: VersionInfoTypeDef](./type_defs.md#versioninfotypedef) 
3. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
4. See [:material-code-braces: PlatformDeviceTypeDef](./type_defs.md#platformdevicetypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: RegisterContainerInstanceResponseTypeDef](./type_defs.md#registercontainerinstanceresponsetypedef) 


```python
# register_container_instance method usage example with argument unpacking

kwargs: RegisterContainerInstanceRequestRequestTypeDef = {  # (1)
    "cluster": ...,
}

parent.register_container_instance(**kwargs)
```

1. See [:material-code-braces: RegisterContainerInstanceRequestRequestTypeDef](./type_defs.md#registercontainerinstancerequestrequesttypedef) 

### register\_task\_definition

Registers a new task definition from the supplied <code>family</code> and
<code>containerDefinitions</code>.

Type annotations and code completion for `#!python session.client("ecs").register_task_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# register_task_definition method definition

await def register_task_definition(
    self,
    *,
    family: str,
    containerDefinitions: Sequence[ContainerDefinitionUnionTypeDef],  # (1)
    taskRoleArn: str = ...,
    executionRoleArn: str = ...,
    networkMode: NetworkModeType = ...,  # (2)
    volumes: Sequence[VolumeUnionTypeDef] = ...,  # (3)
    placementConstraints: Sequence[TaskDefinitionPlacementConstraintTypeDef] = ...,  # (4)
    requiresCompatibilities: Sequence[CompatibilityType] = ...,  # (5)
    cpu: str = ...,
    memory: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (6)
    pidMode: PidModeType = ...,  # (7)
    ipcMode: IpcModeType = ...,  # (8)
    proxyConfiguration: ProxyConfigurationTypeDef = ...,  # (9)
    inferenceAccelerators: Sequence[InferenceAcceleratorTypeDef] = ...,  # (10)
    ephemeralStorage: EphemeralStorageTypeDef = ...,  # (11)
    runtimePlatform: RuntimePlatformTypeDef = ...,  # (12)
) -> RegisterTaskDefinitionResponseTypeDef:  # (13)
    ...
```

1. See [:material-code-braces: ContainerDefinitionTypeDef](./type_defs.md#containerdefinitiontypedef) [:material-code-braces: ContainerDefinitionOutputTypeDef](./type_defs.md#containerdefinitionoutputtypedef) 
2. See [:material-code-brackets: NetworkModeType](./literals.md#networkmodetype) 
3. See [:material-code-braces: VolumeTypeDef](./type_defs.md#volumetypedef) [:material-code-braces: VolumeOutputTypeDef](./type_defs.md#volumeoutputtypedef) 
4. See [:material-code-braces: TaskDefinitionPlacementConstraintTypeDef](./type_defs.md#taskdefinitionplacementconstrainttypedef) 
5. See [:material-code-brackets: CompatibilityType](./literals.md#compatibilitytype) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-brackets: PidModeType](./literals.md#pidmodetype) 
8. See [:material-code-brackets: IpcModeType](./literals.md#ipcmodetype) 
9. See [:material-code-braces: ProxyConfigurationTypeDef](./type_defs.md#proxyconfigurationtypedef) 
10. See [:material-code-braces: InferenceAcceleratorTypeDef](./type_defs.md#inferenceacceleratortypedef) 
11. See [:material-code-braces: EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef) 
12. See [:material-code-braces: RuntimePlatformTypeDef](./type_defs.md#runtimeplatformtypedef) 
13. See [:material-code-braces: RegisterTaskDefinitionResponseTypeDef](./type_defs.md#registertaskdefinitionresponsetypedef) 


```python
# register_task_definition method usage example with argument unpacking

kwargs: RegisterTaskDefinitionRequestRequestTypeDef = {  # (1)
    "family": ...,
    "containerDefinitions": ...,
}

parent.register_task_definition(**kwargs)
```

1. See [:material-code-braces: RegisterTaskDefinitionRequestRequestTypeDef](./type_defs.md#registertaskdefinitionrequestrequesttypedef) 

### run\_task

Starts a new task using the specified task definition.

Type annotations and code completion for `#!python session.client("ecs").run_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# run_task method definition

await def run_task(
    self,
    *,
    taskDefinition: str,
    capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,  # (1)
    cluster: str = ...,
    count: int = ...,
    enableECSManagedTags: bool = ...,
    enableExecuteCommand: bool = ...,
    group: str = ...,
    launchType: LaunchTypeType = ...,  # (2)
    networkConfiguration: NetworkConfigurationTypeDef = ...,  # (3)
    overrides: TaskOverrideTypeDef = ...,  # (4)
    placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,  # (5)
    placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,  # (6)
    platformVersion: str = ...,
    propagateTags: PropagateTagsType = ...,  # (7)
    referenceId: str = ...,
    startedBy: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (8)
    clientToken: str = ...,
    volumeConfigurations: Sequence[TaskVolumeConfigurationTypeDef] = ...,  # (9)
) -> RunTaskResponseTypeDef:  # (10)
    ...
```

1. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
2. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
3. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
4. See [:material-code-braces: TaskOverrideTypeDef](./type_defs.md#taskoverridetypedef) 
5. See [:material-code-braces: PlacementConstraintTypeDef](./type_defs.md#placementconstrainttypedef) 
6. See [:material-code-braces: PlacementStrategyTypeDef](./type_defs.md#placementstrategytypedef) 
7. See [:material-code-brackets: PropagateTagsType](./literals.md#propagatetagstype) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
9. See [:material-code-braces: TaskVolumeConfigurationTypeDef](./type_defs.md#taskvolumeconfigurationtypedef) 
10. See [:material-code-braces: RunTaskResponseTypeDef](./type_defs.md#runtaskresponsetypedef) 


```python
# run_task method usage example with argument unpacking

kwargs: RunTaskRequestRequestTypeDef = {  # (1)
    "taskDefinition": ...,
}

parent.run_task(**kwargs)
```

1. See [:material-code-braces: RunTaskRequestRequestTypeDef](./type_defs.md#runtaskrequestrequesttypedef) 

### start\_task

Starts a new task from the specified task definition on the specified container
instance or instances.

Type annotations and code completion for `#!python session.client("ecs").start_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# start_task method definition

await def start_task(
    self,
    *,
    containerInstances: Sequence[str],
    taskDefinition: str,
    cluster: str = ...,
    enableECSManagedTags: bool = ...,
    enableExecuteCommand: bool = ...,
    group: str = ...,
    networkConfiguration: NetworkConfigurationTypeDef = ...,  # (1)
    overrides: TaskOverrideTypeDef = ...,  # (2)
    propagateTags: PropagateTagsType = ...,  # (3)
    referenceId: str = ...,
    startedBy: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (4)
    volumeConfigurations: Sequence[TaskVolumeConfigurationTypeDef] = ...,  # (5)
) -> StartTaskResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
2. See [:material-code-braces: TaskOverrideTypeDef](./type_defs.md#taskoverridetypedef) 
3. See [:material-code-brackets: PropagateTagsType](./literals.md#propagatetagstype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: TaskVolumeConfigurationTypeDef](./type_defs.md#taskvolumeconfigurationtypedef) 
6. See [:material-code-braces: StartTaskResponseTypeDef](./type_defs.md#starttaskresponsetypedef) 


```python
# start_task method usage example with argument unpacking

kwargs: StartTaskRequestRequestTypeDef = {  # (1)
    "containerInstances": ...,
    "taskDefinition": ...,
}

parent.start_task(**kwargs)
```

1. See [:material-code-braces: StartTaskRequestRequestTypeDef](./type_defs.md#starttaskrequestrequesttypedef) 

### stop\_task

Stops a running task.

Type annotations and code completion for `#!python session.client("ecs").stop_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# stop_task method definition

await def stop_task(
    self,
    *,
    task: str,
    cluster: str = ...,
    reason: str = ...,
) -> StopTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopTaskResponseTypeDef](./type_defs.md#stoptaskresponsetypedef) 


```python
# stop_task method usage example with argument unpacking

kwargs: StopTaskRequestRequestTypeDef = {  # (1)
    "task": ...,
}

parent.stop_task(**kwargs)
```

1. See [:material-code-braces: StopTaskRequestRequestTypeDef](./type_defs.md#stoptaskrequestrequesttypedef) 

### submit\_attachment\_state\_changes

This action is only used by the Amazon ECS agent, and it is not intended for
use outside of the agent.

Type annotations and code completion for `#!python session.client("ecs").submit_attachment_state_changes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# submit_attachment_state_changes method definition

await def submit_attachment_state_changes(
    self,
    *,
    attachments: Sequence[AttachmentStateChangeTypeDef],  # (1)
    cluster: str = ...,
) -> SubmitAttachmentStateChangesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AttachmentStateChangeTypeDef](./type_defs.md#attachmentstatechangetypedef) 
2. See [:material-code-braces: SubmitAttachmentStateChangesResponseTypeDef](./type_defs.md#submitattachmentstatechangesresponsetypedef) 


```python
# submit_attachment_state_changes method usage example with argument unpacking

kwargs: SubmitAttachmentStateChangesRequestRequestTypeDef = {  # (1)
    "attachments": ...,
}

parent.submit_attachment_state_changes(**kwargs)
```

1. See [:material-code-braces: SubmitAttachmentStateChangesRequestRequestTypeDef](./type_defs.md#submitattachmentstatechangesrequestrequesttypedef) 

### submit\_container\_state\_change

This action is only used by the Amazon ECS agent, and it is not intended for
use outside of the agent.

Type annotations and code completion for `#!python session.client("ecs").submit_container_state_change` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# submit_container_state_change method definition

await def submit_container_state_change(
    self,
    *,
    cluster: str = ...,
    task: str = ...,
    containerName: str = ...,
    runtimeId: str = ...,
    status: str = ...,
    exitCode: int = ...,
    reason: str = ...,
    networkBindings: Sequence[NetworkBindingTypeDef] = ...,  # (1)
) -> SubmitContainerStateChangeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: NetworkBindingTypeDef](./type_defs.md#networkbindingtypedef) 
2. See [:material-code-braces: SubmitContainerStateChangeResponseTypeDef](./type_defs.md#submitcontainerstatechangeresponsetypedef) 


```python
# submit_container_state_change method usage example with argument unpacking

kwargs: SubmitContainerStateChangeRequestRequestTypeDef = {  # (1)
    "cluster": ...,
}

parent.submit_container_state_change(**kwargs)
```

1. See [:material-code-braces: SubmitContainerStateChangeRequestRequestTypeDef](./type_defs.md#submitcontainerstatechangerequestrequesttypedef) 

### submit\_task\_state\_change

This action is only used by the Amazon ECS agent, and it is not intended for
use outside of the agent.

Type annotations and code completion for `#!python session.client("ecs").submit_task_state_change` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# submit_task_state_change method definition

await def submit_task_state_change(
    self,
    *,
    cluster: str = ...,
    task: str = ...,
    status: str = ...,
    reason: str = ...,
    containers: Sequence[ContainerStateChangeTypeDef] = ...,  # (1)
    attachments: Sequence[AttachmentStateChangeTypeDef] = ...,  # (2)
    managedAgents: Sequence[ManagedAgentStateChangeTypeDef] = ...,  # (3)
    pullStartedAt: TimestampTypeDef = ...,
    pullStoppedAt: TimestampTypeDef = ...,
    executionStoppedAt: TimestampTypeDef = ...,
) -> SubmitTaskStateChangeResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ContainerStateChangeTypeDef](./type_defs.md#containerstatechangetypedef) 
2. See [:material-code-braces: AttachmentStateChangeTypeDef](./type_defs.md#attachmentstatechangetypedef) 
3. See [:material-code-braces: ManagedAgentStateChangeTypeDef](./type_defs.md#managedagentstatechangetypedef) 
4. See [:material-code-braces: SubmitTaskStateChangeResponseTypeDef](./type_defs.md#submittaskstatechangeresponsetypedef) 


```python
# submit_task_state_change method usage example with argument unpacking

kwargs: SubmitTaskStateChangeRequestRequestTypeDef = {  # (1)
    "cluster": ...,
}

parent.submit_task_state_change(**kwargs)
```

1. See [:material-code-braces: SubmitTaskStateChangeRequestRequestTypeDef](./type_defs.md#submittaskstatechangerequestrequesttypedef) 

### tag\_resource

Associates the specified tags to a resource with the specified
<code>resourceArn</code>.

Type annotations and code completion for `#!python session.client("ecs").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Deletes specified tags from a resource.

Type annotations and code completion for `#!python session.client("ecs").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_capacity\_provider

Modifies the parameters for a capacity provider.

Type annotations and code completion for `#!python session.client("ecs").update_capacity_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# update_capacity_provider method definition

await def update_capacity_provider(
    self,
    *,
    name: str,
    autoScalingGroupProvider: AutoScalingGroupProviderUpdateTypeDef,  # (1)
) -> UpdateCapacityProviderResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AutoScalingGroupProviderUpdateTypeDef](./type_defs.md#autoscalinggroupproviderupdatetypedef) 
2. See [:material-code-braces: UpdateCapacityProviderResponseTypeDef](./type_defs.md#updatecapacityproviderresponsetypedef) 


```python
# update_capacity_provider method usage example with argument unpacking

kwargs: UpdateCapacityProviderRequestRequestTypeDef = {  # (1)
    "name": ...,
    "autoScalingGroupProvider": ...,
}

parent.update_capacity_provider(**kwargs)
```

1. See [:material-code-braces: UpdateCapacityProviderRequestRequestTypeDef](./type_defs.md#updatecapacityproviderrequestrequesttypedef) 

### update\_cluster

Updates the cluster.

Type annotations and code completion for `#!python session.client("ecs").update_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# update_cluster method definition

await def update_cluster(
    self,
    *,
    cluster: str,
    settings: Sequence[ClusterSettingTypeDef] = ...,  # (1)
    configuration: ClusterConfigurationTypeDef = ...,  # (2)
    serviceConnectDefaults: ClusterServiceConnectDefaultsRequestTypeDef = ...,  # (3)
) -> UpdateClusterResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ClusterSettingTypeDef](./type_defs.md#clustersettingtypedef) 
2. See [:material-code-braces: ClusterConfigurationTypeDef](./type_defs.md#clusterconfigurationtypedef) 
3. See [:material-code-braces: ClusterServiceConnectDefaultsRequestTypeDef](./type_defs.md#clusterserviceconnectdefaultsrequesttypedef) 
4. See [:material-code-braces: UpdateClusterResponseTypeDef](./type_defs.md#updateclusterresponsetypedef) 


```python
# update_cluster method usage example with argument unpacking

kwargs: UpdateClusterRequestRequestTypeDef = {  # (1)
    "cluster": ...,
}

parent.update_cluster(**kwargs)
```

1. See [:material-code-braces: UpdateClusterRequestRequestTypeDef](./type_defs.md#updateclusterrequestrequesttypedef) 

### update\_cluster\_settings

Modifies the settings to use for a cluster.

Type annotations and code completion for `#!python session.client("ecs").update_cluster_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# update_cluster_settings method definition

await def update_cluster_settings(
    self,
    *,
    cluster: str,
    settings: Sequence[ClusterSettingTypeDef],  # (1)
) -> UpdateClusterSettingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ClusterSettingTypeDef](./type_defs.md#clustersettingtypedef) 
2. See [:material-code-braces: UpdateClusterSettingsResponseTypeDef](./type_defs.md#updateclustersettingsresponsetypedef) 


```python
# update_cluster_settings method usage example with argument unpacking

kwargs: UpdateClusterSettingsRequestRequestTypeDef = {  # (1)
    "cluster": ...,
    "settings": ...,
}

parent.update_cluster_settings(**kwargs)
```

1. See [:material-code-braces: UpdateClusterSettingsRequestRequestTypeDef](./type_defs.md#updateclustersettingsrequestrequesttypedef) 

### update\_container\_agent

Updates the Amazon ECS container agent on a specified container instance.

Type annotations and code completion for `#!python session.client("ecs").update_container_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# update_container_agent method definition

await def update_container_agent(
    self,
    *,
    containerInstance: str,
    cluster: str = ...,
) -> UpdateContainerAgentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateContainerAgentResponseTypeDef](./type_defs.md#updatecontaineragentresponsetypedef) 


```python
# update_container_agent method usage example with argument unpacking

kwargs: UpdateContainerAgentRequestRequestTypeDef = {  # (1)
    "containerInstance": ...,
}

parent.update_container_agent(**kwargs)
```

1. See [:material-code-braces: UpdateContainerAgentRequestRequestTypeDef](./type_defs.md#updatecontaineragentrequestrequesttypedef) 

### update\_container\_instances\_state

Modifies the status of an Amazon ECS container instance.

Type annotations and code completion for `#!python session.client("ecs").update_container_instances_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# update_container_instances_state method definition

await def update_container_instances_state(
    self,
    *,
    containerInstances: Sequence[str],
    status: ContainerInstanceStatusType,  # (1)
    cluster: str = ...,
) -> UpdateContainerInstancesStateResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ContainerInstanceStatusType](./literals.md#containerinstancestatustype) 
2. See [:material-code-braces: UpdateContainerInstancesStateResponseTypeDef](./type_defs.md#updatecontainerinstancesstateresponsetypedef) 


```python
# update_container_instances_state method usage example with argument unpacking

kwargs: UpdateContainerInstancesStateRequestRequestTypeDef = {  # (1)
    "containerInstances": ...,
    "status": ...,
}

parent.update_container_instances_state(**kwargs)
```

1. See [:material-code-braces: UpdateContainerInstancesStateRequestRequestTypeDef](./type_defs.md#updatecontainerinstancesstaterequestrequesttypedef) 

### update\_service

Modifies the parameters of a service.

Type annotations and code completion for `#!python session.client("ecs").update_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# update_service method definition

await def update_service(
    self,
    *,
    service: str,
    cluster: str = ...,
    desiredCount: int = ...,
    taskDefinition: str = ...,
    capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,  # (1)
    deploymentConfiguration: DeploymentConfigurationTypeDef = ...,  # (2)
    availabilityZoneRebalancing: AvailabilityZoneRebalancingType = ...,  # (3)
    networkConfiguration: NetworkConfigurationTypeDef = ...,  # (4)
    placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,  # (5)
    placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,  # (6)
    platformVersion: str = ...,
    forceNewDeployment: bool = ...,
    healthCheckGracePeriodSeconds: int = ...,
    enableExecuteCommand: bool = ...,
    enableECSManagedTags: bool = ...,
    loadBalancers: Sequence[LoadBalancerTypeDef] = ...,  # (7)
    propagateTags: PropagateTagsType = ...,  # (8)
    serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,  # (9)
    serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...,  # (10)
    volumeConfigurations: Sequence[ServiceVolumeConfigurationTypeDef] = ...,  # (11)
    vpcLatticeConfigurations: Sequence[VpcLatticeConfigurationTypeDef] = ...,  # (12)
) -> UpdateServiceResponseTypeDef:  # (13)
    ...
```

1. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
2. See [:material-code-braces: DeploymentConfigurationTypeDef](./type_defs.md#deploymentconfigurationtypedef) 
3. See [:material-code-brackets: AvailabilityZoneRebalancingType](./literals.md#availabilityzonerebalancingtype) 
4. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
5. See [:material-code-braces: PlacementConstraintTypeDef](./type_defs.md#placementconstrainttypedef) 
6. See [:material-code-braces: PlacementStrategyTypeDef](./type_defs.md#placementstrategytypedef) 
7. See [:material-code-braces: LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef) 
8. See [:material-code-brackets: PropagateTagsType](./literals.md#propagatetagstype) 
9. See [:material-code-braces: ServiceRegistryTypeDef](./type_defs.md#serviceregistrytypedef) 
10. See [:material-code-braces: ServiceConnectConfigurationTypeDef](./type_defs.md#serviceconnectconfigurationtypedef) 
11. See [:material-code-braces: ServiceVolumeConfigurationTypeDef](./type_defs.md#servicevolumeconfigurationtypedef) 
12. See [:material-code-braces: VpcLatticeConfigurationTypeDef](./type_defs.md#vpclatticeconfigurationtypedef) 
13. See [:material-code-braces: UpdateServiceResponseTypeDef](./type_defs.md#updateserviceresponsetypedef) 


```python
# update_service method usage example with argument unpacking

kwargs: UpdateServiceRequestRequestTypeDef = {  # (1)
    "service": ...,
}

parent.update_service(**kwargs)
```

1. See [:material-code-braces: UpdateServiceRequestRequestTypeDef](./type_defs.md#updateservicerequestrequesttypedef) 

### update\_service\_primary\_task\_set

Modifies which task set in a service is the primary task set.

Type annotations and code completion for `#!python session.client("ecs").update_service_primary_task_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# update_service_primary_task_set method definition

await def update_service_primary_task_set(
    self,
    *,
    cluster: str,
    service: str,
    primaryTaskSet: str,
) -> UpdateServicePrimaryTaskSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateServicePrimaryTaskSetResponseTypeDef](./type_defs.md#updateserviceprimarytasksetresponsetypedef) 


```python
# update_service_primary_task_set method usage example with argument unpacking

kwargs: UpdateServicePrimaryTaskSetRequestRequestTypeDef = {  # (1)
    "cluster": ...,
    "service": ...,
    "primaryTaskSet": ...,
}

parent.update_service_primary_task_set(**kwargs)
```

1. See [:material-code-braces: UpdateServicePrimaryTaskSetRequestRequestTypeDef](./type_defs.md#updateserviceprimarytasksetrequestrequesttypedef) 

### update\_task\_protection

Updates the protection status of a task.

Type annotations and code completion for `#!python session.client("ecs").update_task_protection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# update_task_protection method definition

await def update_task_protection(
    self,
    *,
    cluster: str,
    tasks: Sequence[str],
    protectionEnabled: bool,
    expiresInMinutes: int = ...,
) -> UpdateTaskProtectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateTaskProtectionResponseTypeDef](./type_defs.md#updatetaskprotectionresponsetypedef) 


```python
# update_task_protection method usage example with argument unpacking

kwargs: UpdateTaskProtectionRequestRequestTypeDef = {  # (1)
    "cluster": ...,
    "tasks": ...,
    "protectionEnabled": ...,
}

parent.update_task_protection(**kwargs)
```

1. See [:material-code-braces: UpdateTaskProtectionRequestRequestTypeDef](./type_defs.md#updatetaskprotectionrequestrequesttypedef) 

### update\_task\_set

Modifies a task set.

Type annotations and code completion for `#!python session.client("ecs").update_task_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# update_task_set method definition

await def update_task_set(
    self,
    *,
    cluster: str,
    service: str,
    taskSet: str,
    scale: ScaleTypeDef,  # (1)
) -> UpdateTaskSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ScaleTypeDef](./type_defs.md#scaletypedef) 
2. See [:material-code-braces: UpdateTaskSetResponseTypeDef](./type_defs.md#updatetasksetresponsetypedef) 


```python
# update_task_set method usage example with argument unpacking

kwargs: UpdateTaskSetRequestRequestTypeDef = {  # (1)
    "cluster": ...,
    "service": ...,
    "taskSet": ...,
    "scale": ...,
}

parent.update_task_set(**kwargs)
```

1. See [:material-code-braces: UpdateTaskSetRequestRequestTypeDef](./type_defs.md#updatetasksetrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("ecs").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("ecs").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("ecs").get_paginator` method with overloads.

- `client.get_paginator("list_account_settings")` -> [ListAccountSettingsPaginator](./paginators.md#listaccountsettingspaginator)
- `client.get_paginator("list_attributes")` -> [ListAttributesPaginator](./paginators.md#listattributespaginator)
- `client.get_paginator("list_clusters")` -> [ListClustersPaginator](./paginators.md#listclusterspaginator)
- `client.get_paginator("list_container_instances")` -> [ListContainerInstancesPaginator](./paginators.md#listcontainerinstancespaginator)
- `client.get_paginator("list_services_by_namespace")` -> [ListServicesByNamespacePaginator](./paginators.md#listservicesbynamespacepaginator)
- `client.get_paginator("list_services")` -> [ListServicesPaginator](./paginators.md#listservicespaginator)
- `client.get_paginator("list_task_definition_families")` -> [ListTaskDefinitionFamiliesPaginator](./paginators.md#listtaskdefinitionfamiliespaginator)
- `client.get_paginator("list_task_definitions")` -> [ListTaskDefinitionsPaginator](./paginators.md#listtaskdefinitionspaginator)
- `client.get_paginator("list_tasks")` -> [ListTasksPaginator](./paginators.md#listtaskspaginator)




### get_waiter

Type annotations and code completion for `#!python session.client("ecs").get_waiter` method with overloads.

- `client.get_waiter("services_inactive")` -> [ServicesInactiveWaiter](./waiters.md#servicesinactivewaiter)
- `client.get_waiter("services_stable")` -> [ServicesStableWaiter](./waiters.md#servicesstablewaiter)
- `client.get_waiter("tasks_running")` -> [TasksRunningWaiter](./waiters.md#tasksrunningwaiter)
- `client.get_waiter("tasks_stopped")` -> [TasksStoppedWaiter](./waiters.md#tasksstoppedwaiter)
