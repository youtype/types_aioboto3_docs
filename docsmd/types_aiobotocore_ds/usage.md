# Examples

> [Index](../README.md) > [DirectoryService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DirectoryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#directoryservice)
    type annotations stubs module [types-aiobotocore-ds](https://pypi.org/project/types-aiobotocore-ds/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[ds]` package installed.

Write your `DirectoryService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# DirectoryServiceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("ds") as client:  # (1)
    result = await client.accept_shared_directory()  # (2)
```

1. client: [DirectoryServiceClient](./client.md)
2. result: [:material-code-braces: AcceptSharedDirectoryResultTypeDef](./type_defs.md#acceptshareddirectoryresulttypedef)



#### Paginator usage example

```python
# DescribeClientAuthenticationSettingsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("ds") as client:  # (1)
    paginator = client.get_paginator("describe_client_authentication_settings")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [DescribeClientAuthenticationSettingsPaginator](./paginators.md#describeclientauthenticationsettingspaginator)
3. item: [:material-code-braces: DescribeClientAuthenticationSettingsResultTypeDef](./type_defs.md#describeclientauthenticationsettingsresulttypedef)




### Explicit type annotations

With `types-aioboto3-lite[ds]`
or a standalone `types_aiobotocore_ds` package, you have to explicitly specify
`client: DirectoryServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# DirectoryServiceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ds.client import DirectoryServiceClient
from types_aiobotocore_ds.type_defs import AcceptSharedDirectoryResultTypeDef
from types_aiobotocore_ds.type_defs import AcceptSharedDirectoryRequestTypeDef


session = Session()

client: DirectoryServiceClient
async with session.client("ds") as client:  # (1)
    kwargs: AcceptSharedDirectoryRequestTypeDef = {...}  # (2)
    result: AcceptSharedDirectoryResultTypeDef = await client.accept_shared_directory(**kwargs)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. kwargs: [:material-code-braces: AcceptSharedDirectoryRequestTypeDef](./type_defs.md#acceptshareddirectoryrequesttypedef)
3. result: [:material-code-braces: AcceptSharedDirectoryResultTypeDef](./type_defs.md#acceptshareddirectoryresulttypedef)



#### Paginator usage example

```python
# DescribeClientAuthenticationSettingsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ds.client import DirectoryServiceClient
from types_aiobotocore_ds.paginator import DescribeClientAuthenticationSettingsPaginator
from types_aiobotocore_ds.type_defs import DescribeClientAuthenticationSettingsResultTypeDef


session = Session()

client: DirectoryServiceClient
async with session.client("ds") as client:  # (1)
    paginator: DescribeClientAuthenticationSettingsPaginator = client.get_paginator("describe_client_authentication_settings")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeClientAuthenticationSettingsResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [DescribeClientAuthenticationSettingsPaginator](./paginators.md#describeclientauthenticationsettingspaginator)
3. item: [:material-code-braces: DescribeClientAuthenticationSettingsResultTypeDef](./type_defs.md#describeclientauthenticationsettingsresulttypedef)




