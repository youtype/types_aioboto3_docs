# HealthClient

> [Index](../README.md) > [Health](./README.md) > HealthClient

!!! note ""

    Auto-generated documentation for [Health](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#health)
    type annotations stubs module [types-aiobotocore-health](https://pypi.org/project/types-aiobotocore-health/).

## HealthClient

Type annotations and code completion for `#!python session.client("health")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

```python
# HealthClient usage example

from aioboto3.session import Session
from types_aiobotocore_health.client import HealthClient

session = Session()
async with session.client("health") as client:
    client: HealthClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("health").exceptions` structure.

```python
# HealthClient.exceptions usage example

async with session.client("health") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.ConcurrentModificationException,
        client.exceptions.InvalidPaginationToken,
        client.exceptions.UnsupportedLocale,
    ) as e:
        print(e)
```

```python
# HealthClient.exceptions type checking example

from types_aiobotocore_health.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("health").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("health").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### describe\_affected\_accounts\_for\_organization

Returns a list of accounts in the organization from Organizations that are
affected by the provided event.

Type annotations and code completion for `#!python session.client("health").describe_affected_accounts_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

```python
# describe_affected_accounts_for_organization method definition

await def describe_affected_accounts_for_organization(
    self,
    *,
    eventArn: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> DescribeAffectedAccountsForOrganizationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAffectedAccountsForOrganizationResponseTypeDef](./type_defs.md#describeaffectedaccountsfororganizationresponsetypedef) 


```python
# describe_affected_accounts_for_organization method usage example with argument unpacking

kwargs: DescribeAffectedAccountsForOrganizationRequestRequestTypeDef = {  # (1)
    "eventArn": ...,
}

parent.describe_affected_accounts_for_organization(**kwargs)
```

1. See [:material-code-braces: DescribeAffectedAccountsForOrganizationRequestRequestTypeDef](./type_defs.md#describeaffectedaccountsfororganizationrequestrequesttypedef) 

### describe\_affected\_entities

Returns a list of entities that have been affected by the specified events,
based on the specified filter criteria.

Type annotations and code completion for `#!python session.client("health").describe_affected_entities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

```python
# describe_affected_entities method definition

await def describe_affected_entities(
    self,
    *,
    filter: EntityFilterTypeDef,  # (1)
    locale: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> DescribeAffectedEntitiesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EntityFilterTypeDef](./type_defs.md#entityfiltertypedef) 
2. See [:material-code-braces: DescribeAffectedEntitiesResponseTypeDef](./type_defs.md#describeaffectedentitiesresponsetypedef) 


```python
# describe_affected_entities method usage example with argument unpacking

kwargs: DescribeAffectedEntitiesRequestRequestTypeDef = {  # (1)
    "filter": ...,
}

parent.describe_affected_entities(**kwargs)
```

1. See [:material-code-braces: DescribeAffectedEntitiesRequestRequestTypeDef](./type_defs.md#describeaffectedentitiesrequestrequesttypedef) 

### describe\_affected\_entities\_for\_organization

Returns a list of entities that have been affected by one or more events for
one or more accounts in your organization in Organizations, based on the filter
criteria.

Type annotations and code completion for `#!python session.client("health").describe_affected_entities_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

```python
# describe_affected_entities_for_organization method definition

await def describe_affected_entities_for_organization(
    self,
    *,
    organizationEntityFilters: Sequence[EventAccountFilterTypeDef] = ...,  # (1)
    locale: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
    organizationEntityAccountFilters: Sequence[EntityAccountFilterTypeDef] = ...,  # (2)
) -> DescribeAffectedEntitiesForOrganizationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EventAccountFilterTypeDef](./type_defs.md#eventaccountfiltertypedef) 
2. See [:material-code-braces: EntityAccountFilterTypeDef](./type_defs.md#entityaccountfiltertypedef) 
3. See [:material-code-braces: DescribeAffectedEntitiesForOrganizationResponseTypeDef](./type_defs.md#describeaffectedentitiesfororganizationresponsetypedef) 


```python
# describe_affected_entities_for_organization method usage example with argument unpacking

kwargs: DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef = {  # (1)
    "organizationEntityFilters": ...,
}

parent.describe_affected_entities_for_organization(**kwargs)
```

1. See [:material-code-braces: DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef](./type_defs.md#describeaffectedentitiesfororganizationrequestrequesttypedef) 

### describe\_entity\_aggregates

Returns the number of entities that are affected by each of the specified
events.

Type annotations and code completion for `#!python session.client("health").describe_entity_aggregates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

```python
# describe_entity_aggregates method definition

await def describe_entity_aggregates(
    self,
    *,
    eventArns: Sequence[str] = ...,
) -> DescribeEntityAggregatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEntityAggregatesResponseTypeDef](./type_defs.md#describeentityaggregatesresponsetypedef) 


```python
# describe_entity_aggregates method usage example with argument unpacking

kwargs: DescribeEntityAggregatesRequestRequestTypeDef = {  # (1)
    "eventArns": ...,
}

parent.describe_entity_aggregates(**kwargs)
```

1. See [:material-code-braces: DescribeEntityAggregatesRequestRequestTypeDef](./type_defs.md#describeentityaggregatesrequestrequesttypedef) 

### describe\_entity\_aggregates\_for\_organization

Returns a list of entity aggregates for your Organizations that are affected by
each of the specified events.

Type annotations and code completion for `#!python session.client("health").describe_entity_aggregates_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

```python
# describe_entity_aggregates_for_organization method definition

await def describe_entity_aggregates_for_organization(
    self,
    *,
    eventArns: Sequence[str],
    awsAccountIds: Sequence[str] = ...,
) -> DescribeEntityAggregatesForOrganizationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEntityAggregatesForOrganizationResponseTypeDef](./type_defs.md#describeentityaggregatesfororganizationresponsetypedef) 


```python
# describe_entity_aggregates_for_organization method usage example with argument unpacking

kwargs: DescribeEntityAggregatesForOrganizationRequestRequestTypeDef = {  # (1)
    "eventArns": ...,
}

parent.describe_entity_aggregates_for_organization(**kwargs)
```

1. See [:material-code-braces: DescribeEntityAggregatesForOrganizationRequestRequestTypeDef](./type_defs.md#describeentityaggregatesfororganizationrequestrequesttypedef) 

### describe\_event\_aggregates

Returns the number of events of each event type (issue, scheduled change, and
account notification).

Type annotations and code completion for `#!python session.client("health").describe_event_aggregates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

```python
# describe_event_aggregates method definition

await def describe_event_aggregates(
    self,
    *,
    aggregateField: EventAggregateFieldType,  # (1)
    filter: EventFilterTypeDef = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
) -> DescribeEventAggregatesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: EventAggregateFieldType](./literals.md#eventaggregatefieldtype) 
2. See [:material-code-braces: EventFilterTypeDef](./type_defs.md#eventfiltertypedef) 
3. See [:material-code-braces: DescribeEventAggregatesResponseTypeDef](./type_defs.md#describeeventaggregatesresponsetypedef) 


```python
# describe_event_aggregates method usage example with argument unpacking

kwargs: DescribeEventAggregatesRequestRequestTypeDef = {  # (1)
    "aggregateField": ...,
}

parent.describe_event_aggregates(**kwargs)
```

1. See [:material-code-braces: DescribeEventAggregatesRequestRequestTypeDef](./type_defs.md#describeeventaggregatesrequestrequesttypedef) 

### describe\_event\_details

Returns detailed information about one or more specified events.

Type annotations and code completion for `#!python session.client("health").describe_event_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

```python
# describe_event_details method definition

await def describe_event_details(
    self,
    *,
    eventArns: Sequence[str],
    locale: str = ...,
) -> DescribeEventDetailsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEventDetailsResponseTypeDef](./type_defs.md#describeeventdetailsresponsetypedef) 


```python
# describe_event_details method usage example with argument unpacking

kwargs: DescribeEventDetailsRequestRequestTypeDef = {  # (1)
    "eventArns": ...,
}

parent.describe_event_details(**kwargs)
```

1. See [:material-code-braces: DescribeEventDetailsRequestRequestTypeDef](./type_defs.md#describeeventdetailsrequestrequesttypedef) 

### describe\_event\_details\_for\_organization

Returns detailed information about one or more specified events for one or more
Amazon Web Services accounts in your organization.

Type annotations and code completion for `#!python session.client("health").describe_event_details_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

```python
# describe_event_details_for_organization method definition

await def describe_event_details_for_organization(
    self,
    *,
    organizationEventDetailFilters: Sequence[EventAccountFilterTypeDef],  # (1)
    locale: str = ...,
) -> DescribeEventDetailsForOrganizationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EventAccountFilterTypeDef](./type_defs.md#eventaccountfiltertypedef) 
2. See [:material-code-braces: DescribeEventDetailsForOrganizationResponseTypeDef](./type_defs.md#describeeventdetailsfororganizationresponsetypedef) 


```python
# describe_event_details_for_organization method usage example with argument unpacking

kwargs: DescribeEventDetailsForOrganizationRequestRequestTypeDef = {  # (1)
    "organizationEventDetailFilters": ...,
}

parent.describe_event_details_for_organization(**kwargs)
```

1. See [:material-code-braces: DescribeEventDetailsForOrganizationRequestRequestTypeDef](./type_defs.md#describeeventdetailsfororganizationrequestrequesttypedef) 

### describe\_event\_types

Returns the event types that meet the specified filter criteria.

Type annotations and code completion for `#!python session.client("health").describe_event_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

```python
# describe_event_types method definition

await def describe_event_types(
    self,
    *,
    filter: EventTypeFilterTypeDef = ...,  # (1)
    locale: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> DescribeEventTypesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EventTypeFilterTypeDef](./type_defs.md#eventtypefiltertypedef) 
2. See [:material-code-braces: DescribeEventTypesResponseTypeDef](./type_defs.md#describeeventtypesresponsetypedef) 


```python
# describe_event_types method usage example with argument unpacking

kwargs: DescribeEventTypesRequestRequestTypeDef = {  # (1)
    "filter": ...,
}

parent.describe_event_types(**kwargs)
```

1. See [:material-code-braces: DescribeEventTypesRequestRequestTypeDef](./type_defs.md#describeeventtypesrequestrequesttypedef) 

### describe\_events

Returns information about events that meet the specified filter criteria.

Type annotations and code completion for `#!python session.client("health").describe_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

```python
# describe_events method definition

await def describe_events(
    self,
    *,
    filter: EventFilterTypeDef = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
    locale: str = ...,
) -> DescribeEventsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EventFilterTypeDef](./type_defs.md#eventfiltertypedef) 
2. See [:material-code-braces: DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef) 


```python
# describe_events method usage example with argument unpacking

kwargs: DescribeEventsRequestRequestTypeDef = {  # (1)
    "filter": ...,
}

parent.describe_events(**kwargs)
```

1. See [:material-code-braces: DescribeEventsRequestRequestTypeDef](./type_defs.md#describeeventsrequestrequesttypedef) 

### describe\_events\_for\_organization

Returns information about events across your organization in Organizations.

Type annotations and code completion for `#!python session.client("health").describe_events_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

```python
# describe_events_for_organization method definition

await def describe_events_for_organization(
    self,
    *,
    filter: OrganizationEventFilterTypeDef = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
    locale: str = ...,
) -> DescribeEventsForOrganizationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OrganizationEventFilterTypeDef](./type_defs.md#organizationeventfiltertypedef) 
2. See [:material-code-braces: DescribeEventsForOrganizationResponseTypeDef](./type_defs.md#describeeventsfororganizationresponsetypedef) 


```python
# describe_events_for_organization method usage example with argument unpacking

kwargs: DescribeEventsForOrganizationRequestRequestTypeDef = {  # (1)
    "filter": ...,
}

parent.describe_events_for_organization(**kwargs)
```

1. See [:material-code-braces: DescribeEventsForOrganizationRequestRequestTypeDef](./type_defs.md#describeeventsfororganizationrequestrequesttypedef) 

### describe\_health\_service\_status\_for\_organization

This operation provides status information on enabling or disabling Health to
work with your organization.

Type annotations and code completion for `#!python session.client("health").describe_health_service_status_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

```python
# describe_health_service_status_for_organization method definition

await def describe_health_service_status_for_organization(
    self,
) -> DescribeHealthServiceStatusForOrganizationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeHealthServiceStatusForOrganizationResponseTypeDef](./type_defs.md#describehealthservicestatusfororganizationresponsetypedef) 

### disable\_health\_service\_access\_for\_organization

Disables Health from working with Organizations.

Type annotations and code completion for `#!python session.client("health").disable_health_service_access_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

```python
# disable_health_service_access_for_organization method definition

await def disable_health_service_access_for_organization(
    self,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 

### enable\_health\_service\_access\_for\_organization

Enables Health to work with Organizations.

Type annotations and code completion for `#!python session.client("health").enable_health_service_access_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

```python
# enable_health_service_access_for_organization method definition

await def enable_health_service_access_for_organization(
    self,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("health").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("health").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("health").get_paginator` method with overloads.

- `client.get_paginator("describe_affected_accounts_for_organization")` -> [DescribeAffectedAccountsForOrganizationPaginator](./paginators.md#describeaffectedaccountsfororganizationpaginator)
- `client.get_paginator("describe_affected_entities_for_organization")` -> [DescribeAffectedEntitiesForOrganizationPaginator](./paginators.md#describeaffectedentitiesfororganizationpaginator)
- `client.get_paginator("describe_affected_entities")` -> [DescribeAffectedEntitiesPaginator](./paginators.md#describeaffectedentitiespaginator)
- `client.get_paginator("describe_event_aggregates")` -> [DescribeEventAggregatesPaginator](./paginators.md#describeeventaggregatespaginator)
- `client.get_paginator("describe_event_types")` -> [DescribeEventTypesPaginator](./paginators.md#describeeventtypespaginator)
- `client.get_paginator("describe_events_for_organization")` -> [DescribeEventsForOrganizationPaginator](./paginators.md#describeeventsfororganizationpaginator)
- `client.get_paginator("describe_events")` -> [DescribeEventsPaginator](./paginators.md#describeeventspaginator)


