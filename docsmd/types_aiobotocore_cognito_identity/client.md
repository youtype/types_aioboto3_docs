# CognitoIdentityClient

> [Index](../README.md) > [CognitoIdentity](./README.md) > CognitoIdentityClient

!!! note ""

    Auto-generated documentation for [CognitoIdentity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#cognitoidentity)
    type annotations stubs module [types-aiobotocore-cognito-identity](https://pypi.org/project/types-aiobotocore-cognito-identity/).

## CognitoIdentityClient

Type annotations and code completion for `#!python session.client("cognito-identity")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# CognitoIdentityClient usage example

from aioboto3.session import Session
from types_aiobotocore_cognito_identity.client import CognitoIdentityClient

session = Session()
async with session.client("cognito-identity") as client:
    client: CognitoIdentityClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("cognito-identity").exceptions` structure.

```python
# CognitoIdentityClient.exceptions usage example

async with session.client("cognito-identity") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.ConcurrentModificationException,
        client.exceptions.DeveloperUserAlreadyRegisteredException,
        client.exceptions.ExternalServiceException,
        client.exceptions.InternalErrorException,
        client.exceptions.InvalidIdentityPoolConfigurationException,
        client.exceptions.InvalidParameterException,
        client.exceptions.LimitExceededException,
        client.exceptions.NotAuthorizedException,
        client.exceptions.ResourceConflictException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.TooManyRequestsException,
    ) as e:
        print(e)
```

```python
# CognitoIdentityClient.exceptions type checking example

from types_aiobotocore_cognito_identity.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("cognito-identity").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("cognito-identity").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

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


### create\_identity\_pool

Creates a new identity pool.

Type annotations and code completion for `#!python session.client("cognito-identity").create_identity_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# create_identity_pool method definition

await def create_identity_pool(
    self,
    *,
    IdentityPoolName: str,
    AllowUnauthenticatedIdentities: bool,
    AllowClassicFlow: bool = ...,
    SupportedLoginProviders: Mapping[str, str] = ...,
    DeveloperProviderName: str = ...,
    OpenIdConnectProviderARNs: Sequence[str] = ...,
    CognitoIdentityProviders: Sequence[CognitoIdentityProviderTypeDef] = ...,  # (1)
    SamlProviderARNs: Sequence[str] = ...,
    IdentityPoolTags: Mapping[str, str] = ...,
) -> IdentityPoolTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CognitoIdentityProviderTypeDef](./type_defs.md#cognitoidentityprovidertypedef) 
2. See [:material-code-braces: IdentityPoolTypeDef](./type_defs.md#identitypooltypedef) 


```python
# create_identity_pool method usage example with argument unpacking

kwargs: CreateIdentityPoolInputRequestTypeDef = {  # (1)
    "IdentityPoolName": ...,
    "AllowUnauthenticatedIdentities": ...,
}

parent.create_identity_pool(**kwargs)
```

1. See [:material-code-braces: CreateIdentityPoolInputRequestTypeDef](./type_defs.md#createidentitypoolinputrequesttypedef) 

### delete\_identities

Deletes identities from an identity pool.

Type annotations and code completion for `#!python session.client("cognito-identity").delete_identities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# delete_identities method definition

await def delete_identities(
    self,
    *,
    IdentityIdsToDelete: Sequence[str],
) -> DeleteIdentitiesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteIdentitiesResponseTypeDef](./type_defs.md#deleteidentitiesresponsetypedef) 


```python
# delete_identities method usage example with argument unpacking

kwargs: DeleteIdentitiesInputRequestTypeDef = {  # (1)
    "IdentityIdsToDelete": ...,
}

parent.delete_identities(**kwargs)
```

1. See [:material-code-braces: DeleteIdentitiesInputRequestTypeDef](./type_defs.md#deleteidentitiesinputrequesttypedef) 

### delete\_identity\_pool

Deletes an identity pool.

Type annotations and code completion for `#!python session.client("cognito-identity").delete_identity_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# delete_identity_pool method definition

await def delete_identity_pool(
    self,
    *,
    IdentityPoolId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_identity_pool method usage example with argument unpacking

kwargs: DeleteIdentityPoolInputRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
}

parent.delete_identity_pool(**kwargs)
```

1. See [:material-code-braces: DeleteIdentityPoolInputRequestTypeDef](./type_defs.md#deleteidentitypoolinputrequesttypedef) 

### describe\_identity

Returns metadata related to the given identity, including when the identity was
created and any associated linked logins.

Type annotations and code completion for `#!python session.client("cognito-identity").describe_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# describe_identity method definition

await def describe_identity(
    self,
    *,
    IdentityId: str,
) -> IdentityDescriptionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: IdentityDescriptionResponseTypeDef](./type_defs.md#identitydescriptionresponsetypedef) 


```python
# describe_identity method usage example with argument unpacking

kwargs: DescribeIdentityInputRequestTypeDef = {  # (1)
    "IdentityId": ...,
}

parent.describe_identity(**kwargs)
```

1. See [:material-code-braces: DescribeIdentityInputRequestTypeDef](./type_defs.md#describeidentityinputrequesttypedef) 

### describe\_identity\_pool

Gets details about a particular identity pool, including the pool name, ID
description, creation date, and current number of users.

Type annotations and code completion for `#!python session.client("cognito-identity").describe_identity_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# describe_identity_pool method definition

await def describe_identity_pool(
    self,
    *,
    IdentityPoolId: str,
) -> IdentityPoolTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: IdentityPoolTypeDef](./type_defs.md#identitypooltypedef) 


```python
# describe_identity_pool method usage example with argument unpacking

kwargs: DescribeIdentityPoolInputRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
}

parent.describe_identity_pool(**kwargs)
```

1. See [:material-code-braces: DescribeIdentityPoolInputRequestTypeDef](./type_defs.md#describeidentitypoolinputrequesttypedef) 

### get\_credentials\_for\_identity

Returns credentials for the provided identity ID.

Type annotations and code completion for `#!python session.client("cognito-identity").get_credentials_for_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# get_credentials_for_identity method definition

await def get_credentials_for_identity(
    self,
    *,
    IdentityId: str,
    Logins: Mapping[str, str] = ...,
    CustomRoleArn: str = ...,
) -> GetCredentialsForIdentityResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCredentialsForIdentityResponseTypeDef](./type_defs.md#getcredentialsforidentityresponsetypedef) 


```python
# get_credentials_for_identity method usage example with argument unpacking

kwargs: GetCredentialsForIdentityInputRequestTypeDef = {  # (1)
    "IdentityId": ...,
}

parent.get_credentials_for_identity(**kwargs)
```

1. See [:material-code-braces: GetCredentialsForIdentityInputRequestTypeDef](./type_defs.md#getcredentialsforidentityinputrequesttypedef) 

### get\_id

Generates (or retrieves) a Cognito ID.

Type annotations and code completion for `#!python session.client("cognito-identity").get_id` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# get_id method definition

await def get_id(
    self,
    *,
    IdentityPoolId: str,
    AccountId: str = ...,
    Logins: Mapping[str, str] = ...,
) -> GetIdResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIdResponseTypeDef](./type_defs.md#getidresponsetypedef) 


```python
# get_id method usage example with argument unpacking

kwargs: GetIdInputRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
}

parent.get_id(**kwargs)
```

1. See [:material-code-braces: GetIdInputRequestTypeDef](./type_defs.md#getidinputrequesttypedef) 

### get\_identity\_pool\_roles

Gets the roles for an identity pool.

Type annotations and code completion for `#!python session.client("cognito-identity").get_identity_pool_roles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# get_identity_pool_roles method definition

await def get_identity_pool_roles(
    self,
    *,
    IdentityPoolId: str,
) -> GetIdentityPoolRolesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIdentityPoolRolesResponseTypeDef](./type_defs.md#getidentitypoolrolesresponsetypedef) 


```python
# get_identity_pool_roles method usage example with argument unpacking

kwargs: GetIdentityPoolRolesInputRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
}

parent.get_identity_pool_roles(**kwargs)
```

1. See [:material-code-braces: GetIdentityPoolRolesInputRequestTypeDef](./type_defs.md#getidentitypoolrolesinputrequesttypedef) 

### get\_open\_id\_token

Gets an OpenID token, using a known Cognito ID.

Type annotations and code completion for `#!python session.client("cognito-identity").get_open_id_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# get_open_id_token method definition

await def get_open_id_token(
    self,
    *,
    IdentityId: str,
    Logins: Mapping[str, str] = ...,
) -> GetOpenIdTokenResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOpenIdTokenResponseTypeDef](./type_defs.md#getopenidtokenresponsetypedef) 


```python
# get_open_id_token method usage example with argument unpacking

kwargs: GetOpenIdTokenInputRequestTypeDef = {  # (1)
    "IdentityId": ...,
}

parent.get_open_id_token(**kwargs)
```

1. See [:material-code-braces: GetOpenIdTokenInputRequestTypeDef](./type_defs.md#getopenidtokeninputrequesttypedef) 

### get\_open\_id\_token\_for\_developer\_identity

Registers (or retrieves) a Cognito <code>IdentityId</code> and an OpenID
Connect token for a user authenticated by your backend authentication process.

Type annotations and code completion for `#!python session.client("cognito-identity").get_open_id_token_for_developer_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# get_open_id_token_for_developer_identity method definition

await def get_open_id_token_for_developer_identity(
    self,
    *,
    IdentityPoolId: str,
    Logins: Mapping[str, str],
    IdentityId: str = ...,
    PrincipalTags: Mapping[str, str] = ...,
    TokenDuration: int = ...,
) -> GetOpenIdTokenForDeveloperIdentityResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOpenIdTokenForDeveloperIdentityResponseTypeDef](./type_defs.md#getopenidtokenfordeveloperidentityresponsetypedef) 


```python
# get_open_id_token_for_developer_identity method usage example with argument unpacking

kwargs: GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
    "Logins": ...,
}

parent.get_open_id_token_for_developer_identity(**kwargs)
```

1. See [:material-code-braces: GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef](./type_defs.md#getopenidtokenfordeveloperidentityinputrequesttypedef) 

### get\_principal\_tag\_attribute\_map

Use <code>GetPrincipalTagAttributeMap</code> to list all mappings between
<code>PrincipalTags</code> and user attributes.

Type annotations and code completion for `#!python session.client("cognito-identity").get_principal_tag_attribute_map` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# get_principal_tag_attribute_map method definition

await def get_principal_tag_attribute_map(
    self,
    *,
    IdentityPoolId: str,
    IdentityProviderName: str,
) -> GetPrincipalTagAttributeMapResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPrincipalTagAttributeMapResponseTypeDef](./type_defs.md#getprincipaltagattributemapresponsetypedef) 


```python
# get_principal_tag_attribute_map method usage example with argument unpacking

kwargs: GetPrincipalTagAttributeMapInputRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
    "IdentityProviderName": ...,
}

parent.get_principal_tag_attribute_map(**kwargs)
```

1. See [:material-code-braces: GetPrincipalTagAttributeMapInputRequestTypeDef](./type_defs.md#getprincipaltagattributemapinputrequesttypedef) 

### list\_identities

Lists the identities in an identity pool.

Type annotations and code completion for `#!python session.client("cognito-identity").list_identities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# list_identities method definition

await def list_identities(
    self,
    *,
    IdentityPoolId: str,
    MaxResults: int,
    NextToken: str = ...,
    HideDisabled: bool = ...,
) -> ListIdentitiesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIdentitiesResponseTypeDef](./type_defs.md#listidentitiesresponsetypedef) 


```python
# list_identities method usage example with argument unpacking

kwargs: ListIdentitiesInputRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
    "MaxResults": ...,
}

parent.list_identities(**kwargs)
```

1. See [:material-code-braces: ListIdentitiesInputRequestTypeDef](./type_defs.md#listidentitiesinputrequesttypedef) 

### list\_identity\_pools

Lists all of the Cognito identity pools registered for your account.

Type annotations and code completion for `#!python session.client("cognito-identity").list_identity_pools` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# list_identity_pools method definition

await def list_identity_pools(
    self,
    *,
    MaxResults: int,
    NextToken: str = ...,
) -> ListIdentityPoolsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIdentityPoolsResponseTypeDef](./type_defs.md#listidentitypoolsresponsetypedef) 


```python
# list_identity_pools method usage example with argument unpacking

kwargs: ListIdentityPoolsInputRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_identity_pools(**kwargs)
```

1. See [:material-code-braces: ListIdentityPoolsInputRequestTypeDef](./type_defs.md#listidentitypoolsinputrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags that are assigned to an Amazon Cognito identity pool.

Type annotations and code completion for `#!python session.client("cognito-identity").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

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

kwargs: ListTagsForResourceInputRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef) 

### lookup\_developer\_identity

Retrieves the <code>IdentityID</code> associated with a
<code>DeveloperUserIdentifier</code> or the list of
<code>DeveloperUserIdentifier</code> values associated with an
<code>IdentityId</code> for an existing identity.

Type annotations and code completion for `#!python session.client("cognito-identity").lookup_developer_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# lookup_developer_identity method definition

await def lookup_developer_identity(
    self,
    *,
    IdentityPoolId: str,
    IdentityId: str = ...,
    DeveloperUserIdentifier: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> LookupDeveloperIdentityResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: LookupDeveloperIdentityResponseTypeDef](./type_defs.md#lookupdeveloperidentityresponsetypedef) 


```python
# lookup_developer_identity method usage example with argument unpacking

kwargs: LookupDeveloperIdentityInputRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
}

parent.lookup_developer_identity(**kwargs)
```

1. See [:material-code-braces: LookupDeveloperIdentityInputRequestTypeDef](./type_defs.md#lookupdeveloperidentityinputrequesttypedef) 

### merge\_developer\_identities

Merges two users having different <code>IdentityId</code>s, existing in the
same identity pool, and identified by the same developer provider.

Type annotations and code completion for `#!python session.client("cognito-identity").merge_developer_identities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# merge_developer_identities method definition

await def merge_developer_identities(
    self,
    *,
    SourceUserIdentifier: str,
    DestinationUserIdentifier: str,
    DeveloperProviderName: str,
    IdentityPoolId: str,
) -> MergeDeveloperIdentitiesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: MergeDeveloperIdentitiesResponseTypeDef](./type_defs.md#mergedeveloperidentitiesresponsetypedef) 


```python
# merge_developer_identities method usage example with argument unpacking

kwargs: MergeDeveloperIdentitiesInputRequestTypeDef = {  # (1)
    "SourceUserIdentifier": ...,
    "DestinationUserIdentifier": ...,
    "DeveloperProviderName": ...,
    "IdentityPoolId": ...,
}

parent.merge_developer_identities(**kwargs)
```

1. See [:material-code-braces: MergeDeveloperIdentitiesInputRequestTypeDef](./type_defs.md#mergedeveloperidentitiesinputrequesttypedef) 

### set\_identity\_pool\_roles

Sets the roles for an identity pool.

Type annotations and code completion for `#!python session.client("cognito-identity").set_identity_pool_roles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# set_identity_pool_roles method definition

await def set_identity_pool_roles(
    self,
    *,
    IdentityPoolId: str,
    Roles: Mapping[str, str],
    RoleMappings: Mapping[str, RoleMappingUnionTypeDef] = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RoleMappingTypeDef](./type_defs.md#rolemappingtypedef) [:material-code-braces: RoleMappingOutputTypeDef](./type_defs.md#rolemappingoutputtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# set_identity_pool_roles method usage example with argument unpacking

kwargs: SetIdentityPoolRolesInputRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
    "Roles": ...,
}

parent.set_identity_pool_roles(**kwargs)
```

1. See [:material-code-braces: SetIdentityPoolRolesInputRequestTypeDef](./type_defs.md#setidentitypoolrolesinputrequesttypedef) 

### set\_principal\_tag\_attribute\_map

You can use this operation to use default (username and clientID) attribute or
custom attribute mappings.

Type annotations and code completion for `#!python session.client("cognito-identity").set_principal_tag_attribute_map` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# set_principal_tag_attribute_map method definition

await def set_principal_tag_attribute_map(
    self,
    *,
    IdentityPoolId: str,
    IdentityProviderName: str,
    UseDefaults: bool = ...,
    PrincipalTags: Mapping[str, str] = ...,
) -> SetPrincipalTagAttributeMapResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SetPrincipalTagAttributeMapResponseTypeDef](./type_defs.md#setprincipaltagattributemapresponsetypedef) 


```python
# set_principal_tag_attribute_map method usage example with argument unpacking

kwargs: SetPrincipalTagAttributeMapInputRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
    "IdentityProviderName": ...,
}

parent.set_principal_tag_attribute_map(**kwargs)
```

1. See [:material-code-braces: SetPrincipalTagAttributeMapInputRequestTypeDef](./type_defs.md#setprincipaltagattributemapinputrequesttypedef) 

### tag\_resource

Assigns a set of tags to the specified Amazon Cognito identity pool.

Type annotations and code completion for `#!python session.client("cognito-identity").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

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

kwargs: TagResourceInputRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef) 

### unlink\_developer\_identity

Unlinks a <code>DeveloperUserIdentifier</code> from an existing identity.

Type annotations and code completion for `#!python session.client("cognito-identity").unlink_developer_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# unlink_developer_identity method definition

await def unlink_developer_identity(
    self,
    *,
    IdentityId: str,
    IdentityPoolId: str,
    DeveloperProviderName: str,
    DeveloperUserIdentifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# unlink_developer_identity method usage example with argument unpacking

kwargs: UnlinkDeveloperIdentityInputRequestTypeDef = {  # (1)
    "IdentityId": ...,
    "IdentityPoolId": ...,
    "DeveloperProviderName": ...,
    "DeveloperUserIdentifier": ...,
}

parent.unlink_developer_identity(**kwargs)
```

1. See [:material-code-braces: UnlinkDeveloperIdentityInputRequestTypeDef](./type_defs.md#unlinkdeveloperidentityinputrequesttypedef) 

### unlink\_identity

Unlinks a federated identity from an existing account.

Type annotations and code completion for `#!python session.client("cognito-identity").unlink_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# unlink_identity method definition

await def unlink_identity(
    self,
    *,
    IdentityId: str,
    Logins: Mapping[str, str],
    LoginsToRemove: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# unlink_identity method usage example with argument unpacking

kwargs: UnlinkIdentityInputRequestTypeDef = {  # (1)
    "IdentityId": ...,
    "Logins": ...,
    "LoginsToRemove": ...,
}

parent.unlink_identity(**kwargs)
```

1. See [:material-code-braces: UnlinkIdentityInputRequestTypeDef](./type_defs.md#unlinkidentityinputrequesttypedef) 

### untag\_resource

Removes the specified tags from the specified Amazon Cognito identity pool.

Type annotations and code completion for `#!python session.client("cognito-identity").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

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

kwargs: UntagResourceInputRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef) 

### update\_identity\_pool

Updates an identity pool.

Type annotations and code completion for `#!python session.client("cognito-identity").update_identity_pool` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# update_identity_pool method definition

await def update_identity_pool(
    self,
    *,
    IdentityPoolId: str,
    IdentityPoolName: str,
    AllowUnauthenticatedIdentities: bool,
    AllowClassicFlow: bool = ...,
    SupportedLoginProviders: Mapping[str, str] = ...,
    DeveloperProviderName: str = ...,
    OpenIdConnectProviderARNs: Sequence[str] = ...,
    CognitoIdentityProviders: Sequence[CognitoIdentityProviderTypeDef] = ...,  # (1)
    SamlProviderARNs: Sequence[str] = ...,
    IdentityPoolTags: Mapping[str, str] = ...,
) -> IdentityPoolTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CognitoIdentityProviderTypeDef](./type_defs.md#cognitoidentityprovidertypedef) 
2. See [:material-code-braces: IdentityPoolTypeDef](./type_defs.md#identitypooltypedef) 


```python
# update_identity_pool method usage example with argument unpacking

kwargs: IdentityPoolRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
    "IdentityPoolName": ...,
    "AllowUnauthenticatedIdentities": ...,
}

parent.update_identity_pool(**kwargs)
```

1. See [:material-code-braces: IdentityPoolRequestTypeDef](./type_defs.md#identitypoolrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("cognito-identity").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("cognito-identity").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client)

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

Type annotations and code completion for `#!python session.client("cognito-identity").get_paginator` method with overloads.

- `client.get_paginator("list_identity_pools")` -> [ListIdentityPoolsPaginator](./paginators.md#listidentitypoolspaginator)


