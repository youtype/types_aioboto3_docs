# ServiceQuotasClient

> [Index](../README.md) > [ServiceQuotas](./README.md) > ServiceQuotasClient

!!! note ""

    Auto-generated documentation for [ServiceQuotas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#servicequotas)
    type annotations stubs module [types-aiobotocore-service-quotas](https://pypi.org/project/types-aiobotocore-service-quotas/).

## ServiceQuotasClient

Type annotations and code completion for `#!python session.client("service-quotas")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# ServiceQuotasClient usage example

from aioboto3.session import Session
from types_aiobotocore_service_quotas.client import ServiceQuotasClient

session = Session()
async with session.client("service-quotas") as client:
    client: ServiceQuotasClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("service-quotas").exceptions` structure.

```python
# ServiceQuotasClient.exceptions usage example

async with session.client("service-quotas") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AWSServiceAccessNotEnabledException,
        client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.DependencyAccessDeniedException,
        client.exceptions.IllegalArgumentException,
        client.exceptions.InvalidPaginationTokenException,
        client.exceptions.InvalidResourceStateException,
        client.exceptions.NoAvailableOrganizationException,
        client.exceptions.NoSuchResourceException,
        client.exceptions.OrganizationNotInAllFeaturesModeException,
        client.exceptions.QuotaExceededException,
        client.exceptions.ResourceAlreadyExistsException,
        client.exceptions.ServiceException,
        client.exceptions.ServiceQuotaTemplateNotInUseException,
        client.exceptions.TagPolicyViolationException,
        client.exceptions.TemplatesNotAvailableInRegionException,
        client.exceptions.TooManyRequestsException,
        client.exceptions.TooManyTagsException,
    ) as e:
        print(e)
```

```python
# ServiceQuotasClient.exceptions type checking example

from types_aiobotocore_service_quotas.client import Exceptions

def handle_error(exc: Exceptions.AWSServiceAccessNotEnabledException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("service-quotas").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("service-quotas").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

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


### associate\_service\_quota\_template

Associates your quota request template with your organization.

Type annotations and code completion for `#!python session.client("service-quotas").associate_service_quota_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# associate_service_quota_template method definition

await def associate_service_quota_template(
    self,
) -> dict[str, Any]:
    ...
```


### delete\_service\_quota\_increase\_request\_from\_template

Deletes the quota increase request for the specified quota from your quota
request template.

Type annotations and code completion for `#!python session.client("service-quotas").delete_service_quota_increase_request_from_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# delete_service_quota_increase_request_from_template method definition

await def delete_service_quota_increase_request_from_template(
    self,
    *,
    ServiceCode: str,
    QuotaCode: str,
    AwsRegion: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_service_quota_increase_request_from_template method usage example with argument unpacking

kwargs: DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef = {  # (1)
    "ServiceCode": ...,
    "QuotaCode": ...,
    "AwsRegion": ...,
}

parent.delete_service_quota_increase_request_from_template(**kwargs)
```

1. See [:material-code-braces: DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef](./type_defs.md#deleteservicequotaincreaserequestfromtemplaterequestrequesttypedef) 

### disassociate\_service\_quota\_template

Disables your quota request template.

Type annotations and code completion for `#!python session.client("service-quotas").disassociate_service_quota_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# disassociate_service_quota_template method definition

await def disassociate_service_quota_template(
    self,
) -> dict[str, Any]:
    ...
```


### get\_aws\_default\_service\_quota

Retrieves the default value for the specified quota.

Type annotations and code completion for `#!python session.client("service-quotas").get_aws_default_service_quota` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# get_aws_default_service_quota method definition

await def get_aws_default_service_quota(
    self,
    *,
    ServiceCode: str,
    QuotaCode: str,
) -> GetAWSDefaultServiceQuotaResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAWSDefaultServiceQuotaResponseTypeDef](./type_defs.md#getawsdefaultservicequotaresponsetypedef) 


```python
# get_aws_default_service_quota method usage example with argument unpacking

kwargs: GetAWSDefaultServiceQuotaRequestRequestTypeDef = {  # (1)
    "ServiceCode": ...,
    "QuotaCode": ...,
}

parent.get_aws_default_service_quota(**kwargs)
```

1. See [:material-code-braces: GetAWSDefaultServiceQuotaRequestRequestTypeDef](./type_defs.md#getawsdefaultservicequotarequestrequesttypedef) 

### get\_association\_for\_service\_quota\_template

Retrieves the status of the association for the quota request template.

Type annotations and code completion for `#!python session.client("service-quotas").get_association_for_service_quota_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# get_association_for_service_quota_template method definition

await def get_association_for_service_quota_template(
    self,
) -> GetAssociationForServiceQuotaTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAssociationForServiceQuotaTemplateResponseTypeDef](./type_defs.md#getassociationforservicequotatemplateresponsetypedef) 

### get\_requested\_service\_quota\_change

Retrieves information about the specified quota increase request.

Type annotations and code completion for `#!python session.client("service-quotas").get_requested_service_quota_change` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# get_requested_service_quota_change method definition

await def get_requested_service_quota_change(
    self,
    *,
    RequestId: str,
) -> GetRequestedServiceQuotaChangeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRequestedServiceQuotaChangeResponseTypeDef](./type_defs.md#getrequestedservicequotachangeresponsetypedef) 


```python
# get_requested_service_quota_change method usage example with argument unpacking

kwargs: GetRequestedServiceQuotaChangeRequestRequestTypeDef = {  # (1)
    "RequestId": ...,
}

parent.get_requested_service_quota_change(**kwargs)
```

1. See [:material-code-braces: GetRequestedServiceQuotaChangeRequestRequestTypeDef](./type_defs.md#getrequestedservicequotachangerequestrequesttypedef) 

### get\_service\_quota

Retrieves the applied quota value for the specified quota.

Type annotations and code completion for `#!python session.client("service-quotas").get_service_quota` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# get_service_quota method definition

await def get_service_quota(
    self,
    *,
    ServiceCode: str,
    QuotaCode: str,
    ContextId: str = ...,
) -> GetServiceQuotaResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceQuotaResponseTypeDef](./type_defs.md#getservicequotaresponsetypedef) 


```python
# get_service_quota method usage example with argument unpacking

kwargs: GetServiceQuotaRequestRequestTypeDef = {  # (1)
    "ServiceCode": ...,
    "QuotaCode": ...,
}

parent.get_service_quota(**kwargs)
```

1. See [:material-code-braces: GetServiceQuotaRequestRequestTypeDef](./type_defs.md#getservicequotarequestrequesttypedef) 

### get\_service\_quota\_increase\_request\_from\_template

Retrieves information about the specified quota increase request in your quota
request template.

Type annotations and code completion for `#!python session.client("service-quotas").get_service_quota_increase_request_from_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# get_service_quota_increase_request_from_template method definition

await def get_service_quota_increase_request_from_template(
    self,
    *,
    ServiceCode: str,
    QuotaCode: str,
    AwsRegion: str,
) -> GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef](./type_defs.md#getservicequotaincreaserequestfromtemplateresponsetypedef) 


```python
# get_service_quota_increase_request_from_template method usage example with argument unpacking

kwargs: GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef = {  # (1)
    "ServiceCode": ...,
    "QuotaCode": ...,
    "AwsRegion": ...,
}

parent.get_service_quota_increase_request_from_template(**kwargs)
```

1. See [:material-code-braces: GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef](./type_defs.md#getservicequotaincreaserequestfromtemplaterequestrequesttypedef) 

### list\_aws\_default\_service\_quotas

Lists the default values for the quotas for the specified Amazon Web Service.

Type annotations and code completion for `#!python session.client("service-quotas").list_aws_default_service_quotas` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# list_aws_default_service_quotas method definition

await def list_aws_default_service_quotas(
    self,
    *,
    ServiceCode: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAWSDefaultServiceQuotasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAWSDefaultServiceQuotasResponseTypeDef](./type_defs.md#listawsdefaultservicequotasresponsetypedef) 


```python
# list_aws_default_service_quotas method usage example with argument unpacking

kwargs: ListAWSDefaultServiceQuotasRequestRequestTypeDef = {  # (1)
    "ServiceCode": ...,
}

parent.list_aws_default_service_quotas(**kwargs)
```

1. See [:material-code-braces: ListAWSDefaultServiceQuotasRequestRequestTypeDef](./type_defs.md#listawsdefaultservicequotasrequestrequesttypedef) 

### list\_requested\_service\_quota\_change\_history

Retrieves the quota increase requests for the specified Amazon Web Service.

Type annotations and code completion for `#!python session.client("service-quotas").list_requested_service_quota_change_history` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# list_requested_service_quota_change_history method definition

await def list_requested_service_quota_change_history(
    self,
    *,
    ServiceCode: str = ...,
    Status: RequestStatusType = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
    QuotaRequestedAtLevel: AppliedLevelEnumType = ...,  # (2)
) -> ListRequestedServiceQuotaChangeHistoryResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RequestStatusType](./literals.md#requeststatustype) 
2. See [:material-code-brackets: AppliedLevelEnumType](./literals.md#appliedlevelenumtype) 
3. See [:material-code-braces: ListRequestedServiceQuotaChangeHistoryResponseTypeDef](./type_defs.md#listrequestedservicequotachangehistoryresponsetypedef) 


```python
# list_requested_service_quota_change_history method usage example with argument unpacking

kwargs: ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef = {  # (1)
    "ServiceCode": ...,
}

parent.list_requested_service_quota_change_history(**kwargs)
```

1. See [:material-code-braces: ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef](./type_defs.md#listrequestedservicequotachangehistoryrequestrequesttypedef) 

### list\_requested\_service\_quota\_change\_history\_by\_quota

Retrieves the quota increase requests for the specified quota.

Type annotations and code completion for `#!python session.client("service-quotas").list_requested_service_quota_change_history_by_quota` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# list_requested_service_quota_change_history_by_quota method definition

await def list_requested_service_quota_change_history_by_quota(
    self,
    *,
    ServiceCode: str,
    QuotaCode: str,
    Status: RequestStatusType = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
    QuotaRequestedAtLevel: AppliedLevelEnumType = ...,  # (2)
) -> ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RequestStatusType](./literals.md#requeststatustype) 
2. See [:material-code-brackets: AppliedLevelEnumType](./literals.md#appliedlevelenumtype) 
3. See [:material-code-braces: ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef](./type_defs.md#listrequestedservicequotachangehistorybyquotaresponsetypedef) 


```python
# list_requested_service_quota_change_history_by_quota method usage example with argument unpacking

kwargs: ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef = {  # (1)
    "ServiceCode": ...,
    "QuotaCode": ...,
}

parent.list_requested_service_quota_change_history_by_quota(**kwargs)
```

1. See [:material-code-braces: ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef](./type_defs.md#listrequestedservicequotachangehistorybyquotarequestrequesttypedef) 

### list\_service\_quota\_increase\_requests\_in\_template

Lists the quota increase requests in the specified quota request template.

Type annotations and code completion for `#!python session.client("service-quotas").list_service_quota_increase_requests_in_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# list_service_quota_increase_requests_in_template method definition

await def list_service_quota_increase_requests_in_template(
    self,
    *,
    ServiceCode: str = ...,
    AwsRegion: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef](./type_defs.md#listservicequotaincreaserequestsintemplateresponsetypedef) 


```python
# list_service_quota_increase_requests_in_template method usage example with argument unpacking

kwargs: ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef = {  # (1)
    "ServiceCode": ...,
}

parent.list_service_quota_increase_requests_in_template(**kwargs)
```

1. See [:material-code-braces: ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef](./type_defs.md#listservicequotaincreaserequestsintemplaterequestrequesttypedef) 

### list\_service\_quotas

Lists the applied quota values for the specified Amazon Web Service.

Type annotations and code completion for `#!python session.client("service-quotas").list_service_quotas` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# list_service_quotas method definition

await def list_service_quotas(
    self,
    *,
    ServiceCode: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    QuotaCode: str = ...,
    QuotaAppliedAtLevel: AppliedLevelEnumType = ...,  # (1)
) -> ListServiceQuotasResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AppliedLevelEnumType](./literals.md#appliedlevelenumtype) 
2. See [:material-code-braces: ListServiceQuotasResponseTypeDef](./type_defs.md#listservicequotasresponsetypedef) 


```python
# list_service_quotas method usage example with argument unpacking

kwargs: ListServiceQuotasRequestRequestTypeDef = {  # (1)
    "ServiceCode": ...,
}

parent.list_service_quotas(**kwargs)
```

1. See [:material-code-braces: ListServiceQuotasRequestRequestTypeDef](./type_defs.md#listservicequotasrequestrequesttypedef) 

### list\_services

Lists the names and codes for the Amazon Web Services integrated with Service
Quotas.

Type annotations and code completion for `#!python session.client("service-quotas").list_services` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# list_services method definition

await def list_services(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListServicesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServicesResponseTypeDef](./type_defs.md#listservicesresponsetypedef) 


```python
# list_services method usage example with argument unpacking

kwargs: ListServicesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_services(**kwargs)
```

1. See [:material-code-braces: ListServicesRequestRequestTypeDef](./type_defs.md#listservicesrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of the tags assigned to the specified applied quota.

Type annotations and code completion for `#!python session.client("service-quotas").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### put\_service\_quota\_increase\_request\_into\_template

Adds a quota increase request to your quota request template.

Type annotations and code completion for `#!python session.client("service-quotas").put_service_quota_increase_request_into_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# put_service_quota_increase_request_into_template method definition

await def put_service_quota_increase_request_into_template(
    self,
    *,
    QuotaCode: str,
    ServiceCode: str,
    AwsRegion: str,
    DesiredValue: float,
) -> PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef](./type_defs.md#putservicequotaincreaserequestintotemplateresponsetypedef) 


```python
# put_service_quota_increase_request_into_template method usage example with argument unpacking

kwargs: PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef = {  # (1)
    "QuotaCode": ...,
    "ServiceCode": ...,
    "AwsRegion": ...,
    "DesiredValue": ...,
}

parent.put_service_quota_increase_request_into_template(**kwargs)
```

1. See [:material-code-braces: PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef](./type_defs.md#putservicequotaincreaserequestintotemplaterequestrequesttypedef) 

### request\_service\_quota\_increase

Submits a quota increase request for the specified quota.

Type annotations and code completion for `#!python session.client("service-quotas").request_service_quota_increase` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# request_service_quota_increase method definition

await def request_service_quota_increase(
    self,
    *,
    ServiceCode: str,
    QuotaCode: str,
    DesiredValue: float,
    ContextId: str = ...,
) -> RequestServiceQuotaIncreaseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RequestServiceQuotaIncreaseResponseTypeDef](./type_defs.md#requestservicequotaincreaseresponsetypedef) 


```python
# request_service_quota_increase method usage example with argument unpacking

kwargs: RequestServiceQuotaIncreaseRequestRequestTypeDef = {  # (1)
    "ServiceCode": ...,
    "QuotaCode": ...,
    "DesiredValue": ...,
}

parent.request_service_quota_increase(**kwargs)
```

1. See [:material-code-braces: RequestServiceQuotaIncreaseRequestRequestTypeDef](./type_defs.md#requestservicequotaincreaserequestrequesttypedef) 

### tag\_resource

Adds tags to the specified applied quota.

Type annotations and code completion for `#!python session.client("service-quotas").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes tags from the specified applied quota.

Type annotations and code completion for `#!python session.client("service-quotas").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("service-quotas").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("service-quotas").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

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

Type annotations and code completion for `#!python session.client("service-quotas").get_paginator` method with overloads.

- `client.get_paginator("list_aws_default_service_quotas")` -> [ListAWSDefaultServiceQuotasPaginator](./paginators.md#listawsdefaultservicequotaspaginator)
- `client.get_paginator("list_requested_service_quota_change_history_by_quota")` -> [ListRequestedServiceQuotaChangeHistoryByQuotaPaginator](./paginators.md#listrequestedservicequotachangehistorybyquotapaginator)
- `client.get_paginator("list_requested_service_quota_change_history")` -> [ListRequestedServiceQuotaChangeHistoryPaginator](./paginators.md#listrequestedservicequotachangehistorypaginator)
- `client.get_paginator("list_service_quota_increase_requests_in_template")` -> [ListServiceQuotaIncreaseRequestsInTemplatePaginator](./paginators.md#listservicequotaincreaserequestsintemplatepaginator)
- `client.get_paginator("list_service_quotas")` -> [ListServiceQuotasPaginator](./paginators.md#listservicequotaspaginator)
- `client.get_paginator("list_services")` -> [ListServicesPaginator](./paginators.md#listservicespaginator)


