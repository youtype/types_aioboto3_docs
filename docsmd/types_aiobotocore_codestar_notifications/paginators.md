# Paginators

> [Index](../README.md) > [CodeStarNotifications](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CodeStarNotifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
    type annotations stubs module [types-aiobotocore-codestar-notifications](https://pypi.org/project/types-aiobotocore-codestar-notifications/).

## ListEventTypesPaginator

Type annotations and code completion for `#!python session.client("codestar-notifications").get_paginator("list_event_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListEventTypes)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_codestar_notifications.paginator import ListEventTypesPaginator

session = Session()

session = get_session()
async with session.client("codestar-notifications") as client:  # (1)
    paginator: ListEventTypesPaginator = client.get_paginator("list_event_types")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventTypesResultTypeDef
        print(item)  # (3)
```

1. client: [CodeStarNotificationsClient](./client.md)
2. paginator: [ListEventTypesPaginator](./paginators.md#listeventtypespaginator)
3. item: [:material-code-braces: ListEventTypesResultTypeDef](./type_defs.md#listeventtypesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListEventTypesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[ListEventTypesFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListEventTypesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListEventTypesFilterTypeDef](./type_defs.md#listeventtypesfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListEventTypesResultTypeDef](./type_defs.md#listeventtypesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListEventTypesRequestListEventTypesPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventTypesRequestListEventTypesPaginateTypeDef](./type_defs.md#listeventtypesrequestlisteventtypespaginatetypedef) 
## ListNotificationRulesPaginator

Type annotations and code completion for `#!python session.client("codestar-notifications").get_paginator("list_notification_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListNotificationRules)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_codestar_notifications.paginator import ListNotificationRulesPaginator

session = Session()

session = get_session()
async with session.client("codestar-notifications") as client:  # (1)
    paginator: ListNotificationRulesPaginator = client.get_paginator("list_notification_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListNotificationRulesResultTypeDef
        print(item)  # (3)
```

1. client: [CodeStarNotificationsClient](./client.md)
2. paginator: [ListNotificationRulesPaginator](./paginators.md#listnotificationrulespaginator)
3. item: [:material-code-braces: ListNotificationRulesResultTypeDef](./type_defs.md#listnotificationrulesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListNotificationRulesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[ListNotificationRulesFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListNotificationRulesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListNotificationRulesFilterTypeDef](./type_defs.md#listnotificationrulesfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListNotificationRulesResultTypeDef](./type_defs.md#listnotificationrulesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListNotificationRulesRequestListNotificationRulesPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNotificationRulesRequestListNotificationRulesPaginateTypeDef](./type_defs.md#listnotificationrulesrequestlistnotificationrulespaginatetypedef) 
## ListTargetsPaginator

Type annotations and code completion for `#!python session.client("codestar-notifications").get_paginator("list_targets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Paginator.ListTargets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_codestar_notifications.paginator import ListTargetsPaginator

session = Session()

session = get_session()
async with session.client("codestar-notifications") as client:  # (1)
    paginator: ListTargetsPaginator = client.get_paginator("list_targets")  # (2)
    async for item in paginator.paginate(...):
        item: ListTargetsResultTypeDef
        print(item)  # (3)
```

1. client: [CodeStarNotificationsClient](./client.md)
2. paginator: [ListTargetsPaginator](./paginators.md#listtargetspaginator)
3. item: [:material-code-braces: ListTargetsResultTypeDef](./type_defs.md#listtargetsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListTargetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[ListTargetsFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListTargetsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ListTargetsFilterTypeDef](./type_defs.md#listtargetsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListTargetsResultTypeDef](./type_defs.md#listtargetsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListTargetsRequestListTargetsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTargetsRequestListTargetsPaginateTypeDef](./type_defs.md#listtargetsrequestlisttargetspaginatetypedef) 
