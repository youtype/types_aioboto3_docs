# TransferClient

> [Index](../README.md) > [Transfer](./README.md) > TransferClient

!!! note ""

    Auto-generated documentation for [Transfer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#transfer)
    type annotations stubs module [types-aiobotocore-transfer](https://pypi.org/project/types-aiobotocore-transfer/).

## TransferClient

Type annotations and code completion for `#!python session.client("transfer")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# TransferClient usage example

from aioboto3.session import Session
from types_aiobotocore_transfer.client import TransferClient

session = Session()
async with session.client("transfer") as client:
    client: TransferClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("transfer").exceptions` structure.

```python
# TransferClient.exceptions usage example

async with session.client("transfer") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServiceError,
        client.exceptions.InvalidNextTokenException,
        client.exceptions.InvalidRequestException,
        client.exceptions.ResourceExistsException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceUnavailableException,
        client.exceptions.ThrottlingException,
    ) as e:
        print(e)
```

```python
# TransferClient.exceptions type checking example

from types_aiobotocore_transfer.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("transfer").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("transfer").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

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


### create\_access

Used by administrators to choose which groups in the directory should have
access to upload and download files over the enabled protocols using Transfer
Family.

Type annotations and code completion for `#!python session.client("transfer").create_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# create_access method definition

await def create_access(
    self,
    *,
    Role: str,
    ServerId: str,
    ExternalId: str,
    HomeDirectory: str = ...,
    HomeDirectoryType: HomeDirectoryTypeType = ...,  # (1)
    HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,  # (2)
    Policy: str = ...,
    PosixProfile: PosixProfileTypeDef = ...,  # (3)
) -> CreateAccessResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: HomeDirectoryTypeType](./literals.md#homedirectorytypetype) 
2. See [:material-code-braces: HomeDirectoryMapEntryTypeDef](./type_defs.md#homedirectorymapentrytypedef) 
3. See [:material-code-braces: PosixProfileTypeDef](./type_defs.md#posixprofiletypedef) 
4. See [:material-code-braces: CreateAccessResponseTypeDef](./type_defs.md#createaccessresponsetypedef) 


```python
# create_access method usage example with argument unpacking

kwargs: CreateAccessRequestRequestTypeDef = {  # (1)
    "Role": ...,
    "ServerId": ...,
    "ExternalId": ...,
}

parent.create_access(**kwargs)
```

1. See [:material-code-braces: CreateAccessRequestRequestTypeDef](./type_defs.md#createaccessrequestrequesttypedef) 

### create\_agreement

Creates an agreement.

Type annotations and code completion for `#!python session.client("transfer").create_agreement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# create_agreement method definition

await def create_agreement(
    self,
    *,
    ServerId: str,
    LocalProfileId: str,
    PartnerProfileId: str,
    BaseDirectory: str,
    AccessRole: str,
    Description: str = ...,
    Status: AgreementStatusTypeType = ...,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateAgreementResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AgreementStatusTypeType](./literals.md#agreementstatustypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateAgreementResponseTypeDef](./type_defs.md#createagreementresponsetypedef) 


```python
# create_agreement method usage example with argument unpacking

kwargs: CreateAgreementRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
    "LocalProfileId": ...,
    "PartnerProfileId": ...,
    "BaseDirectory": ...,
    "AccessRole": ...,
}

parent.create_agreement(**kwargs)
```

1. See [:material-code-braces: CreateAgreementRequestRequestTypeDef](./type_defs.md#createagreementrequestrequesttypedef) 

### create\_connector

Creates the connector, which captures the parameters for a connection for the
AS2 or SFTP protocol.

Type annotations and code completion for `#!python session.client("transfer").create_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# create_connector method definition

await def create_connector(
    self,
    *,
    Url: str,
    AccessRole: str,
    As2Config: As2ConnectorConfigTypeDef = ...,  # (1)
    LoggingRole: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    SftpConfig: SftpConnectorConfigTypeDef = ...,  # (3)
    SecurityPolicyName: str = ...,
) -> CreateConnectorResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: As2ConnectorConfigTypeDef](./type_defs.md#as2connectorconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: SftpConnectorConfigTypeDef](./type_defs.md#sftpconnectorconfigtypedef) 
4. See [:material-code-braces: CreateConnectorResponseTypeDef](./type_defs.md#createconnectorresponsetypedef) 


```python
# create_connector method usage example with argument unpacking

kwargs: CreateConnectorRequestRequestTypeDef = {  # (1)
    "Url": ...,
    "AccessRole": ...,
}

parent.create_connector(**kwargs)
```

1. See [:material-code-braces: CreateConnectorRequestRequestTypeDef](./type_defs.md#createconnectorrequestrequesttypedef) 

### create\_profile

Creates the local or partner profile to use for AS2 transfers.

Type annotations and code completion for `#!python session.client("transfer").create_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# create_profile method definition

await def create_profile(
    self,
    *,
    As2Id: str,
    ProfileType: ProfileTypeType,  # (1)
    CertificateIds: Sequence[str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateProfileResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ProfileTypeType](./literals.md#profiletypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateProfileResponseTypeDef](./type_defs.md#createprofileresponsetypedef) 


```python
# create_profile method usage example with argument unpacking

kwargs: CreateProfileRequestRequestTypeDef = {  # (1)
    "As2Id": ...,
    "ProfileType": ...,
}

parent.create_profile(**kwargs)
```

1. See [:material-code-braces: CreateProfileRequestRequestTypeDef](./type_defs.md#createprofilerequestrequesttypedef) 

### create\_server

Instantiates an auto-scaling virtual server based on the selected file transfer
protocol in Amazon Web Services.

Type annotations and code completion for `#!python session.client("transfer").create_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# create_server method definition

await def create_server(
    self,
    *,
    Certificate: str = ...,
    Domain: DomainType = ...,  # (1)
    EndpointDetails: EndpointDetailsTypeDef = ...,  # (2)
    EndpointType: EndpointTypeType = ...,  # (3)
    HostKey: str = ...,
    IdentityProviderDetails: IdentityProviderDetailsTypeDef = ...,  # (4)
    IdentityProviderType: IdentityProviderTypeType = ...,  # (5)
    LoggingRole: str = ...,
    PostAuthenticationLoginBanner: str = ...,
    PreAuthenticationLoginBanner: str = ...,
    Protocols: Sequence[ProtocolType] = ...,  # (6)
    ProtocolDetails: ProtocolDetailsTypeDef = ...,  # (7)
    SecurityPolicyName: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (8)
    WorkflowDetails: WorkflowDetailsTypeDef = ...,  # (9)
    StructuredLogDestinations: Sequence[str] = ...,
    S3StorageOptions: S3StorageOptionsTypeDef = ...,  # (10)
) -> CreateServerResponseTypeDef:  # (11)
    ...
```

1. See [:material-code-brackets: DomainType](./literals.md#domaintype) 
2. See [:material-code-braces: EndpointDetailsTypeDef](./type_defs.md#endpointdetailstypedef) 
3. See [:material-code-brackets: EndpointTypeType](./literals.md#endpointtypetype) 
4. See [:material-code-braces: IdentityProviderDetailsTypeDef](./type_defs.md#identityproviderdetailstypedef) 
5. See [:material-code-brackets: IdentityProviderTypeType](./literals.md#identityprovidertypetype) 
6. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
7. See [:material-code-braces: ProtocolDetailsTypeDef](./type_defs.md#protocoldetailstypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
9. See [:material-code-braces: WorkflowDetailsTypeDef](./type_defs.md#workflowdetailstypedef) 
10. See [:material-code-braces: S3StorageOptionsTypeDef](./type_defs.md#s3storageoptionstypedef) 
11. See [:material-code-braces: CreateServerResponseTypeDef](./type_defs.md#createserverresponsetypedef) 


```python
# create_server method usage example with argument unpacking

kwargs: CreateServerRequestRequestTypeDef = {  # (1)
    "Certificate": ...,
}

parent.create_server(**kwargs)
```

1. See [:material-code-braces: CreateServerRequestRequestTypeDef](./type_defs.md#createserverrequestrequesttypedef) 

### create\_user

Creates a user and associates them with an existing file transfer
protocol-enabled server.

Type annotations and code completion for `#!python session.client("transfer").create_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# create_user method definition

await def create_user(
    self,
    *,
    Role: str,
    ServerId: str,
    UserName: str,
    HomeDirectory: str = ...,
    HomeDirectoryType: HomeDirectoryTypeType = ...,  # (1)
    HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,  # (2)
    Policy: str = ...,
    PosixProfile: PosixProfileTypeDef = ...,  # (3)
    SshPublicKeyBody: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateUserResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: HomeDirectoryTypeType](./literals.md#homedirectorytypetype) 
2. See [:material-code-braces: HomeDirectoryMapEntryTypeDef](./type_defs.md#homedirectorymapentrytypedef) 
3. See [:material-code-braces: PosixProfileTypeDef](./type_defs.md#posixprofiletypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateUserResponseTypeDef](./type_defs.md#createuserresponsetypedef) 


```python
# create_user method usage example with argument unpacking

kwargs: CreateUserRequestRequestTypeDef = {  # (1)
    "Role": ...,
    "ServerId": ...,
    "UserName": ...,
}

parent.create_user(**kwargs)
```

1. See [:material-code-braces: CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef) 

### create\_web\_app

Creates a web app based on specified parameters, and returns the ID for the new
web app.

Type annotations and code completion for `#!python session.client("transfer").create_web_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# create_web_app method definition

await def create_web_app(
    self,
    *,
    IdentityProviderDetails: WebAppIdentityProviderDetailsTypeDef,  # (1)
    AccessEndpoint: str = ...,
    WebAppUnits: WebAppUnitsTypeDef = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateWebAppResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: WebAppIdentityProviderDetailsTypeDef](./type_defs.md#webappidentityproviderdetailstypedef) 
2. See [:material-code-braces: WebAppUnitsTypeDef](./type_defs.md#webappunitstypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateWebAppResponseTypeDef](./type_defs.md#createwebappresponsetypedef) 


```python
# create_web_app method usage example with argument unpacking

kwargs: CreateWebAppRequestRequestTypeDef = {  # (1)
    "IdentityProviderDetails": ...,
}

parent.create_web_app(**kwargs)
```

1. See [:material-code-braces: CreateWebAppRequestRequestTypeDef](./type_defs.md#createwebapprequestrequesttypedef) 

### create\_workflow

Allows you to create a workflow with specified steps and step details the
workflow invokes after file transfer completes.

Type annotations and code completion for `#!python session.client("transfer").create_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# create_workflow method definition

await def create_workflow(
    self,
    *,
    Steps: Sequence[WorkflowStepUnionTypeDef],  # (1)
    Description: str = ...,
    OnExceptionSteps: Sequence[WorkflowStepTypeDef] = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateWorkflowResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: WorkflowStepTypeDef](./type_defs.md#workflowsteptypedef) [:material-code-braces: WorkflowStepOutputTypeDef](./type_defs.md#workflowstepoutputtypedef) 
2. See [:material-code-braces: WorkflowStepTypeDef](./type_defs.md#workflowsteptypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateWorkflowResponseTypeDef](./type_defs.md#createworkflowresponsetypedef) 


```python
# create_workflow method usage example with argument unpacking

kwargs: CreateWorkflowRequestRequestTypeDef = {  # (1)
    "Steps": ...,
}

parent.create_workflow(**kwargs)
```

1. See [:material-code-braces: CreateWorkflowRequestRequestTypeDef](./type_defs.md#createworkflowrequestrequesttypedef) 

### delete\_access

Allows you to delete the access specified in the <code>ServerID</code> and
<code>ExternalID</code> parameters.

Type annotations and code completion for `#!python session.client("transfer").delete_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# delete_access method definition

await def delete_access(
    self,
    *,
    ServerId: str,
    ExternalId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_access method usage example with argument unpacking

kwargs: DeleteAccessRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
    "ExternalId": ...,
}

parent.delete_access(**kwargs)
```

1. See [:material-code-braces: DeleteAccessRequestRequestTypeDef](./type_defs.md#deleteaccessrequestrequesttypedef) 

### delete\_agreement

Delete the agreement that's specified in the provided <code>AgreementId</code>.

Type annotations and code completion for `#!python session.client("transfer").delete_agreement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# delete_agreement method definition

await def delete_agreement(
    self,
    *,
    AgreementId: str,
    ServerId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_agreement method usage example with argument unpacking

kwargs: DeleteAgreementRequestRequestTypeDef = {  # (1)
    "AgreementId": ...,
    "ServerId": ...,
}

parent.delete_agreement(**kwargs)
```

1. See [:material-code-braces: DeleteAgreementRequestRequestTypeDef](./type_defs.md#deleteagreementrequestrequesttypedef) 

### delete\_certificate

Deletes the certificate that's specified in the <code>CertificateId</code>
parameter.

Type annotations and code completion for `#!python session.client("transfer").delete_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# delete_certificate method definition

await def delete_certificate(
    self,
    *,
    CertificateId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_certificate method usage example with argument unpacking

kwargs: DeleteCertificateRequestRequestTypeDef = {  # (1)
    "CertificateId": ...,
}

parent.delete_certificate(**kwargs)
```

1. See [:material-code-braces: DeleteCertificateRequestRequestTypeDef](./type_defs.md#deletecertificaterequestrequesttypedef) 

### delete\_connector

Deletes the connector that's specified in the provided <code>ConnectorId</code>.

Type annotations and code completion for `#!python session.client("transfer").delete_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# delete_connector method definition

await def delete_connector(
    self,
    *,
    ConnectorId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_connector method usage example with argument unpacking

kwargs: DeleteConnectorRequestRequestTypeDef = {  # (1)
    "ConnectorId": ...,
}

parent.delete_connector(**kwargs)
```

1. See [:material-code-braces: DeleteConnectorRequestRequestTypeDef](./type_defs.md#deleteconnectorrequestrequesttypedef) 

### delete\_host\_key

Deletes the host key that's specified in the <code>HostKeyId</code> parameter.

Type annotations and code completion for `#!python session.client("transfer").delete_host_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# delete_host_key method definition

await def delete_host_key(
    self,
    *,
    ServerId: str,
    HostKeyId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_host_key method usage example with argument unpacking

kwargs: DeleteHostKeyRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
    "HostKeyId": ...,
}

parent.delete_host_key(**kwargs)
```

1. See [:material-code-braces: DeleteHostKeyRequestRequestTypeDef](./type_defs.md#deletehostkeyrequestrequesttypedef) 

### delete\_profile

Deletes the profile that's specified in the <code>ProfileId</code> parameter.

Type annotations and code completion for `#!python session.client("transfer").delete_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# delete_profile method definition

await def delete_profile(
    self,
    *,
    ProfileId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_profile method usage example with argument unpacking

kwargs: DeleteProfileRequestRequestTypeDef = {  # (1)
    "ProfileId": ...,
}

parent.delete_profile(**kwargs)
```

1. See [:material-code-braces: DeleteProfileRequestRequestTypeDef](./type_defs.md#deleteprofilerequestrequesttypedef) 

### delete\_server

Deletes the file transfer protocol-enabled server that you specify.

Type annotations and code completion for `#!python session.client("transfer").delete_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# delete_server method definition

await def delete_server(
    self,
    *,
    ServerId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_server method usage example with argument unpacking

kwargs: DeleteServerRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
}

parent.delete_server(**kwargs)
```

1. See [:material-code-braces: DeleteServerRequestRequestTypeDef](./type_defs.md#deleteserverrequestrequesttypedef) 

### delete\_ssh\_public\_key

Deletes a user's Secure Shell (SSH) public key.

Type annotations and code completion for `#!python session.client("transfer").delete_ssh_public_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# delete_ssh_public_key method definition

await def delete_ssh_public_key(
    self,
    *,
    ServerId: str,
    SshPublicKeyId: str,
    UserName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_ssh_public_key method usage example with argument unpacking

kwargs: DeleteSshPublicKeyRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
    "SshPublicKeyId": ...,
    "UserName": ...,
}

parent.delete_ssh_public_key(**kwargs)
```

1. See [:material-code-braces: DeleteSshPublicKeyRequestRequestTypeDef](./type_defs.md#deletesshpublickeyrequestrequesttypedef) 

### delete\_user

Deletes the user belonging to a file transfer protocol-enabled server you
specify.

Type annotations and code completion for `#!python session.client("transfer").delete_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# delete_user method definition

await def delete_user(
    self,
    *,
    ServerId: str,
    UserName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_user method usage example with argument unpacking

kwargs: DeleteUserRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
    "UserName": ...,
}

parent.delete_user(**kwargs)
```

1. See [:material-code-braces: DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef) 

### delete\_web\_app

Deletes the specified web app.

Type annotations and code completion for `#!python session.client("transfer").delete_web_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# delete_web_app method definition

await def delete_web_app(
    self,
    *,
    WebAppId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_web_app method usage example with argument unpacking

kwargs: DeleteWebAppRequestRequestTypeDef = {  # (1)
    "WebAppId": ...,
}

parent.delete_web_app(**kwargs)
```

1. See [:material-code-braces: DeleteWebAppRequestRequestTypeDef](./type_defs.md#deletewebapprequestrequesttypedef) 

### delete\_web\_app\_customization

Deletes the <code>WebAppCustomization</code> object that corresponds to the web
app ID specified.

Type annotations and code completion for `#!python session.client("transfer").delete_web_app_customization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# delete_web_app_customization method definition

await def delete_web_app_customization(
    self,
    *,
    WebAppId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_web_app_customization method usage example with argument unpacking

kwargs: DeleteWebAppCustomizationRequestRequestTypeDef = {  # (1)
    "WebAppId": ...,
}

parent.delete_web_app_customization(**kwargs)
```

1. See [:material-code-braces: DeleteWebAppCustomizationRequestRequestTypeDef](./type_defs.md#deletewebappcustomizationrequestrequesttypedef) 

### delete\_workflow

Deletes the specified workflow.

Type annotations and code completion for `#!python session.client("transfer").delete_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# delete_workflow method definition

await def delete_workflow(
    self,
    *,
    WorkflowId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_workflow method usage example with argument unpacking

kwargs: DeleteWorkflowRequestRequestTypeDef = {  # (1)
    "WorkflowId": ...,
}

parent.delete_workflow(**kwargs)
```

1. See [:material-code-braces: DeleteWorkflowRequestRequestTypeDef](./type_defs.md#deleteworkflowrequestrequesttypedef) 

### describe\_access

Describes the access that is assigned to the specific file transfer
protocol-enabled server, as identified by its <code>ServerId</code> property
and its <code>ExternalId</code>.

Type annotations and code completion for `#!python session.client("transfer").describe_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# describe_access method definition

await def describe_access(
    self,
    *,
    ServerId: str,
    ExternalId: str,
) -> DescribeAccessResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAccessResponseTypeDef](./type_defs.md#describeaccessresponsetypedef) 


```python
# describe_access method usage example with argument unpacking

kwargs: DescribeAccessRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
    "ExternalId": ...,
}

parent.describe_access(**kwargs)
```

1. See [:material-code-braces: DescribeAccessRequestRequestTypeDef](./type_defs.md#describeaccessrequestrequesttypedef) 

### describe\_agreement

Describes the agreement that's identified by the <code>AgreementId</code>.

Type annotations and code completion for `#!python session.client("transfer").describe_agreement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# describe_agreement method definition

await def describe_agreement(
    self,
    *,
    AgreementId: str,
    ServerId: str,
) -> DescribeAgreementResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAgreementResponseTypeDef](./type_defs.md#describeagreementresponsetypedef) 


```python
# describe_agreement method usage example with argument unpacking

kwargs: DescribeAgreementRequestRequestTypeDef = {  # (1)
    "AgreementId": ...,
    "ServerId": ...,
}

parent.describe_agreement(**kwargs)
```

1. See [:material-code-braces: DescribeAgreementRequestRequestTypeDef](./type_defs.md#describeagreementrequestrequesttypedef) 

### describe\_certificate

Describes the certificate that's identified by the <code>CertificateId</code>.

Type annotations and code completion for `#!python session.client("transfer").describe_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# describe_certificate method definition

await def describe_certificate(
    self,
    *,
    CertificateId: str,
) -> DescribeCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCertificateResponseTypeDef](./type_defs.md#describecertificateresponsetypedef) 


```python
# describe_certificate method usage example with argument unpacking

kwargs: DescribeCertificateRequestRequestTypeDef = {  # (1)
    "CertificateId": ...,
}

parent.describe_certificate(**kwargs)
```

1. See [:material-code-braces: DescribeCertificateRequestRequestTypeDef](./type_defs.md#describecertificaterequestrequesttypedef) 

### describe\_connector

Describes the connector that's identified by the <code>ConnectorId.</code>.

Type annotations and code completion for `#!python session.client("transfer").describe_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# describe_connector method definition

await def describe_connector(
    self,
    *,
    ConnectorId: str,
) -> DescribeConnectorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeConnectorResponseTypeDef](./type_defs.md#describeconnectorresponsetypedef) 


```python
# describe_connector method usage example with argument unpacking

kwargs: DescribeConnectorRequestRequestTypeDef = {  # (1)
    "ConnectorId": ...,
}

parent.describe_connector(**kwargs)
```

1. See [:material-code-braces: DescribeConnectorRequestRequestTypeDef](./type_defs.md#describeconnectorrequestrequesttypedef) 

### describe\_execution

You can use <code>DescribeExecution</code> to check the details of the
execution of the specified workflow.

Type annotations and code completion for `#!python session.client("transfer").describe_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# describe_execution method definition

await def describe_execution(
    self,
    *,
    ExecutionId: str,
    WorkflowId: str,
) -> DescribeExecutionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeExecutionResponseTypeDef](./type_defs.md#describeexecutionresponsetypedef) 


```python
# describe_execution method usage example with argument unpacking

kwargs: DescribeExecutionRequestRequestTypeDef = {  # (1)
    "ExecutionId": ...,
    "WorkflowId": ...,
}

parent.describe_execution(**kwargs)
```

1. See [:material-code-braces: DescribeExecutionRequestRequestTypeDef](./type_defs.md#describeexecutionrequestrequesttypedef) 

### describe\_host\_key

Returns the details of the host key that's specified by the
<code>HostKeyId</code> and <code>ServerId</code>.

Type annotations and code completion for `#!python session.client("transfer").describe_host_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# describe_host_key method definition

await def describe_host_key(
    self,
    *,
    ServerId: str,
    HostKeyId: str,
) -> DescribeHostKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeHostKeyResponseTypeDef](./type_defs.md#describehostkeyresponsetypedef) 


```python
# describe_host_key method usage example with argument unpacking

kwargs: DescribeHostKeyRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
    "HostKeyId": ...,
}

parent.describe_host_key(**kwargs)
```

1. See [:material-code-braces: DescribeHostKeyRequestRequestTypeDef](./type_defs.md#describehostkeyrequestrequesttypedef) 

### describe\_profile

Returns the details of the profile that's specified by the
<code>ProfileId</code>.

Type annotations and code completion for `#!python session.client("transfer").describe_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# describe_profile method definition

await def describe_profile(
    self,
    *,
    ProfileId: str,
) -> DescribeProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeProfileResponseTypeDef](./type_defs.md#describeprofileresponsetypedef) 


```python
# describe_profile method usage example with argument unpacking

kwargs: DescribeProfileRequestRequestTypeDef = {  # (1)
    "ProfileId": ...,
}

parent.describe_profile(**kwargs)
```

1. See [:material-code-braces: DescribeProfileRequestRequestTypeDef](./type_defs.md#describeprofilerequestrequesttypedef) 

### describe\_security\_policy

Describes the security policy that is attached to your server or SFTP connector.

Type annotations and code completion for `#!python session.client("transfer").describe_security_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# describe_security_policy method definition

await def describe_security_policy(
    self,
    *,
    SecurityPolicyName: str,
) -> DescribeSecurityPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSecurityPolicyResponseTypeDef](./type_defs.md#describesecuritypolicyresponsetypedef) 


```python
# describe_security_policy method usage example with argument unpacking

kwargs: DescribeSecurityPolicyRequestRequestTypeDef = {  # (1)
    "SecurityPolicyName": ...,
}

parent.describe_security_policy(**kwargs)
```

1. See [:material-code-braces: DescribeSecurityPolicyRequestRequestTypeDef](./type_defs.md#describesecuritypolicyrequestrequesttypedef) 

### describe\_server

Describes a file transfer protocol-enabled server that you specify by passing
the <code>ServerId</code> parameter.

Type annotations and code completion for `#!python session.client("transfer").describe_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# describe_server method definition

await def describe_server(
    self,
    *,
    ServerId: str,
) -> DescribeServerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeServerResponseTypeDef](./type_defs.md#describeserverresponsetypedef) 


```python
# describe_server method usage example with argument unpacking

kwargs: DescribeServerRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
}

parent.describe_server(**kwargs)
```

1. See [:material-code-braces: DescribeServerRequestRequestTypeDef](./type_defs.md#describeserverrequestrequesttypedef) 

### describe\_user

Describes the user assigned to the specific file transfer protocol-enabled
server, as identified by its <code>ServerId</code> property.

Type annotations and code completion for `#!python session.client("transfer").describe_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# describe_user method definition

await def describe_user(
    self,
    *,
    ServerId: str,
    UserName: str,
) -> DescribeUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeUserResponseTypeDef](./type_defs.md#describeuserresponsetypedef) 


```python
# describe_user method usage example with argument unpacking

kwargs: DescribeUserRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
    "UserName": ...,
}

parent.describe_user(**kwargs)
```

1. See [:material-code-braces: DescribeUserRequestRequestTypeDef](./type_defs.md#describeuserrequestrequesttypedef) 

### describe\_web\_app

Describes the web app that's identified by <code>WebAppId</code>.

Type annotations and code completion for `#!python session.client("transfer").describe_web_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# describe_web_app method definition

await def describe_web_app(
    self,
    *,
    WebAppId: str,
) -> DescribeWebAppResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWebAppResponseTypeDef](./type_defs.md#describewebappresponsetypedef) 


```python
# describe_web_app method usage example with argument unpacking

kwargs: DescribeWebAppRequestRequestTypeDef = {  # (1)
    "WebAppId": ...,
}

parent.describe_web_app(**kwargs)
```

1. See [:material-code-braces: DescribeWebAppRequestRequestTypeDef](./type_defs.md#describewebapprequestrequesttypedef) 

### describe\_web\_app\_customization

Describes the web app customization object that's identified by
<code>WebAppId</code>.

Type annotations and code completion for `#!python session.client("transfer").describe_web_app_customization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# describe_web_app_customization method definition

await def describe_web_app_customization(
    self,
    *,
    WebAppId: str,
) -> DescribeWebAppCustomizationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWebAppCustomizationResponseTypeDef](./type_defs.md#describewebappcustomizationresponsetypedef) 


```python
# describe_web_app_customization method usage example with argument unpacking

kwargs: DescribeWebAppCustomizationRequestRequestTypeDef = {  # (1)
    "WebAppId": ...,
}

parent.describe_web_app_customization(**kwargs)
```

1. See [:material-code-braces: DescribeWebAppCustomizationRequestRequestTypeDef](./type_defs.md#describewebappcustomizationrequestrequesttypedef) 

### describe\_workflow

Describes the specified workflow.

Type annotations and code completion for `#!python session.client("transfer").describe_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# describe_workflow method definition

await def describe_workflow(
    self,
    *,
    WorkflowId: str,
) -> DescribeWorkflowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWorkflowResponseTypeDef](./type_defs.md#describeworkflowresponsetypedef) 


```python
# describe_workflow method usage example with argument unpacking

kwargs: DescribeWorkflowRequestRequestTypeDef = {  # (1)
    "WorkflowId": ...,
}

parent.describe_workflow(**kwargs)
```

1. See [:material-code-braces: DescribeWorkflowRequestRequestTypeDef](./type_defs.md#describeworkflowrequestrequesttypedef) 

### import\_certificate

Imports the signing and encryption certificates that you need to create local
(AS2) profiles and partner profiles.

Type annotations and code completion for `#!python session.client("transfer").import_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# import_certificate method definition

await def import_certificate(
    self,
    *,
    Usage: CertificateUsageTypeType,  # (1)
    Certificate: str,
    CertificateChain: str = ...,
    PrivateKey: str = ...,
    ActiveDate: TimestampTypeDef = ...,
    InactiveDate: TimestampTypeDef = ...,
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> ImportCertificateResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: CertificateUsageTypeType](./literals.md#certificateusagetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ImportCertificateResponseTypeDef](./type_defs.md#importcertificateresponsetypedef) 


```python
# import_certificate method usage example with argument unpacking

kwargs: ImportCertificateRequestRequestTypeDef = {  # (1)
    "Usage": ...,
    "Certificate": ...,
}

parent.import_certificate(**kwargs)
```

1. See [:material-code-braces: ImportCertificateRequestRequestTypeDef](./type_defs.md#importcertificaterequestrequesttypedef) 

### import\_host\_key

Adds a host key to the server that's specified by the <code>ServerId</code>
parameter.

Type annotations and code completion for `#!python session.client("transfer").import_host_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# import_host_key method definition

await def import_host_key(
    self,
    *,
    ServerId: str,
    HostKeyBody: str,
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> ImportHostKeyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ImportHostKeyResponseTypeDef](./type_defs.md#importhostkeyresponsetypedef) 


```python
# import_host_key method usage example with argument unpacking

kwargs: ImportHostKeyRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
    "HostKeyBody": ...,
}

parent.import_host_key(**kwargs)
```

1. See [:material-code-braces: ImportHostKeyRequestRequestTypeDef](./type_defs.md#importhostkeyrequestrequesttypedef) 

### import\_ssh\_public\_key

Adds a Secure Shell (SSH) public key to a Transfer Family user identified by a
<code>UserName</code> value assigned to the specific file transfer
protocol-enabled server, identified by <code>ServerId</code>.

Type annotations and code completion for `#!python session.client("transfer").import_ssh_public_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# import_ssh_public_key method definition

await def import_ssh_public_key(
    self,
    *,
    ServerId: str,
    SshPublicKeyBody: str,
    UserName: str,
) -> ImportSshPublicKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ImportSshPublicKeyResponseTypeDef](./type_defs.md#importsshpublickeyresponsetypedef) 


```python
# import_ssh_public_key method usage example with argument unpacking

kwargs: ImportSshPublicKeyRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
    "SshPublicKeyBody": ...,
    "UserName": ...,
}

parent.import_ssh_public_key(**kwargs)
```

1. See [:material-code-braces: ImportSshPublicKeyRequestRequestTypeDef](./type_defs.md#importsshpublickeyrequestrequesttypedef) 

### list\_accesses

Lists the details for all the accesses you have on your server.

Type annotations and code completion for `#!python session.client("transfer").list_accesses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# list_accesses method definition

await def list_accesses(
    self,
    *,
    ServerId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAccessesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAccessesResponseTypeDef](./type_defs.md#listaccessesresponsetypedef) 


```python
# list_accesses method usage example with argument unpacking

kwargs: ListAccessesRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
}

parent.list_accesses(**kwargs)
```

1. See [:material-code-braces: ListAccessesRequestRequestTypeDef](./type_defs.md#listaccessesrequestrequesttypedef) 

### list\_agreements

Returns a list of the agreements for the server that's identified by the
<code>ServerId</code> that you supply.

Type annotations and code completion for `#!python session.client("transfer").list_agreements` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# list_agreements method definition

await def list_agreements(
    self,
    *,
    ServerId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAgreementsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAgreementsResponseTypeDef](./type_defs.md#listagreementsresponsetypedef) 


```python
# list_agreements method usage example with argument unpacking

kwargs: ListAgreementsRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
}

parent.list_agreements(**kwargs)
```

1. See [:material-code-braces: ListAgreementsRequestRequestTypeDef](./type_defs.md#listagreementsrequestrequesttypedef) 

### list\_certificates

Returns a list of the current certificates that have been imported into
Transfer Family.

Type annotations and code completion for `#!python session.client("transfer").list_certificates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# list_certificates method definition

await def list_certificates(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListCertificatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCertificatesResponseTypeDef](./type_defs.md#listcertificatesresponsetypedef) 


```python
# list_certificates method usage example with argument unpacking

kwargs: ListCertificatesRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_certificates(**kwargs)
```

1. See [:material-code-braces: ListCertificatesRequestRequestTypeDef](./type_defs.md#listcertificatesrequestrequesttypedef) 

### list\_connectors

Lists the connectors for the specified Region.

Type annotations and code completion for `#!python session.client("transfer").list_connectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# list_connectors method definition

await def list_connectors(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListConnectorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef) 


```python
# list_connectors method usage example with argument unpacking

kwargs: ListConnectorsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_connectors(**kwargs)
```

1. See [:material-code-braces: ListConnectorsRequestRequestTypeDef](./type_defs.md#listconnectorsrequestrequesttypedef) 

### list\_executions

Lists all in-progress executions for the specified workflow.

Type annotations and code completion for `#!python session.client("transfer").list_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# list_executions method definition

await def list_executions(
    self,
    *,
    WorkflowId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListExecutionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListExecutionsResponseTypeDef](./type_defs.md#listexecutionsresponsetypedef) 


```python
# list_executions method usage example with argument unpacking

kwargs: ListExecutionsRequestRequestTypeDef = {  # (1)
    "WorkflowId": ...,
}

parent.list_executions(**kwargs)
```

1. See [:material-code-braces: ListExecutionsRequestRequestTypeDef](./type_defs.md#listexecutionsrequestrequesttypedef) 

### list\_file\_transfer\_results

Returns real-time updates and detailed information on the status of each
individual file being transferred in a specific file transfer operation.

Type annotations and code completion for `#!python session.client("transfer").list_file_transfer_results` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# list_file_transfer_results method definition

await def list_file_transfer_results(
    self,
    *,
    ConnectorId: str,
    TransferId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListFileTransferResultsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFileTransferResultsResponseTypeDef](./type_defs.md#listfiletransferresultsresponsetypedef) 


```python
# list_file_transfer_results method usage example with argument unpacking

kwargs: ListFileTransferResultsRequestRequestTypeDef = {  # (1)
    "ConnectorId": ...,
    "TransferId": ...,
}

parent.list_file_transfer_results(**kwargs)
```

1. See [:material-code-braces: ListFileTransferResultsRequestRequestTypeDef](./type_defs.md#listfiletransferresultsrequestrequesttypedef) 

### list\_host\_keys

Returns a list of host keys for the server that's specified by the
<code>ServerId</code> parameter.

Type annotations and code completion for `#!python session.client("transfer").list_host_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# list_host_keys method definition

await def list_host_keys(
    self,
    *,
    ServerId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListHostKeysResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListHostKeysResponseTypeDef](./type_defs.md#listhostkeysresponsetypedef) 


```python
# list_host_keys method usage example with argument unpacking

kwargs: ListHostKeysRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
}

parent.list_host_keys(**kwargs)
```

1. See [:material-code-braces: ListHostKeysRequestRequestTypeDef](./type_defs.md#listhostkeysrequestrequesttypedef) 

### list\_profiles

Returns a list of the profiles for your system.

Type annotations and code completion for `#!python session.client("transfer").list_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# list_profiles method definition

await def list_profiles(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    ProfileType: ProfileTypeType = ...,  # (1)
) -> ListProfilesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ProfileTypeType](./literals.md#profiletypetype) 
2. See [:material-code-braces: ListProfilesResponseTypeDef](./type_defs.md#listprofilesresponsetypedef) 


```python
# list_profiles method usage example with argument unpacking

kwargs: ListProfilesRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_profiles(**kwargs)
```

1. See [:material-code-braces: ListProfilesRequestRequestTypeDef](./type_defs.md#listprofilesrequestrequesttypedef) 

### list\_security\_policies

Lists the security policies that are attached to your servers and SFTP
connectors.

Type annotations and code completion for `#!python session.client("transfer").list_security_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# list_security_policies method definition

await def list_security_policies(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListSecurityPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSecurityPoliciesResponseTypeDef](./type_defs.md#listsecuritypoliciesresponsetypedef) 


```python
# list_security_policies method usage example with argument unpacking

kwargs: ListSecurityPoliciesRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_security_policies(**kwargs)
```

1. See [:material-code-braces: ListSecurityPoliciesRequestRequestTypeDef](./type_defs.md#listsecuritypoliciesrequestrequesttypedef) 

### list\_servers

Lists the file transfer protocol-enabled servers that are associated with your
Amazon Web Services account.

Type annotations and code completion for `#!python session.client("transfer").list_servers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# list_servers method definition

await def list_servers(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListServersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServersResponseTypeDef](./type_defs.md#listserversresponsetypedef) 


```python
# list_servers method usage example with argument unpacking

kwargs: ListServersRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_servers(**kwargs)
```

1. See [:material-code-braces: ListServersRequestRequestTypeDef](./type_defs.md#listserversrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists all of the tags associated with the Amazon Resource Name (ARN) that you
specify.

Type annotations and code completion for `#!python session.client("transfer").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    Arn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_users

Lists the users for a file transfer protocol-enabled server that you specify by
passing the <code>ServerId</code> parameter.

Type annotations and code completion for `#!python session.client("transfer").list_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# list_users method definition

await def list_users(
    self,
    *,
    ServerId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListUsersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


```python
# list_users method usage example with argument unpacking

kwargs: ListUsersRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
}

parent.list_users(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestRequestTypeDef](./type_defs.md#listusersrequestrequesttypedef) 

### list\_web\_apps

Lists all web apps associated with your Amazon Web Services account for your
current region.

Type annotations and code completion for `#!python session.client("transfer").list_web_apps` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# list_web_apps method definition

await def list_web_apps(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListWebAppsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWebAppsResponseTypeDef](./type_defs.md#listwebappsresponsetypedef) 


```python
# list_web_apps method usage example with argument unpacking

kwargs: ListWebAppsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_web_apps(**kwargs)
```

1. See [:material-code-braces: ListWebAppsRequestRequestTypeDef](./type_defs.md#listwebappsrequestrequesttypedef) 

### list\_workflows

Lists all workflows associated with your Amazon Web Services account for your
current region.

Type annotations and code completion for `#!python session.client("transfer").list_workflows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# list_workflows method definition

await def list_workflows(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListWorkflowsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkflowsResponseTypeDef](./type_defs.md#listworkflowsresponsetypedef) 


```python
# list_workflows method usage example with argument unpacking

kwargs: ListWorkflowsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_workflows(**kwargs)
```

1. See [:material-code-braces: ListWorkflowsRequestRequestTypeDef](./type_defs.md#listworkflowsrequestrequesttypedef) 

### send\_workflow\_step\_state

Sends a callback for asynchronous custom steps.

Type annotations and code completion for `#!python session.client("transfer").send_workflow_step_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# send_workflow_step_state method definition

await def send_workflow_step_state(
    self,
    *,
    WorkflowId: str,
    ExecutionId: str,
    Token: str,
    Status: CustomStepStatusType,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: CustomStepStatusType](./literals.md#customstepstatustype) 


```python
# send_workflow_step_state method usage example with argument unpacking

kwargs: SendWorkflowStepStateRequestRequestTypeDef = {  # (1)
    "WorkflowId": ...,
    "ExecutionId": ...,
    "Token": ...,
    "Status": ...,
}

parent.send_workflow_step_state(**kwargs)
```

1. See [:material-code-braces: SendWorkflowStepStateRequestRequestTypeDef](./type_defs.md#sendworkflowstepstaterequestrequesttypedef) 

### start\_directory\_listing

Retrieves a list of the contents of a directory from a remote SFTP server.

Type annotations and code completion for `#!python session.client("transfer").start_directory_listing` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# start_directory_listing method definition

await def start_directory_listing(
    self,
    *,
    ConnectorId: str,
    RemoteDirectoryPath: str,
    OutputDirectoryPath: str,
    MaxItems: int = ...,
) -> StartDirectoryListingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartDirectoryListingResponseTypeDef](./type_defs.md#startdirectorylistingresponsetypedef) 


```python
# start_directory_listing method usage example with argument unpacking

kwargs: StartDirectoryListingRequestRequestTypeDef = {  # (1)
    "ConnectorId": ...,
    "RemoteDirectoryPath": ...,
    "OutputDirectoryPath": ...,
}

parent.start_directory_listing(**kwargs)
```

1. See [:material-code-braces: StartDirectoryListingRequestRequestTypeDef](./type_defs.md#startdirectorylistingrequestrequesttypedef) 

### start\_file\_transfer

Begins a file transfer between local Amazon Web Services storage and a remote
AS2 or SFTP server.

Type annotations and code completion for `#!python session.client("transfer").start_file_transfer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# start_file_transfer method definition

await def start_file_transfer(
    self,
    *,
    ConnectorId: str,
    SendFilePaths: Sequence[str] = ...,
    RetrieveFilePaths: Sequence[str] = ...,
    LocalDirectoryPath: str = ...,
    RemoteDirectoryPath: str = ...,
) -> StartFileTransferResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartFileTransferResponseTypeDef](./type_defs.md#startfiletransferresponsetypedef) 


```python
# start_file_transfer method usage example with argument unpacking

kwargs: StartFileTransferRequestRequestTypeDef = {  # (1)
    "ConnectorId": ...,
}

parent.start_file_transfer(**kwargs)
```

1. See [:material-code-braces: StartFileTransferRequestRequestTypeDef](./type_defs.md#startfiletransferrequestrequesttypedef) 

### start\_server

Changes the state of a file transfer protocol-enabled server from
<code>OFFLINE</code> to <code>ONLINE</code>.

Type annotations and code completion for `#!python session.client("transfer").start_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# start_server method definition

await def start_server(
    self,
    *,
    ServerId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# start_server method usage example with argument unpacking

kwargs: StartServerRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
}

parent.start_server(**kwargs)
```

1. See [:material-code-braces: StartServerRequestRequestTypeDef](./type_defs.md#startserverrequestrequesttypedef) 

### stop\_server

Changes the state of a file transfer protocol-enabled server from
<code>ONLINE</code> to <code>OFFLINE</code>.

Type annotations and code completion for `#!python session.client("transfer").stop_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# stop_server method definition

await def stop_server(
    self,
    *,
    ServerId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_server method usage example with argument unpacking

kwargs: StopServerRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
}

parent.stop_server(**kwargs)
```

1. See [:material-code-braces: StopServerRequestRequestTypeDef](./type_defs.md#stopserverrequestrequesttypedef) 

### tag\_resource

Attaches a key-value pair to a resource, as identified by its Amazon Resource
Name (ARN).

Type annotations and code completion for `#!python session.client("transfer").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    Arn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "Arn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### test\_connection

Tests whether your SFTP connector is set up successfully.

Type annotations and code completion for `#!python session.client("transfer").test_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# test_connection method definition

await def test_connection(
    self,
    *,
    ConnectorId: str,
) -> TestConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TestConnectionResponseTypeDef](./type_defs.md#testconnectionresponsetypedef) 


```python
# test_connection method usage example with argument unpacking

kwargs: TestConnectionRequestRequestTypeDef = {  # (1)
    "ConnectorId": ...,
}

parent.test_connection(**kwargs)
```

1. See [:material-code-braces: TestConnectionRequestRequestTypeDef](./type_defs.md#testconnectionrequestrequesttypedef) 

### test\_identity\_provider

If the <code>IdentityProviderType</code> of a file transfer protocol-enabled
server is <code>AWS_DIRECTORY_SERVICE</code> or <code>API_Gateway</code>, tests
whether your identity provider is set up successfully.

Type annotations and code completion for `#!python session.client("transfer").test_identity_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# test_identity_provider method definition

await def test_identity_provider(
    self,
    *,
    ServerId: str,
    UserName: str,
    ServerProtocol: ProtocolType = ...,  # (1)
    SourceIp: str = ...,
    UserPassword: str = ...,
) -> TestIdentityProviderResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
2. See [:material-code-braces: TestIdentityProviderResponseTypeDef](./type_defs.md#testidentityproviderresponsetypedef) 


```python
# test_identity_provider method usage example with argument unpacking

kwargs: TestIdentityProviderRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
    "UserName": ...,
}

parent.test_identity_provider(**kwargs)
```

1. See [:material-code-braces: TestIdentityProviderRequestRequestTypeDef](./type_defs.md#testidentityproviderrequestrequesttypedef) 

### untag\_resource

Detaches a key-value pair from a resource, as identified by its Amazon Resource
Name (ARN).

Type annotations and code completion for `#!python session.client("transfer").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    Arn: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "Arn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_access

Allows you to update parameters for the access specified in the
<code>ServerID</code> and <code>ExternalID</code> parameters.

Type annotations and code completion for `#!python session.client("transfer").update_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# update_access method definition

await def update_access(
    self,
    *,
    ServerId: str,
    ExternalId: str,
    HomeDirectory: str = ...,
    HomeDirectoryType: HomeDirectoryTypeType = ...,  # (1)
    HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,  # (2)
    Policy: str = ...,
    PosixProfile: PosixProfileTypeDef = ...,  # (3)
    Role: str = ...,
) -> UpdateAccessResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: HomeDirectoryTypeType](./literals.md#homedirectorytypetype) 
2. See [:material-code-braces: HomeDirectoryMapEntryTypeDef](./type_defs.md#homedirectorymapentrytypedef) 
3. See [:material-code-braces: PosixProfileTypeDef](./type_defs.md#posixprofiletypedef) 
4. See [:material-code-braces: UpdateAccessResponseTypeDef](./type_defs.md#updateaccessresponsetypedef) 


```python
# update_access method usage example with argument unpacking

kwargs: UpdateAccessRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
    "ExternalId": ...,
}

parent.update_access(**kwargs)
```

1. See [:material-code-braces: UpdateAccessRequestRequestTypeDef](./type_defs.md#updateaccessrequestrequesttypedef) 

### update\_agreement

Updates some of the parameters for an existing agreement.

Type annotations and code completion for `#!python session.client("transfer").update_agreement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# update_agreement method definition

await def update_agreement(
    self,
    *,
    AgreementId: str,
    ServerId: str,
    Description: str = ...,
    Status: AgreementStatusTypeType = ...,  # (1)
    LocalProfileId: str = ...,
    PartnerProfileId: str = ...,
    BaseDirectory: str = ...,
    AccessRole: str = ...,
) -> UpdateAgreementResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AgreementStatusTypeType](./literals.md#agreementstatustypetype) 
2. See [:material-code-braces: UpdateAgreementResponseTypeDef](./type_defs.md#updateagreementresponsetypedef) 


```python
# update_agreement method usage example with argument unpacking

kwargs: UpdateAgreementRequestRequestTypeDef = {  # (1)
    "AgreementId": ...,
    "ServerId": ...,
}

parent.update_agreement(**kwargs)
```

1. See [:material-code-braces: UpdateAgreementRequestRequestTypeDef](./type_defs.md#updateagreementrequestrequesttypedef) 

### update\_certificate

Updates the active and inactive dates for a certificate.

Type annotations and code completion for `#!python session.client("transfer").update_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# update_certificate method definition

await def update_certificate(
    self,
    *,
    CertificateId: str,
    ActiveDate: TimestampTypeDef = ...,
    InactiveDate: TimestampTypeDef = ...,
    Description: str = ...,
) -> UpdateCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateCertificateResponseTypeDef](./type_defs.md#updatecertificateresponsetypedef) 


```python
# update_certificate method usage example with argument unpacking

kwargs: UpdateCertificateRequestRequestTypeDef = {  # (1)
    "CertificateId": ...,
}

parent.update_certificate(**kwargs)
```

1. See [:material-code-braces: UpdateCertificateRequestRequestTypeDef](./type_defs.md#updatecertificaterequestrequesttypedef) 

### update\_connector

Updates some of the parameters for an existing connector.

Type annotations and code completion for `#!python session.client("transfer").update_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# update_connector method definition

await def update_connector(
    self,
    *,
    ConnectorId: str,
    Url: str = ...,
    As2Config: As2ConnectorConfigTypeDef = ...,  # (1)
    AccessRole: str = ...,
    LoggingRole: str = ...,
    SftpConfig: SftpConnectorConfigTypeDef = ...,  # (2)
    SecurityPolicyName: str = ...,
) -> UpdateConnectorResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: As2ConnectorConfigTypeDef](./type_defs.md#as2connectorconfigtypedef) 
2. See [:material-code-braces: SftpConnectorConfigTypeDef](./type_defs.md#sftpconnectorconfigtypedef) 
3. See [:material-code-braces: UpdateConnectorResponseTypeDef](./type_defs.md#updateconnectorresponsetypedef) 


```python
# update_connector method usage example with argument unpacking

kwargs: UpdateConnectorRequestRequestTypeDef = {  # (1)
    "ConnectorId": ...,
}

parent.update_connector(**kwargs)
```

1. See [:material-code-braces: UpdateConnectorRequestRequestTypeDef](./type_defs.md#updateconnectorrequestrequesttypedef) 

### update\_host\_key

Updates the description for the host key that's specified by the
<code>ServerId</code> and <code>HostKeyId</code> parameters.

Type annotations and code completion for `#!python session.client("transfer").update_host_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# update_host_key method definition

await def update_host_key(
    self,
    *,
    ServerId: str,
    HostKeyId: str,
    Description: str,
) -> UpdateHostKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateHostKeyResponseTypeDef](./type_defs.md#updatehostkeyresponsetypedef) 


```python
# update_host_key method usage example with argument unpacking

kwargs: UpdateHostKeyRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
    "HostKeyId": ...,
    "Description": ...,
}

parent.update_host_key(**kwargs)
```

1. See [:material-code-braces: UpdateHostKeyRequestRequestTypeDef](./type_defs.md#updatehostkeyrequestrequesttypedef) 

### update\_profile

Updates some of the parameters for an existing profile.

Type annotations and code completion for `#!python session.client("transfer").update_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# update_profile method definition

await def update_profile(
    self,
    *,
    ProfileId: str,
    CertificateIds: Sequence[str] = ...,
) -> UpdateProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateProfileResponseTypeDef](./type_defs.md#updateprofileresponsetypedef) 


```python
# update_profile method usage example with argument unpacking

kwargs: UpdateProfileRequestRequestTypeDef = {  # (1)
    "ProfileId": ...,
}

parent.update_profile(**kwargs)
```

1. See [:material-code-braces: UpdateProfileRequestRequestTypeDef](./type_defs.md#updateprofilerequestrequesttypedef) 

### update\_server

Updates the file transfer protocol-enabled server's properties after that
server has been created.

Type annotations and code completion for `#!python session.client("transfer").update_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# update_server method definition

await def update_server(
    self,
    *,
    ServerId: str,
    Certificate: str = ...,
    ProtocolDetails: ProtocolDetailsTypeDef = ...,  # (1)
    EndpointDetails: EndpointDetailsTypeDef = ...,  # (2)
    EndpointType: EndpointTypeType = ...,  # (3)
    HostKey: str = ...,
    IdentityProviderDetails: IdentityProviderDetailsTypeDef = ...,  # (4)
    LoggingRole: str = ...,
    PostAuthenticationLoginBanner: str = ...,
    PreAuthenticationLoginBanner: str = ...,
    Protocols: Sequence[ProtocolType] = ...,  # (5)
    SecurityPolicyName: str = ...,
    WorkflowDetails: WorkflowDetailsTypeDef = ...,  # (6)
    StructuredLogDestinations: Sequence[str] = ...,
    S3StorageOptions: S3StorageOptionsTypeDef = ...,  # (7)
) -> UpdateServerResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-braces: ProtocolDetailsTypeDef](./type_defs.md#protocoldetailstypedef) 
2. See [:material-code-braces: EndpointDetailsTypeDef](./type_defs.md#endpointdetailstypedef) 
3. See [:material-code-brackets: EndpointTypeType](./literals.md#endpointtypetype) 
4. See [:material-code-braces: IdentityProviderDetailsTypeDef](./type_defs.md#identityproviderdetailstypedef) 
5. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
6. See [:material-code-braces: WorkflowDetailsTypeDef](./type_defs.md#workflowdetailstypedef) 
7. See [:material-code-braces: S3StorageOptionsTypeDef](./type_defs.md#s3storageoptionstypedef) 
8. See [:material-code-braces: UpdateServerResponseTypeDef](./type_defs.md#updateserverresponsetypedef) 


```python
# update_server method usage example with argument unpacking

kwargs: UpdateServerRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
}

parent.update_server(**kwargs)
```

1. See [:material-code-braces: UpdateServerRequestRequestTypeDef](./type_defs.md#updateserverrequestrequesttypedef) 

### update\_user

Assigns new properties to a user.

Type annotations and code completion for `#!python session.client("transfer").update_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# update_user method definition

await def update_user(
    self,
    *,
    ServerId: str,
    UserName: str,
    HomeDirectory: str = ...,
    HomeDirectoryType: HomeDirectoryTypeType = ...,  # (1)
    HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,  # (2)
    Policy: str = ...,
    PosixProfile: PosixProfileTypeDef = ...,  # (3)
    Role: str = ...,
) -> UpdateUserResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: HomeDirectoryTypeType](./literals.md#homedirectorytypetype) 
2. See [:material-code-braces: HomeDirectoryMapEntryTypeDef](./type_defs.md#homedirectorymapentrytypedef) 
3. See [:material-code-braces: PosixProfileTypeDef](./type_defs.md#posixprofiletypedef) 
4. See [:material-code-braces: UpdateUserResponseTypeDef](./type_defs.md#updateuserresponsetypedef) 


```python
# update_user method usage example with argument unpacking

kwargs: UpdateUserRequestRequestTypeDef = {  # (1)
    "ServerId": ...,
    "UserName": ...,
}

parent.update_user(**kwargs)
```

1. See [:material-code-braces: UpdateUserRequestRequestTypeDef](./type_defs.md#updateuserrequestrequesttypedef) 

### update\_web\_app

Assigns new properties to a web app.

Type annotations and code completion for `#!python session.client("transfer").update_web_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# update_web_app method definition

await def update_web_app(
    self,
    *,
    WebAppId: str,
    IdentityProviderDetails: UpdateWebAppIdentityProviderDetailsTypeDef = ...,  # (1)
    AccessEndpoint: str = ...,
    WebAppUnits: WebAppUnitsTypeDef = ...,  # (2)
) -> UpdateWebAppResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: UpdateWebAppIdentityProviderDetailsTypeDef](./type_defs.md#updatewebappidentityproviderdetailstypedef) 
2. See [:material-code-braces: WebAppUnitsTypeDef](./type_defs.md#webappunitstypedef) 
3. See [:material-code-braces: UpdateWebAppResponseTypeDef](./type_defs.md#updatewebappresponsetypedef) 


```python
# update_web_app method usage example with argument unpacking

kwargs: UpdateWebAppRequestRequestTypeDef = {  # (1)
    "WebAppId": ...,
}

parent.update_web_app(**kwargs)
```

1. See [:material-code-braces: UpdateWebAppRequestRequestTypeDef](./type_defs.md#updatewebapprequestrequesttypedef) 

### update\_web\_app\_customization

Assigns new customization properties to a web app.

Type annotations and code completion for `#!python session.client("transfer").update_web_app_customization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# update_web_app_customization method definition

await def update_web_app_customization(
    self,
    *,
    WebAppId: str,
    Title: str = ...,
    LogoFile: BlobTypeDef = ...,
    FaviconFile: BlobTypeDef = ...,
) -> UpdateWebAppCustomizationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateWebAppCustomizationResponseTypeDef](./type_defs.md#updatewebappcustomizationresponsetypedef) 


```python
# update_web_app_customization method usage example with argument unpacking

kwargs: UpdateWebAppCustomizationRequestRequestTypeDef = {  # (1)
    "WebAppId": ...,
}

parent.update_web_app_customization(**kwargs)
```

1. See [:material-code-braces: UpdateWebAppCustomizationRequestRequestTypeDef](./type_defs.md#updatewebappcustomizationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("transfer").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("transfer").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)

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

Type annotations and code completion for `#!python session.client("transfer").get_paginator` method with overloads.

- `client.get_paginator("list_accesses")` -> [ListAccessesPaginator](./paginators.md#listaccessespaginator)
- `client.get_paginator("list_agreements")` -> [ListAgreementsPaginator](./paginators.md#listagreementspaginator)
- `client.get_paginator("list_certificates")` -> [ListCertificatesPaginator](./paginators.md#listcertificatespaginator)
- `client.get_paginator("list_connectors")` -> [ListConnectorsPaginator](./paginators.md#listconnectorspaginator)
- `client.get_paginator("list_executions")` -> [ListExecutionsPaginator](./paginators.md#listexecutionspaginator)
- `client.get_paginator("list_file_transfer_results")` -> [ListFileTransferResultsPaginator](./paginators.md#listfiletransferresultspaginator)
- `client.get_paginator("list_profiles")` -> [ListProfilesPaginator](./paginators.md#listprofilespaginator)
- `client.get_paginator("list_security_policies")` -> [ListSecurityPoliciesPaginator](./paginators.md#listsecuritypoliciespaginator)
- `client.get_paginator("list_servers")` -> [ListServersPaginator](./paginators.md#listserverspaginator)
- `client.get_paginator("list_tags_for_resource")` -> [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
- `client.get_paginator("list_users")` -> [ListUsersPaginator](./paginators.md#listuserspaginator)
- `client.get_paginator("list_web_apps")` -> [ListWebAppsPaginator](./paginators.md#listwebappspaginator)
- `client.get_paginator("list_workflows")` -> [ListWorkflowsPaginator](./paginators.md#listworkflowspaginator)




### get_waiter

Type annotations and code completion for `#!python session.client("transfer").get_waiter` method with overloads.

- `client.get_waiter("server_offline")` -> [ServerOfflineWaiter](./waiters.md#serverofflinewaiter)
- `client.get_waiter("server_online")` -> [ServerOnlineWaiter](./waiters.md#serveronlinewaiter)
