# CostExplorerClient

> [Index](../README.md) > [CostExplorer](./README.md) > CostExplorerClient

!!! note ""

    Auto-generated documentation for [CostExplorer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
    type annotations stubs module [types-aiobotocore-ce](https://pypi.org/project/types-aiobotocore-ce/).

## CostExplorerClient

Type annotations and code completion for `#!python session.client("ce")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client)

```python title="Usage example"
from aioboto3.session import Session
from types_aiobotocore_ce.client import CostExplorerClient

session = Session()
async with session.client("ce") as client:
    client: CostExplorerClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("ce").exceptions` structure.

```python title="Usage example"
async with session.client("ce") as client:
    try:
        do_something(client)
    except (
            client.BillExpirationException,
        client.ClientError,
        client.DataUnavailableException,
        client.InvalidNextTokenException,
        client.LimitExceededException,
        client.RequestChangedException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.UnknownMonitorException,
        client.UnknownSubscriptionException,
        client.UnresolvableUsageUnitException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_ce.client import Exceptions

def handle_error(exc: Exceptions.BillExpirationException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.client("ce").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### create\_anomaly\_monitor

Creates a new cost anomaly detection monitor with the requested type and monitor
specification.

Type annotations and code completion for `#!python session.client("ce").create_anomaly_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_monitor)

```python title="Method definition"
await def create_anomaly_monitor(
    self,
    *,
    AnomalyMonitor: AnomalyMonitorTypeDef,  # (1)
) -> CreateAnomalyMonitorResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AnomalyMonitorTypeDef](./type_defs.md#anomalymonitortypedef) 
2. See [:material-code-braces: CreateAnomalyMonitorResponseTypeDef](./type_defs.md#createanomalymonitorresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: CreateAnomalyMonitorRequestRequestTypeDef = {  # (1)
    "AnomalyMonitor": ...,
}

parent.create_anomaly_monitor(**kwargs)
```

1. See [:material-code-braces: CreateAnomalyMonitorRequestRequestTypeDef](./type_defs.md#createanomalymonitorrequestrequesttypedef) 

### create\_anomaly\_subscription

Adds a subscription to a cost anomaly detection monitor.

Type annotations and code completion for `#!python session.client("ce").create_anomaly_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_subscription)

```python title="Method definition"
await def create_anomaly_subscription(
    self,
    *,
    AnomalySubscription: AnomalySubscriptionTypeDef,  # (1)
) -> CreateAnomalySubscriptionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AnomalySubscriptionTypeDef](./type_defs.md#anomalysubscriptiontypedef) 
2. See [:material-code-braces: CreateAnomalySubscriptionResponseTypeDef](./type_defs.md#createanomalysubscriptionresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: CreateAnomalySubscriptionRequestRequestTypeDef = {  # (1)
    "AnomalySubscription": ...,
}

parent.create_anomaly_subscription(**kwargs)
```

1. See [:material-code-braces: CreateAnomalySubscriptionRequestRequestTypeDef](./type_defs.md#createanomalysubscriptionrequestrequesttypedef) 

### create\_cost\_category\_definition

Creates a new Cost Category with the requested name and rules.

Type annotations and code completion for `#!python session.client("ce").create_cost_category_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_cost_category_definition)

```python title="Method definition"
await def create_cost_category_definition(
    self,
    *,
    Name: str,
    RuleVersion: CostCategoryRuleVersionType,  # (1)
    Rules: Sequence[CostCategoryRuleTypeDef],  # (2)
    DefaultValue: str = ...,
    SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...,  # (3)
) -> CreateCostCategoryDefinitionResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: CostCategoryRuleVersionType](./literals.md#costcategoryruleversiontype) 
2. See [:material-code-braces: CostCategoryRuleTypeDef](./type_defs.md#costcategoryruletypedef) 
3. See [:material-code-braces: CostCategorySplitChargeRuleTypeDef](./type_defs.md#costcategorysplitchargeruletypedef) 
4. See [:material-code-braces: CreateCostCategoryDefinitionResponseTypeDef](./type_defs.md#createcostcategorydefinitionresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: CreateCostCategoryDefinitionRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "RuleVersion": ...,
    "Rules": ...,
}

parent.create_cost_category_definition(**kwargs)
```

1. See [:material-code-braces: CreateCostCategoryDefinitionRequestRequestTypeDef](./type_defs.md#createcostcategorydefinitionrequestrequesttypedef) 

### delete\_anomaly\_monitor

Deletes a cost anomaly monitor.

Type annotations and code completion for `#!python session.client("ce").delete_anomaly_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.delete_anomaly_monitor)

```python title="Method definition"
await def delete_anomaly_monitor(
    self,
    *,
    MonitorArn: str,
) -> Dict[str, Any]:
    ...
```



```python title="Usage example with kwargs"
kwargs: DeleteAnomalyMonitorRequestRequestTypeDef = {  # (1)
    "MonitorArn": ...,
}

parent.delete_anomaly_monitor(**kwargs)
```

1. See [:material-code-braces: DeleteAnomalyMonitorRequestRequestTypeDef](./type_defs.md#deleteanomalymonitorrequestrequesttypedef) 

### delete\_anomaly\_subscription

Deletes a cost anomaly subscription.

Type annotations and code completion for `#!python session.client("ce").delete_anomaly_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.delete_anomaly_subscription)

```python title="Method definition"
await def delete_anomaly_subscription(
    self,
    *,
    SubscriptionArn: str,
) -> Dict[str, Any]:
    ...
```



```python title="Usage example with kwargs"
kwargs: DeleteAnomalySubscriptionRequestRequestTypeDef = {  # (1)
    "SubscriptionArn": ...,
}

parent.delete_anomaly_subscription(**kwargs)
```

1. See [:material-code-braces: DeleteAnomalySubscriptionRequestRequestTypeDef](./type_defs.md#deleteanomalysubscriptionrequestrequesttypedef) 

### delete\_cost\_category\_definition

Deletes a Cost Category.

Type annotations and code completion for `#!python session.client("ce").delete_cost_category_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.delete_cost_category_definition)

```python title="Method definition"
await def delete_cost_category_definition(
    self,
    *,
    CostCategoryArn: str,
) -> DeleteCostCategoryDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteCostCategoryDefinitionResponseTypeDef](./type_defs.md#deletecostcategorydefinitionresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DeleteCostCategoryDefinitionRequestRequestTypeDef = {  # (1)
    "CostCategoryArn": ...,
}

parent.delete_cost_category_definition(**kwargs)
```

1. See [:material-code-braces: DeleteCostCategoryDefinitionRequestRequestTypeDef](./type_defs.md#deletecostcategorydefinitionrequestrequesttypedef) 

### describe\_cost\_category\_definition

Returns the name, ARN, rules, definition, and effective dates of a Cost Category
that's defined in the account.

Type annotations and code completion for `#!python session.client("ce").describe_cost_category_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.describe_cost_category_definition)

```python title="Method definition"
await def describe_cost_category_definition(
    self,
    *,
    CostCategoryArn: str,
    EffectiveOn: str = ...,
) -> DescribeCostCategoryDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCostCategoryDefinitionResponseTypeDef](./type_defs.md#describecostcategorydefinitionresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeCostCategoryDefinitionRequestRequestTypeDef = {  # (1)
    "CostCategoryArn": ...,
}

parent.describe_cost_category_definition(**kwargs)
```

1. See [:material-code-braces: DescribeCostCategoryDefinitionRequestRequestTypeDef](./type_defs.md#describecostcategorydefinitionrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.client("ce").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.generate_presigned_url)

```python title="Method definition"
await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_anomalies

Retrieves all of the cost anomalies detected on your account during the time
period that's specified by the `DateInterval` object.

Type annotations and code completion for `#!python session.client("ce").get_anomalies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_anomalies)

```python title="Method definition"
await def get_anomalies(
    self,
    *,
    DateInterval: AnomalyDateIntervalTypeDef,  # (1)
    MonitorArn: str = ...,
    Feedback: AnomalyFeedbackTypeType = ...,  # (2)
    TotalImpact: TotalImpactFilterTypeDef = ...,  # (3)
    NextPageToken: str = ...,
    MaxResults: int = ...,
) -> GetAnomaliesResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: AnomalyDateIntervalTypeDef](./type_defs.md#anomalydateintervaltypedef) 
2. See [:material-code-brackets: AnomalyFeedbackTypeType](./literals.md#anomalyfeedbacktypetype) 
3. See [:material-code-braces: TotalImpactFilterTypeDef](./type_defs.md#totalimpactfiltertypedef) 
4. See [:material-code-braces: GetAnomaliesResponseTypeDef](./type_defs.md#getanomaliesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetAnomaliesRequestRequestTypeDef = {  # (1)
    "DateInterval": ...,
}

parent.get_anomalies(**kwargs)
```

1. See [:material-code-braces: GetAnomaliesRequestRequestTypeDef](./type_defs.md#getanomaliesrequestrequesttypedef) 

### get\_anomaly\_monitors

Retrieves the cost anomaly monitor definitions for your account.

Type annotations and code completion for `#!python session.client("ce").get_anomaly_monitors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_anomaly_monitors)

```python title="Method definition"
await def get_anomaly_monitors(
    self,
    *,
    MonitorArnList: Sequence[str] = ...,
    NextPageToken: str = ...,
    MaxResults: int = ...,
) -> GetAnomalyMonitorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAnomalyMonitorsResponseTypeDef](./type_defs.md#getanomalymonitorsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetAnomalyMonitorsRequestRequestTypeDef = {  # (1)
    "MonitorArnList": ...,
}

parent.get_anomaly_monitors(**kwargs)
```

1. See [:material-code-braces: GetAnomalyMonitorsRequestRequestTypeDef](./type_defs.md#getanomalymonitorsrequestrequesttypedef) 

### get\_anomaly\_subscriptions

Retrieves the cost anomaly subscription objects for your account.

Type annotations and code completion for `#!python session.client("ce").get_anomaly_subscriptions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_anomaly_subscriptions)

```python title="Method definition"
await def get_anomaly_subscriptions(
    self,
    *,
    SubscriptionArnList: Sequence[str] = ...,
    MonitorArn: str = ...,
    NextPageToken: str = ...,
    MaxResults: int = ...,
) -> GetAnomalySubscriptionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAnomalySubscriptionsResponseTypeDef](./type_defs.md#getanomalysubscriptionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetAnomalySubscriptionsRequestRequestTypeDef = {  # (1)
    "SubscriptionArnList": ...,
}

parent.get_anomaly_subscriptions(**kwargs)
```

1. See [:material-code-braces: GetAnomalySubscriptionsRequestRequestTypeDef](./type_defs.md#getanomalysubscriptionsrequestrequesttypedef) 

### get\_cost\_and\_usage

Retrieves cost and usage metrics for your account.

Type annotations and code completion for `#!python session.client("ce").get_cost_and_usage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_and_usage)

```python title="Method definition"
await def get_cost_and_usage(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    Granularity: GranularityType,  # (2)
    Metrics: Sequence[str],
    Filter: ExpressionTypeDef = ...,  # (3)
    GroupBy: Sequence[GroupDefinitionTypeDef] = ...,  # (4)
    NextPageToken: str = ...,
) -> GetCostAndUsageResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
3. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
4. See [:material-code-braces: GroupDefinitionTypeDef](./type_defs.md#groupdefinitiontypedef) 
5. See [:material-code-braces: GetCostAndUsageResponseTypeDef](./type_defs.md#getcostandusageresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetCostAndUsageRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
    "Granularity": ...,
    "Metrics": ...,
}

parent.get_cost_and_usage(**kwargs)
```

1. See [:material-code-braces: GetCostAndUsageRequestRequestTypeDef](./type_defs.md#getcostandusagerequestrequesttypedef) 

### get\_cost\_and\_usage\_with\_resources

Retrieves cost and usage metrics with resources for your account.

Type annotations and code completion for `#!python session.client("ce").get_cost_and_usage_with_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_and_usage_with_resources)

```python title="Method definition"
await def get_cost_and_usage_with_resources(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    Granularity: GranularityType,  # (2)
    Filter: ExpressionTypeDef,  # (3)
    Metrics: Sequence[str] = ...,
    GroupBy: Sequence[GroupDefinitionTypeDef] = ...,  # (4)
    NextPageToken: str = ...,
) -> GetCostAndUsageWithResourcesResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
3. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
4. See [:material-code-braces: GroupDefinitionTypeDef](./type_defs.md#groupdefinitiontypedef) 
5. See [:material-code-braces: GetCostAndUsageWithResourcesResponseTypeDef](./type_defs.md#getcostandusagewithresourcesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetCostAndUsageWithResourcesRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
    "Granularity": ...,
    "Filter": ...,
}

parent.get_cost_and_usage_with_resources(**kwargs)
```

1. See [:material-code-braces: GetCostAndUsageWithResourcesRequestRequestTypeDef](./type_defs.md#getcostandusagewithresourcesrequestrequesttypedef) 

### get\_cost\_categories

Retrieves an array of Cost Category names and values incurred cost.

Type annotations and code completion for `#!python session.client("ce").get_cost_categories` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_categories)

```python title="Method definition"
await def get_cost_categories(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    SearchString: str = ...,
    CostCategoryName: str = ...,
    Filter: ExpressionTypeDef = ...,  # (2)
    SortBy: Sequence[SortDefinitionTypeDef] = ...,  # (3)
    MaxResults: int = ...,
    NextPageToken: str = ...,
) -> GetCostCategoriesResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
3. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
4. See [:material-code-braces: GetCostCategoriesResponseTypeDef](./type_defs.md#getcostcategoriesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetCostCategoriesRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
}

parent.get_cost_categories(**kwargs)
```

1. See [:material-code-braces: GetCostCategoriesRequestRequestTypeDef](./type_defs.md#getcostcategoriesrequestrequesttypedef) 

### get\_cost\_forecast

Retrieves a forecast for how much Amazon Web Services predicts that you will
spend over the forecast time period that you select, based on your past costs.

Type annotations and code completion for `#!python session.client("ce").get_cost_forecast` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_forecast)

```python title="Method definition"
await def get_cost_forecast(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    Metric: MetricType,  # (2)
    Granularity: GranularityType,  # (3)
    Filter: ExpressionTypeDef = ...,  # (4)
    PredictionIntervalLevel: int = ...,
) -> GetCostForecastResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-brackets: MetricType](./literals.md#metrictype) 
3. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
4. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
5. See [:material-code-braces: GetCostForecastResponseTypeDef](./type_defs.md#getcostforecastresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetCostForecastRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
    "Metric": ...,
    "Granularity": ...,
}

parent.get_cost_forecast(**kwargs)
```

1. See [:material-code-braces: GetCostForecastRequestRequestTypeDef](./type_defs.md#getcostforecastrequestrequesttypedef) 

### get\_dimension\_values

Retrieves all available filter values for a specified filter over a period of
time.

Type annotations and code completion for `#!python session.client("ce").get_dimension_values` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_dimension_values)

```python title="Method definition"
await def get_dimension_values(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    Dimension: DimensionType,  # (2)
    SearchString: str = ...,
    Context: ContextType = ...,  # (3)
    Filter: ExpressionTypeDef = ...,  # (4)
    SortBy: Sequence[SortDefinitionTypeDef] = ...,  # (5)
    MaxResults: int = ...,
    NextPageToken: str = ...,
) -> GetDimensionValuesResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-brackets: DimensionType](./literals.md#dimensiontype) 
3. See [:material-code-brackets: ContextType](./literals.md#contexttype) 
4. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
5. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
6. See [:material-code-braces: GetDimensionValuesResponseTypeDef](./type_defs.md#getdimensionvaluesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetDimensionValuesRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
    "Dimension": ...,
}

parent.get_dimension_values(**kwargs)
```

1. See [:material-code-braces: GetDimensionValuesRequestRequestTypeDef](./type_defs.md#getdimensionvaluesrequestrequesttypedef) 

### get\_reservation\_coverage

Retrieves the reservation coverage for your account.

Type annotations and code completion for `#!python session.client("ce").get_reservation_coverage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_reservation_coverage)

```python title="Method definition"
await def get_reservation_coverage(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    GroupBy: Sequence[GroupDefinitionTypeDef] = ...,  # (2)
    Granularity: GranularityType = ...,  # (3)
    Filter: ExpressionTypeDef = ...,  # (4)
    Metrics: Sequence[str] = ...,
    NextPageToken: str = ...,
    SortBy: SortDefinitionTypeDef = ...,  # (5)
    MaxResults: int = ...,
) -> GetReservationCoverageResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: GroupDefinitionTypeDef](./type_defs.md#groupdefinitiontypedef) 
3. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
4. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
5. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
6. See [:material-code-braces: GetReservationCoverageResponseTypeDef](./type_defs.md#getreservationcoverageresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetReservationCoverageRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
}

parent.get_reservation_coverage(**kwargs)
```

1. See [:material-code-braces: GetReservationCoverageRequestRequestTypeDef](./type_defs.md#getreservationcoveragerequestrequesttypedef) 

### get\_reservation\_purchase\_recommendation

Gets recommendations for which reservations to purchase.

Type annotations and code completion for `#!python session.client("ce").get_reservation_purchase_recommendation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_reservation_purchase_recommendation)

```python title="Method definition"
await def get_reservation_purchase_recommendation(
    self,
    *,
    Service: str,
    AccountId: str = ...,
    Filter: ExpressionTypeDef = ...,  # (1)
    AccountScope: AccountScopeType = ...,  # (2)
    LookbackPeriodInDays: LookbackPeriodInDaysType = ...,  # (3)
    TermInYears: TermInYearsType = ...,  # (4)
    PaymentOption: PaymentOptionType = ...,  # (5)
    ServiceSpecification: ServiceSpecificationTypeDef = ...,  # (6)
    PageSize: int = ...,
    NextPageToken: str = ...,
) -> GetReservationPurchaseRecommendationResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
2. See [:material-code-brackets: AccountScopeType](./literals.md#accountscopetype) 
3. See [:material-code-brackets: LookbackPeriodInDaysType](./literals.md#lookbackperiodindaystype) 
4. See [:material-code-brackets: TermInYearsType](./literals.md#terminyearstype) 
5. See [:material-code-brackets: PaymentOptionType](./literals.md#paymentoptiontype) 
6. See [:material-code-braces: ServiceSpecificationTypeDef](./type_defs.md#servicespecificationtypedef) 
7. See [:material-code-braces: GetReservationPurchaseRecommendationResponseTypeDef](./type_defs.md#getreservationpurchaserecommendationresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetReservationPurchaseRecommendationRequestRequestTypeDef = {  # (1)
    "Service": ...,
}

parent.get_reservation_purchase_recommendation(**kwargs)
```

1. See [:material-code-braces: GetReservationPurchaseRecommendationRequestRequestTypeDef](./type_defs.md#getreservationpurchaserecommendationrequestrequesttypedef) 

### get\_reservation\_utilization

Retrieves the reservation utilization for your account.

Type annotations and code completion for `#!python session.client("ce").get_reservation_utilization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_reservation_utilization)

```python title="Method definition"
await def get_reservation_utilization(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    GroupBy: Sequence[GroupDefinitionTypeDef] = ...,  # (2)
    Granularity: GranularityType = ...,  # (3)
    Filter: ExpressionTypeDef = ...,  # (4)
    SortBy: SortDefinitionTypeDef = ...,  # (5)
    NextPageToken: str = ...,
    MaxResults: int = ...,
) -> GetReservationUtilizationResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: GroupDefinitionTypeDef](./type_defs.md#groupdefinitiontypedef) 
3. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
4. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
5. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
6. See [:material-code-braces: GetReservationUtilizationResponseTypeDef](./type_defs.md#getreservationutilizationresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetReservationUtilizationRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
}

parent.get_reservation_utilization(**kwargs)
```

1. See [:material-code-braces: GetReservationUtilizationRequestRequestTypeDef](./type_defs.md#getreservationutilizationrequestrequesttypedef) 

### get\_rightsizing\_recommendation

Creates recommendations that help you save cost by identifying idle and
underutilized Amazon EC2 instances.

Type annotations and code completion for `#!python session.client("ce").get_rightsizing_recommendation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_rightsizing_recommendation)

```python title="Method definition"
await def get_rightsizing_recommendation(
    self,
    *,
    Service: str,
    Filter: ExpressionTypeDef = ...,  # (1)
    Configuration: RightsizingRecommendationConfigurationTypeDef = ...,  # (2)
    PageSize: int = ...,
    NextPageToken: str = ...,
) -> GetRightsizingRecommendationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
2. See [:material-code-braces: RightsizingRecommendationConfigurationTypeDef](./type_defs.md#rightsizingrecommendationconfigurationtypedef) 
3. See [:material-code-braces: GetRightsizingRecommendationResponseTypeDef](./type_defs.md#getrightsizingrecommendationresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetRightsizingRecommendationRequestRequestTypeDef = {  # (1)
    "Service": ...,
}

parent.get_rightsizing_recommendation(**kwargs)
```

1. See [:material-code-braces: GetRightsizingRecommendationRequestRequestTypeDef](./type_defs.md#getrightsizingrecommendationrequestrequesttypedef) 

### get\_savings\_plans\_coverage

Retrieves the Savings Plans covered for your account.

Type annotations and code completion for `#!python session.client("ce").get_savings_plans_coverage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_coverage)

```python title="Method definition"
await def get_savings_plans_coverage(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    GroupBy: Sequence[GroupDefinitionTypeDef] = ...,  # (2)
    Granularity: GranularityType = ...,  # (3)
    Filter: ExpressionTypeDef = ...,  # (4)
    Metrics: Sequence[str] = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    SortBy: SortDefinitionTypeDef = ...,  # (5)
) -> GetSavingsPlansCoverageResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: GroupDefinitionTypeDef](./type_defs.md#groupdefinitiontypedef) 
3. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
4. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
5. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
6. See [:material-code-braces: GetSavingsPlansCoverageResponseTypeDef](./type_defs.md#getsavingsplanscoverageresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetSavingsPlansCoverageRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
}

parent.get_savings_plans_coverage(**kwargs)
```

1. See [:material-code-braces: GetSavingsPlansCoverageRequestRequestTypeDef](./type_defs.md#getsavingsplanscoveragerequestrequesttypedef) 

### get\_savings\_plans\_purchase\_recommendation

Retrieves your request parameters, Savings Plan Recommendations Summary and
Details.

Type annotations and code completion for `#!python session.client("ce").get_savings_plans_purchase_recommendation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_purchase_recommendation)

```python title="Method definition"
await def get_savings_plans_purchase_recommendation(
    self,
    *,
    SavingsPlansType: SupportedSavingsPlansTypeType,  # (1)
    TermInYears: TermInYearsType,  # (2)
    PaymentOption: PaymentOptionType,  # (3)
    LookbackPeriodInDays: LookbackPeriodInDaysType,  # (4)
    AccountScope: AccountScopeType = ...,  # (5)
    NextPageToken: str = ...,
    PageSize: int = ...,
    Filter: ExpressionTypeDef = ...,  # (6)
) -> GetSavingsPlansPurchaseRecommendationResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: SupportedSavingsPlansTypeType](./literals.md#supportedsavingsplanstypetype) 
2. See [:material-code-brackets: TermInYearsType](./literals.md#terminyearstype) 
3. See [:material-code-brackets: PaymentOptionType](./literals.md#paymentoptiontype) 
4. See [:material-code-brackets: LookbackPeriodInDaysType](./literals.md#lookbackperiodindaystype) 
5. See [:material-code-brackets: AccountScopeType](./literals.md#accountscopetype) 
6. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
7. See [:material-code-braces: GetSavingsPlansPurchaseRecommendationResponseTypeDef](./type_defs.md#getsavingsplanspurchaserecommendationresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef = {  # (1)
    "SavingsPlansType": ...,
    "TermInYears": ...,
    "PaymentOption": ...,
    "LookbackPeriodInDays": ...,
}

parent.get_savings_plans_purchase_recommendation(**kwargs)
```

1. See [:material-code-braces: GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef](./type_defs.md#getsavingsplanspurchaserecommendationrequestrequesttypedef) 

### get\_savings\_plans\_utilization

Retrieves the Savings Plans utilization for your account across date ranges with
daily or monthly granularity.

Type annotations and code completion for `#!python session.client("ce").get_savings_plans_utilization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_utilization)

```python title="Method definition"
await def get_savings_plans_utilization(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    Granularity: GranularityType = ...,  # (2)
    Filter: ExpressionTypeDef = ...,  # (3)
    SortBy: SortDefinitionTypeDef = ...,  # (4)
) -> GetSavingsPlansUtilizationResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
3. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
4. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
5. See [:material-code-braces: GetSavingsPlansUtilizationResponseTypeDef](./type_defs.md#getsavingsplansutilizationresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetSavingsPlansUtilizationRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
}

parent.get_savings_plans_utilization(**kwargs)
```

1. See [:material-code-braces: GetSavingsPlansUtilizationRequestRequestTypeDef](./type_defs.md#getsavingsplansutilizationrequestrequesttypedef) 

### get\_savings\_plans\_utilization\_details

Retrieves attribute data along with aggregate utilization and savings data for a
given time period.

Type annotations and code completion for `#!python session.client("ce").get_savings_plans_utilization_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_utilization_details)

```python title="Method definition"
await def get_savings_plans_utilization_details(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    Filter: ExpressionTypeDef = ...,  # (2)
    DataType: Sequence[SavingsPlansDataTypeType] = ...,  # (3)
    NextToken: str = ...,
    MaxResults: int = ...,
    SortBy: SortDefinitionTypeDef = ...,  # (4)
) -> GetSavingsPlansUtilizationDetailsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
3. See [:material-code-brackets: SavingsPlansDataTypeType](./literals.md#savingsplansdatatypetype) 
4. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
5. See [:material-code-braces: GetSavingsPlansUtilizationDetailsResponseTypeDef](./type_defs.md#getsavingsplansutilizationdetailsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetSavingsPlansUtilizationDetailsRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
}

parent.get_savings_plans_utilization_details(**kwargs)
```

1. See [:material-code-braces: GetSavingsPlansUtilizationDetailsRequestRequestTypeDef](./type_defs.md#getsavingsplansutilizationdetailsrequestrequesttypedef) 

### get\_tags

Queries for available tag keys and tag values for a specified period.

Type annotations and code completion for `#!python session.client("ce").get_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_tags)

```python title="Method definition"
await def get_tags(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    SearchString: str = ...,
    TagKey: str = ...,
    Filter: ExpressionTypeDef = ...,  # (2)
    SortBy: Sequence[SortDefinitionTypeDef] = ...,  # (3)
    MaxResults: int = ...,
    NextPageToken: str = ...,
) -> GetTagsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
3. See [:material-code-braces: SortDefinitionTypeDef](./type_defs.md#sortdefinitiontypedef) 
4. See [:material-code-braces: GetTagsResponseTypeDef](./type_defs.md#gettagsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetTagsRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
}

parent.get_tags(**kwargs)
```

1. See [:material-code-braces: GetTagsRequestRequestTypeDef](./type_defs.md#gettagsrequestrequesttypedef) 

### get\_usage\_forecast

Retrieves a forecast for how much Amazon Web Services predicts that you will use
over the forecast time period that you select, based on your past usage.

Type annotations and code completion for `#!python session.client("ce").get_usage_forecast` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_usage_forecast)

```python title="Method definition"
await def get_usage_forecast(
    self,
    *,
    TimePeriod: DateIntervalTypeDef,  # (1)
    Metric: MetricType,  # (2)
    Granularity: GranularityType,  # (3)
    Filter: ExpressionTypeDef = ...,  # (4)
    PredictionIntervalLevel: int = ...,
) -> GetUsageForecastResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
2. See [:material-code-brackets: MetricType](./literals.md#metrictype) 
3. See [:material-code-brackets: GranularityType](./literals.md#granularitytype) 
4. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) 
5. See [:material-code-braces: GetUsageForecastResponseTypeDef](./type_defs.md#getusageforecastresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetUsageForecastRequestRequestTypeDef = {  # (1)
    "TimePeriod": ...,
    "Metric": ...,
    "Granularity": ...,
}

parent.get_usage_forecast(**kwargs)
```

1. See [:material-code-braces: GetUsageForecastRequestRequestTypeDef](./type_defs.md#getusageforecastrequestrequesttypedef) 

### list\_cost\_category\_definitions

Returns the name, ARN, `NumberOfRules` and effective dates of all Cost
Categories defined in the account.

Type annotations and code completion for `#!python session.client("ce").list_cost_category_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.list_cost_category_definitions)

```python title="Method definition"
await def list_cost_category_definitions(
    self,
    *,
    EffectiveOn: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListCostCategoryDefinitionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCostCategoryDefinitionsResponseTypeDef](./type_defs.md#listcostcategorydefinitionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCostCategoryDefinitionsRequestRequestTypeDef = {  # (1)
    "EffectiveOn": ...,
}

parent.list_cost_category_definitions(**kwargs)
```

1. See [:material-code-braces: ListCostCategoryDefinitionsRequestRequestTypeDef](./type_defs.md#listcostcategorydefinitionsrequestrequesttypedef) 

### provide\_anomaly\_feedback

Modifies the feedback property of a given cost anomaly.

Type annotations and code completion for `#!python session.client("ce").provide_anomaly_feedback` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.provide_anomaly_feedback)

```python title="Method definition"
await def provide_anomaly_feedback(
    self,
    *,
    AnomalyId: str,
    Feedback: AnomalyFeedbackTypeType,  # (1)
) -> ProvideAnomalyFeedbackResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AnomalyFeedbackTypeType](./literals.md#anomalyfeedbacktypetype) 
2. See [:material-code-braces: ProvideAnomalyFeedbackResponseTypeDef](./type_defs.md#provideanomalyfeedbackresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ProvideAnomalyFeedbackRequestRequestTypeDef = {  # (1)
    "AnomalyId": ...,
    "Feedback": ...,
}

parent.provide_anomaly_feedback(**kwargs)
```

1. See [:material-code-braces: ProvideAnomalyFeedbackRequestRequestTypeDef](./type_defs.md#provideanomalyfeedbackrequestrequesttypedef) 

### update\_anomaly\_monitor

Updates an existing cost anomaly monitor.

Type annotations and code completion for `#!python session.client("ce").update_anomaly_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_anomaly_monitor)

```python title="Method definition"
await def update_anomaly_monitor(
    self,
    *,
    MonitorArn: str,
    MonitorName: str = ...,
) -> UpdateAnomalyMonitorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateAnomalyMonitorResponseTypeDef](./type_defs.md#updateanomalymonitorresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: UpdateAnomalyMonitorRequestRequestTypeDef = {  # (1)
    "MonitorArn": ...,
}

parent.update_anomaly_monitor(**kwargs)
```

1. See [:material-code-braces: UpdateAnomalyMonitorRequestRequestTypeDef](./type_defs.md#updateanomalymonitorrequestrequesttypedef) 

### update\_anomaly\_subscription

Updates an existing cost anomaly monitor subscription.

Type annotations and code completion for `#!python session.client("ce").update_anomaly_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_anomaly_subscription)

```python title="Method definition"
await def update_anomaly_subscription(
    self,
    *,
    SubscriptionArn: str,
    Threshold: float = ...,
    Frequency: AnomalySubscriptionFrequencyType = ...,  # (1)
    MonitorArnList: Sequence[str] = ...,
    Subscribers: Sequence[SubscriberTypeDef] = ...,  # (2)
    SubscriptionName: str = ...,
) -> UpdateAnomalySubscriptionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AnomalySubscriptionFrequencyType](./literals.md#anomalysubscriptionfrequencytype) 
2. See [:material-code-braces: SubscriberTypeDef](./type_defs.md#subscribertypedef) 
3. See [:material-code-braces: UpdateAnomalySubscriptionResponseTypeDef](./type_defs.md#updateanomalysubscriptionresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: UpdateAnomalySubscriptionRequestRequestTypeDef = {  # (1)
    "SubscriptionArn": ...,
}

parent.update_anomaly_subscription(**kwargs)
```

1. See [:material-code-braces: UpdateAnomalySubscriptionRequestRequestTypeDef](./type_defs.md#updateanomalysubscriptionrequestrequesttypedef) 

### update\_cost\_category\_definition

Updates an existing Cost Category.

Type annotations and code completion for `#!python session.client("ce").update_cost_category_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_cost_category_definition)

```python title="Method definition"
await def update_cost_category_definition(
    self,
    *,
    CostCategoryArn: str,
    RuleVersion: CostCategoryRuleVersionType,  # (1)
    Rules: Sequence[CostCategoryRuleTypeDef],  # (2)
    DefaultValue: str = ...,
    SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...,  # (3)
) -> UpdateCostCategoryDefinitionResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: CostCategoryRuleVersionType](./literals.md#costcategoryruleversiontype) 
2. See [:material-code-braces: CostCategoryRuleTypeDef](./type_defs.md#costcategoryruletypedef) 
3. See [:material-code-braces: CostCategorySplitChargeRuleTypeDef](./type_defs.md#costcategorysplitchargeruletypedef) 
4. See [:material-code-braces: UpdateCostCategoryDefinitionResponseTypeDef](./type_defs.md#updatecostcategorydefinitionresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: UpdateCostCategoryDefinitionRequestRequestTypeDef = {  # (1)
    "CostCategoryArn": ...,
    "RuleVersion": ...,
    "Rules": ...,
}

parent.update_cost_category_definition(**kwargs)
```

1. See [:material-code-braces: UpdateCostCategoryDefinitionRequestRequestTypeDef](./type_defs.md#updatecostcategorydefinitionrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("ce").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> CostExplorerClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("ce").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





