# Examples

> [Index](../README.md) > [PrometheusService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PrometheusService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#prometheusservice)
    type annotations stubs module [types-aiobotocore-amp](https://pypi.org/project/types-aiobotocore-amp/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[amp]` package installed.

Write your `PrometheusService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# PrometheusServiceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("amp") as client:  # (1)
    result = await client.create_alert_manager_definition()  # (2)
```

1. client: [PrometheusServiceClient](./client.md)
2. result: [:material-code-braces: CreateAlertManagerDefinitionResponseTypeDef](./type_defs.md#createalertmanagerdefinitionresponsetypedef)



#### Paginator usage example

```python
# ListRuleGroupsNamespacesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("amp") as client:  # (1)
    paginator = client.get_paginator("list_rule_groups_namespaces")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [PrometheusServiceClient](./client.md)
2. paginator: [ListRuleGroupsNamespacesPaginator](./paginators.md#listrulegroupsnamespacespaginator)
3. item: [:material-code-braces: ListRuleGroupsNamespacesResponseTypeDef](./type_defs.md#listrulegroupsnamespacesresponsetypedef)



#### Waiter usage example

```python
# ScraperActiveWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("amp") as client:  # (1)
    waiter = client.get_waiter("scraper_active")  # (2)
    await waiter.wait(...)
```

1. client: [PrometheusServiceClient](./client.md)
2. waiter: [ScraperActiveWaiter](./waiters.md#scraperactivewaiter)


### Explicit type annotations

With `types-aioboto3-lite[amp]`
or a standalone `types_aiobotocore_amp` package, you have to explicitly specify
`client: PrometheusServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# PrometheusServiceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_amp.client import PrometheusServiceClient
from types_aiobotocore_amp.type_defs import CreateAlertManagerDefinitionResponseTypeDef
from types_aiobotocore_amp.type_defs import CreateAlertManagerDefinitionRequestTypeDef


session = Session()

client: PrometheusServiceClient
async with session.client("amp") as client:  # (1)
    kwargs: CreateAlertManagerDefinitionRequestTypeDef = {...}  # (2)
    result: CreateAlertManagerDefinitionResponseTypeDef = await client.create_alert_manager_definition(**kwargs)  # (3)
```

1. client: [PrometheusServiceClient](./client.md)
2. kwargs: [:material-code-braces: CreateAlertManagerDefinitionRequestTypeDef](./type_defs.md#createalertmanagerdefinitionrequesttypedef)
3. result: [:material-code-braces: CreateAlertManagerDefinitionResponseTypeDef](./type_defs.md#createalertmanagerdefinitionresponsetypedef)



#### Paginator usage example

```python
# ListRuleGroupsNamespacesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_amp.client import PrometheusServiceClient
from types_aiobotocore_amp.paginator import ListRuleGroupsNamespacesPaginator
from types_aiobotocore_amp.type_defs import ListRuleGroupsNamespacesResponseTypeDef


session = Session()

client: PrometheusServiceClient
async with session.client("amp") as client:  # (1)
    paginator: ListRuleGroupsNamespacesPaginator = client.get_paginator("list_rule_groups_namespaces")  # (2)
    async for item in paginator.paginate(...):
        item: ListRuleGroupsNamespacesResponseTypeDef
        print(item)  # (3)
```

1. client: [PrometheusServiceClient](./client.md)
2. paginator: [ListRuleGroupsNamespacesPaginator](./paginators.md#listrulegroupsnamespacespaginator)
3. item: [:material-code-braces: ListRuleGroupsNamespacesResponseTypeDef](./type_defs.md#listrulegroupsnamespacesresponsetypedef)



#### Waiter usage example

```python
# ScraperActiveWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_amp.client import PrometheusServiceClient
from types_aiobotocore_amp.waiter import ScraperActiveWaiter


session = Session()

async with session.client("amp") as client:  # (1)
    waiter = client.get_waiter("scraper_active")  # (2)
    await waiter.wait(...)
```

1. client: [PrometheusServiceClient](./client.md)
2. waiter: [ScraperActiveWaiter](./waiters.md#scraperactivewaiter)


