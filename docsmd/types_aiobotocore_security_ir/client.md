# SecurityIncidentResponseClient

> [Index](../README.md) > [SecurityIncidentResponse](./README.md) > SecurityIncidentResponseClient

!!! note ""

    Auto-generated documentation for [SecurityIncidentResponse](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#securityincidentresponse)
    type annotations stubs module [types-aiobotocore-security-ir](https://pypi.org/project/types-aiobotocore-security-ir/).

## SecurityIncidentResponseClient

Type annotations and code completion for `#!python session.client("security-ir")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# SecurityIncidentResponseClient usage example

from aioboto3.session import Session
from types_aiobotocore_security_ir.client import SecurityIncidentResponseClient

session = Session()
async with session.client("security-ir") as client:
    client: SecurityIncidentResponseClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("security-ir").exceptions` structure.

```python
# SecurityIncidentResponseClient.exceptions usage example

async with session.client("security-ir") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.InvalidTokenException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.SecurityIncidentResponseNotActiveException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# SecurityIncidentResponseClient.exceptions type checking example

from types_aiobotocore_security_ir.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("security-ir").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("security-ir").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

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


### batch\_get\_member\_account\_details

Grants permission to view an existing membership.

Type annotations and code completion for `#!python session.client("security-ir").batch_get_member_account_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# batch_get_member_account_details method definition

await def batch_get_member_account_details(
    self,
    *,
    membershipId: str,
    accountIds: Sequence[str],
) -> BatchGetMemberAccountDetailsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetMemberAccountDetailsResponseTypeDef](./type_defs.md#batchgetmemberaccountdetailsresponsetypedef) 


```python
# batch_get_member_account_details method usage example with argument unpacking

kwargs: BatchGetMemberAccountDetailsRequestRequestTypeDef = {  # (1)
    "membershipId": ...,
    "accountIds": ...,
}

parent.batch_get_member_account_details(**kwargs)
```

1. See [:material-code-braces: BatchGetMemberAccountDetailsRequestRequestTypeDef](./type_defs.md#batchgetmemberaccountdetailsrequestrequesttypedef) 

### cancel\_membership

Grants permissions to cancel an existing membership.

Type annotations and code completion for `#!python session.client("security-ir").cancel_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# cancel_membership method definition

await def cancel_membership(
    self,
    *,
    membershipId: str,
) -> CancelMembershipResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelMembershipResponseTypeDef](./type_defs.md#cancelmembershipresponsetypedef) 


```python
# cancel_membership method usage example with argument unpacking

kwargs: CancelMembershipRequestRequestTypeDef = {  # (1)
    "membershipId": ...,
}

parent.cancel_membership(**kwargs)
```

1. See [:material-code-braces: CancelMembershipRequestRequestTypeDef](./type_defs.md#cancelmembershiprequestrequesttypedef) 

### close\_case

Grants permission to close an existing case.

Type annotations and code completion for `#!python session.client("security-ir").close_case` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# close_case method definition

await def close_case(
    self,
    *,
    caseId: str,
) -> CloseCaseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CloseCaseResponseTypeDef](./type_defs.md#closecaseresponsetypedef) 


```python
# close_case method usage example with argument unpacking

kwargs: CloseCaseRequestRequestTypeDef = {  # (1)
    "caseId": ...,
}

parent.close_case(**kwargs)
```

1. See [:material-code-braces: CloseCaseRequestRequestTypeDef](./type_defs.md#closecaserequestrequesttypedef) 

### create\_case

Grants permission to create a new case.

Type annotations and code completion for `#!python session.client("security-ir").create_case` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# create_case method definition

await def create_case(
    self,
    *,
    resolverType: ResolverTypeType,  # (1)
    title: str,
    description: str,
    engagementType: EngagementTypeType,  # (2)
    reportedIncidentStartDate: TimestampTypeDef,
    impactedAccounts: Sequence[str],
    watchers: Sequence[WatcherTypeDef],  # (3)
    clientToken: str = ...,
    threatActorIpAddresses: Sequence[ThreatActorIpTypeDef] = ...,  # (4)
    impactedServices: Sequence[str] = ...,
    impactedAwsRegions: Sequence[ImpactedAwsRegionTypeDef] = ...,  # (5)
    tags: Mapping[str, str] = ...,
) -> CreateCaseResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: ResolverTypeType](./literals.md#resolvertypetype) 
2. See [:material-code-brackets: EngagementTypeType](./literals.md#engagementtypetype) 
3. See [:material-code-braces: WatcherTypeDef](./type_defs.md#watchertypedef) 
4. See [:material-code-braces: ThreatActorIpTypeDef](./type_defs.md#threatactoriptypedef) 
5. See [:material-code-braces: ImpactedAwsRegionTypeDef](./type_defs.md#impactedawsregiontypedef) 
6. See [:material-code-braces: CreateCaseResponseTypeDef](./type_defs.md#createcaseresponsetypedef) 


```python
# create_case method usage example with argument unpacking

kwargs: CreateCaseRequestRequestTypeDef = {  # (1)
    "resolverType": ...,
    "title": ...,
    "description": ...,
    "engagementType": ...,
    "reportedIncidentStartDate": ...,
    "impactedAccounts": ...,
    "watchers": ...,
}

parent.create_case(**kwargs)
```

1. See [:material-code-braces: CreateCaseRequestRequestTypeDef](./type_defs.md#createcaserequestrequesttypedef) 

### create\_case\_comment

Grants permission to add a comment to an existing case.

Type annotations and code completion for `#!python session.client("security-ir").create_case_comment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# create_case_comment method definition

await def create_case_comment(
    self,
    *,
    caseId: str,
    body: str,
    clientToken: str = ...,
) -> CreateCaseCommentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateCaseCommentResponseTypeDef](./type_defs.md#createcasecommentresponsetypedef) 


```python
# create_case_comment method usage example with argument unpacking

kwargs: CreateCaseCommentRequestRequestTypeDef = {  # (1)
    "caseId": ...,
    "body": ...,
}

parent.create_case_comment(**kwargs)
```

1. See [:material-code-braces: CreateCaseCommentRequestRequestTypeDef](./type_defs.md#createcasecommentrequestrequesttypedef) 

### create\_membership

Grants permissions to create a new membership.

Type annotations and code completion for `#!python session.client("security-ir").create_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# create_membership method definition

await def create_membership(
    self,
    *,
    membershipName: str,
    incidentResponseTeam: Sequence[IncidentResponderTypeDef],  # (1)
    clientToken: str = ...,
    optInFeatures: Sequence[OptInFeatureTypeDef] = ...,  # (2)
    tags: Mapping[str, str] = ...,
) -> CreateMembershipResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: IncidentResponderTypeDef](./type_defs.md#incidentrespondertypedef) 
2. See [:material-code-braces: OptInFeatureTypeDef](./type_defs.md#optinfeaturetypedef) 
3. See [:material-code-braces: CreateMembershipResponseTypeDef](./type_defs.md#createmembershipresponsetypedef) 


```python
# create_membership method usage example with argument unpacking

kwargs: CreateMembershipRequestRequestTypeDef = {  # (1)
    "membershipName": ...,
    "incidentResponseTeam": ...,
}

parent.create_membership(**kwargs)
```

1. See [:material-code-braces: CreateMembershipRequestRequestTypeDef](./type_defs.md#createmembershiprequestrequesttypedef) 

### get\_case

Grant permission to view a designated case.

Type annotations and code completion for `#!python session.client("security-ir").get_case` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# get_case method definition

await def get_case(
    self,
    *,
    caseId: str,
) -> GetCaseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCaseResponseTypeDef](./type_defs.md#getcaseresponsetypedef) 


```python
# get_case method usage example with argument unpacking

kwargs: GetCaseRequestRequestTypeDef = {  # (1)
    "caseId": ...,
}

parent.get_case(**kwargs)
```

1. See [:material-code-braces: GetCaseRequestRequestTypeDef](./type_defs.md#getcaserequestrequesttypedef) 

### get\_case\_attachment\_download\_url

Grants permission to obtain an Amazon S3 presigned URL to download an
attachment.

Type annotations and code completion for `#!python session.client("security-ir").get_case_attachment_download_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# get_case_attachment_download_url method definition

await def get_case_attachment_download_url(
    self,
    *,
    caseId: str,
    attachmentId: str,
) -> GetCaseAttachmentDownloadUrlResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCaseAttachmentDownloadUrlResponseTypeDef](./type_defs.md#getcaseattachmentdownloadurlresponsetypedef) 


```python
# get_case_attachment_download_url method usage example with argument unpacking

kwargs: GetCaseAttachmentDownloadUrlRequestRequestTypeDef = {  # (1)
    "caseId": ...,
    "attachmentId": ...,
}

parent.get_case_attachment_download_url(**kwargs)
```

1. See [:material-code-braces: GetCaseAttachmentDownloadUrlRequestRequestTypeDef](./type_defs.md#getcaseattachmentdownloadurlrequestrequesttypedef) 

### get\_case\_attachment\_upload\_url

Grants permission to upload an attachment to a case.

Type annotations and code completion for `#!python session.client("security-ir").get_case_attachment_upload_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# get_case_attachment_upload_url method definition

await def get_case_attachment_upload_url(
    self,
    *,
    caseId: str,
    fileName: str,
    contentLength: int,
    clientToken: str = ...,
) -> GetCaseAttachmentUploadUrlResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCaseAttachmentUploadUrlResponseTypeDef](./type_defs.md#getcaseattachmentuploadurlresponsetypedef) 


```python
# get_case_attachment_upload_url method usage example with argument unpacking

kwargs: GetCaseAttachmentUploadUrlRequestRequestTypeDef = {  # (1)
    "caseId": ...,
    "fileName": ...,
    "contentLength": ...,
}

parent.get_case_attachment_upload_url(**kwargs)
```

1. See [:material-code-braces: GetCaseAttachmentUploadUrlRequestRequestTypeDef](./type_defs.md#getcaseattachmentuploadurlrequestrequesttypedef) 

### get\_membership

Grants permission to get details of a designated service membership.

Type annotations and code completion for `#!python session.client("security-ir").get_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# get_membership method definition

await def get_membership(
    self,
    *,
    membershipId: str,
) -> GetMembershipResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMembershipResponseTypeDef](./type_defs.md#getmembershipresponsetypedef) 


```python
# get_membership method usage example with argument unpacking

kwargs: GetMembershipRequestRequestTypeDef = {  # (1)
    "membershipId": ...,
}

parent.get_membership(**kwargs)
```

1. See [:material-code-braces: GetMembershipRequestRequestTypeDef](./type_defs.md#getmembershiprequestrequesttypedef) 

### list\_case\_edits

Grants permissions to view the aidt log for edits made to a designated case.

Type annotations and code completion for `#!python session.client("security-ir").list_case_edits` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# list_case_edits method definition

await def list_case_edits(
    self,
    *,
    caseId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListCaseEditsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCaseEditsResponseTypeDef](./type_defs.md#listcaseeditsresponsetypedef) 


```python
# list_case_edits method usage example with argument unpacking

kwargs: ListCaseEditsRequestRequestTypeDef = {  # (1)
    "caseId": ...,
}

parent.list_case_edits(**kwargs)
```

1. See [:material-code-braces: ListCaseEditsRequestRequestTypeDef](./type_defs.md#listcaseeditsrequestrequesttypedef) 

### list\_cases

Grants permission to list all cases the requester has access to.

Type annotations and code completion for `#!python session.client("security-ir").list_cases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# list_cases method definition

await def list_cases(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListCasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCasesResponseTypeDef](./type_defs.md#listcasesresponsetypedef) 


```python
# list_cases method usage example with argument unpacking

kwargs: ListCasesRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_cases(**kwargs)
```

1. See [:material-code-braces: ListCasesRequestRequestTypeDef](./type_defs.md#listcasesrequestrequesttypedef) 

### list\_comments

Grants permissions to list and view comments for a designated case.

Type annotations and code completion for `#!python session.client("security-ir").list_comments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# list_comments method definition

await def list_comments(
    self,
    *,
    caseId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListCommentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCommentsResponseTypeDef](./type_defs.md#listcommentsresponsetypedef) 


```python
# list_comments method usage example with argument unpacking

kwargs: ListCommentsRequestRequestTypeDef = {  # (1)
    "caseId": ...,
}

parent.list_comments(**kwargs)
```

1. See [:material-code-braces: ListCommentsRequestRequestTypeDef](./type_defs.md#listcommentsrequestrequesttypedef) 

### list\_memberships

Grants permission to query the memberships a principal has access to.

Type annotations and code completion for `#!python session.client("security-ir").list_memberships` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# list_memberships method definition

await def list_memberships(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListMembershipsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMembershipsResponseTypeDef](./type_defs.md#listmembershipsresponsetypedef) 


```python
# list_memberships method usage example with argument unpacking

kwargs: ListMembershipsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_memberships(**kwargs)
```

1. See [:material-code-braces: ListMembershipsRequestRequestTypeDef](./type_defs.md#listmembershipsrequestrequesttypedef) 

### list\_tags\_for\_resource

Grants permission to view currently configured tags on a resource.

Type annotations and code completion for `#!python session.client("security-ir").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef) 

### tag\_resource

Grants permission to add a tag(s) to a designated resource.

Type annotations and code completion for `#!python session.client("security-ir").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef) 

### untag\_resource

Grants permission to remove a tag(s) from a designate resource.

Type annotations and code completion for `#!python session.client("security-ir").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

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

kwargs: UntagResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef) 

### update\_case

Grants permission to update an existing case.

Type annotations and code completion for `#!python session.client("security-ir").update_case` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# update_case method definition

await def update_case(
    self,
    *,
    caseId: str,
    title: str = ...,
    description: str = ...,
    reportedIncidentStartDate: TimestampTypeDef = ...,
    actualIncidentStartDate: TimestampTypeDef = ...,
    engagementType: EngagementTypeType = ...,  # (1)
    watchersToAdd: Sequence[WatcherTypeDef] = ...,  # (2)
    watchersToDelete: Sequence[WatcherTypeDef] = ...,  # (2)
    threatActorIpAddressesToAdd: Sequence[ThreatActorIpTypeDef] = ...,  # (4)
    threatActorIpAddressesToDelete: Sequence[ThreatActorIpTypeDef] = ...,  # (4)
    impactedServicesToAdd: Sequence[str] = ...,
    impactedServicesToDelete: Sequence[str] = ...,
    impactedAwsRegionsToAdd: Sequence[ImpactedAwsRegionTypeDef] = ...,  # (6)
    impactedAwsRegionsToDelete: Sequence[ImpactedAwsRegionTypeDef] = ...,  # (6)
    impactedAccountsToAdd: Sequence[str] = ...,
    impactedAccountsToDelete: Sequence[str] = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: EngagementTypeType](./literals.md#engagementtypetype) 
2. See [:material-code-braces: WatcherTypeDef](./type_defs.md#watchertypedef) 
3. See [:material-code-braces: WatcherTypeDef](./type_defs.md#watchertypedef) 
4. See [:material-code-braces: ThreatActorIpTypeDef](./type_defs.md#threatactoriptypedef) 
5. See [:material-code-braces: ThreatActorIpTypeDef](./type_defs.md#threatactoriptypedef) 
6. See [:material-code-braces: ImpactedAwsRegionTypeDef](./type_defs.md#impactedawsregiontypedef) 
7. See [:material-code-braces: ImpactedAwsRegionTypeDef](./type_defs.md#impactedawsregiontypedef) 


```python
# update_case method usage example with argument unpacking

kwargs: UpdateCaseRequestRequestTypeDef = {  # (1)
    "caseId": ...,
}

parent.update_case(**kwargs)
```

1. See [:material-code-braces: UpdateCaseRequestRequestTypeDef](./type_defs.md#updatecaserequestrequesttypedef) 

### update\_case\_comment

Grants permission to update an existing case comment.

Type annotations and code completion for `#!python session.client("security-ir").update_case_comment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# update_case_comment method definition

await def update_case_comment(
    self,
    *,
    caseId: str,
    commentId: str,
    body: str,
) -> UpdateCaseCommentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateCaseCommentResponseTypeDef](./type_defs.md#updatecasecommentresponsetypedef) 


```python
# update_case_comment method usage example with argument unpacking

kwargs: UpdateCaseCommentRequestRequestTypeDef = {  # (1)
    "caseId": ...,
    "commentId": ...,
    "body": ...,
}

parent.update_case_comment(**kwargs)
```

1. See [:material-code-braces: UpdateCaseCommentRequestRequestTypeDef](./type_defs.md#updatecasecommentrequestrequesttypedef) 

### update\_case\_status

Grants permission to update the status for a designated cases.

Type annotations and code completion for `#!python session.client("security-ir").update_case_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# update_case_status method definition

await def update_case_status(
    self,
    *,
    caseId: str,
    caseStatus: SelfManagedCaseStatusType,  # (1)
) -> UpdateCaseStatusResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SelfManagedCaseStatusType](./literals.md#selfmanagedcasestatustype) 
2. See [:material-code-braces: UpdateCaseStatusResponseTypeDef](./type_defs.md#updatecasestatusresponsetypedef) 


```python
# update_case_status method usage example with argument unpacking

kwargs: UpdateCaseStatusRequestRequestTypeDef = {  # (1)
    "caseId": ...,
    "caseStatus": ...,
}

parent.update_case_status(**kwargs)
```

1. See [:material-code-braces: UpdateCaseStatusRequestRequestTypeDef](./type_defs.md#updatecasestatusrequestrequesttypedef) 

### update\_membership

Grants access to UpdateMembership to change membership configuration.

Type annotations and code completion for `#!python session.client("security-ir").update_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# update_membership method definition

await def update_membership(
    self,
    *,
    membershipId: str,
    membershipName: str = ...,
    incidentResponseTeam: Sequence[IncidentResponderTypeDef] = ...,  # (1)
    optInFeatures: Sequence[OptInFeatureTypeDef] = ...,  # (2)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: IncidentResponderTypeDef](./type_defs.md#incidentrespondertypedef) 
2. See [:material-code-braces: OptInFeatureTypeDef](./type_defs.md#optinfeaturetypedef) 


```python
# update_membership method usage example with argument unpacking

kwargs: UpdateMembershipRequestRequestTypeDef = {  # (1)
    "membershipId": ...,
}

parent.update_membership(**kwargs)
```

1. See [:material-code-braces: UpdateMembershipRequestRequestTypeDef](./type_defs.md#updatemembershiprequestrequesttypedef) 

### update\_resolver\_type

Grants permission to update the resolver type for a case.

Type annotations and code completion for `#!python session.client("security-ir").update_resolver_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# update_resolver_type method definition

await def update_resolver_type(
    self,
    *,
    caseId: str,
    resolverType: ResolverTypeType,  # (1)
) -> UpdateResolverTypeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResolverTypeType](./literals.md#resolvertypetype) 
2. See [:material-code-braces: UpdateResolverTypeResponseTypeDef](./type_defs.md#updateresolvertyperesponsetypedef) 


```python
# update_resolver_type method usage example with argument unpacking

kwargs: UpdateResolverTypeRequestRequestTypeDef = {  # (1)
    "caseId": ...,
    "resolverType": ...,
}

parent.update_resolver_type(**kwargs)
```

1. See [:material-code-braces: UpdateResolverTypeRequestRequestTypeDef](./type_defs.md#updateresolvertyperequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("security-ir").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("security-ir").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

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

Type annotations and code completion for `#!python session.client("security-ir").get_paginator` method with overloads.

- `client.get_paginator("list_case_edits")` -> [ListCaseEditsPaginator](./paginators.md#listcaseeditspaginator)
- `client.get_paginator("list_cases")` -> [ListCasesPaginator](./paginators.md#listcasespaginator)
- `client.get_paginator("list_comments")` -> [ListCommentsPaginator](./paginators.md#listcommentspaginator)
- `client.get_paginator("list_memberships")` -> [ListMembershipsPaginator](./paginators.md#listmembershipspaginator)


