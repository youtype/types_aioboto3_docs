# AccountClient

> [Index](../README.md) > [Account](./README.md) > AccountClient

!!! note ""

    Auto-generated documentation for [Account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#account)
    type annotations stubs module [types-aiobotocore-account](https://pypi.org/project/types-aiobotocore-account/).

## AccountClient

Type annotations and code completion for `#!python session.client("account")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client)

```python
# AccountClient usage example

from aioboto3.session import Session
from types_aiobotocore_account.client import AccountClient

session = Session()
async with session.client("account") as client:
    client: AccountClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("account").exceptions` structure.

```python
# AccountClient.exceptions usage example

async with session.client("account") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.TooManyRequestsException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# AccountClient.exceptions type checking example

from types_aiobotocore_account.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("account").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("account").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client)

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


### accept\_primary\_email\_update

Accepts the request that originated from <a>StartPrimaryEmailUpdate</a> to
update the primary email address (also known as the root user email address)
for the specified account.

Type annotations and code completion for `#!python session.client("account").accept_primary_email_update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client)

```python
# accept_primary_email_update method definition

await def accept_primary_email_update(
    self,
    *,
    AccountId: str,
    Otp: str,
    PrimaryEmail: str,
) -> AcceptPrimaryEmailUpdateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AcceptPrimaryEmailUpdateResponseTypeDef](./type_defs.md#acceptprimaryemailupdateresponsetypedef) 


```python
# accept_primary_email_update method usage example with argument unpacking

kwargs: AcceptPrimaryEmailUpdateRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Otp": ...,
    "PrimaryEmail": ...,
}

parent.accept_primary_email_update(**kwargs)
```

1. See [:material-code-braces: AcceptPrimaryEmailUpdateRequestRequestTypeDef](./type_defs.md#acceptprimaryemailupdaterequestrequesttypedef) 

### delete\_alternate\_contact

Deletes the specified alternate contact from an Amazon Web Services account.

Type annotations and code completion for `#!python session.client("account").delete_alternate_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client)

```python
# delete_alternate_contact method definition

await def delete_alternate_contact(
    self,
    *,
    AlternateContactType: AlternateContactTypeType,  # (1)
    AccountId: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AlternateContactTypeType](./literals.md#alternatecontacttypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_alternate_contact method usage example with argument unpacking

kwargs: DeleteAlternateContactRequestRequestTypeDef = {  # (1)
    "AlternateContactType": ...,
}

parent.delete_alternate_contact(**kwargs)
```

1. See [:material-code-braces: DeleteAlternateContactRequestRequestTypeDef](./type_defs.md#deletealternatecontactrequestrequesttypedef) 

### disable\_region

Disables (opts-out) a particular Region for an account.

Type annotations and code completion for `#!python session.client("account").disable_region` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client)

```python
# disable_region method definition

await def disable_region(
    self,
    *,
    RegionName: str,
    AccountId: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disable_region method usage example with argument unpacking

kwargs: DisableRegionRequestRequestTypeDef = {  # (1)
    "RegionName": ...,
}

parent.disable_region(**kwargs)
```

1. See [:material-code-braces: DisableRegionRequestRequestTypeDef](./type_defs.md#disableregionrequestrequesttypedef) 

### enable\_region

Enables (opts-in) a particular Region for an account.

Type annotations and code completion for `#!python session.client("account").enable_region` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client)

```python
# enable_region method definition

await def enable_region(
    self,
    *,
    RegionName: str,
    AccountId: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# enable_region method usage example with argument unpacking

kwargs: EnableRegionRequestRequestTypeDef = {  # (1)
    "RegionName": ...,
}

parent.enable_region(**kwargs)
```

1. See [:material-code-braces: EnableRegionRequestRequestTypeDef](./type_defs.md#enableregionrequestrequesttypedef) 

### get\_alternate\_contact

Retrieves the specified alternate contact attached to an Amazon Web Services
account.

Type annotations and code completion for `#!python session.client("account").get_alternate_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client)

```python
# get_alternate_contact method definition

await def get_alternate_contact(
    self,
    *,
    AlternateContactType: AlternateContactTypeType,  # (1)
    AccountId: str = ...,
) -> GetAlternateContactResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AlternateContactTypeType](./literals.md#alternatecontacttypetype) 
2. See [:material-code-braces: GetAlternateContactResponseTypeDef](./type_defs.md#getalternatecontactresponsetypedef) 


```python
# get_alternate_contact method usage example with argument unpacking

kwargs: GetAlternateContactRequestRequestTypeDef = {  # (1)
    "AlternateContactType": ...,
}

parent.get_alternate_contact(**kwargs)
```

1. See [:material-code-braces: GetAlternateContactRequestRequestTypeDef](./type_defs.md#getalternatecontactrequestrequesttypedef) 

### get\_contact\_information

Retrieves the primary contact information of an Amazon Web Services account.

Type annotations and code completion for `#!python session.client("account").get_contact_information` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client)

```python
# get_contact_information method definition

await def get_contact_information(
    self,
    *,
    AccountId: str = ...,
) -> GetContactInformationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetContactInformationResponseTypeDef](./type_defs.md#getcontactinformationresponsetypedef) 


```python
# get_contact_information method usage example with argument unpacking

kwargs: GetContactInformationRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.get_contact_information(**kwargs)
```

1. See [:material-code-braces: GetContactInformationRequestRequestTypeDef](./type_defs.md#getcontactinformationrequestrequesttypedef) 

### get\_primary\_email

Retrieves the primary email address for the specified account.

Type annotations and code completion for `#!python session.client("account").get_primary_email` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client)

```python
# get_primary_email method definition

await def get_primary_email(
    self,
    *,
    AccountId: str,
) -> GetPrimaryEmailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPrimaryEmailResponseTypeDef](./type_defs.md#getprimaryemailresponsetypedef) 


```python
# get_primary_email method usage example with argument unpacking

kwargs: GetPrimaryEmailRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.get_primary_email(**kwargs)
```

1. See [:material-code-braces: GetPrimaryEmailRequestRequestTypeDef](./type_defs.md#getprimaryemailrequestrequesttypedef) 

### get\_region\_opt\_status

Retrieves the opt-in status of a particular Region.

Type annotations and code completion for `#!python session.client("account").get_region_opt_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client)

```python
# get_region_opt_status method definition

await def get_region_opt_status(
    self,
    *,
    RegionName: str,
    AccountId: str = ...,
) -> GetRegionOptStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRegionOptStatusResponseTypeDef](./type_defs.md#getregionoptstatusresponsetypedef) 


```python
# get_region_opt_status method usage example with argument unpacking

kwargs: GetRegionOptStatusRequestRequestTypeDef = {  # (1)
    "RegionName": ...,
}

parent.get_region_opt_status(**kwargs)
```

1. See [:material-code-braces: GetRegionOptStatusRequestRequestTypeDef](./type_defs.md#getregionoptstatusrequestrequesttypedef) 

### list\_regions

Lists all the Regions for a given account and their respective opt-in statuses.

Type annotations and code completion for `#!python session.client("account").list_regions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client)

```python
# list_regions method definition

await def list_regions(
    self,
    *,
    AccountId: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    RegionOptStatusContains: Sequence[RegionOptStatusType] = ...,  # (1)
) -> ListRegionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RegionOptStatusType](./literals.md#regionoptstatustype) 
2. See [:material-code-braces: ListRegionsResponseTypeDef](./type_defs.md#listregionsresponsetypedef) 


```python
# list_regions method usage example with argument unpacking

kwargs: ListRegionsRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.list_regions(**kwargs)
```

1. See [:material-code-braces: ListRegionsRequestRequestTypeDef](./type_defs.md#listregionsrequestrequesttypedef) 

### put\_alternate\_contact

Modifies the specified alternate contact attached to an Amazon Web Services
account.

Type annotations and code completion for `#!python session.client("account").put_alternate_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client)

```python
# put_alternate_contact method definition

await def put_alternate_contact(
    self,
    *,
    AlternateContactType: AlternateContactTypeType,  # (1)
    EmailAddress: str,
    Name: str,
    PhoneNumber: str,
    Title: str,
    AccountId: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AlternateContactTypeType](./literals.md#alternatecontacttypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_alternate_contact method usage example with argument unpacking

kwargs: PutAlternateContactRequestRequestTypeDef = {  # (1)
    "AlternateContactType": ...,
    "EmailAddress": ...,
    "Name": ...,
    "PhoneNumber": ...,
    "Title": ...,
}

parent.put_alternate_contact(**kwargs)
```

1. See [:material-code-braces: PutAlternateContactRequestRequestTypeDef](./type_defs.md#putalternatecontactrequestrequesttypedef) 

### put\_contact\_information

Updates the primary contact information of an Amazon Web Services account.

Type annotations and code completion for `#!python session.client("account").put_contact_information` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client)

```python
# put_contact_information method definition

await def put_contact_information(
    self,
    *,
    ContactInformation: ContactInformationTypeDef,  # (1)
    AccountId: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ContactInformationTypeDef](./type_defs.md#contactinformationtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_contact_information method usage example with argument unpacking

kwargs: PutContactInformationRequestRequestTypeDef = {  # (1)
    "ContactInformation": ...,
}

parent.put_contact_information(**kwargs)
```

1. See [:material-code-braces: PutContactInformationRequestRequestTypeDef](./type_defs.md#putcontactinformationrequestrequesttypedef) 

### start\_primary\_email\_update

Starts the process to update the primary email address for the specified
account.

Type annotations and code completion for `#!python session.client("account").start_primary_email_update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client)

```python
# start_primary_email_update method definition

await def start_primary_email_update(
    self,
    *,
    AccountId: str,
    PrimaryEmail: str,
) -> StartPrimaryEmailUpdateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartPrimaryEmailUpdateResponseTypeDef](./type_defs.md#startprimaryemailupdateresponsetypedef) 


```python
# start_primary_email_update method usage example with argument unpacking

kwargs: StartPrimaryEmailUpdateRequestRequestTypeDef = {  # (1)
    "AccountId": ...,
    "PrimaryEmail": ...,
}

parent.start_primary_email_update(**kwargs)
```

1. See [:material-code-braces: StartPrimaryEmailUpdateRequestRequestTypeDef](./type_defs.md#startprimaryemailupdaterequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("account").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("account").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client)

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

Type annotations and code completion for `#!python session.client("account").get_paginator` method with overloads.

- `client.get_paginator("list_regions")` -> [ListRegionsPaginator](./paginators.md#listregionspaginator)


