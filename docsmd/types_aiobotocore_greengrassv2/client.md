# GreengrassV2Client

> [Index](../README.md) > [GreengrassV2](./README.md) > GreengrassV2Client

!!! note ""

    Auto-generated documentation for [GreengrassV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#greengrassv2)
    type annotations stubs module [types-aiobotocore-greengrassv2](https://pypi.org/project/types-aiobotocore-greengrassv2/).

## GreengrassV2Client

Type annotations and code completion for `#!python session.client("greengrassv2")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# GreengrassV2Client usage example

from aioboto3.session import Session
from types_aiobotocore_greengrassv2.client import GreengrassV2Client

session = Session()
async with session.client("greengrassv2") as client:
    client: GreengrassV2Client
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("greengrassv2").exceptions` structure.

```python
# GreengrassV2Client.exceptions usage example

async with session.client("greengrassv2") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.RequestAlreadyInProgressException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# GreengrassV2Client.exceptions type checking example

from types_aiobotocore_greengrassv2.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("greengrassv2").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("greengrassv2").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

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


### associate\_service\_role\_to\_account

Associates a Greengrass service role with IoT Greengrass for your Amazon Web
Services account in this Amazon Web Services Region.

Type annotations and code completion for `#!python session.client("greengrassv2").associate_service_role_to_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# associate_service_role_to_account method definition

await def associate_service_role_to_account(
    self,
    *,
    roleArn: str,
) -> AssociateServiceRoleToAccountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateServiceRoleToAccountResponseTypeDef](./type_defs.md#associateserviceroletoaccountresponsetypedef) 


```python
# associate_service_role_to_account method usage example with argument unpacking

kwargs: AssociateServiceRoleToAccountRequestRequestTypeDef = {  # (1)
    "roleArn": ...,
}

parent.associate_service_role_to_account(**kwargs)
```

1. See [:material-code-braces: AssociateServiceRoleToAccountRequestRequestTypeDef](./type_defs.md#associateserviceroletoaccountrequestrequesttypedef) 

### batch\_associate\_client\_device\_with\_core\_device

Associates a list of client devices with a core device.

Type annotations and code completion for `#!python session.client("greengrassv2").batch_associate_client_device_with_core_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# batch_associate_client_device_with_core_device method definition

await def batch_associate_client_device_with_core_device(
    self,
    *,
    coreDeviceThingName: str,
    entries: Sequence[AssociateClientDeviceWithCoreDeviceEntryTypeDef] = ...,  # (1)
) -> BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AssociateClientDeviceWithCoreDeviceEntryTypeDef](./type_defs.md#associateclientdevicewithcoredeviceentrytypedef) 
2. See [:material-code-braces: BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef](./type_defs.md#batchassociateclientdevicewithcoredeviceresponsetypedef) 


```python
# batch_associate_client_device_with_core_device method usage example with argument unpacking

kwargs: BatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef = {  # (1)
    "coreDeviceThingName": ...,
}

parent.batch_associate_client_device_with_core_device(**kwargs)
```

1. See [:material-code-braces: BatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef](./type_defs.md#batchassociateclientdevicewithcoredevicerequestrequesttypedef) 

### batch\_disassociate\_client\_device\_from\_core\_device

Disassociates a list of client devices from a core device.

Type annotations and code completion for `#!python session.client("greengrassv2").batch_disassociate_client_device_from_core_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# batch_disassociate_client_device_from_core_device method definition

await def batch_disassociate_client_device_from_core_device(
    self,
    *,
    coreDeviceThingName: str,
    entries: Sequence[DisassociateClientDeviceFromCoreDeviceEntryTypeDef] = ...,  # (1)
) -> BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DisassociateClientDeviceFromCoreDeviceEntryTypeDef](./type_defs.md#disassociateclientdevicefromcoredeviceentrytypedef) 
2. See [:material-code-braces: BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef](./type_defs.md#batchdisassociateclientdevicefromcoredeviceresponsetypedef) 


```python
# batch_disassociate_client_device_from_core_device method usage example with argument unpacking

kwargs: BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef = {  # (1)
    "coreDeviceThingName": ...,
}

parent.batch_disassociate_client_device_from_core_device(**kwargs)
```

1. See [:material-code-braces: BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef](./type_defs.md#batchdisassociateclientdevicefromcoredevicerequestrequesttypedef) 

### cancel\_deployment

Cancels a deployment.

Type annotations and code completion for `#!python session.client("greengrassv2").cancel_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# cancel_deployment method definition

await def cancel_deployment(
    self,
    *,
    deploymentId: str,
) -> CancelDeploymentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelDeploymentResponseTypeDef](./type_defs.md#canceldeploymentresponsetypedef) 


```python
# cancel_deployment method usage example with argument unpacking

kwargs: CancelDeploymentRequestRequestTypeDef = {  # (1)
    "deploymentId": ...,
}

parent.cancel_deployment(**kwargs)
```

1. See [:material-code-braces: CancelDeploymentRequestRequestTypeDef](./type_defs.md#canceldeploymentrequestrequesttypedef) 

### create\_component\_version

Creates a component.

Type annotations and code completion for `#!python session.client("greengrassv2").create_component_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# create_component_version method definition

await def create_component_version(
    self,
    *,
    inlineRecipe: BlobTypeDef = ...,
    lambdaFunction: LambdaFunctionRecipeSourceTypeDef = ...,  # (1)
    tags: Mapping[str, str] = ...,
    clientToken: str = ...,
) -> CreateComponentVersionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LambdaFunctionRecipeSourceTypeDef](./type_defs.md#lambdafunctionrecipesourcetypedef) 
2. See [:material-code-braces: CreateComponentVersionResponseTypeDef](./type_defs.md#createcomponentversionresponsetypedef) 


```python
# create_component_version method usage example with argument unpacking

kwargs: CreateComponentVersionRequestRequestTypeDef = {  # (1)
    "inlineRecipe": ...,
}

parent.create_component_version(**kwargs)
```

1. See [:material-code-braces: CreateComponentVersionRequestRequestTypeDef](./type_defs.md#createcomponentversionrequestrequesttypedef) 

### create\_deployment

Creates a continuous deployment for a target, which is a Greengrass core device
or group of core devices.

Type annotations and code completion for `#!python session.client("greengrassv2").create_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# create_deployment method definition

await def create_deployment(
    self,
    *,
    targetArn: str,
    deploymentName: str = ...,
    components: Mapping[str, ComponentDeploymentSpecificationUnionTypeDef] = ...,  # (1)
    iotJobConfiguration: DeploymentIoTJobConfigurationTypeDef = ...,  # (2)
    deploymentPolicies: DeploymentPoliciesTypeDef = ...,  # (3)
    parentTargetArn: str = ...,
    tags: Mapping[str, str] = ...,
    clientToken: str = ...,
) -> CreateDeploymentResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ComponentDeploymentSpecificationTypeDef](./type_defs.md#componentdeploymentspecificationtypedef) [:material-code-braces: ComponentDeploymentSpecificationOutputTypeDef](./type_defs.md#componentdeploymentspecificationoutputtypedef) 
2. See [:material-code-braces: DeploymentIoTJobConfigurationTypeDef](./type_defs.md#deploymentiotjobconfigurationtypedef) 
3. See [:material-code-braces: DeploymentPoliciesTypeDef](./type_defs.md#deploymentpoliciestypedef) 
4. See [:material-code-braces: CreateDeploymentResponseTypeDef](./type_defs.md#createdeploymentresponsetypedef) 


```python
# create_deployment method usage example with argument unpacking

kwargs: CreateDeploymentRequestRequestTypeDef = {  # (1)
    "targetArn": ...,
}

parent.create_deployment(**kwargs)
```

1. See [:material-code-braces: CreateDeploymentRequestRequestTypeDef](./type_defs.md#createdeploymentrequestrequesttypedef) 

### delete\_component

Deletes a version of a component from IoT Greengrass.

Type annotations and code completion for `#!python session.client("greengrassv2").delete_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# delete_component method definition

await def delete_component(
    self,
    *,
    arn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_component method usage example with argument unpacking

kwargs: DeleteComponentRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_component(**kwargs)
```

1. See [:material-code-braces: DeleteComponentRequestRequestTypeDef](./type_defs.md#deletecomponentrequestrequesttypedef) 

### delete\_core\_device

Deletes a Greengrass core device, which is an IoT thing.

Type annotations and code completion for `#!python session.client("greengrassv2").delete_core_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# delete_core_device method definition

await def delete_core_device(
    self,
    *,
    coreDeviceThingName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_core_device method usage example with argument unpacking

kwargs: DeleteCoreDeviceRequestRequestTypeDef = {  # (1)
    "coreDeviceThingName": ...,
}

parent.delete_core_device(**kwargs)
```

1. See [:material-code-braces: DeleteCoreDeviceRequestRequestTypeDef](./type_defs.md#deletecoredevicerequestrequesttypedef) 

### delete\_deployment

Deletes a deployment.

Type annotations and code completion for `#!python session.client("greengrassv2").delete_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# delete_deployment method definition

await def delete_deployment(
    self,
    *,
    deploymentId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_deployment method usage example with argument unpacking

kwargs: DeleteDeploymentRequestRequestTypeDef = {  # (1)
    "deploymentId": ...,
}

parent.delete_deployment(**kwargs)
```

1. See [:material-code-braces: DeleteDeploymentRequestRequestTypeDef](./type_defs.md#deletedeploymentrequestrequesttypedef) 

### describe\_component

Retrieves metadata for a version of a component.

Type annotations and code completion for `#!python session.client("greengrassv2").describe_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# describe_component method definition

await def describe_component(
    self,
    *,
    arn: str,
) -> DescribeComponentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeComponentResponseTypeDef](./type_defs.md#describecomponentresponsetypedef) 


```python
# describe_component method usage example with argument unpacking

kwargs: DescribeComponentRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.describe_component(**kwargs)
```

1. See [:material-code-braces: DescribeComponentRequestRequestTypeDef](./type_defs.md#describecomponentrequestrequesttypedef) 

### disassociate\_service\_role\_from\_account

Disassociates the Greengrass service role from IoT Greengrass for your Amazon
Web Services account in this Amazon Web Services Region.

Type annotations and code completion for `#!python session.client("greengrassv2").disassociate_service_role_from_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# disassociate_service_role_from_account method definition

await def disassociate_service_role_from_account(
    self,
) -> DisassociateServiceRoleFromAccountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisassociateServiceRoleFromAccountResponseTypeDef](./type_defs.md#disassociateservicerolefromaccountresponsetypedef) 

### get\_component

Gets the recipe for a version of a component.

Type annotations and code completion for `#!python session.client("greengrassv2").get_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# get_component method definition

await def get_component(
    self,
    *,
    arn: str,
    recipeOutputFormat: RecipeOutputFormatType = ...,  # (1)
) -> GetComponentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RecipeOutputFormatType](./literals.md#recipeoutputformattype) 
2. See [:material-code-braces: GetComponentResponseTypeDef](./type_defs.md#getcomponentresponsetypedef) 


```python
# get_component method usage example with argument unpacking

kwargs: GetComponentRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_component(**kwargs)
```

1. See [:material-code-braces: GetComponentRequestRequestTypeDef](./type_defs.md#getcomponentrequestrequesttypedef) 

### get\_component\_version\_artifact

Gets the pre-signed URL to download a public or a Lambda component artifact.

Type annotations and code completion for `#!python session.client("greengrassv2").get_component_version_artifact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# get_component_version_artifact method definition

await def get_component_version_artifact(
    self,
    *,
    arn: str,
    artifactName: str,
    s3EndpointType: S3EndpointTypeType = ...,  # (1)
    iotEndpointType: IotEndpointTypeType = ...,  # (2)
) -> GetComponentVersionArtifactResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: S3EndpointTypeType](./literals.md#s3endpointtypetype) 
2. See [:material-code-brackets: IotEndpointTypeType](./literals.md#iotendpointtypetype) 
3. See [:material-code-braces: GetComponentVersionArtifactResponseTypeDef](./type_defs.md#getcomponentversionartifactresponsetypedef) 


```python
# get_component_version_artifact method usage example with argument unpacking

kwargs: GetComponentVersionArtifactRequestRequestTypeDef = {  # (1)
    "arn": ...,
    "artifactName": ...,
}

parent.get_component_version_artifact(**kwargs)
```

1. See [:material-code-braces: GetComponentVersionArtifactRequestRequestTypeDef](./type_defs.md#getcomponentversionartifactrequestrequesttypedef) 

### get\_connectivity\_info

Retrieves connectivity information for a Greengrass core device.

Type annotations and code completion for `#!python session.client("greengrassv2").get_connectivity_info` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# get_connectivity_info method definition

await def get_connectivity_info(
    self,
    *,
    thingName: str,
) -> GetConnectivityInfoResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConnectivityInfoResponseTypeDef](./type_defs.md#getconnectivityinforesponsetypedef) 


```python
# get_connectivity_info method usage example with argument unpacking

kwargs: GetConnectivityInfoRequestRequestTypeDef = {  # (1)
    "thingName": ...,
}

parent.get_connectivity_info(**kwargs)
```

1. See [:material-code-braces: GetConnectivityInfoRequestRequestTypeDef](./type_defs.md#getconnectivityinforequestrequesttypedef) 

### get\_core\_device

Retrieves metadata for a Greengrass core device.

Type annotations and code completion for `#!python session.client("greengrassv2").get_core_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# get_core_device method definition

await def get_core_device(
    self,
    *,
    coreDeviceThingName: str,
) -> GetCoreDeviceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCoreDeviceResponseTypeDef](./type_defs.md#getcoredeviceresponsetypedef) 


```python
# get_core_device method usage example with argument unpacking

kwargs: GetCoreDeviceRequestRequestTypeDef = {  # (1)
    "coreDeviceThingName": ...,
}

parent.get_core_device(**kwargs)
```

1. See [:material-code-braces: GetCoreDeviceRequestRequestTypeDef](./type_defs.md#getcoredevicerequestrequesttypedef) 

### get\_deployment

Gets a deployment.

Type annotations and code completion for `#!python session.client("greengrassv2").get_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# get_deployment method definition

await def get_deployment(
    self,
    *,
    deploymentId: str,
) -> GetDeploymentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeploymentResponseTypeDef](./type_defs.md#getdeploymentresponsetypedef) 


```python
# get_deployment method usage example with argument unpacking

kwargs: GetDeploymentRequestRequestTypeDef = {  # (1)
    "deploymentId": ...,
}

parent.get_deployment(**kwargs)
```

1. See [:material-code-braces: GetDeploymentRequestRequestTypeDef](./type_defs.md#getdeploymentrequestrequesttypedef) 

### get\_service\_role\_for\_account

Gets the service role associated with IoT Greengrass for your Amazon Web
Services account in this Amazon Web Services Region.

Type annotations and code completion for `#!python session.client("greengrassv2").get_service_role_for_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# get_service_role_for_account method definition

await def get_service_role_for_account(
    self,
) -> GetServiceRoleForAccountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceRoleForAccountResponseTypeDef](./type_defs.md#getserviceroleforaccountresponsetypedef) 

### list\_client\_devices\_associated\_with\_core\_device

Retrieves a paginated list of client devices that are associated with a core
device.

Type annotations and code completion for `#!python session.client("greengrassv2").list_client_devices_associated_with_core_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# list_client_devices_associated_with_core_device method definition

await def list_client_devices_associated_with_core_device(
    self,
    *,
    coreDeviceThingName: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef](./type_defs.md#listclientdevicesassociatedwithcoredeviceresponsetypedef) 


```python
# list_client_devices_associated_with_core_device method usage example with argument unpacking

kwargs: ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef = {  # (1)
    "coreDeviceThingName": ...,
}

parent.list_client_devices_associated_with_core_device(**kwargs)
```

1. See [:material-code-braces: ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef](./type_defs.md#listclientdevicesassociatedwithcoredevicerequestrequesttypedef) 

### list\_component\_versions

Retrieves a paginated list of all versions for a component.

Type annotations and code completion for `#!python session.client("greengrassv2").list_component_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# list_component_versions method definition

await def list_component_versions(
    self,
    *,
    arn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListComponentVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListComponentVersionsResponseTypeDef](./type_defs.md#listcomponentversionsresponsetypedef) 


```python
# list_component_versions method usage example with argument unpacking

kwargs: ListComponentVersionsRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.list_component_versions(**kwargs)
```

1. See [:material-code-braces: ListComponentVersionsRequestRequestTypeDef](./type_defs.md#listcomponentversionsrequestrequesttypedef) 

### list\_components

Retrieves a paginated list of component summaries.

Type annotations and code completion for `#!python session.client("greengrassv2").list_components` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# list_components method definition

await def list_components(
    self,
    *,
    scope: ComponentVisibilityScopeType = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListComponentsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ComponentVisibilityScopeType](./literals.md#componentvisibilityscopetype) 
2. See [:material-code-braces: ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef) 


```python
# list_components method usage example with argument unpacking

kwargs: ListComponentsRequestRequestTypeDef = {  # (1)
    "scope": ...,
}

parent.list_components(**kwargs)
```

1. See [:material-code-braces: ListComponentsRequestRequestTypeDef](./type_defs.md#listcomponentsrequestrequesttypedef) 

### list\_core\_devices

Retrieves a paginated list of Greengrass core devices.

Type annotations and code completion for `#!python session.client("greengrassv2").list_core_devices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# list_core_devices method definition

await def list_core_devices(
    self,
    *,
    thingGroupArn: str = ...,
    status: CoreDeviceStatusType = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListCoreDevicesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: CoreDeviceStatusType](./literals.md#coredevicestatustype) 
2. See [:material-code-braces: ListCoreDevicesResponseTypeDef](./type_defs.md#listcoredevicesresponsetypedef) 


```python
# list_core_devices method usage example with argument unpacking

kwargs: ListCoreDevicesRequestRequestTypeDef = {  # (1)
    "thingGroupArn": ...,
}

parent.list_core_devices(**kwargs)
```

1. See [:material-code-braces: ListCoreDevicesRequestRequestTypeDef](./type_defs.md#listcoredevicesrequestrequesttypedef) 

### list\_deployments

Retrieves a paginated list of deployments.

Type annotations and code completion for `#!python session.client("greengrassv2").list_deployments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# list_deployments method definition

await def list_deployments(
    self,
    *,
    targetArn: str = ...,
    historyFilter: DeploymentHistoryFilterType = ...,  # (1)
    parentTargetArn: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListDeploymentsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DeploymentHistoryFilterType](./literals.md#deploymenthistoryfiltertype) 
2. See [:material-code-braces: ListDeploymentsResponseTypeDef](./type_defs.md#listdeploymentsresponsetypedef) 


```python
# list_deployments method usage example with argument unpacking

kwargs: ListDeploymentsRequestRequestTypeDef = {  # (1)
    "targetArn": ...,
}

parent.list_deployments(**kwargs)
```

1. See [:material-code-braces: ListDeploymentsRequestRequestTypeDef](./type_defs.md#listdeploymentsrequestrequesttypedef) 

### list\_effective\_deployments

Retrieves a paginated list of deployment jobs that IoT Greengrass sends to
Greengrass core devices.

Type annotations and code completion for `#!python session.client("greengrassv2").list_effective_deployments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# list_effective_deployments method definition

await def list_effective_deployments(
    self,
    *,
    coreDeviceThingName: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListEffectiveDeploymentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEffectiveDeploymentsResponseTypeDef](./type_defs.md#listeffectivedeploymentsresponsetypedef) 


```python
# list_effective_deployments method usage example with argument unpacking

kwargs: ListEffectiveDeploymentsRequestRequestTypeDef = {  # (1)
    "coreDeviceThingName": ...,
}

parent.list_effective_deployments(**kwargs)
```

1. See [:material-code-braces: ListEffectiveDeploymentsRequestRequestTypeDef](./type_defs.md#listeffectivedeploymentsrequestrequesttypedef) 

### list\_installed\_components

Retrieves a paginated list of the components that a Greengrass core device runs.

Type annotations and code completion for `#!python session.client("greengrassv2").list_installed_components` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# list_installed_components method definition

await def list_installed_components(
    self,
    *,
    coreDeviceThingName: str,
    maxResults: int = ...,
    nextToken: str = ...,
    topologyFilter: InstalledComponentTopologyFilterType = ...,  # (1)
) -> ListInstalledComponentsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: InstalledComponentTopologyFilterType](./literals.md#installedcomponenttopologyfiltertype) 
2. See [:material-code-braces: ListInstalledComponentsResponseTypeDef](./type_defs.md#listinstalledcomponentsresponsetypedef) 


```python
# list_installed_components method usage example with argument unpacking

kwargs: ListInstalledComponentsRequestRequestTypeDef = {  # (1)
    "coreDeviceThingName": ...,
}

parent.list_installed_components(**kwargs)
```

1. See [:material-code-braces: ListInstalledComponentsRequestRequestTypeDef](./type_defs.md#listinstalledcomponentsrequestrequesttypedef) 

### list\_tags\_for\_resource

Retrieves the list of tags for an IoT Greengrass resource.

Type annotations and code completion for `#!python session.client("greengrassv2").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

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

### resolve\_component\_candidates

Retrieves a list of components that meet the component, version, and platform
requirements of a deployment.

Type annotations and code completion for `#!python session.client("greengrassv2").resolve_component_candidates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# resolve_component_candidates method definition

await def resolve_component_candidates(
    self,
    *,
    platform: ComponentPlatformTypeDef = ...,  # (1)
    componentCandidates: Sequence[ComponentCandidateTypeDef] = ...,  # (2)
) -> ResolveComponentCandidatesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ComponentPlatformTypeDef](./type_defs.md#componentplatformtypedef) 
2. See [:material-code-braces: ComponentCandidateTypeDef](./type_defs.md#componentcandidatetypedef) 
3. See [:material-code-braces: ResolveComponentCandidatesResponseTypeDef](./type_defs.md#resolvecomponentcandidatesresponsetypedef) 


```python
# resolve_component_candidates method usage example with argument unpacking

kwargs: ResolveComponentCandidatesRequestRequestTypeDef = {  # (1)
    "platform": ...,
}

parent.resolve_component_candidates(**kwargs)
```

1. See [:material-code-braces: ResolveComponentCandidatesRequestRequestTypeDef](./type_defs.md#resolvecomponentcandidatesrequestrequesttypedef) 

### tag\_resource

Adds tags to an IoT Greengrass resource.

Type annotations and code completion for `#!python session.client("greengrassv2").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> dict[str, Any]:
    ...
```



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

Removes a tag from an IoT Greengrass resource.

Type annotations and code completion for `#!python session.client("greengrassv2").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

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

### update\_connectivity\_info

Updates connectivity information for a Greengrass core device.

Type annotations and code completion for `#!python session.client("greengrassv2").update_connectivity_info` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# update_connectivity_info method definition

await def update_connectivity_info(
    self,
    *,
    thingName: str,
    connectivityInfo: Sequence[ConnectivityInfoTypeDef],  # (1)
) -> UpdateConnectivityInfoResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConnectivityInfoTypeDef](./type_defs.md#connectivityinfotypedef) 
2. See [:material-code-braces: UpdateConnectivityInfoResponseTypeDef](./type_defs.md#updateconnectivityinforesponsetypedef) 


```python
# update_connectivity_info method usage example with argument unpacking

kwargs: UpdateConnectivityInfoRequestRequestTypeDef = {  # (1)
    "thingName": ...,
    "connectivityInfo": ...,
}

parent.update_connectivity_info(**kwargs)
```

1. See [:material-code-braces: UpdateConnectivityInfoRequestRequestTypeDef](./type_defs.md#updateconnectivityinforequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("greengrassv2").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("greengrassv2").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client)

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

Type annotations and code completion for `#!python session.client("greengrassv2").get_paginator` method with overloads.

- `client.get_paginator("list_client_devices_associated_with_core_device")` -> [ListClientDevicesAssociatedWithCoreDevicePaginator](./paginators.md#listclientdevicesassociatedwithcoredevicepaginator)
- `client.get_paginator("list_component_versions")` -> [ListComponentVersionsPaginator](./paginators.md#listcomponentversionspaginator)
- `client.get_paginator("list_components")` -> [ListComponentsPaginator](./paginators.md#listcomponentspaginator)
- `client.get_paginator("list_core_devices")` -> [ListCoreDevicesPaginator](./paginators.md#listcoredevicespaginator)
- `client.get_paginator("list_deployments")` -> [ListDeploymentsPaginator](./paginators.md#listdeploymentspaginator)
- `client.get_paginator("list_effective_deployments")` -> [ListEffectiveDeploymentsPaginator](./paginators.md#listeffectivedeploymentspaginator)
- `client.get_paginator("list_installed_components")` -> [ListInstalledComponentsPaginator](./paginators.md#listinstalledcomponentspaginator)


