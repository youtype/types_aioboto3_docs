# XRayClient

> [Index](../README.md) > [XRay](./README.md) > XRayClient

!!! note ""

    Auto-generated documentation for [XRay](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#xray)
    type annotations stubs module [types-aiobotocore-xray](https://pypi.org/project/types-aiobotocore-xray/).

## XRayClient

Type annotations and code completion for `#!python session.client("xray")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# XRayClient usage example

from aioboto3.session import Session
from types_aiobotocore_xray.client import XRayClient

session = Session()
async with session.client("xray") as client:
    client: XRayClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("xray").exceptions` structure.

```python
# XRayClient.exceptions usage example

async with session.client("xray") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.InvalidPolicyRevisionIdException,
        client.exceptions.InvalidRequestException,
        client.exceptions.LockoutPreventionException,
        client.exceptions.MalformedPolicyDocumentException,
        client.exceptions.PolicyCountLimitExceededException,
        client.exceptions.PolicySizeLimitExceededException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.RuleLimitExceededException,
        client.exceptions.ThrottledException,
        client.exceptions.TooManyTagsException,
    ) as e:
        print(e)
```

```python
# XRayClient.exceptions type checking example

from types_aiobotocore_xray.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("xray").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("xray").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

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


### batch\_get\_traces

You cannot find traces through this API if Transaction Search is enabled since
trace is not indexed in X-Ray.

Type annotations and code completion for `#!python session.client("xray").batch_get_traces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# batch_get_traces method definition

await def batch_get_traces(
    self,
    *,
    TraceIds: Sequence[str],
    NextToken: str = ...,
) -> BatchGetTracesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetTracesResultTypeDef](./type_defs.md#batchgettracesresulttypedef) 


```python
# batch_get_traces method usage example with argument unpacking

kwargs: BatchGetTracesRequestRequestTypeDef = {  # (1)
    "TraceIds": ...,
}

parent.batch_get_traces(**kwargs)
```

1. See [:material-code-braces: BatchGetTracesRequestRequestTypeDef](./type_defs.md#batchgettracesrequestrequesttypedef) 

### cancel\_trace\_retrieval

Cancels an ongoing trace retrieval job initiated by
<code>StartTraceRetrieval</code> using the provided
<code>RetrievalToken</code>.

Type annotations and code completion for `#!python session.client("xray").cancel_trace_retrieval` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# cancel_trace_retrieval method definition

await def cancel_trace_retrieval(
    self,
    *,
    RetrievalToken: str,
) -> dict[str, Any]:
    ...
```



```python
# cancel_trace_retrieval method usage example with argument unpacking

kwargs: CancelTraceRetrievalRequestRequestTypeDef = {  # (1)
    "RetrievalToken": ...,
}

parent.cancel_trace_retrieval(**kwargs)
```

1. See [:material-code-braces: CancelTraceRetrievalRequestRequestTypeDef](./type_defs.md#canceltraceretrievalrequestrequesttypedef) 

### create\_group

Creates a group resource with a name and a filter expression.

Type annotations and code completion for `#!python session.client("xray").create_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# create_group method definition

await def create_group(
    self,
    *,
    GroupName: str,
    FilterExpression: str = ...,
    InsightsConfiguration: InsightsConfigurationTypeDef = ...,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateGroupResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: InsightsConfigurationTypeDef](./type_defs.md#insightsconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateGroupResultTypeDef](./type_defs.md#creategroupresulttypedef) 


```python
# create_group method usage example with argument unpacking

kwargs: CreateGroupRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
}

parent.create_group(**kwargs)
```

1. See [:material-code-braces: CreateGroupRequestRequestTypeDef](./type_defs.md#creategrouprequestrequesttypedef) 

### create\_sampling\_rule

Creates a rule to control sampling behavior for instrumented applications.

Type annotations and code completion for `#!python session.client("xray").create_sampling_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# create_sampling_rule method definition

await def create_sampling_rule(
    self,
    *,
    SamplingRule: SamplingRuleTypeDef,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateSamplingRuleResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SamplingRuleTypeDef](./type_defs.md#samplingruletypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateSamplingRuleResultTypeDef](./type_defs.md#createsamplingruleresulttypedef) 


```python
# create_sampling_rule method usage example with argument unpacking

kwargs: CreateSamplingRuleRequestRequestTypeDef = {  # (1)
    "SamplingRule": ...,
}

parent.create_sampling_rule(**kwargs)
```

1. See [:material-code-braces: CreateSamplingRuleRequestRequestTypeDef](./type_defs.md#createsamplingrulerequestrequesttypedef) 

### delete\_group

Deletes a group resource.

Type annotations and code completion for `#!python session.client("xray").delete_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# delete_group method definition

await def delete_group(
    self,
    *,
    GroupName: str = ...,
    GroupARN: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_group method usage example with argument unpacking

kwargs: DeleteGroupRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
}

parent.delete_group(**kwargs)
```

1. See [:material-code-braces: DeleteGroupRequestRequestTypeDef](./type_defs.md#deletegrouprequestrequesttypedef) 

### delete\_resource\_policy

Deletes a resource policy from the target Amazon Web Services account.

Type annotations and code completion for `#!python session.client("xray").delete_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# delete_resource_policy method definition

await def delete_resource_policy(
    self,
    *,
    PolicyName: str,
    PolicyRevisionId: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_resource_policy method usage example with argument unpacking

kwargs: DeleteResourcePolicyRequestRequestTypeDef = {  # (1)
    "PolicyName": ...,
}

parent.delete_resource_policy(**kwargs)
```

1. See [:material-code-braces: DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef) 

### delete\_sampling\_rule

Deletes a sampling rule.

Type annotations and code completion for `#!python session.client("xray").delete_sampling_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# delete_sampling_rule method definition

await def delete_sampling_rule(
    self,
    *,
    RuleName: str = ...,
    RuleARN: str = ...,
) -> DeleteSamplingRuleResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteSamplingRuleResultTypeDef](./type_defs.md#deletesamplingruleresulttypedef) 


```python
# delete_sampling_rule method usage example with argument unpacking

kwargs: DeleteSamplingRuleRequestRequestTypeDef = {  # (1)
    "RuleName": ...,
}

parent.delete_sampling_rule(**kwargs)
```

1. See [:material-code-braces: DeleteSamplingRuleRequestRequestTypeDef](./type_defs.md#deletesamplingrulerequestrequesttypedef) 

### get\_encryption\_config

Retrieves the current encryption configuration for X-Ray data.

Type annotations and code completion for `#!python session.client("xray").get_encryption_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# get_encryption_config method definition

await def get_encryption_config(
    self,
) -> GetEncryptionConfigResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEncryptionConfigResultTypeDef](./type_defs.md#getencryptionconfigresulttypedef) 

### get\_group

Retrieves group resource details.

Type annotations and code completion for `#!python session.client("xray").get_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# get_group method definition

await def get_group(
    self,
    *,
    GroupName: str = ...,
    GroupARN: str = ...,
) -> GetGroupResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGroupResultTypeDef](./type_defs.md#getgroupresulttypedef) 


```python
# get_group method usage example with argument unpacking

kwargs: GetGroupRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
}

parent.get_group(**kwargs)
```

1. See [:material-code-braces: GetGroupRequestRequestTypeDef](./type_defs.md#getgrouprequestrequesttypedef) 

### get\_groups

Retrieves all active group details.

Type annotations and code completion for `#!python session.client("xray").get_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# get_groups method definition

await def get_groups(
    self,
    *,
    NextToken: str = ...,
) -> GetGroupsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGroupsResultTypeDef](./type_defs.md#getgroupsresulttypedef) 


```python
# get_groups method usage example with argument unpacking

kwargs: GetGroupsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.get_groups(**kwargs)
```

1. See [:material-code-braces: GetGroupsRequestRequestTypeDef](./type_defs.md#getgroupsrequestrequesttypedef) 

### get\_indexing\_rules

Retrieves all indexing rules.

Type annotations and code completion for `#!python session.client("xray").get_indexing_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# get_indexing_rules method definition

await def get_indexing_rules(
    self,
    *,
    NextToken: str = ...,
) -> GetIndexingRulesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIndexingRulesResultTypeDef](./type_defs.md#getindexingrulesresulttypedef) 


```python
# get_indexing_rules method usage example with argument unpacking

kwargs: GetIndexingRulesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.get_indexing_rules(**kwargs)
```

1. See [:material-code-braces: GetIndexingRulesRequestRequestTypeDef](./type_defs.md#getindexingrulesrequestrequesttypedef) 

### get\_insight

Retrieves the summary information of an insight.

Type annotations and code completion for `#!python session.client("xray").get_insight` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# get_insight method definition

await def get_insight(
    self,
    *,
    InsightId: str,
) -> GetInsightResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInsightResultTypeDef](./type_defs.md#getinsightresulttypedef) 


```python
# get_insight method usage example with argument unpacking

kwargs: GetInsightRequestRequestTypeDef = {  # (1)
    "InsightId": ...,
}

parent.get_insight(**kwargs)
```

1. See [:material-code-braces: GetInsightRequestRequestTypeDef](./type_defs.md#getinsightrequestrequesttypedef) 

### get\_insight\_events

X-Ray reevaluates insights periodically until they're resolved, and records
each intermediate state as an event.

Type annotations and code completion for `#!python session.client("xray").get_insight_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# get_insight_events method definition

await def get_insight_events(
    self,
    *,
    InsightId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetInsightEventsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInsightEventsResultTypeDef](./type_defs.md#getinsighteventsresulttypedef) 


```python
# get_insight_events method usage example with argument unpacking

kwargs: GetInsightEventsRequestRequestTypeDef = {  # (1)
    "InsightId": ...,
}

parent.get_insight_events(**kwargs)
```

1. See [:material-code-braces: GetInsightEventsRequestRequestTypeDef](./type_defs.md#getinsighteventsrequestrequesttypedef) 

### get\_insight\_impact\_graph

Retrieves a service graph structure filtered by the specified insight.

Type annotations and code completion for `#!python session.client("xray").get_insight_impact_graph` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# get_insight_impact_graph method definition

await def get_insight_impact_graph(
    self,
    *,
    InsightId: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    NextToken: str = ...,
) -> GetInsightImpactGraphResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInsightImpactGraphResultTypeDef](./type_defs.md#getinsightimpactgraphresulttypedef) 


```python
# get_insight_impact_graph method usage example with argument unpacking

kwargs: GetInsightImpactGraphRequestRequestTypeDef = {  # (1)
    "InsightId": ...,
    "StartTime": ...,
    "EndTime": ...,
}

parent.get_insight_impact_graph(**kwargs)
```

1. See [:material-code-braces: GetInsightImpactGraphRequestRequestTypeDef](./type_defs.md#getinsightimpactgraphrequestrequesttypedef) 

### get\_insight\_summaries

Retrieves the summaries of all insights in the specified group matching the
provided filter values.

Type annotations and code completion for `#!python session.client("xray").get_insight_summaries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# get_insight_summaries method definition

await def get_insight_summaries(
    self,
    *,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    States: Sequence[InsightStateType] = ...,  # (1)
    GroupARN: str = ...,
    GroupName: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetInsightSummariesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: InsightStateType](./literals.md#insightstatetype) 
2. See [:material-code-braces: GetInsightSummariesResultTypeDef](./type_defs.md#getinsightsummariesresulttypedef) 


```python
# get_insight_summaries method usage example with argument unpacking

kwargs: GetInsightSummariesRequestRequestTypeDef = {  # (1)
    "StartTime": ...,
    "EndTime": ...,
}

parent.get_insight_summaries(**kwargs)
```

1. See [:material-code-braces: GetInsightSummariesRequestRequestTypeDef](./type_defs.md#getinsightsummariesrequestrequesttypedef) 

### get\_retrieved\_traces\_graph

Retrieves a service graph for traces based on the specified
<code>RetrievalToken</code> from the CloudWatch log group generated by
Transaction Search.

Type annotations and code completion for `#!python session.client("xray").get_retrieved_traces_graph` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# get_retrieved_traces_graph method definition

await def get_retrieved_traces_graph(
    self,
    *,
    RetrievalToken: str,
    NextToken: str = ...,
) -> GetRetrievedTracesGraphResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRetrievedTracesGraphResultTypeDef](./type_defs.md#getretrievedtracesgraphresulttypedef) 


```python
# get_retrieved_traces_graph method usage example with argument unpacking

kwargs: GetRetrievedTracesGraphRequestRequestTypeDef = {  # (1)
    "RetrievalToken": ...,
}

parent.get_retrieved_traces_graph(**kwargs)
```

1. See [:material-code-braces: GetRetrievedTracesGraphRequestRequestTypeDef](./type_defs.md#getretrievedtracesgraphrequestrequesttypedef) 

### get\_sampling\_rules

Retrieves all sampling rules.

Type annotations and code completion for `#!python session.client("xray").get_sampling_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# get_sampling_rules method definition

await def get_sampling_rules(
    self,
    *,
    NextToken: str = ...,
) -> GetSamplingRulesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSamplingRulesResultTypeDef](./type_defs.md#getsamplingrulesresulttypedef) 


```python
# get_sampling_rules method usage example with argument unpacking

kwargs: GetSamplingRulesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.get_sampling_rules(**kwargs)
```

1. See [:material-code-braces: GetSamplingRulesRequestRequestTypeDef](./type_defs.md#getsamplingrulesrequestrequesttypedef) 

### get\_sampling\_statistic\_summaries

Retrieves information about recent sampling results for all sampling rules.

Type annotations and code completion for `#!python session.client("xray").get_sampling_statistic_summaries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# get_sampling_statistic_summaries method definition

await def get_sampling_statistic_summaries(
    self,
    *,
    NextToken: str = ...,
) -> GetSamplingStatisticSummariesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSamplingStatisticSummariesResultTypeDef](./type_defs.md#getsamplingstatisticsummariesresulttypedef) 


```python
# get_sampling_statistic_summaries method usage example with argument unpacking

kwargs: GetSamplingStatisticSummariesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.get_sampling_statistic_summaries(**kwargs)
```

1. See [:material-code-braces: GetSamplingStatisticSummariesRequestRequestTypeDef](./type_defs.md#getsamplingstatisticsummariesrequestrequesttypedef) 

### get\_sampling\_targets

Requests a sampling quota for rules that the service is using to sample
requests.

Type annotations and code completion for `#!python session.client("xray").get_sampling_targets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# get_sampling_targets method definition

await def get_sampling_targets(
    self,
    *,
    SamplingStatisticsDocuments: Sequence[SamplingStatisticsDocumentTypeDef],  # (1)
) -> GetSamplingTargetsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SamplingStatisticsDocumentTypeDef](./type_defs.md#samplingstatisticsdocumenttypedef) 
2. See [:material-code-braces: GetSamplingTargetsResultTypeDef](./type_defs.md#getsamplingtargetsresulttypedef) 


```python
# get_sampling_targets method usage example with argument unpacking

kwargs: GetSamplingTargetsRequestRequestTypeDef = {  # (1)
    "SamplingStatisticsDocuments": ...,
}

parent.get_sampling_targets(**kwargs)
```

1. See [:material-code-braces: GetSamplingTargetsRequestRequestTypeDef](./type_defs.md#getsamplingtargetsrequestrequesttypedef) 

### get\_service\_graph

Retrieves a document that describes services that process incoming requests,
and downstream services that they call as a result.

Type annotations and code completion for `#!python session.client("xray").get_service_graph` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# get_service_graph method definition

await def get_service_graph(
    self,
    *,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    GroupName: str = ...,
    GroupARN: str = ...,
    NextToken: str = ...,
) -> GetServiceGraphResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceGraphResultTypeDef](./type_defs.md#getservicegraphresulttypedef) 


```python
# get_service_graph method usage example with argument unpacking

kwargs: GetServiceGraphRequestRequestTypeDef = {  # (1)
    "StartTime": ...,
    "EndTime": ...,
}

parent.get_service_graph(**kwargs)
```

1. See [:material-code-braces: GetServiceGraphRequestRequestTypeDef](./type_defs.md#getservicegraphrequestrequesttypedef) 

### get\_time\_series\_service\_statistics

Get an aggregation of service statistics defined by a specific time range.

Type annotations and code completion for `#!python session.client("xray").get_time_series_service_statistics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# get_time_series_service_statistics method definition

await def get_time_series_service_statistics(
    self,
    *,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    GroupName: str = ...,
    GroupARN: str = ...,
    EntitySelectorExpression: str = ...,
    Period: int = ...,
    ForecastStatistics: bool = ...,
    NextToken: str = ...,
) -> GetTimeSeriesServiceStatisticsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTimeSeriesServiceStatisticsResultTypeDef](./type_defs.md#gettimeseriesservicestatisticsresulttypedef) 


```python
# get_time_series_service_statistics method usage example with argument unpacking

kwargs: GetTimeSeriesServiceStatisticsRequestRequestTypeDef = {  # (1)
    "StartTime": ...,
    "EndTime": ...,
}

parent.get_time_series_service_statistics(**kwargs)
```

1. See [:material-code-braces: GetTimeSeriesServiceStatisticsRequestRequestTypeDef](./type_defs.md#gettimeseriesservicestatisticsrequestrequesttypedef) 

### get\_trace\_graph

Retrieves a service graph for one or more specific trace IDs.

Type annotations and code completion for `#!python session.client("xray").get_trace_graph` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# get_trace_graph method definition

await def get_trace_graph(
    self,
    *,
    TraceIds: Sequence[str],
    NextToken: str = ...,
) -> GetTraceGraphResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTraceGraphResultTypeDef](./type_defs.md#gettracegraphresulttypedef) 


```python
# get_trace_graph method usage example with argument unpacking

kwargs: GetTraceGraphRequestRequestTypeDef = {  # (1)
    "TraceIds": ...,
}

parent.get_trace_graph(**kwargs)
```

1. See [:material-code-braces: GetTraceGraphRequestRequestTypeDef](./type_defs.md#gettracegraphrequestrequesttypedef) 

### get\_trace\_segment\_destination

Retrieves the current destination of data sent to <code>PutTraceSegments</code>
and <i>OpenTelemetry</i> API.

Type annotations and code completion for `#!python session.client("xray").get_trace_segment_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# get_trace_segment_destination method definition

await def get_trace_segment_destination(
    self,
) -> GetTraceSegmentDestinationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTraceSegmentDestinationResultTypeDef](./type_defs.md#gettracesegmentdestinationresulttypedef) 

### get\_trace\_summaries

Retrieves IDs and annotations for traces available for a specified time frame
using an optional filter.

Type annotations and code completion for `#!python session.client("xray").get_trace_summaries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# get_trace_summaries method definition

await def get_trace_summaries(
    self,
    *,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    TimeRangeType: TimeRangeTypeType = ...,  # (1)
    Sampling: bool = ...,
    SamplingStrategy: SamplingStrategyTypeDef = ...,  # (2)
    FilterExpression: str = ...,
    NextToken: str = ...,
) -> GetTraceSummariesResultTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: TimeRangeTypeType](./literals.md#timerangetypetype) 
2. See [:material-code-braces: SamplingStrategyTypeDef](./type_defs.md#samplingstrategytypedef) 
3. See [:material-code-braces: GetTraceSummariesResultTypeDef](./type_defs.md#gettracesummariesresulttypedef) 


```python
# get_trace_summaries method usage example with argument unpacking

kwargs: GetTraceSummariesRequestRequestTypeDef = {  # (1)
    "StartTime": ...,
    "EndTime": ...,
}

parent.get_trace_summaries(**kwargs)
```

1. See [:material-code-braces: GetTraceSummariesRequestRequestTypeDef](./type_defs.md#gettracesummariesrequestrequesttypedef) 

### list\_resource\_policies

Returns the list of resource policies in the target Amazon Web Services account.

Type annotations and code completion for `#!python session.client("xray").list_resource_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# list_resource_policies method definition

await def list_resource_policies(
    self,
    *,
    NextToken: str = ...,
) -> ListResourcePoliciesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListResourcePoliciesResultTypeDef](./type_defs.md#listresourcepoliciesresulttypedef) 


```python
# list_resource_policies method usage example with argument unpacking

kwargs: ListResourcePoliciesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_resource_policies(**kwargs)
```

1. See [:material-code-braces: ListResourcePoliciesRequestRequestTypeDef](./type_defs.md#listresourcepoliciesrequestrequesttypedef) 

### list\_retrieved\_traces

Retrieves a list of traces for a given <code>RetrievalToken</code> from the
CloudWatch log group generated by Transaction Search.

Type annotations and code completion for `#!python session.client("xray").list_retrieved_traces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# list_retrieved_traces method definition

await def list_retrieved_traces(
    self,
    *,
    RetrievalToken: str,
    TraceFormat: TraceFormatTypeType = ...,  # (1)
    NextToken: str = ...,
) -> ListRetrievedTracesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TraceFormatTypeType](./literals.md#traceformattypetype) 
2. See [:material-code-braces: ListRetrievedTracesResultTypeDef](./type_defs.md#listretrievedtracesresulttypedef) 


```python
# list_retrieved_traces method usage example with argument unpacking

kwargs: ListRetrievedTracesRequestRequestTypeDef = {  # (1)
    "RetrievalToken": ...,
}

parent.list_retrieved_traces(**kwargs)
```

1. See [:material-code-braces: ListRetrievedTracesRequestRequestTypeDef](./type_defs.md#listretrievedtracesrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of tags that are applied to the specified Amazon Web Services
X-Ray group or sampling rule.

Type annotations and code completion for `#!python session.client("xray").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
    NextToken: str = ...,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### put\_encryption\_config

Updates the encryption configuration for X-Ray data.

Type annotations and code completion for `#!python session.client("xray").put_encryption_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# put_encryption_config method definition

await def put_encryption_config(
    self,
    *,
    Type: EncryptionTypeType,  # (1)
    KeyId: str = ...,
) -> PutEncryptionConfigResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
2. See [:material-code-braces: PutEncryptionConfigResultTypeDef](./type_defs.md#putencryptionconfigresulttypedef) 


```python
# put_encryption_config method usage example with argument unpacking

kwargs: PutEncryptionConfigRequestRequestTypeDef = {  # (1)
    "Type": ...,
}

parent.put_encryption_config(**kwargs)
```

1. See [:material-code-braces: PutEncryptionConfigRequestRequestTypeDef](./type_defs.md#putencryptionconfigrequestrequesttypedef) 

### put\_resource\_policy

Sets the resource policy to grant one or more Amazon Web Services services and
accounts permissions to access X-Ray.

Type annotations and code completion for `#!python session.client("xray").put_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# put_resource_policy method definition

await def put_resource_policy(
    self,
    *,
    PolicyName: str,
    PolicyDocument: str,
    PolicyRevisionId: str = ...,
    BypassPolicyLockoutCheck: bool = ...,
) -> PutResourcePolicyResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutResourcePolicyResultTypeDef](./type_defs.md#putresourcepolicyresulttypedef) 


```python
# put_resource_policy method usage example with argument unpacking

kwargs: PutResourcePolicyRequestRequestTypeDef = {  # (1)
    "PolicyName": ...,
    "PolicyDocument": ...,
}

parent.put_resource_policy(**kwargs)
```

1. See [:material-code-braces: PutResourcePolicyRequestRequestTypeDef](./type_defs.md#putresourcepolicyrequestrequesttypedef) 

### put\_telemetry\_records

Used by the Amazon Web Services X-Ray daemon to upload telemetry.

Type annotations and code completion for `#!python session.client("xray").put_telemetry_records` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# put_telemetry_records method definition

await def put_telemetry_records(
    self,
    *,
    TelemetryRecords: Sequence[TelemetryRecordTypeDef],  # (1)
    EC2InstanceId: str = ...,
    Hostname: str = ...,
    ResourceARN: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: TelemetryRecordTypeDef](./type_defs.md#telemetryrecordtypedef) 


```python
# put_telemetry_records method usage example with argument unpacking

kwargs: PutTelemetryRecordsRequestRequestTypeDef = {  # (1)
    "TelemetryRecords": ...,
}

parent.put_telemetry_records(**kwargs)
```

1. See [:material-code-braces: PutTelemetryRecordsRequestRequestTypeDef](./type_defs.md#puttelemetryrecordsrequestrequesttypedef) 

### put\_trace\_segments

Uploads segment documents to Amazon Web Services X-Ray.

Type annotations and code completion for `#!python session.client("xray").put_trace_segments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# put_trace_segments method definition

await def put_trace_segments(
    self,
    *,
    TraceSegmentDocuments: Sequence[str],
) -> PutTraceSegmentsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutTraceSegmentsResultTypeDef](./type_defs.md#puttracesegmentsresulttypedef) 


```python
# put_trace_segments method usage example with argument unpacking

kwargs: PutTraceSegmentsRequestRequestTypeDef = {  # (1)
    "TraceSegmentDocuments": ...,
}

parent.put_trace_segments(**kwargs)
```

1. See [:material-code-braces: PutTraceSegmentsRequestRequestTypeDef](./type_defs.md#puttracesegmentsrequestrequesttypedef) 

### start\_trace\_retrieval

Initiates a trace retrieval process using the specified time range and for the
give trace IDs on Transaction Search generated by the CloudWatch log group.

Type annotations and code completion for `#!python session.client("xray").start_trace_retrieval` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# start_trace_retrieval method definition

await def start_trace_retrieval(
    self,
    *,
    TraceIds: Sequence[str],
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
) -> StartTraceRetrievalResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartTraceRetrievalResultTypeDef](./type_defs.md#starttraceretrievalresulttypedef) 


```python
# start_trace_retrieval method usage example with argument unpacking

kwargs: StartTraceRetrievalRequestRequestTypeDef = {  # (1)
    "TraceIds": ...,
    "StartTime": ...,
    "EndTime": ...,
}

parent.start_trace_retrieval(**kwargs)
```

1. See [:material-code-braces: StartTraceRetrievalRequestRequestTypeDef](./type_defs.md#starttraceretrievalrequestrequesttypedef) 

### tag\_resource

Applies tags to an existing Amazon Web Services X-Ray group or sampling rule.

Type annotations and code completion for `#!python session.client("xray").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes tags from an Amazon Web Services X-Ray group or sampling rule.

Type annotations and code completion for `#!python session.client("xray").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_group

Updates a group resource.

Type annotations and code completion for `#!python session.client("xray").update_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# update_group method definition

await def update_group(
    self,
    *,
    GroupName: str = ...,
    GroupARN: str = ...,
    FilterExpression: str = ...,
    InsightsConfiguration: InsightsConfigurationTypeDef = ...,  # (1)
) -> UpdateGroupResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InsightsConfigurationTypeDef](./type_defs.md#insightsconfigurationtypedef) 
2. See [:material-code-braces: UpdateGroupResultTypeDef](./type_defs.md#updategroupresulttypedef) 


```python
# update_group method usage example with argument unpacking

kwargs: UpdateGroupRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
}

parent.update_group(**kwargs)
```

1. See [:material-code-braces: UpdateGroupRequestRequestTypeDef](./type_defs.md#updategrouprequestrequesttypedef) 

### update\_indexing\_rule

Modifies an indexing rule's configuration.

Type annotations and code completion for `#!python session.client("xray").update_indexing_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# update_indexing_rule method definition

await def update_indexing_rule(
    self,
    *,
    Name: str,
    Rule: IndexingRuleValueUpdateTypeDef,  # (1)
) -> UpdateIndexingRuleResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: IndexingRuleValueUpdateTypeDef](./type_defs.md#indexingrulevalueupdatetypedef) 
2. See [:material-code-braces: UpdateIndexingRuleResultTypeDef](./type_defs.md#updateindexingruleresulttypedef) 


```python
# update_indexing_rule method usage example with argument unpacking

kwargs: UpdateIndexingRuleRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Rule": ...,
}

parent.update_indexing_rule(**kwargs)
```

1. See [:material-code-braces: UpdateIndexingRuleRequestRequestTypeDef](./type_defs.md#updateindexingrulerequestrequesttypedef) 

### update\_sampling\_rule

Modifies a sampling rule's configuration.

Type annotations and code completion for `#!python session.client("xray").update_sampling_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# update_sampling_rule method definition

await def update_sampling_rule(
    self,
    *,
    SamplingRuleUpdate: SamplingRuleUpdateTypeDef,  # (1)
) -> UpdateSamplingRuleResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SamplingRuleUpdateTypeDef](./type_defs.md#samplingruleupdatetypedef) 
2. See [:material-code-braces: UpdateSamplingRuleResultTypeDef](./type_defs.md#updatesamplingruleresulttypedef) 


```python
# update_sampling_rule method usage example with argument unpacking

kwargs: UpdateSamplingRuleRequestRequestTypeDef = {  # (1)
    "SamplingRuleUpdate": ...,
}

parent.update_sampling_rule(**kwargs)
```

1. See [:material-code-braces: UpdateSamplingRuleRequestRequestTypeDef](./type_defs.md#updatesamplingrulerequestrequesttypedef) 

### update\_trace\_segment\_destination

Modifies the destination of data sent to <code>PutTraceSegments</code>.

Type annotations and code completion for `#!python session.client("xray").update_trace_segment_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# update_trace_segment_destination method definition

await def update_trace_segment_destination(
    self,
    *,
    Destination: TraceSegmentDestinationType = ...,  # (1)
) -> UpdateTraceSegmentDestinationResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TraceSegmentDestinationType](./literals.md#tracesegmentdestinationtype) 
2. See [:material-code-braces: UpdateTraceSegmentDestinationResultTypeDef](./type_defs.md#updatetracesegmentdestinationresulttypedef) 


```python
# update_trace_segment_destination method usage example with argument unpacking

kwargs: UpdateTraceSegmentDestinationRequestRequestTypeDef = {  # (1)
    "Destination": ...,
}

parent.update_trace_segment_destination(**kwargs)
```

1. See [:material-code-braces: UpdateTraceSegmentDestinationRequestRequestTypeDef](./type_defs.md#updatetracesegmentdestinationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("xray").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("xray").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client)

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

Type annotations and code completion for `#!python session.client("xray").get_paginator` method with overloads.

- `client.get_paginator("batch_get_traces")` -> [BatchGetTracesPaginator](./paginators.md#batchgettracespaginator)
- `client.get_paginator("get_groups")` -> [GetGroupsPaginator](./paginators.md#getgroupspaginator)
- `client.get_paginator("get_sampling_rules")` -> [GetSamplingRulesPaginator](./paginators.md#getsamplingrulespaginator)
- `client.get_paginator("get_sampling_statistic_summaries")` -> [GetSamplingStatisticSummariesPaginator](./paginators.md#getsamplingstatisticsummariespaginator)
- `client.get_paginator("get_service_graph")` -> [GetServiceGraphPaginator](./paginators.md#getservicegraphpaginator)
- `client.get_paginator("get_time_series_service_statistics")` -> [GetTimeSeriesServiceStatisticsPaginator](./paginators.md#gettimeseriesservicestatisticspaginator)
- `client.get_paginator("get_trace_graph")` -> [GetTraceGraphPaginator](./paginators.md#gettracegraphpaginator)
- `client.get_paginator("get_trace_summaries")` -> [GetTraceSummariesPaginator](./paginators.md#gettracesummariespaginator)
- `client.get_paginator("list_resource_policies")` -> [ListResourcePoliciesPaginator](./paginators.md#listresourcepoliciespaginator)
- `client.get_paginator("list_tags_for_resource")` -> [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)


