# Type definitions

> [Index](../README.md) > [CostOptimizationHub](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CostOptimizationHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub)
    type annotations stubs module [types-aiobotocore-cost-optimization-hub](https://pypi.org/project/types-aiobotocore-cost-optimization-hub/).



## AccountEnrollmentStatusTypeDef

```python
# AccountEnrollmentStatusTypeDef definition

class AccountEnrollmentStatusTypeDef(TypedDict):
    accountId: NotRequired[str],
    createdTimestamp: NotRequired[datetime],
    lastUpdatedTimestamp: NotRequired[datetime],
    status: NotRequired[EnrollmentStatusType],  # (1)
```

1. See [:material-code-brackets: EnrollmentStatusType](./literals.md#enrollmentstatustype) 
## BlockStoragePerformanceConfigurationTypeDef

```python
# BlockStoragePerformanceConfigurationTypeDef definition

class BlockStoragePerformanceConfigurationTypeDef(TypedDict):
    iops: NotRequired[float],
    throughput: NotRequired[float],
```

## ComputeConfigurationTypeDef

```python
# ComputeConfigurationTypeDef definition

class ComputeConfigurationTypeDef(TypedDict):
    architecture: NotRequired[str],
    memorySizeInMB: NotRequired[int],
    platform: NotRequired[str],
    vCpu: NotRequired[float],
```

## ComputeSavingsPlansConfigurationTypeDef

```python
# ComputeSavingsPlansConfigurationTypeDef definition

class ComputeSavingsPlansConfigurationTypeDef(TypedDict):
    accountScope: NotRequired[str],
    hourlyCommitment: NotRequired[str],
    paymentOption: NotRequired[str],
    term: NotRequired[str],
```

## StorageConfigurationTypeDef

```python
# StorageConfigurationTypeDef definition

class StorageConfigurationTypeDef(TypedDict):
    sizeInGb: NotRequired[float],
    type: NotRequired[str],
```

## InstanceConfigurationTypeDef

```python
# InstanceConfigurationTypeDef definition

class InstanceConfigurationTypeDef(TypedDict):
    type: NotRequired[str],
```

## Ec2InstanceSavingsPlansConfigurationTypeDef

```python
# Ec2InstanceSavingsPlansConfigurationTypeDef definition

class Ec2InstanceSavingsPlansConfigurationTypeDef(TypedDict):
    accountScope: NotRequired[str],
    hourlyCommitment: NotRequired[str],
    instanceFamily: NotRequired[str],
    paymentOption: NotRequired[str],
    savingsPlansRegion: NotRequired[str],
    term: NotRequired[str],
```

## Ec2ReservedInstancesConfigurationTypeDef

```python
# Ec2ReservedInstancesConfigurationTypeDef definition

class Ec2ReservedInstancesConfigurationTypeDef(TypedDict):
    accountScope: NotRequired[str],
    currentGeneration: NotRequired[str],
    instanceFamily: NotRequired[str],
    instanceType: NotRequired[str],
    monthlyRecurringCost: NotRequired[str],
    normalizedUnitsToPurchase: NotRequired[str],
    numberOfInstancesToPurchase: NotRequired[str],
    offeringClass: NotRequired[str],
    paymentOption: NotRequired[str],
    platform: NotRequired[str],
    reservedInstancesRegion: NotRequired[str],
    service: NotRequired[str],
    sizeFlexEligible: NotRequired[bool],
    tenancy: NotRequired[str],
    term: NotRequired[str],
    upfrontCost: NotRequired[str],
```

## ElastiCacheReservedInstancesConfigurationTypeDef

```python
# ElastiCacheReservedInstancesConfigurationTypeDef definition

class ElastiCacheReservedInstancesConfigurationTypeDef(TypedDict):
    accountScope: NotRequired[str],
    currentGeneration: NotRequired[str],
    instanceFamily: NotRequired[str],
    instanceType: NotRequired[str],
    monthlyRecurringCost: NotRequired[str],
    normalizedUnitsToPurchase: NotRequired[str],
    numberOfInstancesToPurchase: NotRequired[str],
    paymentOption: NotRequired[str],
    reservedInstancesRegion: NotRequired[str],
    service: NotRequired[str],
    sizeFlexEligible: NotRequired[bool],
    term: NotRequired[str],
    upfrontCost: NotRequired[str],
```

## EstimatedDiscountsTypeDef

```python
# EstimatedDiscountsTypeDef definition

class EstimatedDiscountsTypeDef(TypedDict):
    otherDiscount: NotRequired[float],
    reservedInstancesDiscount: NotRequired[float],
    savingsPlansDiscount: NotRequired[float],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## GetRecommendationRequestRequestTypeDef

```python
# GetRecommendationRequestRequestTypeDef definition

class GetRecommendationRequestRequestTypeDef(TypedDict):
    recommendationId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListEnrollmentStatusesRequestRequestTypeDef

```python
# ListEnrollmentStatusesRequestRequestTypeDef definition

class ListEnrollmentStatusesRequestRequestTypeDef(TypedDict):
    accountId: NotRequired[str],
    includeOrganizationInfo: NotRequired[bool],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## RecommendationSummaryTypeDef

```python
# RecommendationSummaryTypeDef definition

class RecommendationSummaryTypeDef(TypedDict):
    estimatedMonthlySavings: NotRequired[float],
    group: NotRequired[str],
    recommendationCount: NotRequired[int],
```

## OrderByTypeDef

```python
# OrderByTypeDef definition

class OrderByTypeDef(TypedDict):
    dimension: NotRequired[str],
    order: NotRequired[OrderType],  # (1)
```

1. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
## OpenSearchReservedInstancesConfigurationTypeDef

```python
# OpenSearchReservedInstancesConfigurationTypeDef definition

class OpenSearchReservedInstancesConfigurationTypeDef(TypedDict):
    accountScope: NotRequired[str],
    currentGeneration: NotRequired[str],
    instanceType: NotRequired[str],
    monthlyRecurringCost: NotRequired[str],
    normalizedUnitsToPurchase: NotRequired[str],
    numberOfInstancesToPurchase: NotRequired[str],
    paymentOption: NotRequired[str],
    reservedInstancesRegion: NotRequired[str],
    service: NotRequired[str],
    sizeFlexEligible: NotRequired[bool],
    term: NotRequired[str],
    upfrontCost: NotRequired[str],
```

## RdsReservedInstancesConfigurationTypeDef

```python
# RdsReservedInstancesConfigurationTypeDef definition

class RdsReservedInstancesConfigurationTypeDef(TypedDict):
    accountScope: NotRequired[str],
    currentGeneration: NotRequired[str],
    databaseEdition: NotRequired[str],
    databaseEngine: NotRequired[str],
    deploymentOption: NotRequired[str],
    instanceFamily: NotRequired[str],
    instanceType: NotRequired[str],
    licenseModel: NotRequired[str],
    monthlyRecurringCost: NotRequired[str],
    normalizedUnitsToPurchase: NotRequired[str],
    numberOfInstancesToPurchase: NotRequired[str],
    paymentOption: NotRequired[str],
    reservedInstancesRegion: NotRequired[str],
    service: NotRequired[str],
    sizeFlexEligible: NotRequired[bool],
    term: NotRequired[str],
    upfrontCost: NotRequired[str],
```

## RedshiftReservedInstancesConfigurationTypeDef

```python
# RedshiftReservedInstancesConfigurationTypeDef definition

class RedshiftReservedInstancesConfigurationTypeDef(TypedDict):
    accountScope: NotRequired[str],
    currentGeneration: NotRequired[str],
    instanceFamily: NotRequired[str],
    instanceType: NotRequired[str],
    monthlyRecurringCost: NotRequired[str],
    normalizedUnitsToPurchase: NotRequired[str],
    numberOfInstancesToPurchase: NotRequired[str],
    paymentOption: NotRequired[str],
    reservedInstancesRegion: NotRequired[str],
    service: NotRequired[str],
    sizeFlexEligible: NotRequired[bool],
    term: NotRequired[str],
    upfrontCost: NotRequired[str],
```

## ReservedInstancesPricingTypeDef

```python
# ReservedInstancesPricingTypeDef definition

class ReservedInstancesPricingTypeDef(TypedDict):
    estimatedMonthlyAmortizedReservationCost: NotRequired[float],
    estimatedOnDemandCost: NotRequired[float],
    monthlyReservationEligibleCost: NotRequired[float],
    savingsPercentage: NotRequired[float],
```

## UsageTypeDef

```python
# UsageTypeDef definition

class UsageTypeDef(TypedDict):
    operation: NotRequired[str],
    productCode: NotRequired[str],
    unit: NotRequired[str],
    usageAmount: NotRequired[float],
    usageType: NotRequired[str],
```

## SageMakerSavingsPlansConfigurationTypeDef

```python
# SageMakerSavingsPlansConfigurationTypeDef definition

class SageMakerSavingsPlansConfigurationTypeDef(TypedDict):
    accountScope: NotRequired[str],
    hourlyCommitment: NotRequired[str],
    paymentOption: NotRequired[str],
    term: NotRequired[str],
```

## SavingsPlansPricingTypeDef

```python
# SavingsPlansPricingTypeDef definition

class SavingsPlansPricingTypeDef(TypedDict):
    estimatedMonthlyCommitment: NotRequired[float],
    estimatedOnDemandCost: NotRequired[float],
    monthlySavingsPlansEligibleCost: NotRequired[float],
    savingsPercentage: NotRequired[float],
```

## UpdateEnrollmentStatusRequestRequestTypeDef

```python
# UpdateEnrollmentStatusRequestRequestTypeDef definition

class UpdateEnrollmentStatusRequestRequestTypeDef(TypedDict):
    status: EnrollmentStatusType,  # (1)
    includeMemberAccounts: NotRequired[bool],
```

1. See [:material-code-brackets: EnrollmentStatusType](./literals.md#enrollmentstatustype) 
## UpdatePreferencesRequestRequestTypeDef

```python
# UpdatePreferencesRequestRequestTypeDef definition

class UpdatePreferencesRequestRequestTypeDef(TypedDict):
    memberAccountDiscountVisibility: NotRequired[MemberAccountDiscountVisibilityType],  # (1)
    savingsEstimationMode: NotRequired[SavingsEstimationModeType],  # (2)
```

1. See [:material-code-brackets: MemberAccountDiscountVisibilityType](./literals.md#memberaccountdiscountvisibilitytype) 
2. See [:material-code-brackets: SavingsEstimationModeType](./literals.md#savingsestimationmodetype) 
## EcsServiceConfigurationTypeDef

```python
# EcsServiceConfigurationTypeDef definition

class EcsServiceConfigurationTypeDef(TypedDict):
    compute: NotRequired[ComputeConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ComputeConfigurationTypeDef](./type_defs.md#computeconfigurationtypedef) 
## LambdaFunctionConfigurationTypeDef

```python
# LambdaFunctionConfigurationTypeDef definition

class LambdaFunctionConfigurationTypeDef(TypedDict):
    compute: NotRequired[ComputeConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ComputeConfigurationTypeDef](./type_defs.md#computeconfigurationtypedef) 
## EbsVolumeConfigurationTypeDef

```python
# EbsVolumeConfigurationTypeDef definition

class EbsVolumeConfigurationTypeDef(TypedDict):
    attachmentState: NotRequired[str],
    performance: NotRequired[BlockStoragePerformanceConfigurationTypeDef],  # (1)
    storage: NotRequired[StorageConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: BlockStoragePerformanceConfigurationTypeDef](./type_defs.md#blockstorageperformanceconfigurationtypedef) 
2. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
## Ec2AutoScalingGroupConfigurationTypeDef

```python
# Ec2AutoScalingGroupConfigurationTypeDef definition

class Ec2AutoScalingGroupConfigurationTypeDef(TypedDict):
    instance: NotRequired[InstanceConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceConfigurationTypeDef](./type_defs.md#instanceconfigurationtypedef) 
## Ec2InstanceConfigurationTypeDef

```python
# Ec2InstanceConfigurationTypeDef definition

class Ec2InstanceConfigurationTypeDef(TypedDict):
    instance: NotRequired[InstanceConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceConfigurationTypeDef](./type_defs.md#instanceconfigurationtypedef) 
## ResourcePricingTypeDef

```python
# ResourcePricingTypeDef definition

class ResourcePricingTypeDef(TypedDict):
    estimatedCostAfterDiscounts: NotRequired[float],
    estimatedCostBeforeDiscounts: NotRequired[float],
    estimatedDiscounts: NotRequired[EstimatedDiscountsTypeDef],  # (1)
    estimatedNetUnusedAmortizedCommitments: NotRequired[float],
```

1. See [:material-code-braces: EstimatedDiscountsTypeDef](./type_defs.md#estimateddiscountstypedef) 
## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    accountIds: NotRequired[Sequence[str]],
    actionTypes: NotRequired[Sequence[ActionTypeType]],  # (1)
    implementationEfforts: NotRequired[Sequence[ImplementationEffortType]],  # (2)
    recommendationIds: NotRequired[Sequence[str]],
    regions: NotRequired[Sequence[str]],
    resourceArns: NotRequired[Sequence[str]],
    resourceIds: NotRequired[Sequence[str]],
    resourceTypes: NotRequired[Sequence[ResourceTypeType]],  # (3)
    restartNeeded: NotRequired[bool],
    rollbackPossible: NotRequired[bool],
    tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
2. See [:material-code-brackets: ImplementationEffortType](./literals.md#implementationefforttype) 
3. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## RecommendationTypeDef

```python
# RecommendationTypeDef definition

class RecommendationTypeDef(TypedDict):
    accountId: NotRequired[str],
    actionType: NotRequired[str],
    currencyCode: NotRequired[str],
    currentResourceSummary: NotRequired[str],
    currentResourceType: NotRequired[str],
    estimatedMonthlyCost: NotRequired[float],
    estimatedMonthlySavings: NotRequired[float],
    estimatedSavingsPercentage: NotRequired[float],
    implementationEffort: NotRequired[str],
    lastRefreshTimestamp: NotRequired[datetime],
    recommendationId: NotRequired[str],
    recommendationLookbackPeriodInDays: NotRequired[int],
    recommendedResourceSummary: NotRequired[str],
    recommendedResourceType: NotRequired[str],
    region: NotRequired[str],
    resourceArn: NotRequired[str],
    resourceId: NotRequired[str],
    restartNeeded: NotRequired[bool],
    rollbackPossible: NotRequired[bool],
    source: NotRequired[SourceType],  # (1)
    tags: NotRequired[List[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: SourceType](./literals.md#sourcetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetPreferencesResponseTypeDef

```python
# GetPreferencesResponseTypeDef definition

class GetPreferencesResponseTypeDef(TypedDict):
    memberAccountDiscountVisibility: MemberAccountDiscountVisibilityType,  # (1)
    savingsEstimationMode: SavingsEstimationModeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: MemberAccountDiscountVisibilityType](./literals.md#memberaccountdiscountvisibilitytype) 
2. See [:material-code-brackets: SavingsEstimationModeType](./literals.md#savingsestimationmodetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnrollmentStatusesResponseTypeDef

```python
# ListEnrollmentStatusesResponseTypeDef definition

class ListEnrollmentStatusesResponseTypeDef(TypedDict):
    items: List[AccountEnrollmentStatusTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountEnrollmentStatusTypeDef](./type_defs.md#accountenrollmentstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEnrollmentStatusResponseTypeDef

```python
# UpdateEnrollmentStatusResponseTypeDef definition

class UpdateEnrollmentStatusResponseTypeDef(TypedDict):
    status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePreferencesResponseTypeDef

```python
# UpdatePreferencesResponseTypeDef definition

class UpdatePreferencesResponseTypeDef(TypedDict):
    memberAccountDiscountVisibility: MemberAccountDiscountVisibilityType,  # (1)
    savingsEstimationMode: SavingsEstimationModeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: MemberAccountDiscountVisibilityType](./literals.md#memberaccountdiscountvisibilitytype) 
2. See [:material-code-brackets: SavingsEstimationModeType](./literals.md#savingsestimationmodetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnrollmentStatusesRequestListEnrollmentStatusesPaginateTypeDef

```python
# ListEnrollmentStatusesRequestListEnrollmentStatusesPaginateTypeDef definition

class ListEnrollmentStatusesRequestListEnrollmentStatusesPaginateTypeDef(TypedDict):
    accountId: NotRequired[str],
    includeOrganizationInfo: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecommendationSummariesResponseTypeDef

```python
# ListRecommendationSummariesResponseTypeDef definition

class ListRecommendationSummariesResponseTypeDef(TypedDict):
    currencyCode: str,
    estimatedTotalDedupedSavings: float,
    groupBy: str,
    items: List[RecommendationSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecommendationSummaryTypeDef](./type_defs.md#recommendationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReservedInstancesCostCalculationTypeDef

```python
# ReservedInstancesCostCalculationTypeDef definition

class ReservedInstancesCostCalculationTypeDef(TypedDict):
    pricing: NotRequired[ReservedInstancesPricingTypeDef],  # (1)
```

1. See [:material-code-braces: ReservedInstancesPricingTypeDef](./type_defs.md#reservedinstancespricingtypedef) 
## SavingsPlansCostCalculationTypeDef

```python
# SavingsPlansCostCalculationTypeDef definition

class SavingsPlansCostCalculationTypeDef(TypedDict):
    pricing: NotRequired[SavingsPlansPricingTypeDef],  # (1)
```

1. See [:material-code-braces: SavingsPlansPricingTypeDef](./type_defs.md#savingsplanspricingtypedef) 
## ResourceCostCalculationTypeDef

```python
# ResourceCostCalculationTypeDef definition

class ResourceCostCalculationTypeDef(TypedDict):
    pricing: NotRequired[ResourcePricingTypeDef],  # (1)
    usages: NotRequired[List[UsageTypeDef]],  # (2)
```

1. See [:material-code-braces: ResourcePricingTypeDef](./type_defs.md#resourcepricingtypedef) 
2. See [:material-code-braces: UsageTypeDef](./type_defs.md#usagetypedef) 
## ListRecommendationSummariesRequestListRecommendationSummariesPaginateTypeDef

```python
# ListRecommendationSummariesRequestListRecommendationSummariesPaginateTypeDef definition

class ListRecommendationSummariesRequestListRecommendationSummariesPaginateTypeDef(TypedDict):
    groupBy: str,
    filter: NotRequired[FilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecommendationSummariesRequestRequestTypeDef

```python
# ListRecommendationSummariesRequestRequestTypeDef definition

class ListRecommendationSummariesRequestRequestTypeDef(TypedDict):
    groupBy: str,
    filter: NotRequired[FilterTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListRecommendationsRequestListRecommendationsPaginateTypeDef

```python
# ListRecommendationsRequestListRecommendationsPaginateTypeDef definition

class ListRecommendationsRequestListRecommendationsPaginateTypeDef(TypedDict):
    filter: NotRequired[FilterTypeDef],  # (1)
    includeAllRecommendations: NotRequired[bool],
    orderBy: NotRequired[OrderByTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: OrderByTypeDef](./type_defs.md#orderbytypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecommendationsRequestRequestTypeDef

```python
# ListRecommendationsRequestRequestTypeDef definition

class ListRecommendationsRequestRequestTypeDef(TypedDict):
    filter: NotRequired[FilterTypeDef],  # (1)
    includeAllRecommendations: NotRequired[bool],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    orderBy: NotRequired[OrderByTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: OrderByTypeDef](./type_defs.md#orderbytypedef) 
## ListRecommendationsResponseTypeDef

```python
# ListRecommendationsResponseTypeDef definition

class ListRecommendationsResponseTypeDef(TypedDict):
    items: List[RecommendationTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecommendationTypeDef](./type_defs.md#recommendationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## Ec2ReservedInstancesTypeDef

```python
# Ec2ReservedInstancesTypeDef definition

class Ec2ReservedInstancesTypeDef(TypedDict):
    configuration: NotRequired[Ec2ReservedInstancesConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ReservedInstancesCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: Ec2ReservedInstancesConfigurationTypeDef](./type_defs.md#ec2reservedinstancesconfigurationtypedef) 
2. See [:material-code-braces: ReservedInstancesCostCalculationTypeDef](./type_defs.md#reservedinstancescostcalculationtypedef) 
## ElastiCacheReservedInstancesTypeDef

```python
# ElastiCacheReservedInstancesTypeDef definition

class ElastiCacheReservedInstancesTypeDef(TypedDict):
    configuration: NotRequired[ElastiCacheReservedInstancesConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ReservedInstancesCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: ElastiCacheReservedInstancesConfigurationTypeDef](./type_defs.md#elasticachereservedinstancesconfigurationtypedef) 
2. See [:material-code-braces: ReservedInstancesCostCalculationTypeDef](./type_defs.md#reservedinstancescostcalculationtypedef) 
## OpenSearchReservedInstancesTypeDef

```python
# OpenSearchReservedInstancesTypeDef definition

class OpenSearchReservedInstancesTypeDef(TypedDict):
    configuration: NotRequired[OpenSearchReservedInstancesConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ReservedInstancesCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: OpenSearchReservedInstancesConfigurationTypeDef](./type_defs.md#opensearchreservedinstancesconfigurationtypedef) 
2. See [:material-code-braces: ReservedInstancesCostCalculationTypeDef](./type_defs.md#reservedinstancescostcalculationtypedef) 
## RdsReservedInstancesTypeDef

```python
# RdsReservedInstancesTypeDef definition

class RdsReservedInstancesTypeDef(TypedDict):
    configuration: NotRequired[RdsReservedInstancesConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ReservedInstancesCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: RdsReservedInstancesConfigurationTypeDef](./type_defs.md#rdsreservedinstancesconfigurationtypedef) 
2. See [:material-code-braces: ReservedInstancesCostCalculationTypeDef](./type_defs.md#reservedinstancescostcalculationtypedef) 
## RedshiftReservedInstancesTypeDef

```python
# RedshiftReservedInstancesTypeDef definition

class RedshiftReservedInstancesTypeDef(TypedDict):
    configuration: NotRequired[RedshiftReservedInstancesConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ReservedInstancesCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: RedshiftReservedInstancesConfigurationTypeDef](./type_defs.md#redshiftreservedinstancesconfigurationtypedef) 
2. See [:material-code-braces: ReservedInstancesCostCalculationTypeDef](./type_defs.md#reservedinstancescostcalculationtypedef) 
## ComputeSavingsPlansTypeDef

```python
# ComputeSavingsPlansTypeDef definition

class ComputeSavingsPlansTypeDef(TypedDict):
    configuration: NotRequired[ComputeSavingsPlansConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[SavingsPlansCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: ComputeSavingsPlansConfigurationTypeDef](./type_defs.md#computesavingsplansconfigurationtypedef) 
2. See [:material-code-braces: SavingsPlansCostCalculationTypeDef](./type_defs.md#savingsplanscostcalculationtypedef) 
## Ec2InstanceSavingsPlansTypeDef

```python
# Ec2InstanceSavingsPlansTypeDef definition

class Ec2InstanceSavingsPlansTypeDef(TypedDict):
    configuration: NotRequired[Ec2InstanceSavingsPlansConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[SavingsPlansCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: Ec2InstanceSavingsPlansConfigurationTypeDef](./type_defs.md#ec2instancesavingsplansconfigurationtypedef) 
2. See [:material-code-braces: SavingsPlansCostCalculationTypeDef](./type_defs.md#savingsplanscostcalculationtypedef) 
## SageMakerSavingsPlansTypeDef

```python
# SageMakerSavingsPlansTypeDef definition

class SageMakerSavingsPlansTypeDef(TypedDict):
    configuration: NotRequired[SageMakerSavingsPlansConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[SavingsPlansCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: SageMakerSavingsPlansConfigurationTypeDef](./type_defs.md#sagemakersavingsplansconfigurationtypedef) 
2. See [:material-code-braces: SavingsPlansCostCalculationTypeDef](./type_defs.md#savingsplanscostcalculationtypedef) 
## EbsVolumeTypeDef

```python
# EbsVolumeTypeDef definition

class EbsVolumeTypeDef(TypedDict):
    configuration: NotRequired[EbsVolumeConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ResourceCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: EbsVolumeConfigurationTypeDef](./type_defs.md#ebsvolumeconfigurationtypedef) 
2. See [:material-code-braces: ResourceCostCalculationTypeDef](./type_defs.md#resourcecostcalculationtypedef) 
## Ec2AutoScalingGroupTypeDef

```python
# Ec2AutoScalingGroupTypeDef definition

class Ec2AutoScalingGroupTypeDef(TypedDict):
    configuration: NotRequired[Ec2AutoScalingGroupConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ResourceCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: Ec2AutoScalingGroupConfigurationTypeDef](./type_defs.md#ec2autoscalinggroupconfigurationtypedef) 
2. See [:material-code-braces: ResourceCostCalculationTypeDef](./type_defs.md#resourcecostcalculationtypedef) 
## Ec2InstanceTypeDef

```python
# Ec2InstanceTypeDef definition

class Ec2InstanceTypeDef(TypedDict):
    configuration: NotRequired[Ec2InstanceConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ResourceCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: Ec2InstanceConfigurationTypeDef](./type_defs.md#ec2instanceconfigurationtypedef) 
2. See [:material-code-braces: ResourceCostCalculationTypeDef](./type_defs.md#resourcecostcalculationtypedef) 
## EcsServiceTypeDef

```python
# EcsServiceTypeDef definition

class EcsServiceTypeDef(TypedDict):
    configuration: NotRequired[EcsServiceConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ResourceCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: EcsServiceConfigurationTypeDef](./type_defs.md#ecsserviceconfigurationtypedef) 
2. See [:material-code-braces: ResourceCostCalculationTypeDef](./type_defs.md#resourcecostcalculationtypedef) 
## LambdaFunctionTypeDef

```python
# LambdaFunctionTypeDef definition

class LambdaFunctionTypeDef(TypedDict):
    configuration: NotRequired[LambdaFunctionConfigurationTypeDef],  # (1)
    costCalculation: NotRequired[ResourceCostCalculationTypeDef],  # (2)
```

1. See [:material-code-braces: LambdaFunctionConfigurationTypeDef](./type_defs.md#lambdafunctionconfigurationtypedef) 
2. See [:material-code-braces: ResourceCostCalculationTypeDef](./type_defs.md#resourcecostcalculationtypedef) 
## ResourceDetailsTypeDef

```python
# ResourceDetailsTypeDef definition

class ResourceDetailsTypeDef(TypedDict):
    computeSavingsPlans: NotRequired[ComputeSavingsPlansTypeDef],  # (1)
    ebsVolume: NotRequired[EbsVolumeTypeDef],  # (2)
    ec2AutoScalingGroup: NotRequired[Ec2AutoScalingGroupTypeDef],  # (3)
    ec2Instance: NotRequired[Ec2InstanceTypeDef],  # (4)
    ec2InstanceSavingsPlans: NotRequired[Ec2InstanceSavingsPlansTypeDef],  # (5)
    ec2ReservedInstances: NotRequired[Ec2ReservedInstancesTypeDef],  # (6)
    ecsService: NotRequired[EcsServiceTypeDef],  # (7)
    elastiCacheReservedInstances: NotRequired[ElastiCacheReservedInstancesTypeDef],  # (8)
    lambdaFunction: NotRequired[LambdaFunctionTypeDef],  # (9)
    openSearchReservedInstances: NotRequired[OpenSearchReservedInstancesTypeDef],  # (10)
    rdsReservedInstances: NotRequired[RdsReservedInstancesTypeDef],  # (11)
    redshiftReservedInstances: NotRequired[RedshiftReservedInstancesTypeDef],  # (12)
    sageMakerSavingsPlans: NotRequired[SageMakerSavingsPlansTypeDef],  # (13)
```

1. See [:material-code-braces: ComputeSavingsPlansTypeDef](./type_defs.md#computesavingsplanstypedef) 
2. See [:material-code-braces: EbsVolumeTypeDef](./type_defs.md#ebsvolumetypedef) 
3. See [:material-code-braces: Ec2AutoScalingGroupTypeDef](./type_defs.md#ec2autoscalinggrouptypedef) 
4. See [:material-code-braces: Ec2InstanceTypeDef](./type_defs.md#ec2instancetypedef) 
5. See [:material-code-braces: Ec2InstanceSavingsPlansTypeDef](./type_defs.md#ec2instancesavingsplanstypedef) 
6. See [:material-code-braces: Ec2ReservedInstancesTypeDef](./type_defs.md#ec2reservedinstancestypedef) 
7. See [:material-code-braces: EcsServiceTypeDef](./type_defs.md#ecsservicetypedef) 
8. See [:material-code-braces: ElastiCacheReservedInstancesTypeDef](./type_defs.md#elasticachereservedinstancestypedef) 
9. See [:material-code-braces: LambdaFunctionTypeDef](./type_defs.md#lambdafunctiontypedef) 
10. See [:material-code-braces: OpenSearchReservedInstancesTypeDef](./type_defs.md#opensearchreservedinstancestypedef) 
11. See [:material-code-braces: RdsReservedInstancesTypeDef](./type_defs.md#rdsreservedinstancestypedef) 
12. See [:material-code-braces: RedshiftReservedInstancesTypeDef](./type_defs.md#redshiftreservedinstancestypedef) 
13. See [:material-code-braces: SageMakerSavingsPlansTypeDef](./type_defs.md#sagemakersavingsplanstypedef) 
## GetRecommendationResponseTypeDef

```python
# GetRecommendationResponseTypeDef definition

class GetRecommendationResponseTypeDef(TypedDict):
    accountId: str,
    actionType: ActionTypeType,  # (1)
    costCalculationLookbackPeriodInDays: int,
    currencyCode: str,
    currentResourceDetails: ResourceDetailsTypeDef,  # (2)
    currentResourceType: ResourceTypeType,  # (3)
    estimatedMonthlyCost: float,
    estimatedMonthlySavings: float,
    estimatedSavingsOverCostCalculationLookbackPeriod: float,
    estimatedSavingsPercentage: float,
    implementationEffort: ImplementationEffortType,  # (4)
    lastRefreshTimestamp: datetime,
    recommendationId: str,
    recommendationLookbackPeriodInDays: int,
    recommendedResourceDetails: ResourceDetailsTypeDef,  # (2)
    recommendedResourceType: ResourceTypeType,  # (3)
    region: str,
    resourceArn: str,
    resourceId: str,
    restartNeeded: bool,
    rollbackPossible: bool,
    source: SourceType,  # (7)
    tags: List[TagTypeDef],  # (8)
    ResponseMetadata: ResponseMetadataTypeDef,  # (9)
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
2. See [:material-code-braces: ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef) 
3. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
4. See [:material-code-brackets: ImplementationEffortType](./literals.md#implementationefforttype) 
5. See [:material-code-braces: ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef) 
6. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
7. See [:material-code-brackets: SourceType](./literals.md#sourcetype) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
9. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
