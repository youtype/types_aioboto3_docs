# Budgets module

> [Index](../README.md) > Budgets


!!! note ""

    Auto-generated documentation for [Budgets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#budgets)
    type annotations stubs module [types-aiobotocore-budgets](https://pypi.org/project/types-aiobotocore-budgets/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `Budgets` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `Budgets` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[budgets]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[budgets]'

# standalone installation
python -m pip install types-aiobotocore-budgets
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-budgets
```

## Usage

Code samples can be found in [Examples](./usage.md).

## BudgetsClient

Type annotations and code completion for  `#!python session.client("budgets")` as [BudgetsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client)

```python
# BudgetsClient usage example

from aioboto3.session import Session

from types_aiobotocore_budgets.client import BudgetsClient


session = Session()
async with session.client("budgets") as client:
    client: BudgetsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("budgets").get_paginator("...")`.

```python
# DescribeBudgetActionHistoriesPaginator usage example

from types_aiobotocore_budgets.paginator import DescribeBudgetActionHistoriesPaginator

def get_describe_budget_action_histories_paginator() -> DescribeBudgetActionHistoriesPaginator:
    return client.get_paginator("describe_budget_action_histories"))
```

- [DescribeBudgetActionHistoriesPaginator](./paginators.md#describebudgetactionhistoriespaginator)
- [DescribeBudgetActionsForAccountPaginator](./paginators.md#describebudgetactionsforaccountpaginator)
- [DescribeBudgetActionsForBudgetPaginator](./paginators.md#describebudgetactionsforbudgetpaginator)
- [DescribeBudgetNotificationsForAccountPaginator](./paginators.md#describebudgetnotificationsforaccountpaginator)
- [DescribeBudgetPerformanceHistoryPaginator](./paginators.md#describebudgetperformancehistorypaginator)
- [DescribeBudgetsPaginator](./paginators.md#describebudgetspaginator)
- [DescribeNotificationsForBudgetPaginator](./paginators.md#describenotificationsforbudgetpaginator)
- [DescribeSubscribersForNotificationPaginator](./paginators.md#describesubscribersfornotificationpaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActionStatusType usage example

from types_aiobotocore_budgets.literals import ActionStatusType

def get_value() -> ActionStatusType:
    return "EXECUTION_FAILURE"
```

- [ActionStatusType](./literals.md#actionstatustype)
- [ActionSubTypeType](./literals.md#actionsubtypetype)
- [ActionTypeType](./literals.md#actiontypetype)
- [ApprovalModelType](./literals.md#approvalmodeltype)
- [AutoAdjustTypeType](./literals.md#autoadjusttypetype)
- [BudgetTypeType](./literals.md#budgettypetype)
- [ComparisonOperatorType](./literals.md#comparisonoperatortype)
- [DescribeBudgetActionHistoriesPaginatorName](./literals.md#describebudgetactionhistoriespaginatorname)
- [DescribeBudgetActionsForAccountPaginatorName](./literals.md#describebudgetactionsforaccountpaginatorname)
- [DescribeBudgetActionsForBudgetPaginatorName](./literals.md#describebudgetactionsforbudgetpaginatorname)
- [DescribeBudgetNotificationsForAccountPaginatorName](./literals.md#describebudgetnotificationsforaccountpaginatorname)
- [DescribeBudgetPerformanceHistoryPaginatorName](./literals.md#describebudgetperformancehistorypaginatorname)
- [DescribeBudgetsPaginatorName](./literals.md#describebudgetspaginatorname)
- [DescribeNotificationsForBudgetPaginatorName](./literals.md#describenotificationsforbudgetpaginatorname)
- [DescribeSubscribersForNotificationPaginatorName](./literals.md#describesubscribersfornotificationpaginatorname)
- [EventTypeType](./literals.md#eventtypetype)
- [ExecutionTypeType](./literals.md#executiontypetype)
- [NotificationStateType](./literals.md#notificationstatetype)
- [NotificationTypeType](./literals.md#notificationtypetype)
- [SubscriptionTypeType](./literals.md#subscriptiontypetype)
- [ThresholdTypeType](./literals.md#thresholdtypetype)
- [TimeUnitType](./literals.md#timeunittype)
- [BudgetsServiceName](./literals.md#budgetsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ActionThresholdTypeDef](./type_defs.md#actionthresholdtypedef)
- [SubscriberTypeDef](./type_defs.md#subscribertypedef)
- [HistoricalOptionsTypeDef](./type_defs.md#historicaloptionstypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [NotificationTypeDef](./type_defs.md#notificationtypedef)
- [CostTypesTypeDef](./type_defs.md#costtypestypedef)
- [SpendTypeDef](./type_defs.md#spendtypedef)
- [TimePeriodOutputTypeDef](./type_defs.md#timeperiodoutputtypedef)
- [ResourceTagTypeDef](./type_defs.md#resourcetagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [IamActionDefinitionOutputTypeDef](./type_defs.md#iamactiondefinitionoutputtypedef)
- [ScpActionDefinitionOutputTypeDef](./type_defs.md#scpactiondefinitionoutputtypedef)
- [SsmActionDefinitionOutputTypeDef](./type_defs.md#ssmactiondefinitionoutputtypedef)
- [DeleteBudgetActionRequestRequestTypeDef](./type_defs.md#deletebudgetactionrequestrequesttypedef)
- [DeleteBudgetRequestRequestTypeDef](./type_defs.md#deletebudgetrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeBudgetActionRequestRequestTypeDef](./type_defs.md#describebudgetactionrequestrequesttypedef)
- [DescribeBudgetActionsForAccountRequestRequestTypeDef](./type_defs.md#describebudgetactionsforaccountrequestrequesttypedef)
- [DescribeBudgetActionsForBudgetRequestRequestTypeDef](./type_defs.md#describebudgetactionsforbudgetrequestrequesttypedef)
- [DescribeBudgetNotificationsForAccountRequestRequestTypeDef](./type_defs.md#describebudgetnotificationsforaccountrequestrequesttypedef)
- [DescribeBudgetRequestRequestTypeDef](./type_defs.md#describebudgetrequestrequesttypedef)
- [DescribeBudgetsRequestRequestTypeDef](./type_defs.md#describebudgetsrequestrequesttypedef)
- [DescribeNotificationsForBudgetRequestRequestTypeDef](./type_defs.md#describenotificationsforbudgetrequestrequesttypedef)
- [ExecuteBudgetActionRequestRequestTypeDef](./type_defs.md#executebudgetactionrequestrequesttypedef)
- [IamActionDefinitionTypeDef](./type_defs.md#iamactiondefinitiontypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ScpActionDefinitionTypeDef](./type_defs.md#scpactiondefinitiontypedef)
- [SsmActionDefinitionTypeDef](./type_defs.md#ssmactiondefinitiontypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [AutoAdjustDataOutputTypeDef](./type_defs.md#autoadjustdataoutputtypedef)
- [AutoAdjustDataTypeDef](./type_defs.md#autoadjustdatatypedef)
- [TimePeriodTypeDef](./type_defs.md#timeperiodtypedef)
- [BudgetNotificationsForAccountTypeDef](./type_defs.md#budgetnotificationsforaccounttypedef)
- [CreateNotificationRequestRequestTypeDef](./type_defs.md#createnotificationrequestrequesttypedef)
- [CreateSubscriberRequestRequestTypeDef](./type_defs.md#createsubscriberrequestrequesttypedef)
- [DeleteNotificationRequestRequestTypeDef](./type_defs.md#deletenotificationrequestrequesttypedef)
- [DeleteSubscriberRequestRequestTypeDef](./type_defs.md#deletesubscriberrequestrequesttypedef)
- [DescribeSubscribersForNotificationRequestRequestTypeDef](./type_defs.md#describesubscribersfornotificationrequestrequesttypedef)
- [NotificationWithSubscribersTypeDef](./type_defs.md#notificationwithsubscriberstypedef)
- [UpdateNotificationRequestRequestTypeDef](./type_defs.md#updatenotificationrequestrequesttypedef)
- [UpdateSubscriberRequestRequestTypeDef](./type_defs.md#updatesubscriberrequestrequesttypedef)
- [CalculatedSpendTypeDef](./type_defs.md#calculatedspendtypedef)
- [BudgetedAndActualAmountsTypeDef](./type_defs.md#budgetedandactualamountstypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateBudgetActionResponseTypeDef](./type_defs.md#createbudgetactionresponsetypedef)
- [DescribeNotificationsForBudgetResponseTypeDef](./type_defs.md#describenotificationsforbudgetresponsetypedef)
- [DescribeSubscribersForNotificationResponseTypeDef](./type_defs.md#describesubscribersfornotificationresponsetypedef)
- [ExecuteBudgetActionResponseTypeDef](./type_defs.md#executebudgetactionresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [DefinitionOutputTypeDef](./type_defs.md#definitionoutputtypedef)
- [DescribeBudgetActionsForAccountRequestPaginateTypeDef](./type_defs.md#describebudgetactionsforaccountrequestpaginatetypedef)
- [DescribeBudgetActionsForBudgetRequestPaginateTypeDef](./type_defs.md#describebudgetactionsforbudgetrequestpaginatetypedef)
- [DescribeBudgetNotificationsForAccountRequestPaginateTypeDef](./type_defs.md#describebudgetnotificationsforaccountrequestpaginatetypedef)
- [DescribeBudgetsRequestPaginateTypeDef](./type_defs.md#describebudgetsrequestpaginatetypedef)
- [DescribeNotificationsForBudgetRequestPaginateTypeDef](./type_defs.md#describenotificationsforbudgetrequestpaginatetypedef)
- [DescribeSubscribersForNotificationRequestPaginateTypeDef](./type_defs.md#describesubscribersfornotificationrequestpaginatetypedef)
- [IamActionDefinitionUnionTypeDef](./type_defs.md#iamactiondefinitionuniontypedef)
- [ScpActionDefinitionUnionTypeDef](./type_defs.md#scpactiondefinitionuniontypedef)
- [SsmActionDefinitionUnionTypeDef](./type_defs.md#ssmactiondefinitionuniontypedef)
- [AutoAdjustDataUnionTypeDef](./type_defs.md#autoadjustdatauniontypedef)
- [DescribeBudgetActionHistoriesRequestPaginateTypeDef](./type_defs.md#describebudgetactionhistoriesrequestpaginatetypedef)
- [DescribeBudgetActionHistoriesRequestRequestTypeDef](./type_defs.md#describebudgetactionhistoriesrequestrequesttypedef)
- [DescribeBudgetPerformanceHistoryRequestPaginateTypeDef](./type_defs.md#describebudgetperformancehistoryrequestpaginatetypedef)
- [DescribeBudgetPerformanceHistoryRequestRequestTypeDef](./type_defs.md#describebudgetperformancehistoryrequestrequesttypedef)
- [TimePeriodUnionTypeDef](./type_defs.md#timeperioduniontypedef)
- [DescribeBudgetNotificationsForAccountResponseTypeDef](./type_defs.md#describebudgetnotificationsforaccountresponsetypedef)
- [BudgetOutputTypeDef](./type_defs.md#budgetoutputtypedef)
- [BudgetPerformanceHistoryTypeDef](./type_defs.md#budgetperformancehistorytypedef)
- [ActionTypeDef](./type_defs.md#actiontypedef)
- [DefinitionTypeDef](./type_defs.md#definitiontypedef)
- [BudgetTypeDef](./type_defs.md#budgettypedef)
- [DescribeBudgetResponseTypeDef](./type_defs.md#describebudgetresponsetypedef)
- [DescribeBudgetsResponseTypeDef](./type_defs.md#describebudgetsresponsetypedef)
- [DescribeBudgetPerformanceHistoryResponseTypeDef](./type_defs.md#describebudgetperformancehistoryresponsetypedef)
- [ActionHistoryDetailsTypeDef](./type_defs.md#actionhistorydetailstypedef)
- [DeleteBudgetActionResponseTypeDef](./type_defs.md#deletebudgetactionresponsetypedef)
- [DescribeBudgetActionResponseTypeDef](./type_defs.md#describebudgetactionresponsetypedef)
- [DescribeBudgetActionsForAccountResponseTypeDef](./type_defs.md#describebudgetactionsforaccountresponsetypedef)
- [DescribeBudgetActionsForBudgetResponseTypeDef](./type_defs.md#describebudgetactionsforbudgetresponsetypedef)
- [UpdateBudgetActionResponseTypeDef](./type_defs.md#updatebudgetactionresponsetypedef)
- [CreateBudgetActionRequestRequestTypeDef](./type_defs.md#createbudgetactionrequestrequesttypedef)
- [UpdateBudgetActionRequestRequestTypeDef](./type_defs.md#updatebudgetactionrequestrequesttypedef)
- [CreateBudgetRequestRequestTypeDef](./type_defs.md#createbudgetrequestrequesttypedef)
- [UpdateBudgetRequestRequestTypeDef](./type_defs.md#updatebudgetrequestrequesttypedef)
- [ActionHistoryTypeDef](./type_defs.md#actionhistorytypedef)
- [DescribeBudgetActionHistoriesResponseTypeDef](./type_defs.md#describebudgetactionhistoriesresponsetypedef)
