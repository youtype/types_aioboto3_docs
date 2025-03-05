# Examples

> [Index](../README.md) > [Inspector](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Inspector](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#inspector)
    type annotations stubs module [types-aiobotocore-inspector](https://pypi.org/project/types-aiobotocore-inspector/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[inspector]` package installed.

Write your `Inspector` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# InspectorClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("inspector") as client:  # (1)
    result = await client.add_attributes_to_findings()  # (2)
```

1. client: [InspectorClient](./client.md)
2. result: [:material-code-braces: AddAttributesToFindingsResponseTypeDef](./type_defs.md#addattributestofindingsresponsetypedef)



#### Paginator usage example

```python
# ListAssessmentRunAgentsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("inspector") as client:  # (1)
    paginator = client.get_paginator("list_assessment_run_agents")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [ListAssessmentRunAgentsPaginator](./paginators.md#listassessmentrunagentspaginator)
3. item: [:material-code-braces: ListAssessmentRunAgentsResponseTypeDef](./type_defs.md#listassessmentrunagentsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[inspector]`
or a standalone `types_aiobotocore_inspector` package, you have to explicitly specify
`client: InspectorClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# InspectorClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_inspector.client import InspectorClient
from types_aiobotocore_inspector.type_defs import AddAttributesToFindingsResponseTypeDef
from types_aiobotocore_inspector.type_defs import AddAttributesToFindingsRequestTypeDef


session = Session()

client: InspectorClient
async with session.client("inspector") as client:  # (1)
    kwargs: AddAttributesToFindingsRequestTypeDef = {...}  # (2)
    result: AddAttributesToFindingsResponseTypeDef = await client.add_attributes_to_findings(**kwargs)  # (3)
```

1. client: [InspectorClient](./client.md)
2. kwargs: [:material-code-braces: AddAttributesToFindingsRequestTypeDef](./type_defs.md#addattributestofindingsrequesttypedef)
3. result: [:material-code-braces: AddAttributesToFindingsResponseTypeDef](./type_defs.md#addattributestofindingsresponsetypedef)



#### Paginator usage example

```python
# ListAssessmentRunAgentsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_inspector.client import InspectorClient
from types_aiobotocore_inspector.paginator import ListAssessmentRunAgentsPaginator
from types_aiobotocore_inspector.type_defs import ListAssessmentRunAgentsResponseTypeDef


session = Session()

client: InspectorClient
async with session.client("inspector") as client:  # (1)
    paginator: ListAssessmentRunAgentsPaginator = client.get_paginator("list_assessment_run_agents")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssessmentRunAgentsResponseTypeDef
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [ListAssessmentRunAgentsPaginator](./paginators.md#listassessmentrunagentspaginator)
3. item: [:material-code-braces: ListAssessmentRunAgentsResponseTypeDef](./type_defs.md#listassessmentrunagentsresponsetypedef)




