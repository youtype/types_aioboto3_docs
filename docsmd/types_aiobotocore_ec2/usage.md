# Examples

> [Index](../README.md) > [EC2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EC2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#ec2)
    type annotations stubs module [types-aiobotocore-ec2](https://pypi.org/project/types-aiobotocore-ec2/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[ec2]` package installed.

Write your `EC2` code as usual,
type checking and code completion should work out of the box.



```python
# EC2Client usage example

from aioboto3.session import Session


session = Session()

async with session.client("ec2") as client:  # (1)
    result = await client.accept_address_transfer()  # (2)
```

1. client: [EC2Client](./client.md)
2. result: [:material-code-braces: AcceptAddressTransferResultTypeDef](./type_defs.md#acceptaddresstransferresulttypedef) 



```python
# DescribeAddressTransfersPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("ec2") as client:  # (1)
    paginator = client.get_paginator("describe_address_transfers")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeAddressTransfersPaginator](./paginators.md#describeaddresstransferspaginator)
3. item: [:material-code-braces: DescribeAddressTransfersResultTypeDef](./type_defs.md#describeaddresstransfersresulttypedef) 



```python
# BundleTaskCompleteWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("ec2") as client:  # (1)
    waiter = client.get_waiter("bundle_task_complete")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [BundleTaskCompleteWaiter](./waiters.md#bundletaskcompletewaiter)


### Explicit type annotations

With `types-aioboto3-lite[ec2]`
or a standalone `types_aiobotocore_ec2` package, you have to explicitly specify
`client: EC2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# EC2Client usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ec2.client import EC2Client
from types_aiobotocore_ec2.type_defs import AcceptAddressTransferResultTypeDef
from types_aiobotocore_ec2.type_defs import AcceptAddressTransferRequestRequestTypeDef


session = Session()

client: EC2Client
async with session.client("ec2") as client:  # (1)
    kwargs: AcceptAddressTransferRequestRequestTypeDef = {...}  # (2)
    result: AcceptAddressTransferResultTypeDef = await client.accept_address_transfer(**kwargs)  # (3)
```

1. client: [EC2Client](./client.md)
2. kwargs: [:material-code-braces: AcceptAddressTransferRequestRequestTypeDef](./type_defs.md#acceptaddresstransferrequestrequesttypedef) 
3. result: [:material-code-braces: AcceptAddressTransferResultTypeDef](./type_defs.md#acceptaddresstransferresulttypedef) 



```python
# DescribeAddressTransfersPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ec2.client import EC2Client
from types_aiobotocore_ec2.paginator import DescribeAddressTransfersPaginator
from types_aiobotocore_ec2.type_defs import DescribeAddressTransfersResultTypeDef


session = Session()

client: EC2Client
async with session.client("ec2") as client:  # (1)
    paginator: DescribeAddressTransfersPaginator = client.get_paginator("describe_address_transfers")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAddressTransfersResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeAddressTransfersPaginator](./paginators.md#describeaddresstransferspaginator)
3. item: [:material-code-braces: DescribeAddressTransfersResultTypeDef](./type_defs.md#describeaddresstransfersresulttypedef) 



```python
# BundleTaskCompleteWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ec2.client import EC2Client
from types_aiobotocore_ec2.waiter import BundleTaskCompleteWaiter


session = Session()

async with session.client("ec2") as client:  # (1)
    waiter = client.get_waiter("bundle_task_complete")  # (2)
    await waiter.wait()
```

1. client: [EC2Client](./client.md)
2. waiter: [BundleTaskCompleteWaiter](./waiters.md#bundletaskcompletewaiter)



## Service Resource

### Implicit type annotations

Can be used with `types-aioboto3[ec2]` package installed.


```python
# EC2ServiceResource usage example

from aioboto3.session import Session


session = Session()

async with session.resource("ec2") as resource:  # (1)
    result = resource.get_available_subresources()  # (2)
```

1. resource: [EC2ServiceResource](./service_resource.md)
2. result: 



```python
# ServiceResourceClassicAddressesCollection usage example

from aioboto3.session import Session


session = Session()
resource = session.resource("ec2")  # (1)

collection = resource.classic_addresses  # (2)
for item in collection:
    print(item)  # (3)
```

1. resource: [EC2ServiceResource](./service_resource.md)
2. collection: [EC2ServiceResource](./service_resource.md#serviceresourceclassicaddressescollection)
3. item: ClassicAddress


### Explicit type annotations

With `types-aioboto3-lite[ec2]`
or a standalone `types_aiobotocore_ec2` package, you have to explicitly specify
`resource: EC2ServiceResource` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.



```python
# EC2ServiceResource usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ec2.service_resource import EC2ServiceResource
from types_aiobotocore_ec2.service_resource import get_available_subresources


session = Session()

resource: EC2ServiceResource
async with session.resource("ec2") as resource:  # (1)
    result: get_available_subresources = resource.get_available_subresources() # (2)
```

1. resource: [EC2ServiceResource](./service_resource.md)
2. result: 



```python
# ServiceResourceClassicAddressesCollection usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ec2.service_resource import EC2ServiceResource
from types_aiobotocore_ec2.service_resource import ServiceResourceClassicAddressesCollection
from types_aiobotocore_ec2.service_resource import ClassicAddress


session = Session()

resource: EC2ServiceResource
async with session.resource("ec2") as resource:  # (1)
    collection: ServiceResourceClassicAddressesCollection = resource.classic_addresses  # (2)
    for item in collection:
        item: ClassicAddress
        print(item)  # (3)
```

1. resource: [EC2ServiceResource](./service_resource.md)
2. collection: [EC2ServiceResource](./service_resource.md#serviceresourceclassicaddressescollection)
3. item: ClassicAddress
