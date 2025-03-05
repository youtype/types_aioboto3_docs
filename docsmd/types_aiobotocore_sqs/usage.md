# Examples

> [Index](../README.md) > [SQS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SQS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#sqs)
    type annotations stubs module [types-aiobotocore-sqs](https://pypi.org/project/types-aiobotocore-sqs/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[sqs]` package installed.

Write your `SQS` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SQSClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("sqs") as client:  # (1)
    result = await client.add_permission()  # (2)
```

1. client: [SQSClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# ListDeadLetterSourceQueuesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("sqs") as client:  # (1)
    paginator = client.get_paginator("list_dead_letter_source_queues")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SQSClient](./client.md)
2. paginator: [ListDeadLetterSourceQueuesPaginator](./paginators.md#listdeadlettersourcequeuespaginator)
3. item: [:material-code-braces: ListDeadLetterSourceQueuesResultTypeDef](./type_defs.md#listdeadlettersourcequeuesresulttypedef)




### Explicit type annotations

With `types-aioboto3-lite[sqs]`
or a standalone `types_aiobotocore_sqs` package, you have to explicitly specify
`client: SQSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SQSClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_sqs.client import SQSClient
from types_aiobotocore_sqs.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_sqs.type_defs import AddPermissionRequestTypeDef


session = Session()

client: SQSClient
async with session.client("sqs") as client:  # (1)
    kwargs: AddPermissionRequestTypeDef = {...}  # (2)
    result: EmptyResponseMetadataTypeDef = await client.add_permission(**kwargs)  # (3)
```

1. client: [SQSClient](./client.md)
2. kwargs: [:material-code-braces: AddPermissionRequestTypeDef](./type_defs.md#addpermissionrequesttypedef)
3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# ListDeadLetterSourceQueuesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_sqs.client import SQSClient
from types_aiobotocore_sqs.paginator import ListDeadLetterSourceQueuesPaginator
from types_aiobotocore_sqs.type_defs import ListDeadLetterSourceQueuesResultTypeDef


session = Session()

client: SQSClient
async with session.client("sqs") as client:  # (1)
    paginator: ListDeadLetterSourceQueuesPaginator = client.get_paginator("list_dead_letter_source_queues")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeadLetterSourceQueuesResultTypeDef
        print(item)  # (3)
```

1. client: [SQSClient](./client.md)
2. paginator: [ListDeadLetterSourceQueuesPaginator](./paginators.md#listdeadlettersourcequeuespaginator)
3. item: [:material-code-braces: ListDeadLetterSourceQueuesResultTypeDef](./type_defs.md#listdeadlettersourcequeuesresulttypedef)





## Service Resource

### Implicit type annotations

Can be used with `types-aioboto3[sqs]` package installed.


#### ServiceResource method usage example

```python
# SQSServiceResource usage example

from aioboto3.session import Session


session = Session()

async with session.resource("sqs") as resource:  # (1)
    result = await resource.create_queue(...)  # (2)
```

1. resource: [SQSServiceResource](./service_resource.md)
2. result: [Queue](./service_resource.md#queue)



#### Collection usage example

```python
# ServiceResourceQueuesCollection usage example

from aioboto3.session import Session


session = Session()

async with session.resource("sqs") as resource:  # (1)
    collection = resource.queues  # (2)
    async for item in collection:
        print(item)  # (3)
```

1. resource: [SQSServiceResource](./service_resource.md)
2. collection: [ServiceResourceQueuesCollection](./service_resource.md#serviceresourcequeuescollection)
3. item: [Queue](./service_resource.md#queue)


### Explicit type annotations

With `types-aioboto3-lite[sqs]`
or a standalone `types_aiobotocore_sqs` package, you have to explicitly specify
`resource: SQSServiceResource` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.



#### ServiceResource method usage example

```python
# SQSServiceResource usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_sqs.service_resource import SQSServiceResource
from types_aiobotocore_sqs.service_resource import Queue
from types_aiobotocore_sqs.type_defs import CreateQueueRequestServiceResourceCreateQueueTypeDef


session = Session()

resource: SQSServiceResource
async with session.resource("sqs") as resource:  # (1)
    kwargs: CreateQueueRequestServiceResourceCreateQueueTypeDef = {...}  # (2)
    result: Queue = await resource.create_queue(...) # (3)
```

1. resource: [SQSServiceResource](./service_resource.md)
2. kwargs: [:material-code-braces: CreateQueueRequestServiceResourceCreateQueueTypeDef](./type_defs.md#createqueuerequestserviceresourcecreatequeuetypedef)
3. result: [Queue](./service_resource.md#queue)



#### Collection usage example

```python
# ServiceResourceQueuesCollection usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_sqs.service_resource import SQSServiceResource
from types_aiobotocore_sqs.service_resource import ServiceResourceQueuesCollection
from types_aiobotocore_sqs.service_resource import Queue


session = Session()

resource: SQSServiceResource
async with session.resource("sqs") as resource:  # (1)
    collection: ServiceResourceQueuesCollection = resource.queues  # (2)
    async for item in collection:
        item: Queue
        print(item)  # (3)
```

1. resource: [SQSServiceResource](./service_resource.md)
2. collection: [SQSServiceResource](./service_resource.md#serviceresourcequeuescollection)
3. item: Queue

