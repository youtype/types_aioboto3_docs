# BackupGatewayClient

> [Index](../README.md) > [BackupGateway](./README.md) > BackupGatewayClient

!!! note ""

    Auto-generated documentation for [BackupGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#backupgateway)
    type annotations stubs module [types-aiobotocore-backup-gateway](https://pypi.org/project/types-aiobotocore-backup-gateway/).

## BackupGatewayClient

Type annotations and code completion for `#!python session.client("backup-gateway")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# BackupGatewayClient usage example

from aioboto3.session import Session
from types_aiobotocore_backup_gateway.client import BackupGatewayClient

session = Session()
async with session.client("backup-gateway") as client:
    client: BackupGatewayClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("backup-gateway").exceptions` structure.

```python
# BackupGatewayClient.exceptions usage example

async with session.client("backup-gateway") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# BackupGatewayClient.exceptions type checking example

from types_aiobotocore_backup_gateway.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("backup-gateway").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("backup-gateway").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

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


### associate\_gateway\_to\_server

Associates a backup gateway with your server.

Type annotations and code completion for `#!python session.client("backup-gateway").associate_gateway_to_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# associate_gateway_to_server method definition

await def associate_gateway_to_server(
    self,
    *,
    GatewayArn: str,
    ServerArn: str,
) -> AssociateGatewayToServerOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateGatewayToServerOutputTypeDef](./type_defs.md#associategatewaytoserveroutputtypedef) 


```python
# associate_gateway_to_server method usage example with argument unpacking

kwargs: AssociateGatewayToServerInputRequestTypeDef = {  # (1)
    "GatewayArn": ...,
    "ServerArn": ...,
}

parent.associate_gateway_to_server(**kwargs)
```

1. See [:material-code-braces: AssociateGatewayToServerInputRequestTypeDef](./type_defs.md#associategatewaytoserverinputrequesttypedef) 

### create\_gateway

Creates a backup gateway.

Type annotations and code completion for `#!python session.client("backup-gateway").create_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# create_gateway method definition

await def create_gateway(
    self,
    *,
    ActivationKey: str,
    GatewayDisplayName: str,
    GatewayType: GatewayTypeType,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateGatewayOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: GatewayTypeType](./literals.md#gatewaytypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateGatewayOutputTypeDef](./type_defs.md#creategatewayoutputtypedef) 


```python
# create_gateway method usage example with argument unpacking

kwargs: CreateGatewayInputRequestTypeDef = {  # (1)
    "ActivationKey": ...,
    "GatewayDisplayName": ...,
    "GatewayType": ...,
}

parent.create_gateway(**kwargs)
```

1. See [:material-code-braces: CreateGatewayInputRequestTypeDef](./type_defs.md#creategatewayinputrequesttypedef) 

### delete\_gateway

Deletes a backup gateway.

Type annotations and code completion for `#!python session.client("backup-gateway").delete_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# delete_gateway method definition

await def delete_gateway(
    self,
    *,
    GatewayArn: str,
) -> DeleteGatewayOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteGatewayOutputTypeDef](./type_defs.md#deletegatewayoutputtypedef) 


```python
# delete_gateway method usage example with argument unpacking

kwargs: DeleteGatewayInputRequestTypeDef = {  # (1)
    "GatewayArn": ...,
}

parent.delete_gateway(**kwargs)
```

1. See [:material-code-braces: DeleteGatewayInputRequestTypeDef](./type_defs.md#deletegatewayinputrequesttypedef) 

### delete\_hypervisor

Deletes a hypervisor.

Type annotations and code completion for `#!python session.client("backup-gateway").delete_hypervisor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# delete_hypervisor method definition

await def delete_hypervisor(
    self,
    *,
    HypervisorArn: str,
) -> DeleteHypervisorOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteHypervisorOutputTypeDef](./type_defs.md#deletehypervisoroutputtypedef) 


```python
# delete_hypervisor method usage example with argument unpacking

kwargs: DeleteHypervisorInputRequestTypeDef = {  # (1)
    "HypervisorArn": ...,
}

parent.delete_hypervisor(**kwargs)
```

1. See [:material-code-braces: DeleteHypervisorInputRequestTypeDef](./type_defs.md#deletehypervisorinputrequesttypedef) 

### disassociate\_gateway\_from\_server

Disassociates a backup gateway from the specified server.

Type annotations and code completion for `#!python session.client("backup-gateway").disassociate_gateway_from_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# disassociate_gateway_from_server method definition

await def disassociate_gateway_from_server(
    self,
    *,
    GatewayArn: str,
) -> DisassociateGatewayFromServerOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisassociateGatewayFromServerOutputTypeDef](./type_defs.md#disassociategatewayfromserveroutputtypedef) 


```python
# disassociate_gateway_from_server method usage example with argument unpacking

kwargs: DisassociateGatewayFromServerInputRequestTypeDef = {  # (1)
    "GatewayArn": ...,
}

parent.disassociate_gateway_from_server(**kwargs)
```

1. See [:material-code-braces: DisassociateGatewayFromServerInputRequestTypeDef](./type_defs.md#disassociategatewayfromserverinputrequesttypedef) 

### get\_bandwidth\_rate\_limit\_schedule

Retrieves the bandwidth rate limit schedule for a specified gateway.

Type annotations and code completion for `#!python session.client("backup-gateway").get_bandwidth_rate_limit_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# get_bandwidth_rate_limit_schedule method definition

await def get_bandwidth_rate_limit_schedule(
    self,
    *,
    GatewayArn: str,
) -> GetBandwidthRateLimitScheduleOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBandwidthRateLimitScheduleOutputTypeDef](./type_defs.md#getbandwidthratelimitscheduleoutputtypedef) 


```python
# get_bandwidth_rate_limit_schedule method usage example with argument unpacking

kwargs: GetBandwidthRateLimitScheduleInputRequestTypeDef = {  # (1)
    "GatewayArn": ...,
}

parent.get_bandwidth_rate_limit_schedule(**kwargs)
```

1. See [:material-code-braces: GetBandwidthRateLimitScheduleInputRequestTypeDef](./type_defs.md#getbandwidthratelimitscheduleinputrequesttypedef) 

### get\_gateway

By providing the ARN (Amazon Resource Name), this API returns the gateway.

Type annotations and code completion for `#!python session.client("backup-gateway").get_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# get_gateway method definition

await def get_gateway(
    self,
    *,
    GatewayArn: str,
) -> GetGatewayOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGatewayOutputTypeDef](./type_defs.md#getgatewayoutputtypedef) 


```python
# get_gateway method usage example with argument unpacking

kwargs: GetGatewayInputRequestTypeDef = {  # (1)
    "GatewayArn": ...,
}

parent.get_gateway(**kwargs)
```

1. See [:material-code-braces: GetGatewayInputRequestTypeDef](./type_defs.md#getgatewayinputrequesttypedef) 

### get\_hypervisor

This action requests information about the specified hypervisor to which the
gateway will connect.

Type annotations and code completion for `#!python session.client("backup-gateway").get_hypervisor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# get_hypervisor method definition

await def get_hypervisor(
    self,
    *,
    HypervisorArn: str,
) -> GetHypervisorOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetHypervisorOutputTypeDef](./type_defs.md#gethypervisoroutputtypedef) 


```python
# get_hypervisor method usage example with argument unpacking

kwargs: GetHypervisorInputRequestTypeDef = {  # (1)
    "HypervisorArn": ...,
}

parent.get_hypervisor(**kwargs)
```

1. See [:material-code-braces: GetHypervisorInputRequestTypeDef](./type_defs.md#gethypervisorinputrequesttypedef) 

### get\_hypervisor\_property\_mappings

This action retrieves the property mappings for the specified hypervisor.

Type annotations and code completion for `#!python session.client("backup-gateway").get_hypervisor_property_mappings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# get_hypervisor_property_mappings method definition

await def get_hypervisor_property_mappings(
    self,
    *,
    HypervisorArn: str,
) -> GetHypervisorPropertyMappingsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetHypervisorPropertyMappingsOutputTypeDef](./type_defs.md#gethypervisorpropertymappingsoutputtypedef) 


```python
# get_hypervisor_property_mappings method usage example with argument unpacking

kwargs: GetHypervisorPropertyMappingsInputRequestTypeDef = {  # (1)
    "HypervisorArn": ...,
}

parent.get_hypervisor_property_mappings(**kwargs)
```

1. See [:material-code-braces: GetHypervisorPropertyMappingsInputRequestTypeDef](./type_defs.md#gethypervisorpropertymappingsinputrequesttypedef) 

### get\_virtual\_machine

By providing the ARN (Amazon Resource Name), this API returns the virtual
machine.

Type annotations and code completion for `#!python session.client("backup-gateway").get_virtual_machine` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# get_virtual_machine method definition

await def get_virtual_machine(
    self,
    *,
    ResourceArn: str,
) -> GetVirtualMachineOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVirtualMachineOutputTypeDef](./type_defs.md#getvirtualmachineoutputtypedef) 


```python
# get_virtual_machine method usage example with argument unpacking

kwargs: GetVirtualMachineInputRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_virtual_machine(**kwargs)
```

1. See [:material-code-braces: GetVirtualMachineInputRequestTypeDef](./type_defs.md#getvirtualmachineinputrequesttypedef) 

### import\_hypervisor\_configuration

Connect to a hypervisor by importing its configuration.

Type annotations and code completion for `#!python session.client("backup-gateway").import_hypervisor_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# import_hypervisor_configuration method definition

await def import_hypervisor_configuration(
    self,
    *,
    Host: str,
    Name: str,
    KmsKeyArn: str = ...,
    Password: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    Username: str = ...,
) -> ImportHypervisorConfigurationOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ImportHypervisorConfigurationOutputTypeDef](./type_defs.md#importhypervisorconfigurationoutputtypedef) 


```python
# import_hypervisor_configuration method usage example with argument unpacking

kwargs: ImportHypervisorConfigurationInputRequestTypeDef = {  # (1)
    "Host": ...,
    "Name": ...,
}

parent.import_hypervisor_configuration(**kwargs)
```

1. See [:material-code-braces: ImportHypervisorConfigurationInputRequestTypeDef](./type_defs.md#importhypervisorconfigurationinputrequesttypedef) 

### list\_gateways

Lists backup gateways owned by an Amazon Web Services account in an Amazon Web
Services Region.

Type annotations and code completion for `#!python session.client("backup-gateway").list_gateways` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# list_gateways method definition

await def list_gateways(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListGatewaysOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGatewaysOutputTypeDef](./type_defs.md#listgatewaysoutputtypedef) 


```python
# list_gateways method usage example with argument unpacking

kwargs: ListGatewaysInputRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_gateways(**kwargs)
```

1. See [:material-code-braces: ListGatewaysInputRequestTypeDef](./type_defs.md#listgatewaysinputrequesttypedef) 

### list\_hypervisors

Lists your hypervisors.

Type annotations and code completion for `#!python session.client("backup-gateway").list_hypervisors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# list_hypervisors method definition

await def list_hypervisors(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListHypervisorsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListHypervisorsOutputTypeDef](./type_defs.md#listhypervisorsoutputtypedef) 


```python
# list_hypervisors method usage example with argument unpacking

kwargs: ListHypervisorsInputRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_hypervisors(**kwargs)
```

1. See [:material-code-braces: ListHypervisorsInputRequestTypeDef](./type_defs.md#listhypervisorsinputrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags applied to the resource identified by its Amazon Resource Name
(ARN).

Type annotations and code completion for `#!python session.client("backup-gateway").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef) 

### list\_virtual\_machines

Lists your virtual machines.

Type annotations and code completion for `#!python session.client("backup-gateway").list_virtual_machines` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# list_virtual_machines method definition

await def list_virtual_machines(
    self,
    *,
    HypervisorArn: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListVirtualMachinesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVirtualMachinesOutputTypeDef](./type_defs.md#listvirtualmachinesoutputtypedef) 


```python
# list_virtual_machines method usage example with argument unpacking

kwargs: ListVirtualMachinesInputRequestTypeDef = {  # (1)
    "HypervisorArn": ...,
}

parent.list_virtual_machines(**kwargs)
```

1. See [:material-code-braces: ListVirtualMachinesInputRequestTypeDef](./type_defs.md#listvirtualmachinesinputrequesttypedef) 

### put\_bandwidth\_rate\_limit\_schedule

This action sets the bandwidth rate limit schedule for a specified gateway.

Type annotations and code completion for `#!python session.client("backup-gateway").put_bandwidth_rate_limit_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# put_bandwidth_rate_limit_schedule method definition

await def put_bandwidth_rate_limit_schedule(
    self,
    *,
    BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalUnionTypeDef],  # (1)
    GatewayArn: str,
) -> PutBandwidthRateLimitScheduleOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BandwidthRateLimitIntervalTypeDef](./type_defs.md#bandwidthratelimitintervaltypedef) [:material-code-braces: BandwidthRateLimitIntervalOutputTypeDef](./type_defs.md#bandwidthratelimitintervaloutputtypedef) 
2. See [:material-code-braces: PutBandwidthRateLimitScheduleOutputTypeDef](./type_defs.md#putbandwidthratelimitscheduleoutputtypedef) 


```python
# put_bandwidth_rate_limit_schedule method usage example with argument unpacking

kwargs: PutBandwidthRateLimitScheduleInputRequestTypeDef = {  # (1)
    "BandwidthRateLimitIntervals": ...,
    "GatewayArn": ...,
}

parent.put_bandwidth_rate_limit_schedule(**kwargs)
```

1. See [:material-code-braces: PutBandwidthRateLimitScheduleInputRequestTypeDef](./type_defs.md#putbandwidthratelimitscheduleinputrequesttypedef) 

### put\_hypervisor\_property\_mappings

This action sets the property mappings for the specified hypervisor.

Type annotations and code completion for `#!python session.client("backup-gateway").put_hypervisor_property_mappings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# put_hypervisor_property_mappings method definition

await def put_hypervisor_property_mappings(
    self,
    *,
    HypervisorArn: str,
    IamRoleArn: str,
    VmwareToAwsTagMappings: Sequence[VmwareToAwsTagMappingTypeDef],  # (1)
) -> PutHypervisorPropertyMappingsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VmwareToAwsTagMappingTypeDef](./type_defs.md#vmwaretoawstagmappingtypedef) 
2. See [:material-code-braces: PutHypervisorPropertyMappingsOutputTypeDef](./type_defs.md#puthypervisorpropertymappingsoutputtypedef) 


```python
# put_hypervisor_property_mappings method usage example with argument unpacking

kwargs: PutHypervisorPropertyMappingsInputRequestTypeDef = {  # (1)
    "HypervisorArn": ...,
    "IamRoleArn": ...,
    "VmwareToAwsTagMappings": ...,
}

parent.put_hypervisor_property_mappings(**kwargs)
```

1. See [:material-code-braces: PutHypervisorPropertyMappingsInputRequestTypeDef](./type_defs.md#puthypervisorpropertymappingsinputrequesttypedef) 

### put\_maintenance\_start\_time

Set the maintenance start time for a gateway.

Type annotations and code completion for `#!python session.client("backup-gateway").put_maintenance_start_time` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# put_maintenance_start_time method definition

await def put_maintenance_start_time(
    self,
    *,
    GatewayArn: str,
    HourOfDay: int,
    MinuteOfHour: int,
    DayOfMonth: int = ...,
    DayOfWeek: int = ...,
) -> PutMaintenanceStartTimeOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutMaintenanceStartTimeOutputTypeDef](./type_defs.md#putmaintenancestarttimeoutputtypedef) 


```python
# put_maintenance_start_time method usage example with argument unpacking

kwargs: PutMaintenanceStartTimeInputRequestTypeDef = {  # (1)
    "GatewayArn": ...,
    "HourOfDay": ...,
    "MinuteOfHour": ...,
}

parent.put_maintenance_start_time(**kwargs)
```

1. See [:material-code-braces: PutMaintenanceStartTimeInputRequestTypeDef](./type_defs.md#putmaintenancestarttimeinputrequesttypedef) 

### start\_virtual\_machines\_metadata\_sync

This action sends a request to sync metadata across the specified virtual
machines.

Type annotations and code completion for `#!python session.client("backup-gateway").start_virtual_machines_metadata_sync` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# start_virtual_machines_metadata_sync method definition

await def start_virtual_machines_metadata_sync(
    self,
    *,
    HypervisorArn: str,
) -> StartVirtualMachinesMetadataSyncOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartVirtualMachinesMetadataSyncOutputTypeDef](./type_defs.md#startvirtualmachinesmetadatasyncoutputtypedef) 


```python
# start_virtual_machines_metadata_sync method usage example with argument unpacking

kwargs: StartVirtualMachinesMetadataSyncInputRequestTypeDef = {  # (1)
    "HypervisorArn": ...,
}

parent.start_virtual_machines_metadata_sync(**kwargs)
```

1. See [:material-code-braces: StartVirtualMachinesMetadataSyncInputRequestTypeDef](./type_defs.md#startvirtualmachinesmetadatasyncinputrequesttypedef) 

### tag\_resource

Tag the resource.

Type annotations and code completion for `#!python session.client("backup-gateway").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> TagResourceOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: TagResourceOutputTypeDef](./type_defs.md#tagresourceoutputtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef) 

### test\_hypervisor\_configuration

Tests your hypervisor configuration to validate that backup gateway can connect
with the hypervisor and its resources.

Type annotations and code completion for `#!python session.client("backup-gateway").test_hypervisor_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# test_hypervisor_configuration method definition

await def test_hypervisor_configuration(
    self,
    *,
    GatewayArn: str,
    Host: str,
    Password: str = ...,
    Username: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# test_hypervisor_configuration method usage example with argument unpacking

kwargs: TestHypervisorConfigurationInputRequestTypeDef = {  # (1)
    "GatewayArn": ...,
    "Host": ...,
}

parent.test_hypervisor_configuration(**kwargs)
```

1. See [:material-code-braces: TestHypervisorConfigurationInputRequestTypeDef](./type_defs.md#testhypervisorconfigurationinputrequesttypedef) 

### untag\_resource

Removes tags from the resource.

Type annotations and code completion for `#!python session.client("backup-gateway").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> UntagResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UntagResourceOutputTypeDef](./type_defs.md#untagresourceoutputtypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceInputRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef) 

### update\_gateway\_information

Updates a gateway's name.

Type annotations and code completion for `#!python session.client("backup-gateway").update_gateway_information` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# update_gateway_information method definition

await def update_gateway_information(
    self,
    *,
    GatewayArn: str,
    GatewayDisplayName: str = ...,
) -> UpdateGatewayInformationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateGatewayInformationOutputTypeDef](./type_defs.md#updategatewayinformationoutputtypedef) 


```python
# update_gateway_information method usage example with argument unpacking

kwargs: UpdateGatewayInformationInputRequestTypeDef = {  # (1)
    "GatewayArn": ...,
}

parent.update_gateway_information(**kwargs)
```

1. See [:material-code-braces: UpdateGatewayInformationInputRequestTypeDef](./type_defs.md#updategatewayinformationinputrequesttypedef) 

### update\_gateway\_software\_now

Updates the gateway virtual machine (VM) software.

Type annotations and code completion for `#!python session.client("backup-gateway").update_gateway_software_now` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# update_gateway_software_now method definition

await def update_gateway_software_now(
    self,
    *,
    GatewayArn: str,
) -> UpdateGatewaySoftwareNowOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateGatewaySoftwareNowOutputTypeDef](./type_defs.md#updategatewaysoftwarenowoutputtypedef) 


```python
# update_gateway_software_now method usage example with argument unpacking

kwargs: UpdateGatewaySoftwareNowInputRequestTypeDef = {  # (1)
    "GatewayArn": ...,
}

parent.update_gateway_software_now(**kwargs)
```

1. See [:material-code-braces: UpdateGatewaySoftwareNowInputRequestTypeDef](./type_defs.md#updategatewaysoftwarenowinputrequesttypedef) 

### update\_hypervisor

Updates a hypervisor metadata, including its host, username, and password.

Type annotations and code completion for `#!python session.client("backup-gateway").update_hypervisor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# update_hypervisor method definition

await def update_hypervisor(
    self,
    *,
    HypervisorArn: str,
    Host: str = ...,
    LogGroupArn: str = ...,
    Name: str = ...,
    Password: str = ...,
    Username: str = ...,
) -> UpdateHypervisorOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateHypervisorOutputTypeDef](./type_defs.md#updatehypervisoroutputtypedef) 


```python
# update_hypervisor method usage example with argument unpacking

kwargs: UpdateHypervisorInputRequestTypeDef = {  # (1)
    "HypervisorArn": ...,
}

parent.update_hypervisor(**kwargs)
```

1. See [:material-code-braces: UpdateHypervisorInputRequestTypeDef](./type_defs.md#updatehypervisorinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("backup-gateway").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("backup-gateway").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

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

Type annotations and code completion for `#!python session.client("backup-gateway").get_paginator` method with overloads.

- `client.get_paginator("list_gateways")` -> [ListGatewaysPaginator](./paginators.md#listgatewayspaginator)
- `client.get_paginator("list_hypervisors")` -> [ListHypervisorsPaginator](./paginators.md#listhypervisorspaginator)
- `client.get_paginator("list_virtual_machines")` -> [ListVirtualMachinesPaginator](./paginators.md#listvirtualmachinespaginator)


