# CodeStarNotifications module

> [Index](../README.md) > CodeStarNotifications


!!! note ""

    Auto-generated documentation for [CodeStarNotifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#codestarnotifications)
    type annotations stubs module [types-aiobotocore-codestar-notifications](https://pypi.org/project/types-aiobotocore-codestar-notifications/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `CodeStarNotifications` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `CodeStarNotifications` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[codestar-notifications]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[codestar-notifications]'

# standalone installation
python -m pip install types-aiobotocore-codestar-notifications
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-codestar-notifications
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CodeStarNotificationsClient

Type annotations and code completion for  `#!python session.client("codestar-notifications")` as [CodeStarNotificationsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications.Client)

```python
# CodeStarNotificationsClient usage example

from aioboto3.session import Session

from types_aiobotocore_codestar_notifications.client import CodeStarNotificationsClient


session = Session()
async with session.client("codestar-notifications") as client:
    client: CodeStarNotificationsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("codestar-notifications").get_paginator("...")`.

```python
# ListEventTypesPaginator usage example

from types_aiobotocore_codestar_notifications.paginator import ListEventTypesPaginator

def get_list_event_types_paginator() -> ListEventTypesPaginator:
    return client.get_paginator("list_event_types"))
```

- [ListEventTypesPaginator](./paginators.md#listeventtypespaginator)
- [ListNotificationRulesPaginator](./paginators.md#listnotificationrulespaginator)
- [ListTargetsPaginator](./paginators.md#listtargetspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DetailTypeType usage example

from types_aiobotocore_codestar_notifications.literals import DetailTypeType

def get_value() -> DetailTypeType:
    return "BASIC"
```

- [DetailTypeType](./literals.md#detailtypetype)
- [ListEventTypesFilterNameType](./literals.md#listeventtypesfilternametype)
- [ListEventTypesPaginatorName](./literals.md#listeventtypespaginatorname)
- [ListNotificationRulesFilterNameType](./literals.md#listnotificationrulesfilternametype)
- [ListNotificationRulesPaginatorName](./literals.md#listnotificationrulespaginatorname)
- [ListTargetsFilterNameType](./literals.md#listtargetsfilternametype)
- [ListTargetsPaginatorName](./literals.md#listtargetspaginatorname)
- [NotificationRuleStatusType](./literals.md#notificationrulestatustype)
- [TargetStatusType](./literals.md#targetstatustype)
- [CodeStarNotificationsServiceName](./literals.md#codestarnotificationsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [TargetTypeDef](./type_defs.md#targettypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteNotificationRuleRequestRequestTypeDef](./type_defs.md#deletenotificationrulerequestrequesttypedef)
- [DeleteTargetRequestRequestTypeDef](./type_defs.md#deletetargetrequestrequesttypedef)
- [DescribeNotificationRuleRequestRequestTypeDef](./type_defs.md#describenotificationrulerequestrequesttypedef)
- [EventTypeSummaryTypeDef](./type_defs.md#eventtypesummarytypedef)
- [TargetSummaryTypeDef](./type_defs.md#targetsummarytypedef)
- [ListEventTypesFilterTypeDef](./type_defs.md#listeventtypesfiltertypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListNotificationRulesFilterTypeDef](./type_defs.md#listnotificationrulesfiltertypedef)
- [NotificationRuleSummaryTypeDef](./type_defs.md#notificationrulesummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTargetsFilterTypeDef](./type_defs.md#listtargetsfiltertypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UnsubscribeRequestRequestTypeDef](./type_defs.md#unsubscriberequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [CreateNotificationRuleRequestRequestTypeDef](./type_defs.md#createnotificationrulerequestrequesttypedef)
- [SubscribeRequestRequestTypeDef](./type_defs.md#subscriberequestrequesttypedef)
- [UpdateNotificationRuleRequestRequestTypeDef](./type_defs.md#updatenotificationrulerequestrequesttypedef)
- [CreateNotificationRuleResultTypeDef](./type_defs.md#createnotificationruleresulttypedef)
- [DeleteNotificationRuleResultTypeDef](./type_defs.md#deletenotificationruleresulttypedef)
- [ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef)
- [SubscribeResultTypeDef](./type_defs.md#subscriberesulttypedef)
- [TagResourceResultTypeDef](./type_defs.md#tagresourceresulttypedef)
- [UnsubscribeResultTypeDef](./type_defs.md#unsubscriberesulttypedef)
- [ListEventTypesResultTypeDef](./type_defs.md#listeventtypesresulttypedef)
- [DescribeNotificationRuleResultTypeDef](./type_defs.md#describenotificationruleresulttypedef)
- [ListTargetsResultTypeDef](./type_defs.md#listtargetsresulttypedef)
- [ListEventTypesRequestRequestTypeDef](./type_defs.md#listeventtypesrequestrequesttypedef)
- [ListEventTypesRequestPaginateTypeDef](./type_defs.md#listeventtypesrequestpaginatetypedef)
- [ListNotificationRulesRequestPaginateTypeDef](./type_defs.md#listnotificationrulesrequestpaginatetypedef)
- [ListNotificationRulesRequestRequestTypeDef](./type_defs.md#listnotificationrulesrequestrequesttypedef)
- [ListNotificationRulesResultTypeDef](./type_defs.md#listnotificationrulesresulttypedef)
- [ListTargetsRequestPaginateTypeDef](./type_defs.md#listtargetsrequestpaginatetypedef)
- [ListTargetsRequestRequestTypeDef](./type_defs.md#listtargetsrequestrequesttypedef)
