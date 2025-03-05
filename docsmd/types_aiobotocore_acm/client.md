# ACMClient

> [Index](../README.md) > [ACM](./README.md) > ACMClient

!!! note ""

    Auto-generated documentation for [ACM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#acm)
    type annotations stubs module [types-aiobotocore-acm](https://pypi.org/project/types-aiobotocore-acm/).

## ACMClient

Type annotations and code completion for `#!python session.client("acm")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

```python
# ACMClient usage example

from aioboto3.session import Session
from types_aiobotocore_acm.client import ACMClient

session = Session()
async with session.client("acm") as client:
    client: ACMClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("acm").exceptions` structure.

```python
# ACMClient.exceptions usage example

async with session.client("acm") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InvalidArgsException,
        client.exceptions.InvalidArnException,
        client.exceptions.InvalidDomainValidationOptionsException,
        client.exceptions.InvalidParameterException,
        client.exceptions.InvalidStateException,
        client.exceptions.InvalidTagException,
        client.exceptions.LimitExceededException,
        client.exceptions.RequestInProgressException,
        client.exceptions.ResourceInUseException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.TagPolicyException,
        client.exceptions.ThrottlingException,
        client.exceptions.TooManyTagsException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# ACMClient.exceptions type checking example

from types_aiobotocore_acm.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("acm").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("acm").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

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


### add\_tags\_to\_certificate

Adds one or more tags to an ACM certificate.

Type annotations and code completion for `#!python session.client("acm").add_tags_to_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

```python
# add_tags_to_certificate method definition

await def add_tags_to_certificate(
    self,
    *,
    CertificateArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See `Sequence[TagTypeDef]`
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# add_tags_to_certificate method usage example with argument unpacking

kwargs: AddTagsToCertificateRequestTypeDef = {  # (1)
    "CertificateArn": ...,
    "Tags": ...,
}

parent.add_tags_to_certificate(**kwargs)
```

1. See [:material-code-braces: AddTagsToCertificateRequestTypeDef](./type_defs.md#addtagstocertificaterequesttypedef)

### delete\_certificate

Deletes a certificate and its associated private key.

Type annotations and code completion for `#!python session.client("acm").delete_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

```python
# delete_certificate method definition

await def delete_certificate(
    self,
    *,
    CertificateArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_certificate method usage example with argument unpacking

kwargs: DeleteCertificateRequestTypeDef = {  # (1)
    "CertificateArn": ...,
}

parent.delete_certificate(**kwargs)
```

1. See [:material-code-braces: DeleteCertificateRequestTypeDef](./type_defs.md#deletecertificaterequesttypedef)

### describe\_certificate

Returns detailed metadata about the specified ACM certificate.

Type annotations and code completion for `#!python session.client("acm").describe_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

```python
# describe_certificate method definition

await def describe_certificate(
    self,
    *,
    CertificateArn: str,
) -> DescribeCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCertificateResponseTypeDef](./type_defs.md#describecertificateresponsetypedef)


```python
# describe_certificate method usage example with argument unpacking

kwargs: DescribeCertificateRequestTypeDef = {  # (1)
    "CertificateArn": ...,
}

parent.describe_certificate(**kwargs)
```

1. See [:material-code-braces: DescribeCertificateRequestTypeDef](./type_defs.md#describecertificaterequesttypedef)

### export\_certificate

Exports a private certificate issued by a private certificate authority (CA)
for use anywhere.

Type annotations and code completion for `#!python session.client("acm").export_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

```python
# export_certificate method definition

await def export_certificate(
    self,
    *,
    CertificateArn: str,
    Passphrase: BlobTypeDef,
) -> ExportCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExportCertificateResponseTypeDef](./type_defs.md#exportcertificateresponsetypedef)


```python
# export_certificate method usage example with argument unpacking

kwargs: ExportCertificateRequestTypeDef = {  # (1)
    "CertificateArn": ...,
    "Passphrase": ...,
}

parent.export_certificate(**kwargs)
```

1. See [:material-code-braces: ExportCertificateRequestTypeDef](./type_defs.md#exportcertificaterequesttypedef)

### get\_account\_configuration

Returns the account configuration options associated with an Amazon Web
Services account.

Type annotations and code completion for `#!python session.client("acm").get_account_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

```python
# get_account_configuration method definition

await def get_account_configuration(
    self,
) -> GetAccountConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccountConfigurationResponseTypeDef](./type_defs.md#getaccountconfigurationresponsetypedef)



### get\_certificate

Retrieves a certificate and its certificate chain.

Type annotations and code completion for `#!python session.client("acm").get_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

```python
# get_certificate method definition

await def get_certificate(
    self,
    *,
    CertificateArn: str,
) -> GetCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCertificateResponseTypeDef](./type_defs.md#getcertificateresponsetypedef)


```python
# get_certificate method usage example with argument unpacking

kwargs: GetCertificateRequestTypeDef = {  # (1)
    "CertificateArn": ...,
}

parent.get_certificate(**kwargs)
```

1. See [:material-code-braces: GetCertificateRequestTypeDef](./type_defs.md#getcertificaterequesttypedef)

### import\_certificate

Imports a certificate into Certificate Manager (ACM) to use with services that
are integrated with ACM.

Type annotations and code completion for `#!python session.client("acm").import_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

```python
# import_certificate method definition

await def import_certificate(
    self,
    *,
    Certificate: BlobTypeDef,
    PrivateKey: BlobTypeDef,
    CertificateArn: str = ...,
    CertificateChain: BlobTypeDef = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> ImportCertificateResponseTypeDef:  # (2)
    ...
```

1. See `Sequence[TagTypeDef]`
2. See [:material-code-braces: ImportCertificateResponseTypeDef](./type_defs.md#importcertificateresponsetypedef)


```python
# import_certificate method usage example with argument unpacking

kwargs: ImportCertificateRequestTypeDef = {  # (1)
    "Certificate": ...,
    "PrivateKey": ...,
}

parent.import_certificate(**kwargs)
```

1. See [:material-code-braces: ImportCertificateRequestTypeDef](./type_defs.md#importcertificaterequesttypedef)

### list\_certificates

Retrieves a list of certificate ARNs and domain names.

Type annotations and code completion for `#!python session.client("acm").list_certificates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

```python
# list_certificates method definition

await def list_certificates(
    self,
    *,
    CertificateStatuses: Sequence[CertificateStatusType] = ...,  # (1)
    Includes: FiltersTypeDef = ...,  # (2)
    NextToken: str = ...,
    MaxItems: int = ...,
    SortBy: SortByType = ...,  # (3)
    SortOrder: SortOrderType = ...,  # (4)
) -> ListCertificatesResponseTypeDef:  # (5)
    ...
```

1. See `Sequence[CertificateStatusType]`
2. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef)
3. See [:material-code-brackets: SortByType](./literals.md#sortbytype)
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype)
5. See [:material-code-braces: ListCertificatesResponseTypeDef](./type_defs.md#listcertificatesresponsetypedef)


```python
# list_certificates method usage example with argument unpacking

kwargs: ListCertificatesRequestTypeDef = {  # (1)
    "CertificateStatuses": ...,
}

parent.list_certificates(**kwargs)
```

1. See [:material-code-braces: ListCertificatesRequestTypeDef](./type_defs.md#listcertificatesrequesttypedef)

### list\_tags\_for\_certificate

Lists the tags that have been applied to the ACM certificate.

Type annotations and code completion for `#!python session.client("acm").list_tags_for_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

```python
# list_tags_for_certificate method definition

await def list_tags_for_certificate(
    self,
    *,
    CertificateArn: str,
) -> ListTagsForCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForCertificateResponseTypeDef](./type_defs.md#listtagsforcertificateresponsetypedef)


```python
# list_tags_for_certificate method usage example with argument unpacking

kwargs: ListTagsForCertificateRequestTypeDef = {  # (1)
    "CertificateArn": ...,
}

parent.list_tags_for_certificate(**kwargs)
```

1. See [:material-code-braces: ListTagsForCertificateRequestTypeDef](./type_defs.md#listtagsforcertificaterequesttypedef)

### put\_account\_configuration

Adds or modifies account-level configurations in ACM.

Type annotations and code completion for `#!python session.client("acm").put_account_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

```python
# put_account_configuration method definition

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


```python
# put_account_configuration method usage example with argument unpacking

kwargs: PutAccountConfigurationRequestTypeDef = {  # (1)
    "IdempotencyToken": ...,
}

parent.put_account_configuration(**kwargs)
```

1. See [:material-code-braces: PutAccountConfigurationRequestTypeDef](./type_defs.md#putaccountconfigurationrequesttypedef)

### remove\_tags\_from\_certificate

Remove one or more tags from an ACM certificate.

Type annotations and code completion for `#!python session.client("acm").remove_tags_from_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

```python
# remove_tags_from_certificate method definition

await def remove_tags_from_certificate(
    self,
    *,
    CertificateArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See `Sequence[TagTypeDef]`
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# remove_tags_from_certificate method usage example with argument unpacking

kwargs: RemoveTagsFromCertificateRequestTypeDef = {  # (1)
    "CertificateArn": ...,
    "Tags": ...,
}

parent.remove_tags_from_certificate(**kwargs)
```

1. See [:material-code-braces: RemoveTagsFromCertificateRequestTypeDef](./type_defs.md#removetagsfromcertificaterequesttypedef)

### renew\_certificate

Renews an eligible ACM certificate.

Type annotations and code completion for `#!python session.client("acm").renew_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

```python
# renew_certificate method definition

await def renew_certificate(
    self,
    *,
    CertificateArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# renew_certificate method usage example with argument unpacking

kwargs: RenewCertificateRequestTypeDef = {  # (1)
    "CertificateArn": ...,
}

parent.renew_certificate(**kwargs)
```

1. See [:material-code-braces: RenewCertificateRequestTypeDef](./type_defs.md#renewcertificaterequesttypedef)

### request\_certificate

Requests an ACM certificate for use with other Amazon Web Services services.

Type annotations and code completion for `#!python session.client("acm").request_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

```python
# request_certificate method definition

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
    KeyAlgorithm: KeyAlgorithmType = ...,  # (5)
) -> RequestCertificateResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: ValidationMethodType](./literals.md#validationmethodtype)
2. See `Sequence[DomainValidationOptionTypeDef]`
3. See [:material-code-braces: CertificateOptionsTypeDef](./type_defs.md#certificateoptionstypedef)
4. See `Sequence[TagTypeDef]`
5. See [:material-code-brackets: KeyAlgorithmType](./literals.md#keyalgorithmtype)
6. See [:material-code-braces: RequestCertificateResponseTypeDef](./type_defs.md#requestcertificateresponsetypedef)


```python
# request_certificate method usage example with argument unpacking

kwargs: RequestCertificateRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.request_certificate(**kwargs)
```

1. See [:material-code-braces: RequestCertificateRequestTypeDef](./type_defs.md#requestcertificaterequesttypedef)

### resend\_validation\_email

Resends the email that requests domain ownership validation.

Type annotations and code completion for `#!python session.client("acm").resend_validation_email` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

```python
# resend_validation_email method definition

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


```python
# resend_validation_email method usage example with argument unpacking

kwargs: ResendValidationEmailRequestTypeDef = {  # (1)
    "CertificateArn": ...,
    "Domain": ...,
    "ValidationDomain": ...,
}

parent.resend_validation_email(**kwargs)
```

1. See [:material-code-braces: ResendValidationEmailRequestTypeDef](./type_defs.md#resendvalidationemailrequesttypedef)

### update\_certificate\_options

Updates a certificate.

Type annotations and code completion for `#!python session.client("acm").update_certificate_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

```python
# update_certificate_options method definition

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


```python
# update_certificate_options method usage example with argument unpacking

kwargs: UpdateCertificateOptionsRequestTypeDef = {  # (1)
    "CertificateArn": ...,
    "Options": ...,
}

parent.update_certificate_options(**kwargs)
```

1. See [:material-code-braces: UpdateCertificateOptionsRequestTypeDef](./type_defs.md#updatecertificateoptionsrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("acm").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("acm").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client)

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

Type annotations and code completion for `#!python session.client("acm").get_paginator` method with overloads.

- `client.get_paginator("list_certificates")` -> [ListCertificatesPaginator](./paginators.md#listcertificatespaginator)




### get_waiter

Type annotations and code completion for `#!python session.client("acm").get_waiter` method with overloads.

- `client.get_waiter("certificate_validated")` -> [CertificateValidatedWaiter](./waiters.md#certificatevalidatedwaiter)

