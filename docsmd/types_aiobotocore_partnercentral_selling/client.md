# PartnerCentralSellingAPIClient

> [Index](../README.md) > [PartnerCentralSellingAPI](./README.md) > PartnerCentralSellingAPIClient

!!! note ""

    Auto-generated documentation for [PartnerCentralSellingAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#partnercentralsellingapi)
    type annotations stubs module [types-aiobotocore-partnercentral-selling](https://pypi.org/project/types-aiobotocore-partnercentral-selling/).

## PartnerCentralSellingAPIClient

Type annotations and code completion for `#!python session.client("partnercentral-selling")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# PartnerCentralSellingAPIClient usage example

from aioboto3.session import Session
from types_aiobotocore_partnercentral_selling.client import PartnerCentralSellingAPIClient

session = Session()
async with session.client("partnercentral-selling") as client:
    client: PartnerCentralSellingAPIClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("partnercentral-selling").exceptions` structure.

```python
# PartnerCentralSellingAPIClient.exceptions usage example

async with session.client("partnercentral-selling") as client:
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
# PartnerCentralSellingAPIClient.exceptions type checking example

from types_aiobotocore_partnercentral_selling.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("partnercentral-selling").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("partnercentral-selling").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

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


### accept\_engagement\_invitation

Use the <code>AcceptEngagementInvitation</code> action to accept an engagement
invitation shared by AWS.

Type annotations and code completion for `#!python session.client("partnercentral-selling").accept_engagement_invitation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# accept_engagement_invitation method definition

await def accept_engagement_invitation(
    self,
    *,
    Catalog: str,
    Identifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# accept_engagement_invitation method usage example with argument unpacking

kwargs: AcceptEngagementInvitationRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "Identifier": ...,
}

parent.accept_engagement_invitation(**kwargs)
```

1. See [:material-code-braces: AcceptEngagementInvitationRequestRequestTypeDef](./type_defs.md#acceptengagementinvitationrequestrequesttypedef) 

### assign\_opportunity

Enables you to reassign an existing <code>Opportunity</code> to another user
within your Partner Central account.

Type annotations and code completion for `#!python session.client("partnercentral-selling").assign_opportunity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# assign_opportunity method definition

await def assign_opportunity(
    self,
    *,
    Assignee: AssigneeContactTypeDef,  # (1)
    Catalog: str,
    Identifier: str,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AssigneeContactTypeDef](./type_defs.md#assigneecontacttypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# assign_opportunity method usage example with argument unpacking

kwargs: AssignOpportunityRequestRequestTypeDef = {  # (1)
    "Assignee": ...,
    "Catalog": ...,
    "Identifier": ...,
}

parent.assign_opportunity(**kwargs)
```

1. See [:material-code-braces: AssignOpportunityRequestRequestTypeDef](./type_defs.md#assignopportunityrequestrequesttypedef) 

### associate\_opportunity

Enables you to create a formal association between an <code>Opportunity</code>
and various related entities, enriching the context and details of the
opportunity for better collaboration and decision making.

Type annotations and code completion for `#!python session.client("partnercentral-selling").associate_opportunity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# associate_opportunity method definition

await def associate_opportunity(
    self,
    *,
    Catalog: str,
    OpportunityIdentifier: str,
    RelatedEntityIdentifier: str,
    RelatedEntityType: RelatedEntityTypeType,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RelatedEntityTypeType](./literals.md#relatedentitytypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_opportunity method usage example with argument unpacking

kwargs: AssociateOpportunityRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "OpportunityIdentifier": ...,
    "RelatedEntityIdentifier": ...,
    "RelatedEntityType": ...,
}

parent.associate_opportunity(**kwargs)
```

1. See [:material-code-braces: AssociateOpportunityRequestRequestTypeDef](./type_defs.md#associateopportunityrequestrequesttypedef) 

### create\_engagement

The <code>CreateEngagement</code> action allows you to create an
<code>Engagement</code>, which serves as a collaborative space between
different parties such as AWS Partners and AWS Sellers.

Type annotations and code completion for `#!python session.client("partnercentral-selling").create_engagement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# create_engagement method definition

await def create_engagement(
    self,
    *,
    Catalog: str,
    ClientToken: str,
    Description: str,
    Title: str,
    Contexts: Sequence[EngagementContextDetailsTypeDef] = ...,  # (1)
) -> CreateEngagementResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EngagementContextDetailsTypeDef](./type_defs.md#engagementcontextdetailstypedef) 
2. See [:material-code-braces: CreateEngagementResponseTypeDef](./type_defs.md#createengagementresponsetypedef) 


```python
# create_engagement method usage example with argument unpacking

kwargs: CreateEngagementRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ClientToken": ...,
    "Description": ...,
    "Title": ...,
}

parent.create_engagement(**kwargs)
```

1. See [:material-code-braces: CreateEngagementRequestRequestTypeDef](./type_defs.md#createengagementrequestrequesttypedef) 

### create\_engagement\_invitation

This action creates an invitation from a sender to a single receiver to join an
engagement.

Type annotations and code completion for `#!python session.client("partnercentral-selling").create_engagement_invitation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# create_engagement_invitation method definition

await def create_engagement_invitation(
    self,
    *,
    Catalog: str,
    ClientToken: str,
    EngagementIdentifier: str,
    Invitation: InvitationTypeDef,  # (1)
) -> CreateEngagementInvitationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InvitationTypeDef](./type_defs.md#invitationtypedef) 
2. See [:material-code-braces: CreateEngagementInvitationResponseTypeDef](./type_defs.md#createengagementinvitationresponsetypedef) 


```python
# create_engagement_invitation method usage example with argument unpacking

kwargs: CreateEngagementInvitationRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ClientToken": ...,
    "EngagementIdentifier": ...,
    "Invitation": ...,
}

parent.create_engagement_invitation(**kwargs)
```

1. See [:material-code-braces: CreateEngagementInvitationRequestRequestTypeDef](./type_defs.md#createengagementinvitationrequestrequesttypedef) 

### create\_opportunity

Creates an <code>Opportunity</code> record in Partner Central.

Type annotations and code completion for `#!python session.client("partnercentral-selling").create_opportunity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# create_opportunity method definition

await def create_opportunity(
    self,
    *,
    Catalog: str,
    ClientToken: str,
    Customer: CustomerTypeDef = ...,  # (1)
    LifeCycle: LifeCycleTypeDef = ...,  # (2)
    Marketing: MarketingTypeDef = ...,  # (3)
    NationalSecurity: NationalSecurityType = ...,  # (4)
    OpportunityTeam: Sequence[ContactTypeDef] = ...,  # (5)
    OpportunityType: OpportunityTypeType = ...,  # (6)
    Origin: OpportunityOriginType = ...,  # (7)
    PartnerOpportunityIdentifier: str = ...,
    PrimaryNeedsFromAws: Sequence[PrimaryNeedFromAwsType] = ...,  # (8)
    Project: ProjectTypeDef = ...,  # (9)
    SoftwareRevenue: SoftwareRevenueTypeDef = ...,  # (10)
) -> CreateOpportunityResponseTypeDef:  # (11)
    ...
```

1. See [:material-code-braces: CustomerTypeDef](./type_defs.md#customertypedef) 
2. See [:material-code-braces: LifeCycleTypeDef](./type_defs.md#lifecycletypedef) 
3. See [:material-code-braces: MarketingTypeDef](./type_defs.md#marketingtypedef) 
4. See [:material-code-brackets: NationalSecurityType](./literals.md#nationalsecuritytype) 
5. See [:material-code-braces: ContactTypeDef](./type_defs.md#contacttypedef) 
6. See [:material-code-brackets: OpportunityTypeType](./literals.md#opportunitytypetype) 
7. See [:material-code-brackets: OpportunityOriginType](./literals.md#opportunityorigintype) 
8. See [:material-code-brackets: PrimaryNeedFromAwsType](./literals.md#primaryneedfromawstype) 
9. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
10. See [:material-code-braces: SoftwareRevenueTypeDef](./type_defs.md#softwarerevenuetypedef) 
11. See [:material-code-braces: CreateOpportunityResponseTypeDef](./type_defs.md#createopportunityresponsetypedef) 


```python
# create_opportunity method usage example with argument unpacking

kwargs: CreateOpportunityRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ClientToken": ...,
}

parent.create_opportunity(**kwargs)
```

1. See [:material-code-braces: CreateOpportunityRequestRequestTypeDef](./type_defs.md#createopportunityrequestrequesttypedef) 

### create\_resource\_snapshot

This action allows you to create an immutable snapshot of a specific resource,
such as an opportunity, within the context of an engagement.

Type annotations and code completion for `#!python session.client("partnercentral-selling").create_resource_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# create_resource_snapshot method definition

await def create_resource_snapshot(
    self,
    *,
    Catalog: str,
    ClientToken: str,
    EngagementIdentifier: str,
    ResourceIdentifier: str,
    ResourceSnapshotTemplateIdentifier: str,
    ResourceType: ResourceTypeType,  # (1)
) -> CreateResourceSnapshotResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: CreateResourceSnapshotResponseTypeDef](./type_defs.md#createresourcesnapshotresponsetypedef) 


```python
# create_resource_snapshot method usage example with argument unpacking

kwargs: CreateResourceSnapshotRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ClientToken": ...,
    "EngagementIdentifier": ...,
    "ResourceIdentifier": ...,
    "ResourceSnapshotTemplateIdentifier": ...,
    "ResourceType": ...,
}

parent.create_resource_snapshot(**kwargs)
```

1. See [:material-code-braces: CreateResourceSnapshotRequestRequestTypeDef](./type_defs.md#createresourcesnapshotrequestrequesttypedef) 

### create\_resource\_snapshot\_job

Use this action to create a job to generate a snapshot of the specified
resource within an engagement.

Type annotations and code completion for `#!python session.client("partnercentral-selling").create_resource_snapshot_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# create_resource_snapshot_job method definition

await def create_resource_snapshot_job(
    self,
    *,
    Catalog: str,
    ClientToken: str,
    EngagementIdentifier: str,
    ResourceIdentifier: str,
    ResourceSnapshotTemplateIdentifier: str,
    ResourceType: ResourceTypeType,  # (1)
) -> CreateResourceSnapshotJobResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: CreateResourceSnapshotJobResponseTypeDef](./type_defs.md#createresourcesnapshotjobresponsetypedef) 


```python
# create_resource_snapshot_job method usage example with argument unpacking

kwargs: CreateResourceSnapshotJobRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ClientToken": ...,
    "EngagementIdentifier": ...,
    "ResourceIdentifier": ...,
    "ResourceSnapshotTemplateIdentifier": ...,
    "ResourceType": ...,
}

parent.create_resource_snapshot_job(**kwargs)
```

1. See [:material-code-braces: CreateResourceSnapshotJobRequestRequestTypeDef](./type_defs.md#createresourcesnapshotjobrequestrequesttypedef) 

### delete\_resource\_snapshot\_job

Use this action to deletes a previously created resource snapshot job.

Type annotations and code completion for `#!python session.client("partnercentral-selling").delete_resource_snapshot_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# delete_resource_snapshot_job method definition

await def delete_resource_snapshot_job(
    self,
    *,
    Catalog: str,
    ResourceSnapshotJobIdentifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_resource_snapshot_job method usage example with argument unpacking

kwargs: DeleteResourceSnapshotJobRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ResourceSnapshotJobIdentifier": ...,
}

parent.delete_resource_snapshot_job(**kwargs)
```

1. See [:material-code-braces: DeleteResourceSnapshotJobRequestRequestTypeDef](./type_defs.md#deleteresourcesnapshotjobrequestrequesttypedef) 

### disassociate\_opportunity

Allows you to remove an existing association between an
<code>Opportunity</code> and related entities, such as a Partner Solution,
Amazon Web Services product, or an Amazon Web Services Marketplace offer.

Type annotations and code completion for `#!python session.client("partnercentral-selling").disassociate_opportunity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# disassociate_opportunity method definition

await def disassociate_opportunity(
    self,
    *,
    Catalog: str,
    OpportunityIdentifier: str,
    RelatedEntityIdentifier: str,
    RelatedEntityType: RelatedEntityTypeType,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RelatedEntityTypeType](./literals.md#relatedentitytypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_opportunity method usage example with argument unpacking

kwargs: DisassociateOpportunityRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "OpportunityIdentifier": ...,
    "RelatedEntityIdentifier": ...,
    "RelatedEntityType": ...,
}

parent.disassociate_opportunity(**kwargs)
```

1. See [:material-code-braces: DisassociateOpportunityRequestRequestTypeDef](./type_defs.md#disassociateopportunityrequestrequesttypedef) 

### get\_aws\_opportunity\_summary

Retrieves a summary of an AWS Opportunity.

Type annotations and code completion for `#!python session.client("partnercentral-selling").get_aws_opportunity_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# get_aws_opportunity_summary method definition

await def get_aws_opportunity_summary(
    self,
    *,
    Catalog: str,
    RelatedOpportunityIdentifier: str,
) -> GetAwsOpportunitySummaryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAwsOpportunitySummaryResponseTypeDef](./type_defs.md#getawsopportunitysummaryresponsetypedef) 


```python
# get_aws_opportunity_summary method usage example with argument unpacking

kwargs: GetAwsOpportunitySummaryRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "RelatedOpportunityIdentifier": ...,
}

parent.get_aws_opportunity_summary(**kwargs)
```

1. See [:material-code-braces: GetAwsOpportunitySummaryRequestRequestTypeDef](./type_defs.md#getawsopportunitysummaryrequestrequesttypedef) 

### get\_engagement

Use this action to retrieve the engagement record for a given
<code>EngagementIdentifier</code>.

Type annotations and code completion for `#!python session.client("partnercentral-selling").get_engagement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# get_engagement method definition

await def get_engagement(
    self,
    *,
    Catalog: str,
    Identifier: str,
) -> GetEngagementResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEngagementResponseTypeDef](./type_defs.md#getengagementresponsetypedef) 


```python
# get_engagement method usage example with argument unpacking

kwargs: GetEngagementRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "Identifier": ...,
}

parent.get_engagement(**kwargs)
```

1. See [:material-code-braces: GetEngagementRequestRequestTypeDef](./type_defs.md#getengagementrequestrequesttypedef) 

### get\_engagement\_invitation

Retrieves the details of an engagement invitation shared by AWS with a partner.

Type annotations and code completion for `#!python session.client("partnercentral-selling").get_engagement_invitation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# get_engagement_invitation method definition

await def get_engagement_invitation(
    self,
    *,
    Catalog: str,
    Identifier: str,
) -> GetEngagementInvitationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEngagementInvitationResponseTypeDef](./type_defs.md#getengagementinvitationresponsetypedef) 


```python
# get_engagement_invitation method usage example with argument unpacking

kwargs: GetEngagementInvitationRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "Identifier": ...,
}

parent.get_engagement_invitation(**kwargs)
```

1. See [:material-code-braces: GetEngagementInvitationRequestRequestTypeDef](./type_defs.md#getengagementinvitationrequestrequesttypedef) 

### get\_opportunity

Fetches the <code>Opportunity</code> record from Partner Central by a given
<code>Identifier</code>.

Type annotations and code completion for `#!python session.client("partnercentral-selling").get_opportunity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# get_opportunity method definition

await def get_opportunity(
    self,
    *,
    Catalog: str,
    Identifier: str,
) -> GetOpportunityResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOpportunityResponseTypeDef](./type_defs.md#getopportunityresponsetypedef) 


```python
# get_opportunity method usage example with argument unpacking

kwargs: GetOpportunityRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "Identifier": ...,
}

parent.get_opportunity(**kwargs)
```

1. See [:material-code-braces: GetOpportunityRequestRequestTypeDef](./type_defs.md#getopportunityrequestrequesttypedef) 

### get\_resource\_snapshot

Use this action to retrieve a specific snapshot record.

Type annotations and code completion for `#!python session.client("partnercentral-selling").get_resource_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# get_resource_snapshot method definition

await def get_resource_snapshot(
    self,
    *,
    Catalog: str,
    EngagementIdentifier: str,
    ResourceIdentifier: str,
    ResourceSnapshotTemplateIdentifier: str,
    ResourceType: ResourceTypeType,  # (1)
    Revision: int = ...,
) -> GetResourceSnapshotResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: GetResourceSnapshotResponseTypeDef](./type_defs.md#getresourcesnapshotresponsetypedef) 


```python
# get_resource_snapshot method usage example with argument unpacking

kwargs: GetResourceSnapshotRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "EngagementIdentifier": ...,
    "ResourceIdentifier": ...,
    "ResourceSnapshotTemplateIdentifier": ...,
    "ResourceType": ...,
}

parent.get_resource_snapshot(**kwargs)
```

1. See [:material-code-braces: GetResourceSnapshotRequestRequestTypeDef](./type_defs.md#getresourcesnapshotrequestrequesttypedef) 

### get\_resource\_snapshot\_job

Use this action to retrieves information about a specific resource snapshot job.

Type annotations and code completion for `#!python session.client("partnercentral-selling").get_resource_snapshot_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# get_resource_snapshot_job method definition

await def get_resource_snapshot_job(
    self,
    *,
    Catalog: str,
    ResourceSnapshotJobIdentifier: str,
) -> GetResourceSnapshotJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResourceSnapshotJobResponseTypeDef](./type_defs.md#getresourcesnapshotjobresponsetypedef) 


```python
# get_resource_snapshot_job method usage example with argument unpacking

kwargs: GetResourceSnapshotJobRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ResourceSnapshotJobIdentifier": ...,
}

parent.get_resource_snapshot_job(**kwargs)
```

1. See [:material-code-braces: GetResourceSnapshotJobRequestRequestTypeDef](./type_defs.md#getresourcesnapshotjobrequestrequesttypedef) 

### get\_selling\_system\_settings

Retrieves the currently set system settings, which include the IAM Role used
for resource snapshot jobs.

Type annotations and code completion for `#!python session.client("partnercentral-selling").get_selling_system_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# get_selling_system_settings method definition

await def get_selling_system_settings(
    self,
    *,
    Catalog: str,
) -> GetSellingSystemSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSellingSystemSettingsResponseTypeDef](./type_defs.md#getsellingsystemsettingsresponsetypedef) 


```python
# get_selling_system_settings method usage example with argument unpacking

kwargs: GetSellingSystemSettingsRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
}

parent.get_selling_system_settings(**kwargs)
```

1. See [:material-code-braces: GetSellingSystemSettingsRequestRequestTypeDef](./type_defs.md#getsellingsystemsettingsrequestrequesttypedef) 

### list\_engagement\_by\_accepting\_invitation\_tasks

Lists all in-progress, completed, or failed
StartEngagementByAcceptingInvitationTask tasks that were initiated by the
caller's account.

Type annotations and code completion for `#!python session.client("partnercentral-selling").list_engagement_by_accepting_invitation_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# list_engagement_by_accepting_invitation_tasks method definition

await def list_engagement_by_accepting_invitation_tasks(
    self,
    *,
    Catalog: str,
    EngagementInvitationIdentifier: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    OpportunityIdentifier: Sequence[str] = ...,
    Sort: ListTasksSortBaseTypeDef = ...,  # (1)
    TaskIdentifier: Sequence[str] = ...,
    TaskStatus: Sequence[TaskStatusType] = ...,  # (2)
) -> ListEngagementByAcceptingInvitationTasksResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ListTasksSortBaseTypeDef](./type_defs.md#listtaskssortbasetypedef) 
2. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
3. See [:material-code-braces: ListEngagementByAcceptingInvitationTasksResponseTypeDef](./type_defs.md#listengagementbyacceptinginvitationtasksresponsetypedef) 


```python
# list_engagement_by_accepting_invitation_tasks method usage example with argument unpacking

kwargs: ListEngagementByAcceptingInvitationTasksRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
}

parent.list_engagement_by_accepting_invitation_tasks(**kwargs)
```

1. See [:material-code-braces: ListEngagementByAcceptingInvitationTasksRequestRequestTypeDef](./type_defs.md#listengagementbyacceptinginvitationtasksrequestrequesttypedef) 

### list\_engagement\_from\_opportunity\_tasks

Lists all in-progress, completed, or failed
<code>EngagementFromOpportunity</code> tasks that were initiated by the
caller's account.

Type annotations and code completion for `#!python session.client("partnercentral-selling").list_engagement_from_opportunity_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# list_engagement_from_opportunity_tasks method definition

await def list_engagement_from_opportunity_tasks(
    self,
    *,
    Catalog: str,
    EngagementIdentifier: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    OpportunityIdentifier: Sequence[str] = ...,
    Sort: ListTasksSortBaseTypeDef = ...,  # (1)
    TaskIdentifier: Sequence[str] = ...,
    TaskStatus: Sequence[TaskStatusType] = ...,  # (2)
) -> ListEngagementFromOpportunityTasksResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ListTasksSortBaseTypeDef](./type_defs.md#listtaskssortbasetypedef) 
2. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
3. See [:material-code-braces: ListEngagementFromOpportunityTasksResponseTypeDef](./type_defs.md#listengagementfromopportunitytasksresponsetypedef) 


```python
# list_engagement_from_opportunity_tasks method usage example with argument unpacking

kwargs: ListEngagementFromOpportunityTasksRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
}

parent.list_engagement_from_opportunity_tasks(**kwargs)
```

1. See [:material-code-braces: ListEngagementFromOpportunityTasksRequestRequestTypeDef](./type_defs.md#listengagementfromopportunitytasksrequestrequesttypedef) 

### list\_engagement\_invitations

Retrieves a list of engagement invitations sent to the partner.

Type annotations and code completion for `#!python session.client("partnercentral-selling").list_engagement_invitations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# list_engagement_invitations method definition

await def list_engagement_invitations(
    self,
    *,
    Catalog: str,
    ParticipantType: ParticipantTypeType,  # (1)
    EngagementIdentifier: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    PayloadType: Sequence[EngagementInvitationPayloadTypeType] = ...,  # (2)
    SenderAwsAccountId: Sequence[str] = ...,
    Sort: OpportunityEngagementInvitationSortTypeDef = ...,  # (3)
    Status: Sequence[InvitationStatusType] = ...,  # (4)
) -> ListEngagementInvitationsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: ParticipantTypeType](./literals.md#participanttypetype) 
2. See [:material-code-brackets: EngagementInvitationPayloadTypeType](./literals.md#engagementinvitationpayloadtypetype) 
3. See [:material-code-braces: OpportunityEngagementInvitationSortTypeDef](./type_defs.md#opportunityengagementinvitationsorttypedef) 
4. See [:material-code-brackets: InvitationStatusType](./literals.md#invitationstatustype) 
5. See [:material-code-braces: ListEngagementInvitationsResponseTypeDef](./type_defs.md#listengagementinvitationsresponsetypedef) 


```python
# list_engagement_invitations method usage example with argument unpacking

kwargs: ListEngagementInvitationsRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ParticipantType": ...,
}

parent.list_engagement_invitations(**kwargs)
```

1. See [:material-code-braces: ListEngagementInvitationsRequestRequestTypeDef](./type_defs.md#listengagementinvitationsrequestrequesttypedef) 

### list\_engagement\_members

Retrieves the details of member partners in an engagement.

Type annotations and code completion for `#!python session.client("partnercentral-selling").list_engagement_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# list_engagement_members method definition

await def list_engagement_members(
    self,
    *,
    Catalog: str,
    Identifier: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListEngagementMembersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEngagementMembersResponseTypeDef](./type_defs.md#listengagementmembersresponsetypedef) 


```python
# list_engagement_members method usage example with argument unpacking

kwargs: ListEngagementMembersRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "Identifier": ...,
}

parent.list_engagement_members(**kwargs)
```

1. See [:material-code-braces: ListEngagementMembersRequestRequestTypeDef](./type_defs.md#listengagementmembersrequestrequesttypedef) 

### list\_engagement\_resource\_associations

Lists the associations between resources and engagements where the caller is a
member and has at least one snapshot in the engagement.

Type annotations and code completion for `#!python session.client("partnercentral-selling").list_engagement_resource_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# list_engagement_resource_associations method definition

await def list_engagement_resource_associations(
    self,
    *,
    Catalog: str,
    CreatedBy: str = ...,
    EngagementIdentifier: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    ResourceIdentifier: str = ...,
    ResourceType: ResourceTypeType = ...,  # (1)
) -> ListEngagementResourceAssociationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ListEngagementResourceAssociationsResponseTypeDef](./type_defs.md#listengagementresourceassociationsresponsetypedef) 


```python
# list_engagement_resource_associations method usage example with argument unpacking

kwargs: ListEngagementResourceAssociationsRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
}

parent.list_engagement_resource_associations(**kwargs)
```

1. See [:material-code-braces: ListEngagementResourceAssociationsRequestRequestTypeDef](./type_defs.md#listengagementresourceassociationsrequestrequesttypedef) 

### list\_engagements

This action allows users to retrieve a list of engagement records from Partner
Central.

Type annotations and code completion for `#!python session.client("partnercentral-selling").list_engagements` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# list_engagements method definition

await def list_engagements(
    self,
    *,
    Catalog: str,
    CreatedBy: Sequence[str] = ...,
    EngagementIdentifier: Sequence[str] = ...,
    ExcludeCreatedBy: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    Sort: EngagementSortTypeDef = ...,  # (1)
) -> ListEngagementsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EngagementSortTypeDef](./type_defs.md#engagementsorttypedef) 
2. See [:material-code-braces: ListEngagementsResponseTypeDef](./type_defs.md#listengagementsresponsetypedef) 


```python
# list_engagements method usage example with argument unpacking

kwargs: ListEngagementsRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
}

parent.list_engagements(**kwargs)
```

1. See [:material-code-braces: ListEngagementsRequestRequestTypeDef](./type_defs.md#listengagementsrequestrequesttypedef) 

### list\_opportunities

This request accepts a list of filters that retrieve opportunity subsets as
well as sort options.

Type annotations and code completion for `#!python session.client("partnercentral-selling").list_opportunities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# list_opportunities method definition

await def list_opportunities(
    self,
    *,
    Catalog: str,
    CustomerCompanyName: Sequence[str] = ...,
    Identifier: Sequence[str] = ...,
    LastModifiedDate: LastModifiedDateTypeDef = ...,  # (1)
    LifeCycleReviewStatus: Sequence[ReviewStatusType] = ...,  # (2)
    LifeCycleStage: Sequence[StageType] = ...,  # (3)
    MaxResults: int = ...,
    NextToken: str = ...,
    Sort: OpportunitySortTypeDef = ...,  # (4)
) -> ListOpportunitiesResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: LastModifiedDateTypeDef](./type_defs.md#lastmodifieddatetypedef) 
2. See [:material-code-brackets: ReviewStatusType](./literals.md#reviewstatustype) 
3. See [:material-code-brackets: StageType](./literals.md#stagetype) 
4. See [:material-code-braces: OpportunitySortTypeDef](./type_defs.md#opportunitysorttypedef) 
5. See [:material-code-braces: ListOpportunitiesResponseTypeDef](./type_defs.md#listopportunitiesresponsetypedef) 


```python
# list_opportunities method usage example with argument unpacking

kwargs: ListOpportunitiesRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
}

parent.list_opportunities(**kwargs)
```

1. See [:material-code-braces: ListOpportunitiesRequestRequestTypeDef](./type_defs.md#listopportunitiesrequestrequesttypedef) 

### list\_resource\_snapshot\_jobs

Lists resource snapshot jobs owned by the customer.

Type annotations and code completion for `#!python session.client("partnercentral-selling").list_resource_snapshot_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# list_resource_snapshot_jobs method definition

await def list_resource_snapshot_jobs(
    self,
    *,
    Catalog: str,
    EngagementIdentifier: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    Sort: SortObjectTypeDef = ...,  # (1)
    Status: ResourceSnapshotJobStatusType = ...,  # (2)
) -> ListResourceSnapshotJobsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SortObjectTypeDef](./type_defs.md#sortobjecttypedef) 
2. See [:material-code-brackets: ResourceSnapshotJobStatusType](./literals.md#resourcesnapshotjobstatustype) 
3. See [:material-code-braces: ListResourceSnapshotJobsResponseTypeDef](./type_defs.md#listresourcesnapshotjobsresponsetypedef) 


```python
# list_resource_snapshot_jobs method usage example with argument unpacking

kwargs: ListResourceSnapshotJobsRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
}

parent.list_resource_snapshot_jobs(**kwargs)
```

1. See [:material-code-braces: ListResourceSnapshotJobsRequestRequestTypeDef](./type_defs.md#listresourcesnapshotjobsrequestrequesttypedef) 

### list\_resource\_snapshots

Retrieves a list of resource view snapshots based on specified criteria.

Type annotations and code completion for `#!python session.client("partnercentral-selling").list_resource_snapshots` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# list_resource_snapshots method definition

await def list_resource_snapshots(
    self,
    *,
    Catalog: str,
    EngagementIdentifier: str,
    CreatedBy: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    ResourceIdentifier: str = ...,
    ResourceSnapshotTemplateIdentifier: str = ...,
    ResourceType: ResourceTypeType = ...,  # (1)
) -> ListResourceSnapshotsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ListResourceSnapshotsResponseTypeDef](./type_defs.md#listresourcesnapshotsresponsetypedef) 


```python
# list_resource_snapshots method usage example with argument unpacking

kwargs: ListResourceSnapshotsRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "EngagementIdentifier": ...,
}

parent.list_resource_snapshots(**kwargs)
```

1. See [:material-code-braces: ListResourceSnapshotsRequestRequestTypeDef](./type_defs.md#listresourcesnapshotsrequestrequesttypedef) 

### list\_solutions

Retrieves a list of Partner Solutions that the partner registered on Partner
Central.

Type annotations and code completion for `#!python session.client("partnercentral-selling").list_solutions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# list_solutions method definition

await def list_solutions(
    self,
    *,
    Catalog: str,
    Category: Sequence[str] = ...,
    Identifier: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    Sort: SolutionSortTypeDef = ...,  # (1)
    Status: Sequence[SolutionStatusType] = ...,  # (2)
) -> ListSolutionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SolutionSortTypeDef](./type_defs.md#solutionsorttypedef) 
2. See [:material-code-brackets: SolutionStatusType](./literals.md#solutionstatustype) 
3. See [:material-code-braces: ListSolutionsResponseTypeDef](./type_defs.md#listsolutionsresponsetypedef) 


```python
# list_solutions method usage example with argument unpacking

kwargs: ListSolutionsRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
}

parent.list_solutions(**kwargs)
```

1. See [:material-code-braces: ListSolutionsRequestRequestTypeDef](./type_defs.md#listsolutionsrequestrequesttypedef) 

### put\_selling\_system\_settings

Updates the currently set system settings, which include the IAM Role used for
resource snapshot jobs.

Type annotations and code completion for `#!python session.client("partnercentral-selling").put_selling_system_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# put_selling_system_settings method definition

await def put_selling_system_settings(
    self,
    *,
    Catalog: str,
    ResourceSnapshotJobRoleIdentifier: str = ...,
) -> PutSellingSystemSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutSellingSystemSettingsResponseTypeDef](./type_defs.md#putsellingsystemsettingsresponsetypedef) 


```python
# put_selling_system_settings method usage example with argument unpacking

kwargs: PutSellingSystemSettingsRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
}

parent.put_selling_system_settings(**kwargs)
```

1. See [:material-code-braces: PutSellingSystemSettingsRequestRequestTypeDef](./type_defs.md#putsellingsystemsettingsrequestrequesttypedef) 

### reject\_engagement\_invitation

This action rejects an <code>EngagementInvitation</code> that AWS shared.

Type annotations and code completion for `#!python session.client("partnercentral-selling").reject_engagement_invitation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# reject_engagement_invitation method definition

await def reject_engagement_invitation(
    self,
    *,
    Catalog: str,
    Identifier: str,
    RejectionReason: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# reject_engagement_invitation method usage example with argument unpacking

kwargs: RejectEngagementInvitationRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "Identifier": ...,
}

parent.reject_engagement_invitation(**kwargs)
```

1. See [:material-code-braces: RejectEngagementInvitationRequestRequestTypeDef](./type_defs.md#rejectengagementinvitationrequestrequesttypedef) 

### start\_engagement\_by\_accepting\_invitation\_task

This action starts the engagement by accepting an
<code>EngagementInvitation</code>.

Type annotations and code completion for `#!python session.client("partnercentral-selling").start_engagement_by_accepting_invitation_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# start_engagement_by_accepting_invitation_task method definition

await def start_engagement_by_accepting_invitation_task(
    self,
    *,
    Catalog: str,
    ClientToken: str,
    Identifier: str,
) -> StartEngagementByAcceptingInvitationTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartEngagementByAcceptingInvitationTaskResponseTypeDef](./type_defs.md#startengagementbyacceptinginvitationtaskresponsetypedef) 


```python
# start_engagement_by_accepting_invitation_task method usage example with argument unpacking

kwargs: StartEngagementByAcceptingInvitationTaskRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ClientToken": ...,
    "Identifier": ...,
}

parent.start_engagement_by_accepting_invitation_task(**kwargs)
```

1. See [:material-code-braces: StartEngagementByAcceptingInvitationTaskRequestRequestTypeDef](./type_defs.md#startengagementbyacceptinginvitationtaskrequestrequesttypedef) 

### start\_engagement\_from\_opportunity\_task

This action initiates the engagement process from an existing opportunity by
accepting the engagement invitation and creating a corresponding opportunity in
the partner's system.

Type annotations and code completion for `#!python session.client("partnercentral-selling").start_engagement_from_opportunity_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# start_engagement_from_opportunity_task method definition

await def start_engagement_from_opportunity_task(
    self,
    *,
    AwsSubmission: AwsSubmissionTypeDef,  # (1)
    Catalog: str,
    ClientToken: str,
    Identifier: str,
) -> StartEngagementFromOpportunityTaskResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AwsSubmissionTypeDef](./type_defs.md#awssubmissiontypedef) 
2. See [:material-code-braces: StartEngagementFromOpportunityTaskResponseTypeDef](./type_defs.md#startengagementfromopportunitytaskresponsetypedef) 


```python
# start_engagement_from_opportunity_task method usage example with argument unpacking

kwargs: StartEngagementFromOpportunityTaskRequestRequestTypeDef = {  # (1)
    "AwsSubmission": ...,
    "Catalog": ...,
    "ClientToken": ...,
    "Identifier": ...,
}

parent.start_engagement_from_opportunity_task(**kwargs)
```

1. See [:material-code-braces: StartEngagementFromOpportunityTaskRequestRequestTypeDef](./type_defs.md#startengagementfromopportunitytaskrequestrequesttypedef) 

### start\_resource\_snapshot\_job

Starts a resource snapshot job that has been previously created.

Type annotations and code completion for `#!python session.client("partnercentral-selling").start_resource_snapshot_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# start_resource_snapshot_job method definition

await def start_resource_snapshot_job(
    self,
    *,
    Catalog: str,
    ResourceSnapshotJobIdentifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# start_resource_snapshot_job method usage example with argument unpacking

kwargs: StartResourceSnapshotJobRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ResourceSnapshotJobIdentifier": ...,
}

parent.start_resource_snapshot_job(**kwargs)
```

1. See [:material-code-braces: StartResourceSnapshotJobRequestRequestTypeDef](./type_defs.md#startresourcesnapshotjobrequestrequesttypedef) 

### stop\_resource\_snapshot\_job

Stops a resource snapshot job.

Type annotations and code completion for `#!python session.client("partnercentral-selling").stop_resource_snapshot_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# stop_resource_snapshot_job method definition

await def stop_resource_snapshot_job(
    self,
    *,
    Catalog: str,
    ResourceSnapshotJobIdentifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_resource_snapshot_job method usage example with argument unpacking

kwargs: StopResourceSnapshotJobRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ResourceSnapshotJobIdentifier": ...,
}

parent.stop_resource_snapshot_job(**kwargs)
```

1. See [:material-code-braces: StopResourceSnapshotJobRequestRequestTypeDef](./type_defs.md#stopresourcesnapshotjobrequestrequesttypedef) 

### submit\_opportunity

Use this action to submit an opportunity that was previously created by partner
for AWS review.

Type annotations and code completion for `#!python session.client("partnercentral-selling").submit_opportunity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# submit_opportunity method definition

await def submit_opportunity(
    self,
    *,
    Catalog: str,
    Identifier: str,
    InvolvementType: SalesInvolvementTypeType,  # (1)
    Visibility: VisibilityType = ...,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SalesInvolvementTypeType](./literals.md#salesinvolvementtypetype) 
2. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# submit_opportunity method usage example with argument unpacking

kwargs: SubmitOpportunityRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "Identifier": ...,
    "InvolvementType": ...,
}

parent.submit_opportunity(**kwargs)
```

1. See [:material-code-braces: SubmitOpportunityRequestRequestTypeDef](./type_defs.md#submitopportunityrequestrequesttypedef) 

### update\_opportunity

Updates the <code>Opportunity</code> record identified by a given
<code>Identifier</code>.

Type annotations and code completion for `#!python session.client("partnercentral-selling").update_opportunity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# update_opportunity method definition

await def update_opportunity(
    self,
    *,
    Catalog: str,
    Identifier: str,
    LastModifiedDate: TimestampTypeDef,
    Customer: CustomerTypeDef = ...,  # (1)
    LifeCycle: LifeCycleTypeDef = ...,  # (2)
    Marketing: MarketingTypeDef = ...,  # (3)
    NationalSecurity: NationalSecurityType = ...,  # (4)
    OpportunityType: OpportunityTypeType = ...,  # (5)
    PartnerOpportunityIdentifier: str = ...,
    PrimaryNeedsFromAws: Sequence[PrimaryNeedFromAwsType] = ...,  # (6)
    Project: ProjectTypeDef = ...,  # (7)
    SoftwareRevenue: SoftwareRevenueTypeDef = ...,  # (8)
) -> UpdateOpportunityResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: CustomerTypeDef](./type_defs.md#customertypedef) 
2. See [:material-code-braces: LifeCycleTypeDef](./type_defs.md#lifecycletypedef) 
3. See [:material-code-braces: MarketingTypeDef](./type_defs.md#marketingtypedef) 
4. See [:material-code-brackets: NationalSecurityType](./literals.md#nationalsecuritytype) 
5. See [:material-code-brackets: OpportunityTypeType](./literals.md#opportunitytypetype) 
6. See [:material-code-brackets: PrimaryNeedFromAwsType](./literals.md#primaryneedfromawstype) 
7. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
8. See [:material-code-braces: SoftwareRevenueTypeDef](./type_defs.md#softwarerevenuetypedef) 
9. See [:material-code-braces: UpdateOpportunityResponseTypeDef](./type_defs.md#updateopportunityresponsetypedef) 


```python
# update_opportunity method usage example with argument unpacking

kwargs: UpdateOpportunityRequestRequestTypeDef = {  # (1)
    "Catalog": ...,
    "Identifier": ...,
    "LastModifiedDate": ...,
}

parent.update_opportunity(**kwargs)
```

1. See [:material-code-braces: UpdateOpportunityRequestRequestTypeDef](./type_defs.md#updateopportunityrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("partnercentral-selling").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("partnercentral-selling").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

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

Type annotations and code completion for `#!python session.client("partnercentral-selling").get_paginator` method with overloads.

- `client.get_paginator("list_engagement_by_accepting_invitation_tasks")` -> [ListEngagementByAcceptingInvitationTasksPaginator](./paginators.md#listengagementbyacceptinginvitationtaskspaginator)
- `client.get_paginator("list_engagement_from_opportunity_tasks")` -> [ListEngagementFromOpportunityTasksPaginator](./paginators.md#listengagementfromopportunitytaskspaginator)
- `client.get_paginator("list_engagement_invitations")` -> [ListEngagementInvitationsPaginator](./paginators.md#listengagementinvitationspaginator)
- `client.get_paginator("list_engagement_members")` -> [ListEngagementMembersPaginator](./paginators.md#listengagementmemberspaginator)
- `client.get_paginator("list_engagement_resource_associations")` -> [ListEngagementResourceAssociationsPaginator](./paginators.md#listengagementresourceassociationspaginator)
- `client.get_paginator("list_engagements")` -> [ListEngagementsPaginator](./paginators.md#listengagementspaginator)
- `client.get_paginator("list_opportunities")` -> [ListOpportunitiesPaginator](./paginators.md#listopportunitiespaginator)
- `client.get_paginator("list_resource_snapshot_jobs")` -> [ListResourceSnapshotJobsPaginator](./paginators.md#listresourcesnapshotjobspaginator)
- `client.get_paginator("list_resource_snapshots")` -> [ListResourceSnapshotsPaginator](./paginators.md#listresourcesnapshotspaginator)
- `client.get_paginator("list_solutions")` -> [ListSolutionsPaginator](./paginators.md#listsolutionspaginator)


