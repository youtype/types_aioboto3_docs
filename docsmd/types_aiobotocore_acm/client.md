# ACMClient

> [Index](../README.md) > [ACM](./README.md) > ACMClient

!!! note ""

    Auto-generated documentation for [ACM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
    type annotations stubs module [types-aiobotocore-acm](https://pypi.org/project/types-aiobotocore-acm/).

## ACMClient

Type annotations and code completion for `#!python session.client("acm")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

```python title="Usage example"
from aioboto3.session import Session
from types_aiobotocore_acm.client import ACMClient

session = Session()
async with session.client("acm") as client:
    client: ACMClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("acm").exceptions` structure.

```python title="Usage example"
async with session.client("acm") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InvalidArgsException,
        client.InvalidArnException,
        client.InvalidDomainValidationOptionsException,
        client.InvalidParameterException,
        client.InvalidStateException,
        client.InvalidTagException,
        client.LimitExceededException,
        client.RequestInProgressException,
        client.ResourceInUseException,
        client.ResourceNotFoundException,
        client.TagPolicyException,
        client.ThrottlingException,
        client.TooManyTagsException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_acm.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### add\_tags\_to\_certificate

Adds one or more tags to an ACM certificate.

Type annotations and code completion for `#!python session.client("acm").add_tags_to_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.add_tags_to_certificate)

```python title="Method definition"
await def add_tags_to_certificate(
    self,
    *,
    CertificateArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python title="Usage example with kwargs"
kwargs: AddTagsToCertificateRequestRequestTypeDef = {  # (1)
    "CertificateArn": ...,
    "Tags": ...,
}

parent.add_tags_to_certificate(**kwargs)
```

1. See [:material-code-braces: AddTagsToCertificateRequestRequestTypeDef](./type_defs.md#addtagstocertificaterequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.client("acm").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.client("acm").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.close)

```python title="Method definition"
await def close(
    self,
) -> None:
    ...
```


### delete\_certificate

Deletes a certificate and its associated private key.

Type annotations and code completion for `#!python session.client("acm").delete_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.delete_certificate)

```python title="Method definition"
await def delete_certificate(
    self,
    *,
    CertificateArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python title="Usage example with kwargs"
kwargs: DeleteCertificateRequestRequestTypeDef = {  # (1)
    "CertificateArn": ...,
}

parent.delete_certificate(**kwargs)
```

1. See [:material-code-braces: DeleteCertificateRequestRequestTypeDef](./type_defs.md#deletecertificaterequestrequesttypedef) 

### describe\_certificate

Returns detailed metadata about the specified ACM certificate.

Type annotations and code completion for `#!python session.client("acm").describe_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.describe_certificate)

```python title="Method definition"
await def describe_certificate(
    self,
    *,
    CertificateArn: str,
) -> DescribeCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCertificateResponseTypeDef](./type_defs.md#describecertificateresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeCertificateRequestRequestTypeDef = {  # (1)
    "CertificateArn": ...,
}

parent.describe_certificate(**kwargs)
```

1. See [:material-code-braces: DescribeCertificateRequestRequestTypeDef](./type_defs.md#describecertificaterequestrequesttypedef) 

### export\_certificate

Exports a private certificate issued by a private certificate authority (CA) for
use anywhere.

Type annotations and code completion for `#!python session.client("acm").export_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.export_certificate)

```python title="Method definition"
await def export_certificate(
    self,
    *,
    CertificateArn: str,
    Passphrase: Union[str, bytes, IO[Any], StreamingBody],
) -> ExportCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExportCertificateResponseTypeDef](./type_defs.md#exportcertificateresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ExportCertificateRequestRequestTypeDef = {  # (1)
    "CertificateArn": ...,
    "Passphrase": ...,
}

parent.export_certificate(**kwargs)
```

1. See [:material-code-braces: ExportCertificateRequestRequestTypeDef](./type_defs.md#exportcertificaterequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.client("acm").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.generate_presigned_url)

```python title="Method definition"
await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_account\_configuration

Returns the account configuration options associated with an Amazon Web Services
account.

Type annotations and code completion for `#!python session.client("acm").get_account_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.get_account_configuration)

```python title="Method definition"
await def get_account_configuration(
    self,
) -> GetAccountConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccountConfigurationResponseTypeDef](./type_defs.md#getaccountconfigurationresponsetypedef) 

### get\_certificate

Retrieves an Amazon-issued certificate and its certificate chain.

Type annotations and code completion for `#!python session.client("acm").get_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.get_certificate)

```python title="Method definition"
await def get_certificate(
    self,
    *,
    CertificateArn: str,
) -> GetCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCertificateResponseTypeDef](./type_defs.md#getcertificateresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetCertificateRequestRequestTypeDef = {  # (1)
    "CertificateArn": ...,
}

parent.get_certificate(**kwargs)
```

1. See [:material-code-braces: GetCertificateRequestRequestTypeDef](./type_defs.md#getcertificaterequestrequesttypedef) 

### import\_certificate

Imports a certificate into Amazon Web Services Certificate Manager (ACM) to use
with services that are integrated with ACM.

Type annotations and code completion for `#!python session.client("acm").import_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.import_certificate)

```python title="Method definition"
await def import_certificate(
    self,
    *,
    Certificate: Union[str, bytes, IO[Any], StreamingBody],
    PrivateKey: Union[str, bytes, IO[Any], StreamingBody],
    CertificateArn: str = ...,
    CertificateChain: Union[str, bytes, IO[Any], StreamingBody] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> ImportCertificateResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ImportCertificateResponseTypeDef](./type_defs.md#importcertificateresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ImportCertificateRequestRequestTypeDef = {  # (1)
    "Certificate": ...,
    "PrivateKey": ...,
}

parent.import_certificate(**kwargs)
```

1. See [:material-code-braces: ImportCertificateRequestRequestTypeDef](./type_defs.md#importcertificaterequestrequesttypedef) 

### list\_certificates

Retrieves a list of certificate ARNs and domain names.

Type annotations and code completion for `#!python session.client("acm").list_certificates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.list_certificates)

```python title="Method definition"
await def list_certificates(
    self,
    *,
    CertificateStatuses: Sequence[CertificateStatusType] = ...,  # (1)
    Includes: FiltersTypeDef = ...,  # (2)
    NextToken: str = ...,
    MaxItems: int = ...,
) -> ListCertificatesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: CertificateStatusType](./literals.md#certificatestatustype) 
2. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef) 
3. See [:material-code-braces: ListCertificatesResponseTypeDef](./type_defs.md#listcertificatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCertificatesRequestRequestTypeDef = {  # (1)
    "CertificateStatuses": ...,
}

parent.list_certificates(**kwargs)
```

1. See [:material-code-braces: ListCertificatesRequestRequestTypeDef](./type_defs.md#listcertificatesrequestrequesttypedef) 

### list\_tags\_for\_certificate

Lists the tags that have been applied to the ACM certificate.

Type annotations and code completion for `#!python session.client("acm").list_tags_for_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.list_tags_for_certificate)

```python title="Method definition"
await def list_tags_for_certificate(
    self,
    *,
    CertificateArn: str,
) -> ListTagsForCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForCertificateResponseTypeDef](./type_defs.md#listtagsforcertificateresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsForCertificateRequestRequestTypeDef = {  # (1)
    "CertificateArn": ...,
}

parent.list_tags_for_certificate(**kwargs)
```

1. See [:material-code-braces: ListTagsForCertificateRequestRequestTypeDef](./type_defs.md#listtagsforcertificaterequestrequesttypedef) 

### put\_account\_configuration

Adds or modifies account-level configurations in ACM.

Type annotations and code completion for `#!python session.client("acm").put_account_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.put_account_configuration)

```python title="Method definition"
await def put_account_configuration(
    self,
    *,
    IdempotencyToken: str,
    ExpiryEvents: ExpiryEventsConfigurationTypeDef = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ExpiryEventsConfigurationTypeDef](./type_defs.md#expiryeventsconfigurationtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python title="Usage example with kwargs"
kwargs: PutAccountConfigurationRequestRequestTypeDef = {  # (1)
    "IdempotencyToken": ...,
}

parent.put_account_configuration(**kwargs)
```

1. See [:material-code-braces: PutAccountConfigurationRequestRequestTypeDef](./type_defs.md#putaccountconfigurationrequestrequesttypedef) 

### remove\_tags\_from\_certificate

Remove one or more tags from an ACM certificate.

Type annotations and code completion for `#!python session.client("acm").remove_tags_from_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.remove_tags_from_certificate)

```python title="Method definition"
await def remove_tags_from_certificate(
    self,
    *,
    CertificateArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python title="Usage example with kwargs"
kwargs: RemoveTagsFromCertificateRequestRequestTypeDef = {  # (1)
    "CertificateArn": ...,
    "Tags": ...,
}

parent.remove_tags_from_certificate(**kwargs)
```

1. See [:material-code-braces: RemoveTagsFromCertificateRequestRequestTypeDef](./type_defs.md#removetagsfromcertificaterequestrequesttypedef) 

### renew\_certificate

Renews an eligible ACM certificate.

Type annotations and code completion for `#!python session.client("acm").renew_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.renew_certificate)

```python title="Method definition"
await def renew_certificate(
    self,
    *,
    CertificateArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python title="Usage example with kwargs"
kwargs: RenewCertificateRequestRequestTypeDef = {  # (1)
    "CertificateArn": ...,
}

parent.renew_certificate(**kwargs)
```

1. See [:material-code-braces: RenewCertificateRequestRequestTypeDef](./type_defs.md#renewcertificaterequestrequesttypedef) 

### request\_certificate

Requests an ACM certificate for use with other Amazon Web Services services.

Type annotations and code completion for `#!python session.client("acm").request_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.request_certificate)

```python title="Method definition"
await def request_certificate(
    self,
    *,
    DomainName: str,
    ValidationMethod: ValidationMethodType = ...,  # (1)
    SubjectAlternativeNames: Sequence[str] = ...,
    IdempotencyToken: str = ...,
    DomainValidationOptions: Sequence[DomainValidationOptionTypeDef] = ...,  # (2)
    Options: CertificateOptionsTypeDef = ...,  # (3)
    CertificateAuthorityArn: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> RequestCertificateResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: ValidationMethodType](./literals.md#validationmethodtype) 
2. See [:material-code-braces: DomainValidationOptionTypeDef](./type_defs.md#domainvalidationoptiontypedef) 
3. See [:material-code-braces: CertificateOptionsTypeDef](./type_defs.md#certificateoptionstypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: RequestCertificateResponseTypeDef](./type_defs.md#requestcertificateresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: RequestCertificateRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.request_certificate(**kwargs)
```

1. See [:material-code-braces: RequestCertificateRequestRequestTypeDef](./type_defs.md#requestcertificaterequestrequesttypedef) 

### resend\_validation\_email

Resends the email that requests domain ownership validation.

Type annotations and code completion for `#!python session.client("acm").resend_validation_email` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.resend_validation_email)

```python title="Method definition"
await def resend_validation_email(
    self,
    *,
    CertificateArn: str,
    Domain: str,
    ValidationDomain: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python title="Usage example with kwargs"
kwargs: ResendValidationEmailRequestRequestTypeDef = {  # (1)
    "CertificateArn": ...,
    "Domain": ...,
    "ValidationDomain": ...,
}

parent.resend_validation_email(**kwargs)
```

1. See [:material-code-braces: ResendValidationEmailRequestRequestTypeDef](./type_defs.md#resendvalidationemailrequestrequesttypedef) 

### update\_certificate\_options

Updates a certificate.

Type annotations and code completion for `#!python session.client("acm").update_certificate_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.update_certificate_options)

```python title="Method definition"
await def update_certificate_options(
    self,
    *,
    CertificateArn: str,
    Options: CertificateOptionsTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CertificateOptionsTypeDef](./type_defs.md#certificateoptionstypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python title="Usage example with kwargs"
kwargs: UpdateCertificateOptionsRequestRequestTypeDef = {  # (1)
    "CertificateArn": ...,
    "Options": ...,
}

parent.update_certificate_options(**kwargs)
```

1. See [:material-code-braces: UpdateCertificateOptionsRequestRequestTypeDef](./type_defs.md#updatecertificateoptionsrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("acm").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> ACMClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("acm").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("acm").get_paginator` method with overloads.

- `client.get_paginator("list_certificates")` -> [ListCertificatesPaginator](./paginators.md#listcertificatespaginator)




### get_waiter

Type annotations and code completion for `#!python session.client("acm").get_waiter` method with overloads.

- `client.get_waiter("certificate_validated")` -> [CertificateValidatedWaiter](./waiters.md#certificatevalidatedwaiter)

