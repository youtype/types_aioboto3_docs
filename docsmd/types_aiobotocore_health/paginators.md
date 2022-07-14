# Paginators

> [Index](../README.md) > [Health](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Health](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
    type annotations stubs module [types-aiobotocore-health](https://pypi.org/project/types-aiobotocore-health/).

## DescribeAffectedAccountsForOrganizationPaginator

Type annotations and code completion for `#!python session.client("health").get_paginator("describe_affected_accounts_for_organization")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedAccountsForOrganization)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_health.paginator import DescribeAffectedAccountsForOrganizationPaginator

session = Session()

session = get_session()
async with session.client("health") as client:  # (1)
    paginator: DescribeAffectedAccountsForOrganizationPaginator = client.get_paginator("describe_affected_accounts_for_organization")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAffectedAccountsForOrganizationResponseTypeDef
        print(item)  # (3)
```

1. client: [HealthClient](./client.md)
2. paginator: [DescribeAffectedAccountsForOrganizationPaginator](./paginators.md#describeaffectedaccountsfororganizationpaginator)
3. item: [:material-code-braces: DescribeAffectedAccountsForOrganizationResponseTypeDef](./type_defs.md#describeaffectedaccountsfororganizationresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAffectedAccountsForOrganizationPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    eventArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeAffectedAccountsForOrganizationResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeAffectedAccountsForOrganizationResponseTypeDef](./type_defs.md#describeaffectedaccountsfororganizationresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = {  # (1)
    "eventArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef](./type_defs.md#describeaffectedaccountsfororganizationrequestdescribeaffectedaccountsfororganizationpaginatetypedef) 
## DescribeAffectedEntitiesPaginator

Type annotations and code completion for `#!python session.client("health").get_paginator("describe_affected_entities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedEntities)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_health.paginator import DescribeAffectedEntitiesPaginator

session = Session()

session = get_session()
async with session.client("health") as client:  # (1)
    paginator: DescribeAffectedEntitiesPaginator = client.get_paginator("describe_affected_entities")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAffectedEntitiesResponseTypeDef
        print(item)  # (3)
```

1. client: [HealthClient](./client.md)
2. paginator: [DescribeAffectedEntitiesPaginator](./paginators.md#describeaffectedentitiespaginator)
3. item: [:material-code-braces: DescribeAffectedEntitiesResponseTypeDef](./type_defs.md#describeaffectedentitiesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAffectedEntitiesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filter: EntityFilterTypeDef,  # (1)
    locale: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeAffectedEntitiesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: EntityFilterTypeDef](./type_defs.md#entityfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeAffectedEntitiesResponseTypeDef](./type_defs.md#describeaffectedentitiesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef = {  # (1)
    "filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef](./type_defs.md#describeaffectedentitiesrequestdescribeaffectedentitiespaginatetypedef) 
## DescribeAffectedEntitiesForOrganizationPaginator

Type annotations and code completion for `#!python session.client("health").get_paginator("describe_affected_entities_for_organization")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedEntitiesForOrganization)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_health.paginator import DescribeAffectedEntitiesForOrganizationPaginator

session = Session()

session = get_session()
async with session.client("health") as client:  # (1)
    paginator: DescribeAffectedEntitiesForOrganizationPaginator = client.get_paginator("describe_affected_entities_for_organization")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAffectedEntitiesForOrganizationResponseTypeDef
        print(item)  # (3)
```

1. client: [HealthClient](./client.md)
2. paginator: [DescribeAffectedEntitiesForOrganizationPaginator](./paginators.md#describeaffectedentitiesfororganizationpaginator)
3. item: [:material-code-braces: DescribeAffectedEntitiesForOrganizationResponseTypeDef](./type_defs.md#describeaffectedentitiesfororganizationresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAffectedEntitiesForOrganizationPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    organizationEntityFilters: Sequence[EventAccountFilterTypeDef],  # (1)
    locale: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeAffectedEntitiesForOrganizationResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: EventAccountFilterTypeDef](./type_defs.md#eventaccountfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeAffectedEntitiesForOrganizationResponseTypeDef](./type_defs.md#describeaffectedentitiesfororganizationresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef = {  # (1)
    "organizationEntityFilters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef](./type_defs.md#describeaffectedentitiesfororganizationrequestdescribeaffectedentitiesfororganizationpaginatetypedef) 
## DescribeEventAggregatesPaginator

Type annotations and code completion for `#!python session.client("health").get_paginator("describe_event_aggregates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventAggregates)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_health.paginator import DescribeEventAggregatesPaginator

session = Session()

session = get_session()
async with session.client("health") as client:  # (1)
    paginator: DescribeEventAggregatesPaginator = client.get_paginator("describe_event_aggregates")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEventAggregatesResponseTypeDef
        print(item)  # (3)
```

1. client: [HealthClient](./client.md)
2. paginator: [DescribeEventAggregatesPaginator](./paginators.md#describeeventaggregatespaginator)
3. item: [:material-code-braces: DescribeEventAggregatesResponseTypeDef](./type_defs.md#describeeventaggregatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEventAggregatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    aggregateField: eventAggregateFieldType,  # (1)
    filter: EventFilterTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[DescribeEventAggregatesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: eventAggregateFieldType](./literals.md#eventaggregatefieldtype) 
2. See [:material-code-braces: EventFilterTypeDef](./type_defs.md#eventfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeEventAggregatesResponseTypeDef](./type_defs.md#describeeventaggregatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef = {  # (1)
    "aggregateField": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef](./type_defs.md#describeeventaggregatesrequestdescribeeventaggregatespaginatetypedef) 
## DescribeEventTypesPaginator

Type annotations and code completion for `#!python session.client("health").get_paginator("describe_event_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventTypes)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_health.paginator import DescribeEventTypesPaginator

session = Session()

session = get_session()
async with session.client("health") as client:  # (1)
    paginator: DescribeEventTypesPaginator = client.get_paginator("describe_event_types")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEventTypesResponseTypeDef
        print(item)  # (3)
```

1. client: [HealthClient](./client.md)
2. paginator: [DescribeEventTypesPaginator](./paginators.md#describeeventtypespaginator)
3. item: [:material-code-braces: DescribeEventTypesResponseTypeDef](./type_defs.md#describeeventtypesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEventTypesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filter: EventTypeFilterTypeDef = ...,  # (1)
    locale: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeEventTypesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: EventTypeFilterTypeDef](./type_defs.md#eventtypefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeEventTypesResponseTypeDef](./type_defs.md#describeeventtypesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef = {  # (1)
    "filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef](./type_defs.md#describeeventtypesrequestdescribeeventtypespaginatetypedef) 
## DescribeEventsPaginator

Type annotations and code completion for `#!python session.client("health").get_paginator("describe_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEvents)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_health.paginator import DescribeEventsPaginator

session = Session()

session = get_session()
async with session.client("health") as client:  # (1)
    paginator: DescribeEventsPaginator = client.get_paginator("describe_events")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEventsResponseTypeDef
        print(item)  # (3)
```

1. client: [HealthClient](./client.md)
2. paginator: [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
3. item: [:material-code-braces: DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEventsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filter: EventFilterTypeDef = ...,  # (1)
    locale: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeEventsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: EventFilterTypeDef](./type_defs.md#eventfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEventsRequestDescribeEventsPaginateTypeDef = {  # (1)
    "filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventsRequestDescribeEventsPaginateTypeDef](./type_defs.md#describeeventsrequestdescribeeventspaginatetypedef) 
## DescribeEventsForOrganizationPaginator

Type annotations and code completion for `#!python session.client("health").get_paginator("describe_events_for_organization")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventsForOrganization)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_health.paginator import DescribeEventsForOrganizationPaginator

session = Session()

session = get_session()
async with session.client("health") as client:  # (1)
    paginator: DescribeEventsForOrganizationPaginator = client.get_paginator("describe_events_for_organization")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEventsForOrganizationResponseTypeDef
        print(item)  # (3)
```

1. client: [HealthClient](./client.md)
2. paginator: [DescribeEventsForOrganizationPaginator](./paginators.md#describeeventsfororganizationpaginator)
3. item: [:material-code-braces: DescribeEventsForOrganizationResponseTypeDef](./type_defs.md#describeeventsfororganizationresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEventsForOrganizationPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filter: OrganizationEventFilterTypeDef = ...,  # (1)
    locale: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeEventsForOrganizationResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: OrganizationEventFilterTypeDef](./type_defs.md#organizationeventfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeEventsForOrganizationResponseTypeDef](./type_defs.md#describeeventsfororganizationresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef = {  # (1)
    "filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef](./type_defs.md#describeeventsfororganizationrequestdescribeeventsfororganizationpaginatetypedef) 
