# Examples

> [Index](../README.md) > [PartnerCentralSellingAPI](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PartnerCentralSellingAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#partnercentralsellingapi)
    type annotations stubs module [types-aiobotocore-partnercentral-selling](https://pypi.org/project/types-aiobotocore-partnercentral-selling/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[partnercentral-selling]` package installed.

Write your `PartnerCentralSellingAPI` code as usual,
type checking and code completion should work out of the box.



```python
# PartnerCentralSellingAPIClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("partnercentral-selling") as client:  # (1)
    result = await client.accept_engagement_invitation()  # (2)
```

1. client: [PartnerCentralSellingAPIClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# ListEngagementByAcceptingInvitationTasksPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("partnercentral-selling") as client:  # (1)
    paginator = client.get_paginator("list_engagement_by_accepting_invitation_tasks")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [PartnerCentralSellingAPIClient](./client.md)
2. paginator: [ListEngagementByAcceptingInvitationTasksPaginator](./paginators.md#listengagementbyacceptinginvitationtaskspaginator)
3. item: [:material-code-braces: ListEngagementByAcceptingInvitationTasksResponseTypeDef](./type_defs.md#listengagementbyacceptinginvitationtasksresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[partnercentral-selling]`
or a standalone `types_aiobotocore_partnercentral_selling` package, you have to explicitly specify
`client: PartnerCentralSellingAPIClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# PartnerCentralSellingAPIClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_partnercentral_selling.client import PartnerCentralSellingAPIClient
from types_aiobotocore_partnercentral_selling.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_partnercentral_selling.type_defs import AcceptEngagementInvitationRequestRequestTypeDef


session = Session()

client: PartnerCentralSellingAPIClient
async with session.client("partnercentral-selling") as client:  # (1)
    kwargs: AcceptEngagementInvitationRequestRequestTypeDef = {...}  # (2)
    result: EmptyResponseMetadataTypeDef = await client.accept_engagement_invitation(**kwargs)  # (3)
```

1. client: [PartnerCentralSellingAPIClient](./client.md)
2. kwargs: [:material-code-braces: AcceptEngagementInvitationRequestRequestTypeDef](./type_defs.md#acceptengagementinvitationrequestrequesttypedef) 
3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# ListEngagementByAcceptingInvitationTasksPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_partnercentral_selling.client import PartnerCentralSellingAPIClient
from types_aiobotocore_partnercentral_selling.paginator import ListEngagementByAcceptingInvitationTasksPaginator
from types_aiobotocore_partnercentral_selling.type_defs import ListEngagementByAcceptingInvitationTasksResponseTypeDef


session = Session()

client: PartnerCentralSellingAPIClient
async with session.client("partnercentral-selling") as client:  # (1)
    paginator: ListEngagementByAcceptingInvitationTasksPaginator = client.get_paginator("list_engagement_by_accepting_invitation_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: ListEngagementByAcceptingInvitationTasksResponseTypeDef
        print(item)  # (3)
```

1. client: [PartnerCentralSellingAPIClient](./client.md)
2. paginator: [ListEngagementByAcceptingInvitationTasksPaginator](./paginators.md#listengagementbyacceptinginvitationtaskspaginator)
3. item: [:material-code-braces: ListEngagementByAcceptingInvitationTasksResponseTypeDef](./type_defs.md#listengagementbyacceptinginvitationtasksresponsetypedef) 



