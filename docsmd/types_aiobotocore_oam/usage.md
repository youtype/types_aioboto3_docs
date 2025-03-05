# Examples

> [Index](../README.md) > [CloudWatchObservabilityAccessManager](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudWatchObservabilityAccessManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#cloudwatchobservabilityaccessmanager)
    type annotations stubs module [types-aiobotocore-oam](https://pypi.org/project/types-aiobotocore-oam/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[oam]` package installed.

Write your `CloudWatchObservabilityAccessManager` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# CloudWatchObservabilityAccessManagerClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("oam") as client:  # (1)
    result = await client.create_link()  # (2)
```

1. client: [CloudWatchObservabilityAccessManagerClient](./client.md)
2. result: [:material-code-braces: CreateLinkOutputTypeDef](./type_defs.md#createlinkoutputtypedef)



#### Paginator usage example

```python
# ListAttachedLinksPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("oam") as client:  # (1)
    paginator = client.get_paginator("list_attached_links")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudWatchObservabilityAccessManagerClient](./client.md)
2. paginator: [ListAttachedLinksPaginator](./paginators.md#listattachedlinkspaginator)
3. item: [:material-code-braces: ListAttachedLinksOutputTypeDef](./type_defs.md#listattachedlinksoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[oam]`
or a standalone `types_aiobotocore_oam` package, you have to explicitly specify
`client: CloudWatchObservabilityAccessManagerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# CloudWatchObservabilityAccessManagerClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_oam.client import CloudWatchObservabilityAccessManagerClient
from types_aiobotocore_oam.type_defs import CreateLinkOutputTypeDef
from types_aiobotocore_oam.type_defs import CreateLinkInputTypeDef


session = Session()

client: CloudWatchObservabilityAccessManagerClient
async with session.client("oam") as client:  # (1)
    kwargs: CreateLinkInputTypeDef = {...}  # (2)
    result: CreateLinkOutputTypeDef = await client.create_link(**kwargs)  # (3)
```

1. client: [CloudWatchObservabilityAccessManagerClient](./client.md)
2. kwargs: [:material-code-braces: CreateLinkInputTypeDef](./type_defs.md#createlinkinputtypedef)
3. result: [:material-code-braces: CreateLinkOutputTypeDef](./type_defs.md#createlinkoutputtypedef)



#### Paginator usage example

```python
# ListAttachedLinksPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_oam.client import CloudWatchObservabilityAccessManagerClient
from types_aiobotocore_oam.paginator import ListAttachedLinksPaginator
from types_aiobotocore_oam.type_defs import ListAttachedLinksOutputTypeDef


session = Session()

client: CloudWatchObservabilityAccessManagerClient
async with session.client("oam") as client:  # (1)
    paginator: ListAttachedLinksPaginator = client.get_paginator("list_attached_links")  # (2)
    async for item in paginator.paginate(...):
        item: ListAttachedLinksOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchObservabilityAccessManagerClient](./client.md)
2. paginator: [ListAttachedLinksPaginator](./paginators.md#listattachedlinkspaginator)
3. item: [:material-code-braces: ListAttachedLinksOutputTypeDef](./type_defs.md#listattachedlinksoutputtypedef)




