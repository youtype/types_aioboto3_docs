# IAMRolesAnywhereClient

> [Index](../README.md) > [IAMRolesAnywhere](./README.md) > IAMRolesAnywhereClient

!!! note ""

    Auto-generated documentation for [IAMRolesAnywhere](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#iamrolesanywhere)
    type annotations stubs module [types-aiobotocore-rolesanywhere](https://pypi.org/project/types-aiobotocore-rolesanywhere/).

## IAMRolesAnywhereClient

Type annotations and code completion for `#!python session.client("rolesanywhere")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# IAMRolesAnywhereClient usage example

from aioboto3.session import Session
from types_aiobotocore_rolesanywhere.client import IAMRolesAnywhereClient

session = Session()
async with session.client("rolesanywhere") as client:
    client: IAMRolesAnywhereClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("rolesanywhere").exceptions` structure.

```python
# IAMRolesAnywhereClient.exceptions usage example

async with session.client("rolesanywhere") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.TooManyTagsException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# IAMRolesAnywhereClient.exceptions type checking example

from types_aiobotocore_rolesanywhere.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("rolesanywhere").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("rolesanywhere").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

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


### create\_profile

Creates a <i>profile</i>, a list of the roles that Roles Anywhere service is
trusted to assume.

Type annotations and code completion for `#!python session.client("rolesanywhere").create_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# create_profile method definition

await def create_profile(
    self,
    *,
    name: str,
    roleArns: Sequence[str],
    acceptRoleSessionName: bool = ...,
    durationSeconds: int = ...,
    enabled: bool = ...,
    managedPolicyArns: Sequence[str] = ...,
    requireInstanceProperties: bool = ...,
    sessionPolicy: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (1)
) -> ProfileDetailResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ProfileDetailResponseTypeDef](./type_defs.md#profiledetailresponsetypedef) 


```python
# create_profile method usage example with argument unpacking

kwargs: CreateProfileRequestRequestTypeDef = {  # (1)
    "name": ...,
    "roleArns": ...,
}

parent.create_profile(**kwargs)
```

1. See [:material-code-braces: CreateProfileRequestRequestTypeDef](./type_defs.md#createprofilerequestrequesttypedef) 

### create\_trust\_anchor

Creates a trust anchor to establish trust between IAM Roles Anywhere and your
certificate authority (CA).

Type annotations and code completion for `#!python session.client("rolesanywhere").create_trust_anchor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# create_trust_anchor method definition

await def create_trust_anchor(
    self,
    *,
    name: str,
    source: SourceTypeDef,  # (1)
    enabled: bool = ...,
    notificationSettings: Sequence[NotificationSettingTypeDef] = ...,  # (2)
    tags: Sequence[TagTypeDef] = ...,  # (3)
) -> TrustAnchorDetailResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-braces: NotificationSettingTypeDef](./type_defs.md#notificationsettingtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: TrustAnchorDetailResponseTypeDef](./type_defs.md#trustanchordetailresponsetypedef) 


```python
# create_trust_anchor method usage example with argument unpacking

kwargs: CreateTrustAnchorRequestRequestTypeDef = {  # (1)
    "name": ...,
    "source": ...,
}

parent.create_trust_anchor(**kwargs)
```

1. See [:material-code-braces: CreateTrustAnchorRequestRequestTypeDef](./type_defs.md#createtrustanchorrequestrequesttypedef) 

### delete\_attribute\_mapping

Delete an entry from the attribute mapping rules enforced by a given profile.

Type annotations and code completion for `#!python session.client("rolesanywhere").delete_attribute_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# delete_attribute_mapping method definition

await def delete_attribute_mapping(
    self,
    *,
    certificateField: CertificateFieldType,  # (1)
    profileId: str,
    specifiers: Sequence[str] = ...,
) -> DeleteAttributeMappingResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: CertificateFieldType](./literals.md#certificatefieldtype) 
2. See [:material-code-braces: DeleteAttributeMappingResponseTypeDef](./type_defs.md#deleteattributemappingresponsetypedef) 


```python
# delete_attribute_mapping method usage example with argument unpacking

kwargs: DeleteAttributeMappingRequestRequestTypeDef = {  # (1)
    "certificateField": ...,
    "profileId": ...,
}

parent.delete_attribute_mapping(**kwargs)
```

1. See [:material-code-braces: DeleteAttributeMappingRequestRequestTypeDef](./type_defs.md#deleteattributemappingrequestrequesttypedef) 

### delete\_crl

Deletes a certificate revocation list (CRL).

Type annotations and code completion for `#!python session.client("rolesanywhere").delete_crl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# delete_crl method definition

await def delete_crl(
    self,
    *,
    crlId: str,
) -> CrlDetailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CrlDetailResponseTypeDef](./type_defs.md#crldetailresponsetypedef) 


```python
# delete_crl method usage example with argument unpacking

kwargs: ScalarCrlRequestRequestTypeDef = {  # (1)
    "crlId": ...,
}

parent.delete_crl(**kwargs)
```

1. See [:material-code-braces: ScalarCrlRequestRequestTypeDef](./type_defs.md#scalarcrlrequestrequesttypedef) 

### delete\_profile

Deletes a profile.

Type annotations and code completion for `#!python session.client("rolesanywhere").delete_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# delete_profile method definition

await def delete_profile(
    self,
    *,
    profileId: str,
) -> ProfileDetailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ProfileDetailResponseTypeDef](./type_defs.md#profiledetailresponsetypedef) 


```python
# delete_profile method usage example with argument unpacking

kwargs: ScalarProfileRequestRequestTypeDef = {  # (1)
    "profileId": ...,
}

parent.delete_profile(**kwargs)
```

1. See [:material-code-braces: ScalarProfileRequestRequestTypeDef](./type_defs.md#scalarprofilerequestrequesttypedef) 

### delete\_trust\_anchor

Deletes a trust anchor.

Type annotations and code completion for `#!python session.client("rolesanywhere").delete_trust_anchor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# delete_trust_anchor method definition

await def delete_trust_anchor(
    self,
    *,
    trustAnchorId: str,
) -> TrustAnchorDetailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TrustAnchorDetailResponseTypeDef](./type_defs.md#trustanchordetailresponsetypedef) 


```python
# delete_trust_anchor method usage example with argument unpacking

kwargs: ScalarTrustAnchorRequestRequestTypeDef = {  # (1)
    "trustAnchorId": ...,
}

parent.delete_trust_anchor(**kwargs)
```

1. See [:material-code-braces: ScalarTrustAnchorRequestRequestTypeDef](./type_defs.md#scalartrustanchorrequestrequesttypedef) 

### disable\_crl

Disables a certificate revocation list (CRL).

Type annotations and code completion for `#!python session.client("rolesanywhere").disable_crl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# disable_crl method definition

await def disable_crl(
    self,
    *,
    crlId: str,
) -> CrlDetailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CrlDetailResponseTypeDef](./type_defs.md#crldetailresponsetypedef) 


```python
# disable_crl method usage example with argument unpacking

kwargs: ScalarCrlRequestRequestTypeDef = {  # (1)
    "crlId": ...,
}

parent.disable_crl(**kwargs)
```

1. See [:material-code-braces: ScalarCrlRequestRequestTypeDef](./type_defs.md#scalarcrlrequestrequesttypedef) 

### disable\_profile

Disables a profile.

Type annotations and code completion for `#!python session.client("rolesanywhere").disable_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# disable_profile method definition

await def disable_profile(
    self,
    *,
    profileId: str,
) -> ProfileDetailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ProfileDetailResponseTypeDef](./type_defs.md#profiledetailresponsetypedef) 


```python
# disable_profile method usage example with argument unpacking

kwargs: ScalarProfileRequestRequestTypeDef = {  # (1)
    "profileId": ...,
}

parent.disable_profile(**kwargs)
```

1. See [:material-code-braces: ScalarProfileRequestRequestTypeDef](./type_defs.md#scalarprofilerequestrequesttypedef) 

### disable\_trust\_anchor

Disables a trust anchor.

Type annotations and code completion for `#!python session.client("rolesanywhere").disable_trust_anchor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# disable_trust_anchor method definition

await def disable_trust_anchor(
    self,
    *,
    trustAnchorId: str,
) -> TrustAnchorDetailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TrustAnchorDetailResponseTypeDef](./type_defs.md#trustanchordetailresponsetypedef) 


```python
# disable_trust_anchor method usage example with argument unpacking

kwargs: ScalarTrustAnchorRequestRequestTypeDef = {  # (1)
    "trustAnchorId": ...,
}

parent.disable_trust_anchor(**kwargs)
```

1. See [:material-code-braces: ScalarTrustAnchorRequestRequestTypeDef](./type_defs.md#scalartrustanchorrequestrequesttypedef) 

### enable\_crl

Enables a certificate revocation list (CRL).

Type annotations and code completion for `#!python session.client("rolesanywhere").enable_crl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# enable_crl method definition

await def enable_crl(
    self,
    *,
    crlId: str,
) -> CrlDetailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CrlDetailResponseTypeDef](./type_defs.md#crldetailresponsetypedef) 


```python
# enable_crl method usage example with argument unpacking

kwargs: ScalarCrlRequestRequestTypeDef = {  # (1)
    "crlId": ...,
}

parent.enable_crl(**kwargs)
```

1. See [:material-code-braces: ScalarCrlRequestRequestTypeDef](./type_defs.md#scalarcrlrequestrequesttypedef) 

### enable\_profile

Enables temporary credential requests for a profile.

Type annotations and code completion for `#!python session.client("rolesanywhere").enable_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# enable_profile method definition

await def enable_profile(
    self,
    *,
    profileId: str,
) -> ProfileDetailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ProfileDetailResponseTypeDef](./type_defs.md#profiledetailresponsetypedef) 


```python
# enable_profile method usage example with argument unpacking

kwargs: ScalarProfileRequestRequestTypeDef = {  # (1)
    "profileId": ...,
}

parent.enable_profile(**kwargs)
```

1. See [:material-code-braces: ScalarProfileRequestRequestTypeDef](./type_defs.md#scalarprofilerequestrequesttypedef) 

### enable\_trust\_anchor

Enables a trust anchor.

Type annotations and code completion for `#!python session.client("rolesanywhere").enable_trust_anchor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# enable_trust_anchor method definition

await def enable_trust_anchor(
    self,
    *,
    trustAnchorId: str,
) -> TrustAnchorDetailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TrustAnchorDetailResponseTypeDef](./type_defs.md#trustanchordetailresponsetypedef) 


```python
# enable_trust_anchor method usage example with argument unpacking

kwargs: ScalarTrustAnchorRequestRequestTypeDef = {  # (1)
    "trustAnchorId": ...,
}

parent.enable_trust_anchor(**kwargs)
```

1. See [:material-code-braces: ScalarTrustAnchorRequestRequestTypeDef](./type_defs.md#scalartrustanchorrequestrequesttypedef) 

### get\_crl

Gets a certificate revocation list (CRL).

Type annotations and code completion for `#!python session.client("rolesanywhere").get_crl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# get_crl method definition

await def get_crl(
    self,
    *,
    crlId: str,
) -> CrlDetailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CrlDetailResponseTypeDef](./type_defs.md#crldetailresponsetypedef) 


```python
# get_crl method usage example with argument unpacking

kwargs: ScalarCrlRequestRequestTypeDef = {  # (1)
    "crlId": ...,
}

parent.get_crl(**kwargs)
```

1. See [:material-code-braces: ScalarCrlRequestRequestTypeDef](./type_defs.md#scalarcrlrequestrequesttypedef) 

### get\_profile

Gets a profile.

Type annotations and code completion for `#!python session.client("rolesanywhere").get_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# get_profile method definition

await def get_profile(
    self,
    *,
    profileId: str,
) -> ProfileDetailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ProfileDetailResponseTypeDef](./type_defs.md#profiledetailresponsetypedef) 


```python
# get_profile method usage example with argument unpacking

kwargs: ScalarProfileRequestRequestTypeDef = {  # (1)
    "profileId": ...,
}

parent.get_profile(**kwargs)
```

1. See [:material-code-braces: ScalarProfileRequestRequestTypeDef](./type_defs.md#scalarprofilerequestrequesttypedef) 

### get\_subject

Gets a <i>subject</i>, which associates a certificate identity with
authentication attempts.

Type annotations and code completion for `#!python session.client("rolesanywhere").get_subject` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# get_subject method definition

await def get_subject(
    self,
    *,
    subjectId: str,
) -> SubjectDetailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SubjectDetailResponseTypeDef](./type_defs.md#subjectdetailresponsetypedef) 


```python
# get_subject method usage example with argument unpacking

kwargs: ScalarSubjectRequestRequestTypeDef = {  # (1)
    "subjectId": ...,
}

parent.get_subject(**kwargs)
```

1. See [:material-code-braces: ScalarSubjectRequestRequestTypeDef](./type_defs.md#scalarsubjectrequestrequesttypedef) 

### get\_trust\_anchor

Gets a trust anchor.

Type annotations and code completion for `#!python session.client("rolesanywhere").get_trust_anchor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# get_trust_anchor method definition

await def get_trust_anchor(
    self,
    *,
    trustAnchorId: str,
) -> TrustAnchorDetailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TrustAnchorDetailResponseTypeDef](./type_defs.md#trustanchordetailresponsetypedef) 


```python
# get_trust_anchor method usage example with argument unpacking

kwargs: ScalarTrustAnchorRequestRequestTypeDef = {  # (1)
    "trustAnchorId": ...,
}

parent.get_trust_anchor(**kwargs)
```

1. See [:material-code-braces: ScalarTrustAnchorRequestRequestTypeDef](./type_defs.md#scalartrustanchorrequestrequesttypedef) 

### import\_crl

Imports the certificate revocation list (CRL).

Type annotations and code completion for `#!python session.client("rolesanywhere").import_crl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# import_crl method definition

await def import_crl(
    self,
    *,
    crlData: BlobTypeDef,
    name: str,
    trustAnchorArn: str,
    enabled: bool = ...,
    tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CrlDetailResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CrlDetailResponseTypeDef](./type_defs.md#crldetailresponsetypedef) 


```python
# import_crl method usage example with argument unpacking

kwargs: ImportCrlRequestRequestTypeDef = {  # (1)
    "crlData": ...,
    "name": ...,
    "trustAnchorArn": ...,
}

parent.import_crl(**kwargs)
```

1. See [:material-code-braces: ImportCrlRequestRequestTypeDef](./type_defs.md#importcrlrequestrequesttypedef) 

### list\_crls

Lists all certificate revocation lists (CRL) in the authenticated account and
Amazon Web Services Region.

Type annotations and code completion for `#!python session.client("rolesanywhere").list_crls` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# list_crls method definition

await def list_crls(
    self,
    *,
    nextToken: str = ...,
    pageSize: int = ...,
) -> ListCrlsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCrlsResponseTypeDef](./type_defs.md#listcrlsresponsetypedef) 


```python
# list_crls method usage example with argument unpacking

kwargs: ListRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_crls(**kwargs)
```

1. See [:material-code-braces: ListRequestRequestTypeDef](./type_defs.md#listrequestrequesttypedef) 

### list\_profiles

Lists all profiles in the authenticated account and Amazon Web Services Region.

Type annotations and code completion for `#!python session.client("rolesanywhere").list_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# list_profiles method definition

await def list_profiles(
    self,
    *,
    nextToken: str = ...,
    pageSize: int = ...,
) -> ListProfilesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListProfilesResponseTypeDef](./type_defs.md#listprofilesresponsetypedef) 


```python
# list_profiles method usage example with argument unpacking

kwargs: ListRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_profiles(**kwargs)
```

1. See [:material-code-braces: ListRequestRequestTypeDef](./type_defs.md#listrequestrequesttypedef) 

### list\_subjects

Lists the subjects in the authenticated account and Amazon Web Services Region.

Type annotations and code completion for `#!python session.client("rolesanywhere").list_subjects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# list_subjects method definition

await def list_subjects(
    self,
    *,
    nextToken: str = ...,
    pageSize: int = ...,
) -> ListSubjectsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSubjectsResponseTypeDef](./type_defs.md#listsubjectsresponsetypedef) 


```python
# list_subjects method usage example with argument unpacking

kwargs: ListRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_subjects(**kwargs)
```

1. See [:material-code-braces: ListRequestRequestTypeDef](./type_defs.md#listrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags attached to the resource.

Type annotations and code completion for `#!python session.client("rolesanywhere").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

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

### list\_trust\_anchors

Lists the trust anchors in the authenticated account and Amazon Web Services
Region.

Type annotations and code completion for `#!python session.client("rolesanywhere").list_trust_anchors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# list_trust_anchors method definition

await def list_trust_anchors(
    self,
    *,
    nextToken: str = ...,
    pageSize: int = ...,
) -> ListTrustAnchorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTrustAnchorsResponseTypeDef](./type_defs.md#listtrustanchorsresponsetypedef) 


```python
# list_trust_anchors method usage example with argument unpacking

kwargs: ListRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_trust_anchors(**kwargs)
```

1. See [:material-code-braces: ListRequestRequestTypeDef](./type_defs.md#listrequestrequesttypedef) 

### put\_attribute\_mapping

Put an entry in the attribute mapping rules that will be enforced by a given
profile.

Type annotations and code completion for `#!python session.client("rolesanywhere").put_attribute_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# put_attribute_mapping method definition

await def put_attribute_mapping(
    self,
    *,
    certificateField: CertificateFieldType,  # (1)
    mappingRules: Sequence[MappingRuleTypeDef],  # (2)
    profileId: str,
) -> PutAttributeMappingResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: CertificateFieldType](./literals.md#certificatefieldtype) 
2. See [:material-code-braces: MappingRuleTypeDef](./type_defs.md#mappingruletypedef) 
3. See [:material-code-braces: PutAttributeMappingResponseTypeDef](./type_defs.md#putattributemappingresponsetypedef) 


```python
# put_attribute_mapping method usage example with argument unpacking

kwargs: PutAttributeMappingRequestRequestTypeDef = {  # (1)
    "certificateField": ...,
    "mappingRules": ...,
    "profileId": ...,
}

parent.put_attribute_mapping(**kwargs)
```

1. See [:material-code-braces: PutAttributeMappingRequestRequestTypeDef](./type_defs.md#putattributemappingrequestrequesttypedef) 

### put\_notification\_settings

Attaches a list of <i>notification settings</i> to a trust anchor.

Type annotations and code completion for `#!python session.client("rolesanywhere").put_notification_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# put_notification_settings method definition

await def put_notification_settings(
    self,
    *,
    notificationSettings: Sequence[NotificationSettingTypeDef],  # (1)
    trustAnchorId: str,
) -> PutNotificationSettingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: NotificationSettingTypeDef](./type_defs.md#notificationsettingtypedef) 
2. See [:material-code-braces: PutNotificationSettingsResponseTypeDef](./type_defs.md#putnotificationsettingsresponsetypedef) 


```python
# put_notification_settings method usage example with argument unpacking

kwargs: PutNotificationSettingsRequestRequestTypeDef = {  # (1)
    "notificationSettings": ...,
    "trustAnchorId": ...,
}

parent.put_notification_settings(**kwargs)
```

1. See [:material-code-braces: PutNotificationSettingsRequestRequestTypeDef](./type_defs.md#putnotificationsettingsrequestrequesttypedef) 

### reset\_notification\_settings

Resets the <i>custom notification setting</i> to IAM Roles Anywhere default
setting.

Type annotations and code completion for `#!python session.client("rolesanywhere").reset_notification_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# reset_notification_settings method definition

await def reset_notification_settings(
    self,
    *,
    notificationSettingKeys: Sequence[NotificationSettingKeyTypeDef],  # (1)
    trustAnchorId: str,
) -> ResetNotificationSettingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: NotificationSettingKeyTypeDef](./type_defs.md#notificationsettingkeytypedef) 
2. See [:material-code-braces: ResetNotificationSettingsResponseTypeDef](./type_defs.md#resetnotificationsettingsresponsetypedef) 


```python
# reset_notification_settings method usage example with argument unpacking

kwargs: ResetNotificationSettingsRequestRequestTypeDef = {  # (1)
    "notificationSettingKeys": ...,
    "trustAnchorId": ...,
}

parent.reset_notification_settings(**kwargs)
```

1. See [:material-code-braces: ResetNotificationSettingsRequestRequestTypeDef](./type_defs.md#resetnotificationsettingsrequestrequesttypedef) 

### tag\_resource

Attaches tags to a resource.

Type annotations and code completion for `#!python session.client("rolesanywhere").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

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

Removes tags from the resource.

Type annotations and code completion for `#!python session.client("rolesanywhere").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

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

### update\_crl

Updates the certificate revocation list (CRL).

Type annotations and code completion for `#!python session.client("rolesanywhere").update_crl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# update_crl method definition

await def update_crl(
    self,
    *,
    crlId: str,
    crlData: BlobTypeDef = ...,
    name: str = ...,
) -> CrlDetailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CrlDetailResponseTypeDef](./type_defs.md#crldetailresponsetypedef) 


```python
# update_crl method usage example with argument unpacking

kwargs: UpdateCrlRequestRequestTypeDef = {  # (1)
    "crlId": ...,
}

parent.update_crl(**kwargs)
```

1. See [:material-code-braces: UpdateCrlRequestRequestTypeDef](./type_defs.md#updatecrlrequestrequesttypedef) 

### update\_profile

Updates a <i>profile</i>, a list of the roles that IAM Roles Anywhere service
is trusted to assume.

Type annotations and code completion for `#!python session.client("rolesanywhere").update_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# update_profile method definition

await def update_profile(
    self,
    *,
    profileId: str,
    acceptRoleSessionName: bool = ...,
    durationSeconds: int = ...,
    managedPolicyArns: Sequence[str] = ...,
    name: str = ...,
    roleArns: Sequence[str] = ...,
    sessionPolicy: str = ...,
) -> ProfileDetailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ProfileDetailResponseTypeDef](./type_defs.md#profiledetailresponsetypedef) 


```python
# update_profile method usage example with argument unpacking

kwargs: UpdateProfileRequestRequestTypeDef = {  # (1)
    "profileId": ...,
}

parent.update_profile(**kwargs)
```

1. See [:material-code-braces: UpdateProfileRequestRequestTypeDef](./type_defs.md#updateprofilerequestrequesttypedef) 

### update\_trust\_anchor

Updates a trust anchor.

Type annotations and code completion for `#!python session.client("rolesanywhere").update_trust_anchor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# update_trust_anchor method definition

await def update_trust_anchor(
    self,
    *,
    trustAnchorId: str,
    name: str = ...,
    source: SourceTypeDef = ...,  # (1)
) -> TrustAnchorDetailResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-braces: TrustAnchorDetailResponseTypeDef](./type_defs.md#trustanchordetailresponsetypedef) 


```python
# update_trust_anchor method usage example with argument unpacking

kwargs: UpdateTrustAnchorRequestRequestTypeDef = {  # (1)
    "trustAnchorId": ...,
}

parent.update_trust_anchor(**kwargs)
```

1. See [:material-code-braces: UpdateTrustAnchorRequestRequestTypeDef](./type_defs.md#updatetrustanchorrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("rolesanywhere").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("rolesanywhere").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Client)

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

Type annotations and code completion for `#!python session.client("rolesanywhere").get_paginator` method with overloads.

- `client.get_paginator("list_crls")` -> [ListCrlsPaginator](./paginators.md#listcrlspaginator)
- `client.get_paginator("list_profiles")` -> [ListProfilesPaginator](./paginators.md#listprofilespaginator)
- `client.get_paginator("list_subjects")` -> [ListSubjectsPaginator](./paginators.md#listsubjectspaginator)
- `client.get_paginator("list_trust_anchors")` -> [ListTrustAnchorsPaginator](./paginators.md#listtrustanchorspaginator)


