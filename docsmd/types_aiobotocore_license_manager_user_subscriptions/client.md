# LicenseManagerUserSubscriptionsClient

> [Index](../README.md) > [LicenseManagerUserSubscriptions](./README.md) > LicenseManagerUserSubscriptionsClient

!!! note ""

    Auto-generated documentation for [LicenseManagerUserSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#licensemanagerusersubscriptions)
    type annotations stubs module [types-aiobotocore-license-manager-user-subscriptions](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions/).

## LicenseManagerUserSubscriptionsClient

Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# LicenseManagerUserSubscriptionsClient usage example

from aioboto3.session import Session
from types_aiobotocore_license_manager_user_subscriptions.client import LicenseManagerUserSubscriptionsClient

session = Session()
async with session.client("license-manager-user-subscriptions") as client:
    client: LicenseManagerUserSubscriptionsClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("license-manager-user-subscriptions").exceptions` structure.

```python
# LicenseManagerUserSubscriptionsClient.exceptions usage example

async with session.client("license-manager-user-subscriptions") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# LicenseManagerUserSubscriptionsClient.exceptions type checking example

from types_aiobotocore_license_manager_user_subscriptions.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

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


### associate\_user

Associates the user to an EC2 instance to utilize user-based subscriptions.

Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").associate_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# associate_user method definition

await def associate_user(
    self,
    *,
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    InstanceId: str,
    Username: str,
    Domain: str = ...,
    Tags: Mapping[str, str] = ...,
) -> AssociateUserResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: AssociateUserResponseTypeDef](./type_defs.md#associateuserresponsetypedef) 


```python
# associate_user method usage example with argument unpacking

kwargs: AssociateUserRequestRequestTypeDef = {  # (1)
    "IdentityProvider": ...,
    "InstanceId": ...,
    "Username": ...,
}

parent.associate_user(**kwargs)
```

1. See [:material-code-braces: AssociateUserRequestRequestTypeDef](./type_defs.md#associateuserrequestrequesttypedef) 

### create\_license\_server\_endpoint

Creates a network endpoint for the Remote Desktop Services (RDS) license server.

Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").create_license_server_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# create_license_server_endpoint method definition

await def create_license_server_endpoint(
    self,
    *,
    IdentityProviderArn: str,
    LicenseServerSettings: LicenseServerSettingsTypeDef,  # (1)
    Tags: Mapping[str, str] = ...,
) -> CreateLicenseServerEndpointResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LicenseServerSettingsTypeDef](./type_defs.md#licenseserversettingstypedef) 
2. See [:material-code-braces: CreateLicenseServerEndpointResponseTypeDef](./type_defs.md#createlicenseserverendpointresponsetypedef) 


```python
# create_license_server_endpoint method usage example with argument unpacking

kwargs: CreateLicenseServerEndpointRequestRequestTypeDef = {  # (1)
    "IdentityProviderArn": ...,
    "LicenseServerSettings": ...,
}

parent.create_license_server_endpoint(**kwargs)
```

1. See [:material-code-braces: CreateLicenseServerEndpointRequestRequestTypeDef](./type_defs.md#createlicenseserverendpointrequestrequesttypedef) 

### delete\_license\_server\_endpoint

Deletes a <code>LicenseServerEndpoint</code> resource.

Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").delete_license_server_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# delete_license_server_endpoint method definition

await def delete_license_server_endpoint(
    self,
    *,
    LicenseServerEndpointArn: str,
    ServerType: ServerTypeType,  # (1)
) -> DeleteLicenseServerEndpointResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ServerTypeType](./literals.md#servertypetype) 
2. See [:material-code-braces: DeleteLicenseServerEndpointResponseTypeDef](./type_defs.md#deletelicenseserverendpointresponsetypedef) 


```python
# delete_license_server_endpoint method usage example with argument unpacking

kwargs: DeleteLicenseServerEndpointRequestRequestTypeDef = {  # (1)
    "LicenseServerEndpointArn": ...,
    "ServerType": ...,
}

parent.delete_license_server_endpoint(**kwargs)
```

1. See [:material-code-braces: DeleteLicenseServerEndpointRequestRequestTypeDef](./type_defs.md#deletelicenseserverendpointrequestrequesttypedef) 

### deregister\_identity\_provider

Deregisters the Active Directory identity provider from License Manager
user-based subscriptions.

Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").deregister_identity_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# deregister_identity_provider method definition

await def deregister_identity_provider(
    self,
    *,
    IdentityProvider: IdentityProviderTypeDef = ...,  # (1)
    IdentityProviderArn: str = ...,
    Product: str = ...,
) -> DeregisterIdentityProviderResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: DeregisterIdentityProviderResponseTypeDef](./type_defs.md#deregisteridentityproviderresponsetypedef) 


```python
# deregister_identity_provider method usage example with argument unpacking

kwargs: DeregisterIdentityProviderRequestRequestTypeDef = {  # (1)
    "IdentityProvider": ...,
}

parent.deregister_identity_provider(**kwargs)
```

1. See [:material-code-braces: DeregisterIdentityProviderRequestRequestTypeDef](./type_defs.md#deregisteridentityproviderrequestrequesttypedef) 

### disassociate\_user

Disassociates the user from an EC2 instance providing user-based subscriptions.

Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").disassociate_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# disassociate_user method definition

await def disassociate_user(
    self,
    *,
    Domain: str = ...,
    IdentityProvider: IdentityProviderTypeDef = ...,  # (1)
    InstanceId: str = ...,
    InstanceUserArn: str = ...,
    Username: str = ...,
) -> DisassociateUserResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: DisassociateUserResponseTypeDef](./type_defs.md#disassociateuserresponsetypedef) 


```python
# disassociate_user method usage example with argument unpacking

kwargs: DisassociateUserRequestRequestTypeDef = {  # (1)
    "Domain": ...,
}

parent.disassociate_user(**kwargs)
```

1. See [:material-code-braces: DisassociateUserRequestRequestTypeDef](./type_defs.md#disassociateuserrequestrequesttypedef) 

### list\_identity\_providers

Lists the Active Directory identity providers for user-based subscriptions.

Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").list_identity_providers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# list_identity_providers method definition

await def list_identity_providers(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListIdentityProvidersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListIdentityProvidersResponseTypeDef](./type_defs.md#listidentityprovidersresponsetypedef) 


```python
# list_identity_providers method usage example with argument unpacking

kwargs: ListIdentityProvidersRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.list_identity_providers(**kwargs)
```

1. See [:material-code-braces: ListIdentityProvidersRequestRequestTypeDef](./type_defs.md#listidentityprovidersrequestrequesttypedef) 

### list\_instances

Lists the EC2 instances providing user-based subscriptions.

Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").list_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# list_instances method definition

await def list_instances(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListInstancesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef) 


```python
# list_instances method usage example with argument unpacking

kwargs: ListInstancesRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.list_instances(**kwargs)
```

1. See [:material-code-braces: ListInstancesRequestRequestTypeDef](./type_defs.md#listinstancesrequestrequesttypedef) 

### list\_license\_server\_endpoints

List the Remote Desktop Services (RDS) License Server endpoints.

Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").list_license_server_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# list_license_server_endpoints method definition

await def list_license_server_endpoints(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListLicenseServerEndpointsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListLicenseServerEndpointsResponseTypeDef](./type_defs.md#listlicenseserverendpointsresponsetypedef) 


```python
# list_license_server_endpoints method usage example with argument unpacking

kwargs: ListLicenseServerEndpointsRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.list_license_server_endpoints(**kwargs)
```

1. See [:material-code-braces: ListLicenseServerEndpointsRequestRequestTypeDef](./type_defs.md#listlicenseserverendpointsrequestrequesttypedef) 

### list\_product\_subscriptions

Lists the user-based subscription products available from an identity provider.

Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").list_product_subscriptions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# list_product_subscriptions method definition

await def list_product_subscriptions(
    self,
    *,
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    Filters: Sequence[FilterTypeDef] = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
    Product: str = ...,
) -> ListProductSubscriptionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: ListProductSubscriptionsResponseTypeDef](./type_defs.md#listproductsubscriptionsresponsetypedef) 


```python
# list_product_subscriptions method usage example with argument unpacking

kwargs: ListProductSubscriptionsRequestRequestTypeDef = {  # (1)
    "IdentityProvider": ...,
}

parent.list_product_subscriptions(**kwargs)
```

1. See [:material-code-braces: ListProductSubscriptionsRequestRequestTypeDef](./type_defs.md#listproductsubscriptionsrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns the list of tags for the specified resource.

Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_user\_associations

Lists user associations for an identity provider.

Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").list_user_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# list_user_associations method definition

await def list_user_associations(
    self,
    *,
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    InstanceId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListUserAssociationsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: ListUserAssociationsResponseTypeDef](./type_defs.md#listuserassociationsresponsetypedef) 


```python
# list_user_associations method usage example with argument unpacking

kwargs: ListUserAssociationsRequestRequestTypeDef = {  # (1)
    "IdentityProvider": ...,
    "InstanceId": ...,
}

parent.list_user_associations(**kwargs)
```

1. See [:material-code-braces: ListUserAssociationsRequestRequestTypeDef](./type_defs.md#listuserassociationsrequestrequesttypedef) 

### register\_identity\_provider

Registers an identity provider for user-based subscriptions.

Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").register_identity_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# register_identity_provider method definition

await def register_identity_provider(
    self,
    *,
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    Product: str,
    Settings: SettingsTypeDef = ...,  # (2)
    Tags: Mapping[str, str] = ...,
) -> RegisterIdentityProviderResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: SettingsTypeDef](./type_defs.md#settingstypedef) 
3. See [:material-code-braces: RegisterIdentityProviderResponseTypeDef](./type_defs.md#registeridentityproviderresponsetypedef) 


```python
# register_identity_provider method usage example with argument unpacking

kwargs: RegisterIdentityProviderRequestRequestTypeDef = {  # (1)
    "IdentityProvider": ...,
    "Product": ...,
}

parent.register_identity_provider(**kwargs)
```

1. See [:material-code-braces: RegisterIdentityProviderRequestRequestTypeDef](./type_defs.md#registeridentityproviderrequestrequesttypedef) 

### start\_product\_subscription

Starts a product subscription for a user with the specified identity provider.

Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").start_product_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# start_product_subscription method definition

await def start_product_subscription(
    self,
    *,
    IdentityProvider: IdentityProviderTypeDef,  # (1)
    Product: str,
    Username: str,
    Domain: str = ...,
    Tags: Mapping[str, str] = ...,
) -> StartProductSubscriptionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: StartProductSubscriptionResponseTypeDef](./type_defs.md#startproductsubscriptionresponsetypedef) 


```python
# start_product_subscription method usage example with argument unpacking

kwargs: StartProductSubscriptionRequestRequestTypeDef = {  # (1)
    "IdentityProvider": ...,
    "Product": ...,
    "Username": ...,
}

parent.start_product_subscription(**kwargs)
```

1. See [:material-code-braces: StartProductSubscriptionRequestRequestTypeDef](./type_defs.md#startproductsubscriptionrequestrequesttypedef) 

### stop\_product\_subscription

Stops a product subscription for a user with the specified identity provider.

Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").stop_product_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# stop_product_subscription method definition

await def stop_product_subscription(
    self,
    *,
    Domain: str = ...,
    IdentityProvider: IdentityProviderTypeDef = ...,  # (1)
    Product: str = ...,
    ProductUserArn: str = ...,
    Username: str = ...,
) -> StopProductSubscriptionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
2. See [:material-code-braces: StopProductSubscriptionResponseTypeDef](./type_defs.md#stopproductsubscriptionresponsetypedef) 


```python
# stop_product_subscription method usage example with argument unpacking

kwargs: StopProductSubscriptionRequestRequestTypeDef = {  # (1)
    "Domain": ...,
}

parent.stop_product_subscription(**kwargs)
```

1. See [:material-code-braces: StopProductSubscriptionRequestRequestTypeDef](./type_defs.md#stopproductsubscriptionrequestrequesttypedef) 

### tag\_resource

Adds tags to a resource.

Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes tags from a resource.

Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_identity\_provider\_settings

Updates additional product configuration settings for the registered identity
provider.

Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").update_identity_provider_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# update_identity_provider_settings method definition

await def update_identity_provider_settings(
    self,
    *,
    UpdateSettings: UpdateSettingsTypeDef,  # (1)
    IdentityProvider: IdentityProviderTypeDef = ...,  # (2)
    IdentityProviderArn: str = ...,
    Product: str = ...,
) -> UpdateIdentityProviderSettingsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: UpdateSettingsTypeDef](./type_defs.md#updatesettingstypedef) 
2. See [:material-code-braces: IdentityProviderTypeDef](./type_defs.md#identityprovidertypedef) 
3. See [:material-code-braces: UpdateIdentityProviderSettingsResponseTypeDef](./type_defs.md#updateidentityprovidersettingsresponsetypedef) 


```python
# update_identity_provider_settings method usage example with argument unpacking

kwargs: UpdateIdentityProviderSettingsRequestRequestTypeDef = {  # (1)
    "UpdateSettings": ...,
}

parent.update_identity_provider_settings(**kwargs)
```

1. See [:material-code-braces: UpdateIdentityProviderSettingsRequestRequestTypeDef](./type_defs.md#updateidentityprovidersettingsrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client)

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

Type annotations and code completion for `#!python session.client("license-manager-user-subscriptions").get_paginator` method with overloads.

- `client.get_paginator("list_identity_providers")` -> [ListIdentityProvidersPaginator](./paginators.md#listidentityproviderspaginator)
- `client.get_paginator("list_instances")` -> [ListInstancesPaginator](./paginators.md#listinstancespaginator)
- `client.get_paginator("list_license_server_endpoints")` -> [ListLicenseServerEndpointsPaginator](./paginators.md#listlicenseserverendpointspaginator)
- `client.get_paginator("list_product_subscriptions")` -> [ListProductSubscriptionsPaginator](./paginators.md#listproductsubscriptionspaginator)
- `client.get_paginator("list_user_associations")` -> [ListUserAssociationsPaginator](./paginators.md#listuserassociationspaginator)


