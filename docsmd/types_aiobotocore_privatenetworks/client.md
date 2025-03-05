# Private5GClient

> [Index](../README.md) > [Private5G](./README.md) > Private5GClient

!!! note ""

    Auto-generated documentation for [Private5G](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#private5g)
    type annotations stubs module [types-aiobotocore-privatenetworks](https://pypi.org/project/types-aiobotocore-privatenetworks/).

## Private5GClient

Type annotations and code completion for `#!python session.client("privatenetworks")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# Private5GClient usage example

from aioboto3.session import Session
from types_aiobotocore_privatenetworks.client import Private5GClient

session = Session()
async with session.client("privatenetworks") as client:
    client: Private5GClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("privatenetworks").exceptions` structure.

```python
# Private5GClient.exceptions usage example

async with session.client("privatenetworks") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.InternalServerException,
        client.exceptions.LimitExceededException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# Private5GClient.exceptions type checking example

from types_aiobotocore_privatenetworks.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("privatenetworks").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("privatenetworks").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

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


### acknowledge\_order\_receipt

Acknowledges that the specified network order was received.

Type annotations and code completion for `#!python session.client("privatenetworks").acknowledge_order_receipt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# acknowledge_order_receipt method definition

await def acknowledge_order_receipt(
    self,
    *,
    orderArn: str,
) -> AcknowledgeOrderReceiptResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AcknowledgeOrderReceiptResponseTypeDef](./type_defs.md#acknowledgeorderreceiptresponsetypedef)


```python
# acknowledge_order_receipt method usage example with argument unpacking

kwargs: AcknowledgeOrderReceiptRequestTypeDef = {  # (1)
    "orderArn": ...,
}

parent.acknowledge_order_receipt(**kwargs)
```

1. See [:material-code-braces: AcknowledgeOrderReceiptRequestTypeDef](./type_defs.md#acknowledgeorderreceiptrequesttypedef)

### activate\_device\_identifier

Activates the specified device identifier.

Type annotations and code completion for `#!python session.client("privatenetworks").activate_device_identifier` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# activate_device_identifier method definition

await def activate_device_identifier(
    self,
    *,
    deviceIdentifierArn: str,
    clientToken: str = ...,
) -> ActivateDeviceIdentifierResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ActivateDeviceIdentifierResponseTypeDef](./type_defs.md#activatedeviceidentifierresponsetypedef)


```python
# activate_device_identifier method usage example with argument unpacking

kwargs: ActivateDeviceIdentifierRequestTypeDef = {  # (1)
    "deviceIdentifierArn": ...,
}

parent.activate_device_identifier(**kwargs)
```

1. See [:material-code-braces: ActivateDeviceIdentifierRequestTypeDef](./type_defs.md#activatedeviceidentifierrequesttypedef)

### activate\_network\_site

Activates the specified network site.

Type annotations and code completion for `#!python session.client("privatenetworks").activate_network_site` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# activate_network_site method definition

await def activate_network_site(
    self,
    *,
    networkSiteArn: str,
    shippingAddress: AddressTypeDef,  # (1)
    clientToken: str = ...,
    commitmentConfiguration: CommitmentConfigurationTypeDef = ...,  # (2)
) -> ActivateNetworkSiteResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef)
2. See [:material-code-braces: CommitmentConfigurationTypeDef](./type_defs.md#commitmentconfigurationtypedef)
3. See [:material-code-braces: ActivateNetworkSiteResponseTypeDef](./type_defs.md#activatenetworksiteresponsetypedef)


```python
# activate_network_site method usage example with argument unpacking

kwargs: ActivateNetworkSiteRequestTypeDef = {  # (1)
    "networkSiteArn": ...,
    "shippingAddress": ...,
}

parent.activate_network_site(**kwargs)
```

1. See [:material-code-braces: ActivateNetworkSiteRequestTypeDef](./type_defs.md#activatenetworksiterequesttypedef)

### configure\_access\_point

Configures the specified network resource.

Type annotations and code completion for `#!python session.client("privatenetworks").configure_access_point` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# configure_access_point method definition

await def configure_access_point(
    self,
    *,
    accessPointArn: str,
    cpiSecretKey: str = ...,
    cpiUserId: str = ...,
    cpiUserPassword: str = ...,
    cpiUsername: str = ...,
    position: PositionTypeDef = ...,  # (1)
) -> ConfigureAccessPointResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PositionTypeDef](./type_defs.md#positiontypedef)
2. See [:material-code-braces: ConfigureAccessPointResponseTypeDef](./type_defs.md#configureaccesspointresponsetypedef)


```python
# configure_access_point method usage example with argument unpacking

kwargs: ConfigureAccessPointRequestTypeDef = {  # (1)
    "accessPointArn": ...,
}

parent.configure_access_point(**kwargs)
```

1. See [:material-code-braces: ConfigureAccessPointRequestTypeDef](./type_defs.md#configureaccesspointrequesttypedef)

### create\_network

Creates a network.

Type annotations and code completion for `#!python session.client("privatenetworks").create_network` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# create_network method definition

await def create_network(
    self,
    *,
    networkName: str,
    clientToken: str = ...,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateNetworkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateNetworkResponseTypeDef](./type_defs.md#createnetworkresponsetypedef)


```python
# create_network method usage example with argument unpacking

kwargs: CreateNetworkRequestTypeDef = {  # (1)
    "networkName": ...,
}

parent.create_network(**kwargs)
```

1. See [:material-code-braces: CreateNetworkRequestTypeDef](./type_defs.md#createnetworkrequesttypedef)

### create\_network\_site

Creates a network site.

Type annotations and code completion for `#!python session.client("privatenetworks").create_network_site` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# create_network_site method definition

await def create_network_site(
    self,
    *,
    networkArn: str,
    networkSiteName: str,
    availabilityZone: str = ...,
    availabilityZoneId: str = ...,
    clientToken: str = ...,
    description: str = ...,
    pendingPlan: SitePlanUnionTypeDef = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> CreateNetworkSiteResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SitePlanUnionTypeDef](#siteplanuniontypedef)
2. See [:material-code-braces: CreateNetworkSiteResponseTypeDef](./type_defs.md#createnetworksiteresponsetypedef)


```python
# create_network_site method usage example with argument unpacking

kwargs: CreateNetworkSiteRequestTypeDef = {  # (1)
    "networkArn": ...,
    "networkSiteName": ...,
}

parent.create_network_site(**kwargs)
```

1. See [:material-code-braces: CreateNetworkSiteRequestTypeDef](./type_defs.md#createnetworksiterequesttypedef)

### deactivate\_device\_identifier

Deactivates the specified device identifier.

Type annotations and code completion for `#!python session.client("privatenetworks").deactivate_device_identifier` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# deactivate_device_identifier method definition

await def deactivate_device_identifier(
    self,
    *,
    deviceIdentifierArn: str,
    clientToken: str = ...,
) -> DeactivateDeviceIdentifierResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeactivateDeviceIdentifierResponseTypeDef](./type_defs.md#deactivatedeviceidentifierresponsetypedef)


```python
# deactivate_device_identifier method usage example with argument unpacking

kwargs: DeactivateDeviceIdentifierRequestTypeDef = {  # (1)
    "deviceIdentifierArn": ...,
}

parent.deactivate_device_identifier(**kwargs)
```

1. See [:material-code-braces: DeactivateDeviceIdentifierRequestTypeDef](./type_defs.md#deactivatedeviceidentifierrequesttypedef)

### delete\_network

Deletes the specified network.

Type annotations and code completion for `#!python session.client("privatenetworks").delete_network` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# delete_network method definition

await def delete_network(
    self,
    *,
    networkArn: str,
    clientToken: str = ...,
) -> DeleteNetworkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteNetworkResponseTypeDef](./type_defs.md#deletenetworkresponsetypedef)


```python
# delete_network method usage example with argument unpacking

kwargs: DeleteNetworkRequestTypeDef = {  # (1)
    "networkArn": ...,
}

parent.delete_network(**kwargs)
```

1. See [:material-code-braces: DeleteNetworkRequestTypeDef](./type_defs.md#deletenetworkrequesttypedef)

### delete\_network\_site

Deletes the specified network site.

Type annotations and code completion for `#!python session.client("privatenetworks").delete_network_site` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# delete_network_site method definition

await def delete_network_site(
    self,
    *,
    networkSiteArn: str,
    clientToken: str = ...,
) -> DeleteNetworkSiteResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteNetworkSiteResponseTypeDef](./type_defs.md#deletenetworksiteresponsetypedef)


```python
# delete_network_site method usage example with argument unpacking

kwargs: DeleteNetworkSiteRequestTypeDef = {  # (1)
    "networkSiteArn": ...,
}

parent.delete_network_site(**kwargs)
```

1. See [:material-code-braces: DeleteNetworkSiteRequestTypeDef](./type_defs.md#deletenetworksiterequesttypedef)

### get\_device\_identifier

Gets the specified device identifier.

Type annotations and code completion for `#!python session.client("privatenetworks").get_device_identifier` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# get_device_identifier method definition

await def get_device_identifier(
    self,
    *,
    deviceIdentifierArn: str,
) -> GetDeviceIdentifierResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeviceIdentifierResponseTypeDef](./type_defs.md#getdeviceidentifierresponsetypedef)


```python
# get_device_identifier method usage example with argument unpacking

kwargs: GetDeviceIdentifierRequestTypeDef = {  # (1)
    "deviceIdentifierArn": ...,
}

parent.get_device_identifier(**kwargs)
```

1. See [:material-code-braces: GetDeviceIdentifierRequestTypeDef](./type_defs.md#getdeviceidentifierrequesttypedef)

### get\_network

Gets the specified network.

Type annotations and code completion for `#!python session.client("privatenetworks").get_network` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# get_network method definition

await def get_network(
    self,
    *,
    networkArn: str,
) -> GetNetworkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetNetworkResponseTypeDef](./type_defs.md#getnetworkresponsetypedef)


```python
# get_network method usage example with argument unpacking

kwargs: GetNetworkRequestTypeDef = {  # (1)
    "networkArn": ...,
}

parent.get_network(**kwargs)
```

1. See [:material-code-braces: GetNetworkRequestTypeDef](./type_defs.md#getnetworkrequesttypedef)

### get\_network\_resource

Gets the specified network resource.

Type annotations and code completion for `#!python session.client("privatenetworks").get_network_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# get_network_resource method definition

await def get_network_resource(
    self,
    *,
    networkResourceArn: str,
) -> GetNetworkResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetNetworkResourceResponseTypeDef](./type_defs.md#getnetworkresourceresponsetypedef)


```python
# get_network_resource method usage example with argument unpacking

kwargs: GetNetworkResourceRequestTypeDef = {  # (1)
    "networkResourceArn": ...,
}

parent.get_network_resource(**kwargs)
```

1. See [:material-code-braces: GetNetworkResourceRequestTypeDef](./type_defs.md#getnetworkresourcerequesttypedef)

### get\_network\_site

Gets the specified network site.

Type annotations and code completion for `#!python session.client("privatenetworks").get_network_site` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# get_network_site method definition

await def get_network_site(
    self,
    *,
    networkSiteArn: str,
) -> GetNetworkSiteResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetNetworkSiteResponseTypeDef](./type_defs.md#getnetworksiteresponsetypedef)


```python
# get_network_site method usage example with argument unpacking

kwargs: GetNetworkSiteRequestTypeDef = {  # (1)
    "networkSiteArn": ...,
}

parent.get_network_site(**kwargs)
```

1. See [:material-code-braces: GetNetworkSiteRequestTypeDef](./type_defs.md#getnetworksiterequesttypedef)

### get\_order

Gets the specified order.

Type annotations and code completion for `#!python session.client("privatenetworks").get_order` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# get_order method definition

await def get_order(
    self,
    *,
    orderArn: str,
) -> GetOrderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOrderResponseTypeDef](./type_defs.md#getorderresponsetypedef)


```python
# get_order method usage example with argument unpacking

kwargs: GetOrderRequestTypeDef = {  # (1)
    "orderArn": ...,
}

parent.get_order(**kwargs)
```

1. See [:material-code-braces: GetOrderRequestTypeDef](./type_defs.md#getorderrequesttypedef)

### list\_device\_identifiers

Lists device identifiers.

Type annotations and code completion for `#!python session.client("privatenetworks").list_device_identifiers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# list_device_identifiers method definition

await def list_device_identifiers(
    self,
    *,
    networkArn: str,
    filters: Mapping[DeviceIdentifierFilterKeysType, Sequence[str]] = ...,  # (1)
    maxResults: int = ...,
    startToken: str = ...,
) -> ListDeviceIdentifiersResponseTypeDef:  # (2)
    ...
```

1. See `Mapping[DeviceIdentifierFilterKeysType, Sequence[str]]`
2. See [:material-code-braces: ListDeviceIdentifiersResponseTypeDef](./type_defs.md#listdeviceidentifiersresponsetypedef)


```python
# list_device_identifiers method usage example with argument unpacking

kwargs: ListDeviceIdentifiersRequestTypeDef = {  # (1)
    "networkArn": ...,
}

parent.list_device_identifiers(**kwargs)
```

1. See [:material-code-braces: ListDeviceIdentifiersRequestTypeDef](./type_defs.md#listdeviceidentifiersrequesttypedef)

### list\_network\_resources

Lists network resources.

Type annotations and code completion for `#!python session.client("privatenetworks").list_network_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# list_network_resources method definition

await def list_network_resources(
    self,
    *,
    networkArn: str,
    filters: Mapping[NetworkResourceFilterKeysType, Sequence[str]] = ...,  # (1)
    maxResults: int = ...,
    startToken: str = ...,
) -> ListNetworkResourcesResponseTypeDef:  # (2)
    ...
```

1. See `Mapping[NetworkResourceFilterKeysType, Sequence[str]]`
2. See [:material-code-braces: ListNetworkResourcesResponseTypeDef](./type_defs.md#listnetworkresourcesresponsetypedef)


```python
# list_network_resources method usage example with argument unpacking

kwargs: ListNetworkResourcesRequestTypeDef = {  # (1)
    "networkArn": ...,
}

parent.list_network_resources(**kwargs)
```

1. See [:material-code-braces: ListNetworkResourcesRequestTypeDef](./type_defs.md#listnetworkresourcesrequesttypedef)

### list\_network\_sites

Lists network sites.

Type annotations and code completion for `#!python session.client("privatenetworks").list_network_sites` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# list_network_sites method definition

await def list_network_sites(
    self,
    *,
    networkArn: str,
    filters: Mapping[NetworkSiteFilterKeysType, Sequence[str]] = ...,  # (1)
    maxResults: int = ...,
    startToken: str = ...,
) -> ListNetworkSitesResponseTypeDef:  # (2)
    ...
```

1. See `Mapping[Literal['STATUS'], Sequence[str]]`
2. See [:material-code-braces: ListNetworkSitesResponseTypeDef](./type_defs.md#listnetworksitesresponsetypedef)


```python
# list_network_sites method usage example with argument unpacking

kwargs: ListNetworkSitesRequestTypeDef = {  # (1)
    "networkArn": ...,
}

parent.list_network_sites(**kwargs)
```

1. See [:material-code-braces: ListNetworkSitesRequestTypeDef](./type_defs.md#listnetworksitesrequesttypedef)

### list\_networks

Lists networks.

Type annotations and code completion for `#!python session.client("privatenetworks").list_networks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# list_networks method definition

await def list_networks(
    self,
    *,
    filters: Mapping[NetworkFilterKeysType, Sequence[str]] = ...,  # (1)
    maxResults: int = ...,
    startToken: str = ...,
) -> ListNetworksResponseTypeDef:  # (2)
    ...
```

1. See `Mapping[Literal['STATUS'], Sequence[str]]`
2. See [:material-code-braces: ListNetworksResponseTypeDef](./type_defs.md#listnetworksresponsetypedef)


```python
# list_networks method usage example with argument unpacking

kwargs: ListNetworksRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.list_networks(**kwargs)
```

1. See [:material-code-braces: ListNetworksRequestTypeDef](./type_defs.md#listnetworksrequesttypedef)

### list\_orders

Lists orders.

Type annotations and code completion for `#!python session.client("privatenetworks").list_orders` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# list_orders method definition

await def list_orders(
    self,
    *,
    networkArn: str,
    filters: Mapping[OrderFilterKeysType, Sequence[str]] = ...,  # (1)
    maxResults: int = ...,
    startToken: str = ...,
) -> ListOrdersResponseTypeDef:  # (2)
    ...
```

1. See `Mapping[OrderFilterKeysType, Sequence[str]]`
2. See [:material-code-braces: ListOrdersResponseTypeDef](./type_defs.md#listordersresponsetypedef)


```python
# list_orders method usage example with argument unpacking

kwargs: ListOrdersRequestTypeDef = {  # (1)
    "networkArn": ...,
}

parent.list_orders(**kwargs)
```

1. See [:material-code-braces: ListOrdersRequestTypeDef](./type_defs.md#listordersrequesttypedef)

### list\_tags\_for\_resource

Lists the tags for the specified resource.

Type annotations and code completion for `#!python session.client("privatenetworks").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

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

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)

### ping

Checks the health of the service.

Type annotations and code completion for `#!python session.client("privatenetworks").ping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# ping method definition

await def ping(
    self,
) -> PingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PingResponseTypeDef](./type_defs.md#pingresponsetypedef)



### start\_network\_resource\_update

Use this action to do the following tasks:.

Type annotations and code completion for `#!python session.client("privatenetworks").start_network_resource_update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# start_network_resource_update method definition

await def start_network_resource_update(
    self,
    *,
    networkResourceArn: str,
    updateType: UpdateTypeType,  # (1)
    commitmentConfiguration: CommitmentConfigurationTypeDef = ...,  # (2)
    returnReason: str = ...,
    shippingAddress: AddressTypeDef = ...,  # (3)
) -> StartNetworkResourceUpdateResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: UpdateTypeType](./literals.md#updatetypetype)
2. See [:material-code-braces: CommitmentConfigurationTypeDef](./type_defs.md#commitmentconfigurationtypedef)
3. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef)
4. See [:material-code-braces: StartNetworkResourceUpdateResponseTypeDef](./type_defs.md#startnetworkresourceupdateresponsetypedef)


```python
# start_network_resource_update method usage example with argument unpacking

kwargs: StartNetworkResourceUpdateRequestTypeDef = {  # (1)
    "networkResourceArn": ...,
    "updateType": ...,
}

parent.start_network_resource_update(**kwargs)
```

1. See [:material-code-braces: StartNetworkResourceUpdateRequestTypeDef](./type_defs.md#startnetworkresourceupdaterequesttypedef)

### tag\_resource

Adds tags to the specified resource.

Type annotations and code completion for `#!python session.client("privatenetworks").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```

```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)

### untag\_resource

Removes tags from the specified resource.

Type annotations and code completion for `#!python session.client("privatenetworks").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```

```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)

### update\_network\_site

Updates the specified network site.

Type annotations and code completion for `#!python session.client("privatenetworks").update_network_site` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# update_network_site method definition

await def update_network_site(
    self,
    *,
    networkSiteArn: str,
    clientToken: str = ...,
    description: str = ...,
) -> UpdateNetworkSiteResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateNetworkSiteResponseTypeDef](./type_defs.md#updatenetworksiteresponsetypedef)


```python
# update_network_site method usage example with argument unpacking

kwargs: UpdateNetworkSiteRequestTypeDef = {  # (1)
    "networkSiteArn": ...,
}

parent.update_network_site(**kwargs)
```

1. See [:material-code-braces: UpdateNetworkSiteRequestTypeDef](./type_defs.md#updatenetworksiterequesttypedef)

### update\_network\_site\_plan

Updates the specified network site plan.

Type annotations and code completion for `#!python session.client("privatenetworks").update_network_site_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# update_network_site_plan method definition

await def update_network_site_plan(
    self,
    *,
    networkSiteArn: str,
    pendingPlan: SitePlanUnionTypeDef,  # (1)
    clientToken: str = ...,
) -> UpdateNetworkSiteResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SitePlanUnionTypeDef](#siteplanuniontypedef)
2. See [:material-code-braces: UpdateNetworkSiteResponseTypeDef](./type_defs.md#updatenetworksiteresponsetypedef)


```python
# update_network_site_plan method usage example with argument unpacking

kwargs: UpdateNetworkSitePlanRequestTypeDef = {  # (1)
    "networkSiteArn": ...,
    "pendingPlan": ...,
}

parent.update_network_site_plan(**kwargs)
```

1. See [:material-code-braces: UpdateNetworkSitePlanRequestTypeDef](./type_defs.md#updatenetworksiteplanrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("privatenetworks").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("privatenetworks").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("privatenetworks").get_paginator` method with overloads.

- `client.get_paginator("list_device_identifiers")` -> [ListDeviceIdentifiersPaginator](./paginators.md#listdeviceidentifierspaginator)
- `client.get_paginator("list_network_resources")` -> [ListNetworkResourcesPaginator](./paginators.md#listnetworkresourcespaginator)
- `client.get_paginator("list_network_sites")` -> [ListNetworkSitesPaginator](./paginators.md#listnetworksitespaginator)
- `client.get_paginator("list_networks")` -> [ListNetworksPaginator](./paginators.md#listnetworkspaginator)
- `client.get_paginator("list_orders")` -> [ListOrdersPaginator](./paginators.md#listorderspaginator)



