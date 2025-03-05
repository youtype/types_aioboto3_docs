# Examples

> [Index](../README.md) > [ConnectCampaignService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ConnectCampaignService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#connectcampaignservice)
    type annotations stubs module [types-aiobotocore-connectcampaigns](https://pypi.org/project/types-aiobotocore-connectcampaigns/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[connectcampaigns]` package installed.

Write your `ConnectCampaignService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ConnectCampaignServiceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("connectcampaigns") as client:  # (1)
    result = await client.create_campaign()  # (2)
```

1. client: [ConnectCampaignServiceClient](./client.md)
2. result: [:material-code-braces: CreateCampaignResponseTypeDef](./type_defs.md#createcampaignresponsetypedef)



#### Paginator usage example

```python
# ListCampaignsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("connectcampaigns") as client:  # (1)
    paginator = client.get_paginator("list_campaigns")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ConnectCampaignServiceClient](./client.md)
2. paginator: [ListCampaignsPaginator](./paginators.md#listcampaignspaginator)
3. item: [:material-code-braces: ListCampaignsResponseTypeDef](./type_defs.md#listcampaignsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[connectcampaigns]`
or a standalone `types_aiobotocore_connectcampaigns` package, you have to explicitly specify
`client: ConnectCampaignServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ConnectCampaignServiceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_connectcampaigns.client import ConnectCampaignServiceClient
from types_aiobotocore_connectcampaigns.type_defs import CreateCampaignResponseTypeDef
from types_aiobotocore_connectcampaigns.type_defs import CreateCampaignRequestTypeDef


session = Session()

client: ConnectCampaignServiceClient
async with session.client("connectcampaigns") as client:  # (1)
    kwargs: CreateCampaignRequestTypeDef = {...}  # (2)
    result: CreateCampaignResponseTypeDef = await client.create_campaign(**kwargs)  # (3)
```

1. client: [ConnectCampaignServiceClient](./client.md)
2. kwargs: [:material-code-braces: CreateCampaignRequestTypeDef](./type_defs.md#createcampaignrequesttypedef)
3. result: [:material-code-braces: CreateCampaignResponseTypeDef](./type_defs.md#createcampaignresponsetypedef)



#### Paginator usage example

```python
# ListCampaignsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_connectcampaigns.client import ConnectCampaignServiceClient
from types_aiobotocore_connectcampaigns.paginator import ListCampaignsPaginator
from types_aiobotocore_connectcampaigns.type_defs import ListCampaignsResponseTypeDef


session = Session()

client: ConnectCampaignServiceClient
async with session.client("connectcampaigns") as client:  # (1)
    paginator: ListCampaignsPaginator = client.get_paginator("list_campaigns")  # (2)
    async for item in paginator.paginate(...):
        item: ListCampaignsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectCampaignServiceClient](./client.md)
2. paginator: [ListCampaignsPaginator](./paginators.md#listcampaignspaginator)
3. item: [:material-code-braces: ListCampaignsResponseTypeDef](./type_defs.md#listcampaignsresponsetypedef)




