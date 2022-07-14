# Paginators

> [Index](../README.md) > [Inspector](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Inspector](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
    type annotations stubs module [types-aiobotocore-inspector](https://pypi.org/project/types-aiobotocore-inspector/).

## ListAssessmentRunAgentsPaginator

Type annotations and code completion for `#!python session.client("inspector").get_paginator("list_assessment_run_agents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRunAgents)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_inspector.paginator import ListAssessmentRunAgentsPaginator

session = Session()

session = get_session()
async with session.client("inspector") as client:  # (1)
    paginator: ListAssessmentRunAgentsPaginator = client.get_paginator("list_assessment_run_agents")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssessmentRunAgentsResponseTypeDef
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [ListAssessmentRunAgentsPaginator](./paginators.md#listassessmentrunagentspaginator)
3. item: [:material-code-braces: ListAssessmentRunAgentsResponseTypeDef](./type_defs.md#listassessmentrunagentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssessmentRunAgentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    assessmentRunArn: str,
    filter: AgentFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAssessmentRunAgentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: AgentFilterTypeDef](./type_defs.md#agentfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAssessmentRunAgentsResponseTypeDef](./type_defs.md#listassessmentrunagentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = {  # (1)
    "assessmentRunArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef](./type_defs.md#listassessmentrunagentsrequestlistassessmentrunagentspaginatetypedef) 
## ListAssessmentRunsPaginator

Type annotations and code completion for `#!python session.client("inspector").get_paginator("list_assessment_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRuns)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_inspector.paginator import ListAssessmentRunsPaginator

session = Session()

session = get_session()
async with session.client("inspector") as client:  # (1)
    paginator: ListAssessmentRunsPaginator = client.get_paginator("list_assessment_runs")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssessmentRunsResponseTypeDef
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [ListAssessmentRunsPaginator](./paginators.md#listassessmentrunspaginator)
3. item: [:material-code-braces: ListAssessmentRunsResponseTypeDef](./type_defs.md#listassessmentrunsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssessmentRunsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    assessmentTemplateArns: Sequence[str] = ...,
    filter: AssessmentRunFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAssessmentRunsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: AssessmentRunFilterTypeDef](./type_defs.md#assessmentrunfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAssessmentRunsResponseTypeDef](./type_defs.md#listassessmentrunsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef = {  # (1)
    "assessmentTemplateArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef](./type_defs.md#listassessmentrunsrequestlistassessmentrunspaginatetypedef) 
## ListAssessmentTargetsPaginator

Type annotations and code completion for `#!python session.client("inspector").get_paginator("list_assessment_targets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTargets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_inspector.paginator import ListAssessmentTargetsPaginator

session = Session()

session = get_session()
async with session.client("inspector") as client:  # (1)
    paginator: ListAssessmentTargetsPaginator = client.get_paginator("list_assessment_targets")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssessmentTargetsResponseTypeDef
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [ListAssessmentTargetsPaginator](./paginators.md#listassessmenttargetspaginator)
3. item: [:material-code-braces: ListAssessmentTargetsResponseTypeDef](./type_defs.md#listassessmenttargetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssessmentTargetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filter: AssessmentTargetFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAssessmentTargetsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: AssessmentTargetFilterTypeDef](./type_defs.md#assessmenttargetfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAssessmentTargetsResponseTypeDef](./type_defs.md#listassessmenttargetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef = {  # (1)
    "filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef](./type_defs.md#listassessmenttargetsrequestlistassessmenttargetspaginatetypedef) 
## ListAssessmentTemplatesPaginator

Type annotations and code completion for `#!python session.client("inspector").get_paginator("list_assessment_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTemplates)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_inspector.paginator import ListAssessmentTemplatesPaginator

session = Session()

session = get_session()
async with session.client("inspector") as client:  # (1)
    paginator: ListAssessmentTemplatesPaginator = client.get_paginator("list_assessment_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssessmentTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [ListAssessmentTemplatesPaginator](./paginators.md#listassessmenttemplatespaginator)
3. item: [:material-code-braces: ListAssessmentTemplatesResponseTypeDef](./type_defs.md#listassessmenttemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssessmentTemplatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    assessmentTargetArns: Sequence[str] = ...,
    filter: AssessmentTemplateFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAssessmentTemplatesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: AssessmentTemplateFilterTypeDef](./type_defs.md#assessmenttemplatefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAssessmentTemplatesResponseTypeDef](./type_defs.md#listassessmenttemplatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef = {  # (1)
    "assessmentTargetArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef](./type_defs.md#listassessmenttemplatesrequestlistassessmenttemplatespaginatetypedef) 
## ListEventSubscriptionsPaginator

Type annotations and code completion for `#!python session.client("inspector").get_paginator("list_event_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListEventSubscriptions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_inspector.paginator import ListEventSubscriptionsPaginator

session = Session()

session = get_session()
async with session.client("inspector") as client:  # (1)
    paginator: ListEventSubscriptionsPaginator = client.get_paginator("list_event_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventSubscriptionsResponseTypeDef
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [ListEventSubscriptionsPaginator](./paginators.md#listeventsubscriptionspaginator)
3. item: [:material-code-braces: ListEventSubscriptionsResponseTypeDef](./type_defs.md#listeventsubscriptionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEventSubscriptionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    resourceArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEventSubscriptionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEventSubscriptionsResponseTypeDef](./type_defs.md#listeventsubscriptionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef](./type_defs.md#listeventsubscriptionsrequestlisteventsubscriptionspaginatetypedef) 
## ListExclusionsPaginator

Type annotations and code completion for `#!python session.client("inspector").get_paginator("list_exclusions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListExclusions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_inspector.paginator import ListExclusionsPaginator

session = Session()

session = get_session()
async with session.client("inspector") as client:  # (1)
    paginator: ListExclusionsPaginator = client.get_paginator("list_exclusions")  # (2)
    async for item in paginator.paginate(...):
        item: ListExclusionsResponseTypeDef
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [ListExclusionsPaginator](./paginators.md#listexclusionspaginator)
3. item: [:material-code-braces: ListExclusionsResponseTypeDef](./type_defs.md#listexclusionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListExclusionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    assessmentRunArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListExclusionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListExclusionsResponseTypeDef](./type_defs.md#listexclusionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListExclusionsRequestListExclusionsPaginateTypeDef = {  # (1)
    "assessmentRunArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExclusionsRequestListExclusionsPaginateTypeDef](./type_defs.md#listexclusionsrequestlistexclusionspaginatetypedef) 
## ListFindingsPaginator

Type annotations and code completion for `#!python session.client("inspector").get_paginator("list_findings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListFindings)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_inspector.paginator import ListFindingsPaginator

session = Session()

session = get_session()
async with session.client("inspector") as client:  # (1)
    paginator: ListFindingsPaginator = client.get_paginator("list_findings")  # (2)
    async for item in paginator.paginate(...):
        item: ListFindingsResponseTypeDef
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [ListFindingsPaginator](./paginators.md#listfindingspaginator)
3. item: [:material-code-braces: ListFindingsResponseTypeDef](./type_defs.md#listfindingsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFindingsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    assessmentRunArns: Sequence[str] = ...,
    filter: FindingFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListFindingsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FindingFilterTypeDef](./type_defs.md#findingfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListFindingsResponseTypeDef](./type_defs.md#listfindingsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListFindingsRequestListFindingsPaginateTypeDef = {  # (1)
    "assessmentRunArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFindingsRequestListFindingsPaginateTypeDef](./type_defs.md#listfindingsrequestlistfindingspaginatetypedef) 
## ListRulesPackagesPaginator

Type annotations and code completion for `#!python session.client("inspector").get_paginator("list_rules_packages")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListRulesPackages)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_inspector.paginator import ListRulesPackagesPaginator

session = Session()

session = get_session()
async with session.client("inspector") as client:  # (1)
    paginator: ListRulesPackagesPaginator = client.get_paginator("list_rules_packages")  # (2)
    async for item in paginator.paginate(...):
        item: ListRulesPackagesResponseTypeDef
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [ListRulesPackagesPaginator](./paginators.md#listrulespackagespaginator)
3. item: [:material-code-braces: ListRulesPackagesResponseTypeDef](./type_defs.md#listrulespackagesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRulesPackagesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRulesPackagesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRulesPackagesResponseTypeDef](./type_defs.md#listrulespackagesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRulesPackagesRequestListRulesPackagesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRulesPackagesRequestListRulesPackagesPaginateTypeDef](./type_defs.md#listrulespackagesrequestlistrulespackagespaginatetypedef) 
## PreviewAgentsPaginator

Type annotations and code completion for `#!python session.client("inspector").get_paginator("preview_agents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.PreviewAgents)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_inspector.paginator import PreviewAgentsPaginator

session = Session()

session = get_session()
async with session.client("inspector") as client:  # (1)
    paginator: PreviewAgentsPaginator = client.get_paginator("preview_agents")  # (2)
    async for item in paginator.paginate(...):
        item: PreviewAgentsResponseTypeDef
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [PreviewAgentsPaginator](./paginators.md#previewagentspaginator)
3. item: [:material-code-braces: PreviewAgentsResponseTypeDef](./type_defs.md#previewagentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python PreviewAgentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    previewAgentsArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[PreviewAgentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: PreviewAgentsResponseTypeDef](./type_defs.md#previewagentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: PreviewAgentsRequestPreviewAgentsPaginateTypeDef = {  # (1)
    "previewAgentsArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: PreviewAgentsRequestPreviewAgentsPaginateTypeDef](./type_defs.md#previewagentsrequestpreviewagentspaginatetypedef) 
