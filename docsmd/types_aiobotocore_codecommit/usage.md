# Examples

> [Index](../README.md) > [CodeCommit](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodeCommit](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#codecommit)
    type annotations stubs module [types-aiobotocore-codecommit](https://pypi.org/project/types-aiobotocore-codecommit/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[codecommit]` package installed.

Write your `CodeCommit` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# CodeCommitClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("codecommit") as client:  # (1)
    result = await client.associate_approval_rule_template_with_repository()  # (2)
```

1. client: [CodeCommitClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# DescribePullRequestEventsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("codecommit") as client:  # (1)
    paginator = client.get_paginator("describe_pull_request_events")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CodeCommitClient](./client.md)
2. paginator: [DescribePullRequestEventsPaginator](./paginators.md#describepullrequesteventspaginator)
3. item: [:material-code-braces: DescribePullRequestEventsOutputTypeDef](./type_defs.md#describepullrequesteventsoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[codecommit]`
or a standalone `types_aiobotocore_codecommit` package, you have to explicitly specify
`client: CodeCommitClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# CodeCommitClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_codecommit.client import CodeCommitClient
from types_aiobotocore_codecommit.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_codecommit.type_defs import AssociateApprovalRuleTemplateWithRepositoryInputTypeDef


session = Session()

client: CodeCommitClient
async with session.client("codecommit") as client:  # (1)
    kwargs: AssociateApprovalRuleTemplateWithRepositoryInputTypeDef = {...}  # (2)
    result: EmptyResponseMetadataTypeDef = await client.associate_approval_rule_template_with_repository(**kwargs)  # (3)
```

1. client: [CodeCommitClient](./client.md)
2. kwargs: [:material-code-braces: AssociateApprovalRuleTemplateWithRepositoryInputTypeDef](./type_defs.md#associateapprovalruletemplatewithrepositoryinputtypedef)
3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# DescribePullRequestEventsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_codecommit.client import CodeCommitClient
from types_aiobotocore_codecommit.paginator import DescribePullRequestEventsPaginator
from types_aiobotocore_codecommit.type_defs import DescribePullRequestEventsOutputTypeDef


session = Session()

client: CodeCommitClient
async with session.client("codecommit") as client:  # (1)
    paginator: DescribePullRequestEventsPaginator = client.get_paginator("describe_pull_request_events")  # (2)
    async for item in paginator.paginate(...):
        item: DescribePullRequestEventsOutputTypeDef
        print(item)  # (3)
```

1. client: [CodeCommitClient](./client.md)
2. paginator: [DescribePullRequestEventsPaginator](./paginators.md#describepullrequesteventspaginator)
3. item: [:material-code-braces: DescribePullRequestEventsOutputTypeDef](./type_defs.md#describepullrequesteventsoutputtypedef)




