# Examples

> [Index](../README.md) > [CodeDeploy](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodeDeploy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#codedeploy)
    type annotations stubs module [types-aiobotocore-codedeploy](https://pypi.org/project/types-aiobotocore-codedeploy/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[codedeploy]` package installed.

Write your `CodeDeploy` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# CodeDeployClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("codedeploy") as client:  # (1)
    result = await client.add_tags_to_on_premises_instances()  # (2)
```

1. client: [CodeDeployClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# ListApplicationRevisionsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("codedeploy") as client:  # (1)
    paginator = client.get_paginator("list_application_revisions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CodeDeployClient](./client.md)
2. paginator: [ListApplicationRevisionsPaginator](./paginators.md#listapplicationrevisionspaginator)
3. item: [:material-code-braces: ListApplicationRevisionsOutputTypeDef](./type_defs.md#listapplicationrevisionsoutputtypedef)



#### Waiter usage example

```python
# DeploymentSuccessfulWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("codedeploy") as client:  # (1)
    waiter = client.get_waiter("deployment_successful")  # (2)
    await waiter.wait(...)
```

1. client: [CodeDeployClient](./client.md)
2. waiter: [DeploymentSuccessfulWaiter](./waiters.md#deploymentsuccessfulwaiter)


### Explicit type annotations

With `types-aioboto3-lite[codedeploy]`
or a standalone `types_aiobotocore_codedeploy` package, you have to explicitly specify
`client: CodeDeployClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# CodeDeployClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_codedeploy.client import CodeDeployClient
from types_aiobotocore_codedeploy.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_codedeploy.type_defs import AddTagsToOnPremisesInstancesInputTypeDef


session = Session()

client: CodeDeployClient
async with session.client("codedeploy") as client:  # (1)
    kwargs: AddTagsToOnPremisesInstancesInputTypeDef = {...}  # (2)
    result: EmptyResponseMetadataTypeDef = await client.add_tags_to_on_premises_instances(**kwargs)  # (3)
```

1. client: [CodeDeployClient](./client.md)
2. kwargs: [:material-code-braces: AddTagsToOnPremisesInstancesInputTypeDef](./type_defs.md#addtagstoonpremisesinstancesinputtypedef)
3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# ListApplicationRevisionsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_codedeploy.client import CodeDeployClient
from types_aiobotocore_codedeploy.paginator import ListApplicationRevisionsPaginator
from types_aiobotocore_codedeploy.type_defs import ListApplicationRevisionsOutputTypeDef


session = Session()

client: CodeDeployClient
async with session.client("codedeploy") as client:  # (1)
    paginator: ListApplicationRevisionsPaginator = client.get_paginator("list_application_revisions")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationRevisionsOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeDeployClient](./client.md)
2. paginator: [ListApplicationRevisionsPaginator](./paginators.md#listapplicationrevisionspaginator)
3. item: [:material-code-braces: ListApplicationRevisionsOutputTypeDef](./type_defs.md#listapplicationrevisionsoutputtypedef)



#### Waiter usage example

```python
# DeploymentSuccessfulWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_codedeploy.client import CodeDeployClient
from types_aiobotocore_codedeploy.waiter import DeploymentSuccessfulWaiter


session = Session()

async with session.client("codedeploy") as client:  # (1)
    waiter = client.get_waiter("deployment_successful")  # (2)
    await waiter.wait(...)
```

1. client: [CodeDeployClient](./client.md)
2. waiter: [DeploymentSuccessfulWaiter](./waiters.md#deploymentsuccessfulwaiter)


