# ConfigServiceClient

> [Index](../README.md) > [ConfigService](./README.md) > ConfigServiceClient

!!! note ""

    Auto-generated documentation for [ConfigService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#configservice)
    type annotations stubs module [types-aiobotocore-config](https://pypi.org/project/types-aiobotocore-config/).

## ConfigServiceClient

Type annotations and code completion for `#!python session.client("config")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# ConfigServiceClient usage example

from aioboto3.session import Session
from types_aiobotocore_config.client import ConfigServiceClient

session = Session()
async with session.client("config") as client:
    client: ConfigServiceClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("config").exceptions` structure.

```python
# ConfigServiceClient.exceptions usage example

async with session.client("config") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.ConformancePackTemplateValidationException,
        client.exceptions.IdempotentParameterMismatch,
        client.exceptions.InsufficientDeliveryPolicyException,
        client.exceptions.InsufficientPermissionsException,
        client.exceptions.InvalidConfigurationRecorderNameException,
        client.exceptions.InvalidDeliveryChannelNameException,
        client.exceptions.InvalidExpressionException,
        client.exceptions.InvalidLimitException,
        client.exceptions.InvalidNextTokenException,
        client.exceptions.InvalidParameterValueException,
        client.exceptions.InvalidRecordingGroupException,
        client.exceptions.InvalidResultTokenException,
        client.exceptions.InvalidRoleException,
        client.exceptions.InvalidS3KeyPrefixException,
        client.exceptions.InvalidS3KmsKeyArnException,
        client.exceptions.InvalidSNSTopicARNException,
        client.exceptions.InvalidTimeRangeException,
        client.exceptions.LastDeliveryChannelDeleteFailedException,
        client.exceptions.LimitExceededException,
        client.exceptions.MaxActiveResourcesExceededException,
        client.exceptions.MaxNumberOfConfigRulesExceededException,
        client.exceptions.MaxNumberOfConfigurationRecordersExceededException,
        client.exceptions.MaxNumberOfConformancePacksExceededException,
        client.exceptions.MaxNumberOfDeliveryChannelsExceededException,
        client.exceptions.MaxNumberOfOrganizationConfigRulesExceededException,
        client.exceptions.MaxNumberOfOrganizationConformancePacksExceededException,
        client.exceptions.MaxNumberOfRetentionConfigurationsExceededException,
        client.exceptions.NoAvailableConfigurationRecorderException,
        client.exceptions.NoAvailableDeliveryChannelException,
        client.exceptions.NoAvailableOrganizationException,
        client.exceptions.NoRunningConfigurationRecorderException,
        client.exceptions.NoSuchBucketException,
        client.exceptions.NoSuchConfigRuleException,
        client.exceptions.NoSuchConfigRuleInConformancePackException,
        client.exceptions.NoSuchConfigurationAggregatorException,
        client.exceptions.NoSuchConfigurationRecorderException,
        client.exceptions.NoSuchConformancePackException,
        client.exceptions.NoSuchDeliveryChannelException,
        client.exceptions.NoSuchOrganizationConfigRuleException,
        client.exceptions.NoSuchOrganizationConformancePackException,
        client.exceptions.NoSuchRemediationConfigurationException,
        client.exceptions.NoSuchRemediationExceptionException,
        client.exceptions.NoSuchRetentionConfigurationException,
        client.exceptions.OrganizationAccessDeniedException,
        client.exceptions.OrganizationAllFeaturesNotEnabledException,
        client.exceptions.OrganizationConformancePackTemplateValidationException,
        client.exceptions.OversizedConfigurationItemException,
        client.exceptions.RemediationInProgressException,
        client.exceptions.ResourceConcurrentModificationException,
        client.exceptions.ResourceInUseException,
        client.exceptions.ResourceNotDiscoveredException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.TooManyTagsException,
        client.exceptions.UnmodifiableEntityException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# ConfigServiceClient.exceptions type checking example

from types_aiobotocore_config.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("config").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("config").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

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


### associate\_resource\_types

Adds all resource types specified in the <code>ResourceTypes</code> list to the
<a
href="https://docs.aws.amazon.com/config/latest/APIReference/API_RecordingGroup.html">RecordingGroup</a>
of specified configuration recorder and includes those resource types when
recording.

Type annotations and code completion for `#!python session.client("config").associate_resource_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# associate_resource_types method definition

await def associate_resource_types(
    self,
    *,
    ConfigurationRecorderArn: str,
    ResourceTypes: Sequence[ResourceTypeType],  # (1)
) -> AssociateResourceTypesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: AssociateResourceTypesResponseTypeDef](./type_defs.md#associateresourcetypesresponsetypedef) 


```python
# associate_resource_types method usage example with argument unpacking

kwargs: AssociateResourceTypesRequestRequestTypeDef = {  # (1)
    "ConfigurationRecorderArn": ...,
    "ResourceTypes": ...,
}

parent.associate_resource_types(**kwargs)
```

1. See [:material-code-braces: AssociateResourceTypesRequestRequestTypeDef](./type_defs.md#associateresourcetypesrequestrequesttypedef) 

### batch\_get\_aggregate\_resource\_config

Returns the current configuration items for resources that are present in your
Config aggregator.

Type annotations and code completion for `#!python session.client("config").batch_get_aggregate_resource_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# batch_get_aggregate_resource_config method definition

await def batch_get_aggregate_resource_config(
    self,
    *,
    ConfigurationAggregatorName: str,
    ResourceIdentifiers: Sequence[AggregateResourceIdentifierTypeDef],  # (1)
) -> BatchGetAggregateResourceConfigResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AggregateResourceIdentifierTypeDef](./type_defs.md#aggregateresourceidentifiertypedef) 
2. See [:material-code-braces: BatchGetAggregateResourceConfigResponseTypeDef](./type_defs.md#batchgetaggregateresourceconfigresponsetypedef) 


```python
# batch_get_aggregate_resource_config method usage example with argument unpacking

kwargs: BatchGetAggregateResourceConfigRequestRequestTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
    "ResourceIdentifiers": ...,
}

parent.batch_get_aggregate_resource_config(**kwargs)
```

1. See [:material-code-braces: BatchGetAggregateResourceConfigRequestRequestTypeDef](./type_defs.md#batchgetaggregateresourceconfigrequestrequesttypedef) 

### batch\_get\_resource\_config

Returns the <code>BaseConfigurationItem</code> for one or more requested
resources.

Type annotations and code completion for `#!python session.client("config").batch_get_resource_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# batch_get_resource_config method definition

await def batch_get_resource_config(
    self,
    *,
    resourceKeys: Sequence[ResourceKeyTypeDef],  # (1)
) -> BatchGetResourceConfigResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ResourceKeyTypeDef](./type_defs.md#resourcekeytypedef) 
2. See [:material-code-braces: BatchGetResourceConfigResponseTypeDef](./type_defs.md#batchgetresourceconfigresponsetypedef) 


```python
# batch_get_resource_config method usage example with argument unpacking

kwargs: BatchGetResourceConfigRequestRequestTypeDef = {  # (1)
    "resourceKeys": ...,
}

parent.batch_get_resource_config(**kwargs)
```

1. See [:material-code-braces: BatchGetResourceConfigRequestRequestTypeDef](./type_defs.md#batchgetresourceconfigrequestrequesttypedef) 

### delete\_aggregation\_authorization

Deletes the authorization granted to the specified configuration aggregator
account in a specified region.

Type annotations and code completion for `#!python session.client("config").delete_aggregation_authorization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# delete_aggregation_authorization method definition

await def delete_aggregation_authorization(
    self,
    *,
    AuthorizedAccountId: str,
    AuthorizedAwsRegion: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_aggregation_authorization method usage example with argument unpacking

kwargs: DeleteAggregationAuthorizationRequestRequestTypeDef = {  # (1)
    "AuthorizedAccountId": ...,
    "AuthorizedAwsRegion": ...,
}

parent.delete_aggregation_authorization(**kwargs)
```

1. See [:material-code-braces: DeleteAggregationAuthorizationRequestRequestTypeDef](./type_defs.md#deleteaggregationauthorizationrequestrequesttypedef) 

### delete\_config\_rule

Deletes the specified Config rule and all of its evaluation results.

Type annotations and code completion for `#!python session.client("config").delete_config_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# delete_config_rule method definition

await def delete_config_rule(
    self,
    *,
    ConfigRuleName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_config_rule method usage example with argument unpacking

kwargs: DeleteConfigRuleRequestRequestTypeDef = {  # (1)
    "ConfigRuleName": ...,
}

parent.delete_config_rule(**kwargs)
```

1. See [:material-code-braces: DeleteConfigRuleRequestRequestTypeDef](./type_defs.md#deleteconfigrulerequestrequesttypedef) 

### delete\_configuration\_aggregator

Deletes the specified configuration aggregator and the aggregated data
associated with the aggregator.

Type annotations and code completion for `#!python session.client("config").delete_configuration_aggregator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# delete_configuration_aggregator method definition

await def delete_configuration_aggregator(
    self,
    *,
    ConfigurationAggregatorName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_configuration_aggregator method usage example with argument unpacking

kwargs: DeleteConfigurationAggregatorRequestRequestTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
}

parent.delete_configuration_aggregator(**kwargs)
```

1. See [:material-code-braces: DeleteConfigurationAggregatorRequestRequestTypeDef](./type_defs.md#deleteconfigurationaggregatorrequestrequesttypedef) 

### delete\_configuration\_recorder

Deletes the customer managed configuration recorder.

Type annotations and code completion for `#!python session.client("config").delete_configuration_recorder` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# delete_configuration_recorder method definition

await def delete_configuration_recorder(
    self,
    *,
    ConfigurationRecorderName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_configuration_recorder method usage example with argument unpacking

kwargs: DeleteConfigurationRecorderRequestRequestTypeDef = {  # (1)
    "ConfigurationRecorderName": ...,
}

parent.delete_configuration_recorder(**kwargs)
```

1. See [:material-code-braces: DeleteConfigurationRecorderRequestRequestTypeDef](./type_defs.md#deleteconfigurationrecorderrequestrequesttypedef) 

### delete\_conformance\_pack

Deletes the specified conformance pack and all the Config rules, remediation
actions, and all evaluation results within that conformance pack.

Type annotations and code completion for `#!python session.client("config").delete_conformance_pack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# delete_conformance_pack method definition

await def delete_conformance_pack(
    self,
    *,
    ConformancePackName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_conformance_pack method usage example with argument unpacking

kwargs: DeleteConformancePackRequestRequestTypeDef = {  # (1)
    "ConformancePackName": ...,
}

parent.delete_conformance_pack(**kwargs)
```

1. See [:material-code-braces: DeleteConformancePackRequestRequestTypeDef](./type_defs.md#deleteconformancepackrequestrequesttypedef) 

### delete\_delivery\_channel

Deletes the delivery channel.

Type annotations and code completion for `#!python session.client("config").delete_delivery_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# delete_delivery_channel method definition

await def delete_delivery_channel(
    self,
    *,
    DeliveryChannelName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_delivery_channel method usage example with argument unpacking

kwargs: DeleteDeliveryChannelRequestRequestTypeDef = {  # (1)
    "DeliveryChannelName": ...,
}

parent.delete_delivery_channel(**kwargs)
```

1. See [:material-code-braces: DeleteDeliveryChannelRequestRequestTypeDef](./type_defs.md#deletedeliverychannelrequestrequesttypedef) 

### delete\_evaluation\_results

Deletes the evaluation results for the specified Config rule.

Type annotations and code completion for `#!python session.client("config").delete_evaluation_results` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# delete_evaluation_results method definition

await def delete_evaluation_results(
    self,
    *,
    ConfigRuleName: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_evaluation_results method usage example with argument unpacking

kwargs: DeleteEvaluationResultsRequestRequestTypeDef = {  # (1)
    "ConfigRuleName": ...,
}

parent.delete_evaluation_results(**kwargs)
```

1. See [:material-code-braces: DeleteEvaluationResultsRequestRequestTypeDef](./type_defs.md#deleteevaluationresultsrequestrequesttypedef) 

### delete\_organization\_config\_rule

Deletes the specified organization Config rule and all of its evaluation
results from all member accounts in that organization.

Type annotations and code completion for `#!python session.client("config").delete_organization_config_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# delete_organization_config_rule method definition

await def delete_organization_config_rule(
    self,
    *,
    OrganizationConfigRuleName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_organization_config_rule method usage example with argument unpacking

kwargs: DeleteOrganizationConfigRuleRequestRequestTypeDef = {  # (1)
    "OrganizationConfigRuleName": ...,
}

parent.delete_organization_config_rule(**kwargs)
```

1. See [:material-code-braces: DeleteOrganizationConfigRuleRequestRequestTypeDef](./type_defs.md#deleteorganizationconfigrulerequestrequesttypedef) 

### delete\_organization\_conformance\_pack

Deletes the specified organization conformance pack and all of the Config rules
and remediation actions from all member accounts in that organization.

Type annotations and code completion for `#!python session.client("config").delete_organization_conformance_pack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# delete_organization_conformance_pack method definition

await def delete_organization_conformance_pack(
    self,
    *,
    OrganizationConformancePackName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_organization_conformance_pack method usage example with argument unpacking

kwargs: DeleteOrganizationConformancePackRequestRequestTypeDef = {  # (1)
    "OrganizationConformancePackName": ...,
}

parent.delete_organization_conformance_pack(**kwargs)
```

1. See [:material-code-braces: DeleteOrganizationConformancePackRequestRequestTypeDef](./type_defs.md#deleteorganizationconformancepackrequestrequesttypedef) 

### delete\_pending\_aggregation\_request

Deletes pending authorization requests for a specified aggregator account in a
specified region.

Type annotations and code completion for `#!python session.client("config").delete_pending_aggregation_request` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# delete_pending_aggregation_request method definition

await def delete_pending_aggregation_request(
    self,
    *,
    RequesterAccountId: str,
    RequesterAwsRegion: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_pending_aggregation_request method usage example with argument unpacking

kwargs: DeletePendingAggregationRequestRequestRequestTypeDef = {  # (1)
    "RequesterAccountId": ...,
    "RequesterAwsRegion": ...,
}

parent.delete_pending_aggregation_request(**kwargs)
```

1. See [:material-code-braces: DeletePendingAggregationRequestRequestRequestTypeDef](./type_defs.md#deletependingaggregationrequestrequestrequesttypedef) 

### delete\_remediation\_configuration

Deletes the remediation configuration.

Type annotations and code completion for `#!python session.client("config").delete_remediation_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# delete_remediation_configuration method definition

await def delete_remediation_configuration(
    self,
    *,
    ConfigRuleName: str,
    ResourceType: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_remediation_configuration method usage example with argument unpacking

kwargs: DeleteRemediationConfigurationRequestRequestTypeDef = {  # (1)
    "ConfigRuleName": ...,
}

parent.delete_remediation_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteRemediationConfigurationRequestRequestTypeDef](./type_defs.md#deleteremediationconfigurationrequestrequesttypedef) 

### delete\_remediation\_exceptions

Deletes one or more remediation exceptions mentioned in the resource keys.

Type annotations and code completion for `#!python session.client("config").delete_remediation_exceptions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# delete_remediation_exceptions method definition

await def delete_remediation_exceptions(
    self,
    *,
    ConfigRuleName: str,
    ResourceKeys: Sequence[RemediationExceptionResourceKeyTypeDef],  # (1)
) -> DeleteRemediationExceptionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RemediationExceptionResourceKeyTypeDef](./type_defs.md#remediationexceptionresourcekeytypedef) 
2. See [:material-code-braces: DeleteRemediationExceptionsResponseTypeDef](./type_defs.md#deleteremediationexceptionsresponsetypedef) 


```python
# delete_remediation_exceptions method usage example with argument unpacking

kwargs: DeleteRemediationExceptionsRequestRequestTypeDef = {  # (1)
    "ConfigRuleName": ...,
    "ResourceKeys": ...,
}

parent.delete_remediation_exceptions(**kwargs)
```

1. See [:material-code-braces: DeleteRemediationExceptionsRequestRequestTypeDef](./type_defs.md#deleteremediationexceptionsrequestrequesttypedef) 

### delete\_resource\_config

Records the configuration state for a custom resource that has been deleted.

Type annotations and code completion for `#!python session.client("config").delete_resource_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# delete_resource_config method definition

await def delete_resource_config(
    self,
    *,
    ResourceType: str,
    ResourceId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_resource_config method usage example with argument unpacking

kwargs: DeleteResourceConfigRequestRequestTypeDef = {  # (1)
    "ResourceType": ...,
    "ResourceId": ...,
}

parent.delete_resource_config(**kwargs)
```

1. See [:material-code-braces: DeleteResourceConfigRequestRequestTypeDef](./type_defs.md#deleteresourceconfigrequestrequesttypedef) 

### delete\_retention\_configuration

Deletes the retention configuration.

Type annotations and code completion for `#!python session.client("config").delete_retention_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# delete_retention_configuration method definition

await def delete_retention_configuration(
    self,
    *,
    RetentionConfigurationName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_retention_configuration method usage example with argument unpacking

kwargs: DeleteRetentionConfigurationRequestRequestTypeDef = {  # (1)
    "RetentionConfigurationName": ...,
}

parent.delete_retention_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteRetentionConfigurationRequestRequestTypeDef](./type_defs.md#deleteretentionconfigurationrequestrequesttypedef) 

### delete\_service\_linked\_configuration\_recorder

Deletes an existing service-linked configuration recorder.

Type annotations and code completion for `#!python session.client("config").delete_service_linked_configuration_recorder` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# delete_service_linked_configuration_recorder method definition

await def delete_service_linked_configuration_recorder(
    self,
    *,
    ServicePrincipal: str,
) -> DeleteServiceLinkedConfigurationRecorderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteServiceLinkedConfigurationRecorderResponseTypeDef](./type_defs.md#deleteservicelinkedconfigurationrecorderresponsetypedef) 


```python
# delete_service_linked_configuration_recorder method usage example with argument unpacking

kwargs: DeleteServiceLinkedConfigurationRecorderRequestRequestTypeDef = {  # (1)
    "ServicePrincipal": ...,
}

parent.delete_service_linked_configuration_recorder(**kwargs)
```

1. See [:material-code-braces: DeleteServiceLinkedConfigurationRecorderRequestRequestTypeDef](./type_defs.md#deleteservicelinkedconfigurationrecorderrequestrequesttypedef) 

### delete\_stored\_query

Deletes the stored query for a single Amazon Web Services account and a single
Amazon Web Services Region.

Type annotations and code completion for `#!python session.client("config").delete_stored_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# delete_stored_query method definition

await def delete_stored_query(
    self,
    *,
    QueryName: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_stored_query method usage example with argument unpacking

kwargs: DeleteStoredQueryRequestRequestTypeDef = {  # (1)
    "QueryName": ...,
}

parent.delete_stored_query(**kwargs)
```

1. See [:material-code-braces: DeleteStoredQueryRequestRequestTypeDef](./type_defs.md#deletestoredqueryrequestrequesttypedef) 

### deliver\_config\_snapshot

Schedules delivery of a configuration snapshot to the Amazon S3 bucket in the
specified delivery channel.

Type annotations and code completion for `#!python session.client("config").deliver_config_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# deliver_config_snapshot method definition

await def deliver_config_snapshot(
    self,
    *,
    deliveryChannelName: str,
) -> DeliverConfigSnapshotResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeliverConfigSnapshotResponseTypeDef](./type_defs.md#deliverconfigsnapshotresponsetypedef) 


```python
# deliver_config_snapshot method usage example with argument unpacking

kwargs: DeliverConfigSnapshotRequestRequestTypeDef = {  # (1)
    "deliveryChannelName": ...,
}

parent.deliver_config_snapshot(**kwargs)
```

1. See [:material-code-braces: DeliverConfigSnapshotRequestRequestTypeDef](./type_defs.md#deliverconfigsnapshotrequestrequesttypedef) 

### describe\_aggregate\_compliance\_by\_config\_rules

Returns a list of compliant and noncompliant rules with the number of resources
for compliant and noncompliant rules.

Type annotations and code completion for `#!python session.client("config").describe_aggregate_compliance_by_config_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_aggregate_compliance_by_config_rules method definition

await def describe_aggregate_compliance_by_config_rules(
    self,
    *,
    ConfigurationAggregatorName: str,
    Filters: ConfigRuleComplianceFiltersTypeDef = ...,  # (1)
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeAggregateComplianceByConfigRulesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConfigRuleComplianceFiltersTypeDef](./type_defs.md#configrulecompliancefilterstypedef) 
2. See [:material-code-braces: DescribeAggregateComplianceByConfigRulesResponseTypeDef](./type_defs.md#describeaggregatecompliancebyconfigrulesresponsetypedef) 


```python
# describe_aggregate_compliance_by_config_rules method usage example with argument unpacking

kwargs: DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
}

parent.describe_aggregate_compliance_by_config_rules(**kwargs)
```

1. See [:material-code-braces: DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef](./type_defs.md#describeaggregatecompliancebyconfigrulesrequestrequesttypedef) 

### describe\_aggregate\_compliance\_by\_conformance\_packs

Returns a list of the existing and deleted conformance packs and their
associated compliance status with the count of compliant and noncompliant
Config rules within each conformance pack.

Type annotations and code completion for `#!python session.client("config").describe_aggregate_compliance_by_conformance_packs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_aggregate_compliance_by_conformance_packs method definition

await def describe_aggregate_compliance_by_conformance_packs(
    self,
    *,
    ConfigurationAggregatorName: str,
    Filters: AggregateConformancePackComplianceFiltersTypeDef = ...,  # (1)
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeAggregateComplianceByConformancePacksResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AggregateConformancePackComplianceFiltersTypeDef](./type_defs.md#aggregateconformancepackcompliancefilterstypedef) 
2. See [:material-code-braces: DescribeAggregateComplianceByConformancePacksResponseTypeDef](./type_defs.md#describeaggregatecompliancebyconformancepacksresponsetypedef) 


```python
# describe_aggregate_compliance_by_conformance_packs method usage example with argument unpacking

kwargs: DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
}

parent.describe_aggregate_compliance_by_conformance_packs(**kwargs)
```

1. See [:material-code-braces: DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef](./type_defs.md#describeaggregatecompliancebyconformancepacksrequestrequesttypedef) 

### describe\_aggregation\_authorizations

Returns a list of authorizations granted to various aggregator accounts and
regions.

Type annotations and code completion for `#!python session.client("config").describe_aggregation_authorizations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_aggregation_authorizations method definition

await def describe_aggregation_authorizations(
    self,
    *,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeAggregationAuthorizationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAggregationAuthorizationsResponseTypeDef](./type_defs.md#describeaggregationauthorizationsresponsetypedef) 


```python
# describe_aggregation_authorizations method usage example with argument unpacking

kwargs: DescribeAggregationAuthorizationsRequestRequestTypeDef = {  # (1)
    "Limit": ...,
}

parent.describe_aggregation_authorizations(**kwargs)
```

1. See [:material-code-braces: DescribeAggregationAuthorizationsRequestRequestTypeDef](./type_defs.md#describeaggregationauthorizationsrequestrequesttypedef) 

### describe\_compliance\_by\_config\_rule

Indicates whether the specified Config rules are compliant.

Type annotations and code completion for `#!python session.client("config").describe_compliance_by_config_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_compliance_by_config_rule method definition

await def describe_compliance_by_config_rule(
    self,
    *,
    ConfigRuleNames: Sequence[str] = ...,
    ComplianceTypes: Sequence[ComplianceTypeType] = ...,  # (1)
    NextToken: str = ...,
) -> DescribeComplianceByConfigRuleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: DescribeComplianceByConfigRuleResponseTypeDef](./type_defs.md#describecompliancebyconfigruleresponsetypedef) 


```python
# describe_compliance_by_config_rule method usage example with argument unpacking

kwargs: DescribeComplianceByConfigRuleRequestRequestTypeDef = {  # (1)
    "ConfigRuleNames": ...,
}

parent.describe_compliance_by_config_rule(**kwargs)
```

1. See [:material-code-braces: DescribeComplianceByConfigRuleRequestRequestTypeDef](./type_defs.md#describecompliancebyconfigrulerequestrequesttypedef) 

### describe\_compliance\_by\_resource

Indicates whether the specified Amazon Web Services resources are compliant.

Type annotations and code completion for `#!python session.client("config").describe_compliance_by_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_compliance_by_resource method definition

await def describe_compliance_by_resource(
    self,
    *,
    ResourceType: str = ...,
    ResourceId: str = ...,
    ComplianceTypes: Sequence[ComplianceTypeType] = ...,  # (1)
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeComplianceByResourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: DescribeComplianceByResourceResponseTypeDef](./type_defs.md#describecompliancebyresourceresponsetypedef) 


```python
# describe_compliance_by_resource method usage example with argument unpacking

kwargs: DescribeComplianceByResourceRequestRequestTypeDef = {  # (1)
    "ResourceType": ...,
}

parent.describe_compliance_by_resource(**kwargs)
```

1. See [:material-code-braces: DescribeComplianceByResourceRequestRequestTypeDef](./type_defs.md#describecompliancebyresourcerequestrequesttypedef) 

### describe\_config\_rule\_evaluation\_status

Returns status information for each of your Config managed rules.

Type annotations and code completion for `#!python session.client("config").describe_config_rule_evaluation_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_config_rule_evaluation_status method definition

await def describe_config_rule_evaluation_status(
    self,
    *,
    ConfigRuleNames: Sequence[str] = ...,
    NextToken: str = ...,
    Limit: int = ...,
) -> DescribeConfigRuleEvaluationStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeConfigRuleEvaluationStatusResponseTypeDef](./type_defs.md#describeconfigruleevaluationstatusresponsetypedef) 


```python
# describe_config_rule_evaluation_status method usage example with argument unpacking

kwargs: DescribeConfigRuleEvaluationStatusRequestRequestTypeDef = {  # (1)
    "ConfigRuleNames": ...,
}

parent.describe_config_rule_evaluation_status(**kwargs)
```

1. See [:material-code-braces: DescribeConfigRuleEvaluationStatusRequestRequestTypeDef](./type_defs.md#describeconfigruleevaluationstatusrequestrequesttypedef) 

### describe\_config\_rules

Returns details about your Config rules.

Type annotations and code completion for `#!python session.client("config").describe_config_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_config_rules method definition

await def describe_config_rules(
    self,
    *,
    ConfigRuleNames: Sequence[str] = ...,
    NextToken: str = ...,
    Filters: DescribeConfigRulesFiltersTypeDef = ...,  # (1)
) -> DescribeConfigRulesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DescribeConfigRulesFiltersTypeDef](./type_defs.md#describeconfigrulesfilterstypedef) 
2. See [:material-code-braces: DescribeConfigRulesResponseTypeDef](./type_defs.md#describeconfigrulesresponsetypedef) 


```python
# describe_config_rules method usage example with argument unpacking

kwargs: DescribeConfigRulesRequestRequestTypeDef = {  # (1)
    "ConfigRuleNames": ...,
}

parent.describe_config_rules(**kwargs)
```

1. See [:material-code-braces: DescribeConfigRulesRequestRequestTypeDef](./type_defs.md#describeconfigrulesrequestrequesttypedef) 

### describe\_configuration\_aggregator\_sources\_status

Returns status information for sources within an aggregator.

Type annotations and code completion for `#!python session.client("config").describe_configuration_aggregator_sources_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_configuration_aggregator_sources_status method definition

await def describe_configuration_aggregator_sources_status(
    self,
    *,
    ConfigurationAggregatorName: str,
    UpdateStatus: Sequence[AggregatedSourceStatusTypeType] = ...,  # (1)
    NextToken: str = ...,
    Limit: int = ...,
) -> DescribeConfigurationAggregatorSourcesStatusResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AggregatedSourceStatusTypeType](./literals.md#aggregatedsourcestatustypetype) 
2. See [:material-code-braces: DescribeConfigurationAggregatorSourcesStatusResponseTypeDef](./type_defs.md#describeconfigurationaggregatorsourcesstatusresponsetypedef) 


```python
# describe_configuration_aggregator_sources_status method usage example with argument unpacking

kwargs: DescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
}

parent.describe_configuration_aggregator_sources_status(**kwargs)
```

1. See [:material-code-braces: DescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef](./type_defs.md#describeconfigurationaggregatorsourcesstatusrequestrequesttypedef) 

### describe\_configuration\_aggregators

Returns the details of one or more configuration aggregators.

Type annotations and code completion for `#!python session.client("config").describe_configuration_aggregators` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_configuration_aggregators method definition

await def describe_configuration_aggregators(
    self,
    *,
    ConfigurationAggregatorNames: Sequence[str] = ...,
    NextToken: str = ...,
    Limit: int = ...,
) -> DescribeConfigurationAggregatorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeConfigurationAggregatorsResponseTypeDef](./type_defs.md#describeconfigurationaggregatorsresponsetypedef) 


```python
# describe_configuration_aggregators method usage example with argument unpacking

kwargs: DescribeConfigurationAggregatorsRequestRequestTypeDef = {  # (1)
    "ConfigurationAggregatorNames": ...,
}

parent.describe_configuration_aggregators(**kwargs)
```

1. See [:material-code-braces: DescribeConfigurationAggregatorsRequestRequestTypeDef](./type_defs.md#describeconfigurationaggregatorsrequestrequesttypedef) 

### describe\_configuration\_recorder\_status

Returns the current status of the configuration recorder you specify as well as
the status of the last recording event for the configuration recorders.

Type annotations and code completion for `#!python session.client("config").describe_configuration_recorder_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_configuration_recorder_status method definition

await def describe_configuration_recorder_status(
    self,
    *,
    ConfigurationRecorderNames: Sequence[str] = ...,
    ServicePrincipal: str = ...,
    Arn: str = ...,
) -> DescribeConfigurationRecorderStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeConfigurationRecorderStatusResponseTypeDef](./type_defs.md#describeconfigurationrecorderstatusresponsetypedef) 


```python
# describe_configuration_recorder_status method usage example with argument unpacking

kwargs: DescribeConfigurationRecorderStatusRequestRequestTypeDef = {  # (1)
    "ConfigurationRecorderNames": ...,
}

parent.describe_configuration_recorder_status(**kwargs)
```

1. See [:material-code-braces: DescribeConfigurationRecorderStatusRequestRequestTypeDef](./type_defs.md#describeconfigurationrecorderstatusrequestrequesttypedef) 

### describe\_configuration\_recorders

Returns details for the configuration recorder you specify.

Type annotations and code completion for `#!python session.client("config").describe_configuration_recorders` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_configuration_recorders method definition

await def describe_configuration_recorders(
    self,
    *,
    ConfigurationRecorderNames: Sequence[str] = ...,
    ServicePrincipal: str = ...,
    Arn: str = ...,
) -> DescribeConfigurationRecordersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeConfigurationRecordersResponseTypeDef](./type_defs.md#describeconfigurationrecordersresponsetypedef) 


```python
# describe_configuration_recorders method usage example with argument unpacking

kwargs: DescribeConfigurationRecordersRequestRequestTypeDef = {  # (1)
    "ConfigurationRecorderNames": ...,
}

parent.describe_configuration_recorders(**kwargs)
```

1. See [:material-code-braces: DescribeConfigurationRecordersRequestRequestTypeDef](./type_defs.md#describeconfigurationrecordersrequestrequesttypedef) 

### describe\_conformance\_pack\_compliance

Returns compliance details for each rule in that conformance pack.

Type annotations and code completion for `#!python session.client("config").describe_conformance_pack_compliance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_conformance_pack_compliance method definition

await def describe_conformance_pack_compliance(
    self,
    *,
    ConformancePackName: str,
    Filters: ConformancePackComplianceFiltersTypeDef = ...,  # (1)
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeConformancePackComplianceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConformancePackComplianceFiltersTypeDef](./type_defs.md#conformancepackcompliancefilterstypedef) 
2. See [:material-code-braces: DescribeConformancePackComplianceResponseTypeDef](./type_defs.md#describeconformancepackcomplianceresponsetypedef) 


```python
# describe_conformance_pack_compliance method usage example with argument unpacking

kwargs: DescribeConformancePackComplianceRequestRequestTypeDef = {  # (1)
    "ConformancePackName": ...,
}

parent.describe_conformance_pack_compliance(**kwargs)
```

1. See [:material-code-braces: DescribeConformancePackComplianceRequestRequestTypeDef](./type_defs.md#describeconformancepackcompliancerequestrequesttypedef) 

### describe\_conformance\_pack\_status

Provides one or more conformance packs deployment status.

Type annotations and code completion for `#!python session.client("config").describe_conformance_pack_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_conformance_pack_status method definition

await def describe_conformance_pack_status(
    self,
    *,
    ConformancePackNames: Sequence[str] = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeConformancePackStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeConformancePackStatusResponseTypeDef](./type_defs.md#describeconformancepackstatusresponsetypedef) 


```python
# describe_conformance_pack_status method usage example with argument unpacking

kwargs: DescribeConformancePackStatusRequestRequestTypeDef = {  # (1)
    "ConformancePackNames": ...,
}

parent.describe_conformance_pack_status(**kwargs)
```

1. See [:material-code-braces: DescribeConformancePackStatusRequestRequestTypeDef](./type_defs.md#describeconformancepackstatusrequestrequesttypedef) 

### describe\_conformance\_packs

Returns a list of one or more conformance packs.

Type annotations and code completion for `#!python session.client("config").describe_conformance_packs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_conformance_packs method definition

await def describe_conformance_packs(
    self,
    *,
    ConformancePackNames: Sequence[str] = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeConformancePacksResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeConformancePacksResponseTypeDef](./type_defs.md#describeconformancepacksresponsetypedef) 


```python
# describe_conformance_packs method usage example with argument unpacking

kwargs: DescribeConformancePacksRequestRequestTypeDef = {  # (1)
    "ConformancePackNames": ...,
}

parent.describe_conformance_packs(**kwargs)
```

1. See [:material-code-braces: DescribeConformancePacksRequestRequestTypeDef](./type_defs.md#describeconformancepacksrequestrequesttypedef) 

### describe\_delivery\_channel\_status

Returns the current status of the specified delivery channel.

Type annotations and code completion for `#!python session.client("config").describe_delivery_channel_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_delivery_channel_status method definition

await def describe_delivery_channel_status(
    self,
    *,
    DeliveryChannelNames: Sequence[str] = ...,
) -> DescribeDeliveryChannelStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDeliveryChannelStatusResponseTypeDef](./type_defs.md#describedeliverychannelstatusresponsetypedef) 


```python
# describe_delivery_channel_status method usage example with argument unpacking

kwargs: DescribeDeliveryChannelStatusRequestRequestTypeDef = {  # (1)
    "DeliveryChannelNames": ...,
}

parent.describe_delivery_channel_status(**kwargs)
```

1. See [:material-code-braces: DescribeDeliveryChannelStatusRequestRequestTypeDef](./type_defs.md#describedeliverychannelstatusrequestrequesttypedef) 

### describe\_delivery\_channels

Returns details about the specified delivery channel.

Type annotations and code completion for `#!python session.client("config").describe_delivery_channels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_delivery_channels method definition

await def describe_delivery_channels(
    self,
    *,
    DeliveryChannelNames: Sequence[str] = ...,
) -> DescribeDeliveryChannelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDeliveryChannelsResponseTypeDef](./type_defs.md#describedeliverychannelsresponsetypedef) 


```python
# describe_delivery_channels method usage example with argument unpacking

kwargs: DescribeDeliveryChannelsRequestRequestTypeDef = {  # (1)
    "DeliveryChannelNames": ...,
}

parent.describe_delivery_channels(**kwargs)
```

1. See [:material-code-braces: DescribeDeliveryChannelsRequestRequestTypeDef](./type_defs.md#describedeliverychannelsrequestrequesttypedef) 

### describe\_organization\_config\_rule\_statuses

Provides organization Config rule deployment status for an organization.

Type annotations and code completion for `#!python session.client("config").describe_organization_config_rule_statuses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_organization_config_rule_statuses method definition

await def describe_organization_config_rule_statuses(
    self,
    *,
    OrganizationConfigRuleNames: Sequence[str] = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeOrganizationConfigRuleStatusesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeOrganizationConfigRuleStatusesResponseTypeDef](./type_defs.md#describeorganizationconfigrulestatusesresponsetypedef) 


```python
# describe_organization_config_rule_statuses method usage example with argument unpacking

kwargs: DescribeOrganizationConfigRuleStatusesRequestRequestTypeDef = {  # (1)
    "OrganizationConfigRuleNames": ...,
}

parent.describe_organization_config_rule_statuses(**kwargs)
```

1. See [:material-code-braces: DescribeOrganizationConfigRuleStatusesRequestRequestTypeDef](./type_defs.md#describeorganizationconfigrulestatusesrequestrequesttypedef) 

### describe\_organization\_config\_rules

Returns a list of organization Config rules.

Type annotations and code completion for `#!python session.client("config").describe_organization_config_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_organization_config_rules method definition

await def describe_organization_config_rules(
    self,
    *,
    OrganizationConfigRuleNames: Sequence[str] = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeOrganizationConfigRulesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeOrganizationConfigRulesResponseTypeDef](./type_defs.md#describeorganizationconfigrulesresponsetypedef) 


```python
# describe_organization_config_rules method usage example with argument unpacking

kwargs: DescribeOrganizationConfigRulesRequestRequestTypeDef = {  # (1)
    "OrganizationConfigRuleNames": ...,
}

parent.describe_organization_config_rules(**kwargs)
```

1. See [:material-code-braces: DescribeOrganizationConfigRulesRequestRequestTypeDef](./type_defs.md#describeorganizationconfigrulesrequestrequesttypedef) 

### describe\_organization\_conformance\_pack\_statuses

Provides organization conformance pack deployment status for an organization.

Type annotations and code completion for `#!python session.client("config").describe_organization_conformance_pack_statuses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_organization_conformance_pack_statuses method definition

await def describe_organization_conformance_pack_statuses(
    self,
    *,
    OrganizationConformancePackNames: Sequence[str] = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeOrganizationConformancePackStatusesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeOrganizationConformancePackStatusesResponseTypeDef](./type_defs.md#describeorganizationconformancepackstatusesresponsetypedef) 


```python
# describe_organization_conformance_pack_statuses method usage example with argument unpacking

kwargs: DescribeOrganizationConformancePackStatusesRequestRequestTypeDef = {  # (1)
    "OrganizationConformancePackNames": ...,
}

parent.describe_organization_conformance_pack_statuses(**kwargs)
```

1. See [:material-code-braces: DescribeOrganizationConformancePackStatusesRequestRequestTypeDef](./type_defs.md#describeorganizationconformancepackstatusesrequestrequesttypedef) 

### describe\_organization\_conformance\_packs

Returns a list of organization conformance packs.

Type annotations and code completion for `#!python session.client("config").describe_organization_conformance_packs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_organization_conformance_packs method definition

await def describe_organization_conformance_packs(
    self,
    *,
    OrganizationConformancePackNames: Sequence[str] = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeOrganizationConformancePacksResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeOrganizationConformancePacksResponseTypeDef](./type_defs.md#describeorganizationconformancepacksresponsetypedef) 


```python
# describe_organization_conformance_packs method usage example with argument unpacking

kwargs: DescribeOrganizationConformancePacksRequestRequestTypeDef = {  # (1)
    "OrganizationConformancePackNames": ...,
}

parent.describe_organization_conformance_packs(**kwargs)
```

1. See [:material-code-braces: DescribeOrganizationConformancePacksRequestRequestTypeDef](./type_defs.md#describeorganizationconformancepacksrequestrequesttypedef) 

### describe\_pending\_aggregation\_requests

Returns a list of all pending aggregation requests.

Type annotations and code completion for `#!python session.client("config").describe_pending_aggregation_requests` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_pending_aggregation_requests method definition

await def describe_pending_aggregation_requests(
    self,
    *,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribePendingAggregationRequestsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePendingAggregationRequestsResponseTypeDef](./type_defs.md#describependingaggregationrequestsresponsetypedef) 


```python
# describe_pending_aggregation_requests method usage example with argument unpacking

kwargs: DescribePendingAggregationRequestsRequestRequestTypeDef = {  # (1)
    "Limit": ...,
}

parent.describe_pending_aggregation_requests(**kwargs)
```

1. See [:material-code-braces: DescribePendingAggregationRequestsRequestRequestTypeDef](./type_defs.md#describependingaggregationrequestsrequestrequesttypedef) 

### describe\_remediation\_configurations

Returns the details of one or more remediation configurations.

Type annotations and code completion for `#!python session.client("config").describe_remediation_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_remediation_configurations method definition

await def describe_remediation_configurations(
    self,
    *,
    ConfigRuleNames: Sequence[str],
) -> DescribeRemediationConfigurationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRemediationConfigurationsResponseTypeDef](./type_defs.md#describeremediationconfigurationsresponsetypedef) 


```python
# describe_remediation_configurations method usage example with argument unpacking

kwargs: DescribeRemediationConfigurationsRequestRequestTypeDef = {  # (1)
    "ConfigRuleNames": ...,
}

parent.describe_remediation_configurations(**kwargs)
```

1. See [:material-code-braces: DescribeRemediationConfigurationsRequestRequestTypeDef](./type_defs.md#describeremediationconfigurationsrequestrequesttypedef) 

### describe\_remediation\_exceptions

Returns the details of one or more remediation exceptions.

Type annotations and code completion for `#!python session.client("config").describe_remediation_exceptions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_remediation_exceptions method definition

await def describe_remediation_exceptions(
    self,
    *,
    ConfigRuleName: str,
    ResourceKeys: Sequence[RemediationExceptionResourceKeyTypeDef] = ...,  # (1)
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeRemediationExceptionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RemediationExceptionResourceKeyTypeDef](./type_defs.md#remediationexceptionresourcekeytypedef) 
2. See [:material-code-braces: DescribeRemediationExceptionsResponseTypeDef](./type_defs.md#describeremediationexceptionsresponsetypedef) 


```python
# describe_remediation_exceptions method usage example with argument unpacking

kwargs: DescribeRemediationExceptionsRequestRequestTypeDef = {  # (1)
    "ConfigRuleName": ...,
}

parent.describe_remediation_exceptions(**kwargs)
```

1. See [:material-code-braces: DescribeRemediationExceptionsRequestRequestTypeDef](./type_defs.md#describeremediationexceptionsrequestrequesttypedef) 

### describe\_remediation\_execution\_status

Provides a detailed view of a Remediation Execution for a set of resources
including state, timestamps for when steps for the remediation execution occur,
and any error messages for steps that have failed.

Type annotations and code completion for `#!python session.client("config").describe_remediation_execution_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_remediation_execution_status method definition

await def describe_remediation_execution_status(
    self,
    *,
    ConfigRuleName: str,
    ResourceKeys: Sequence[ResourceKeyTypeDef] = ...,  # (1)
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeRemediationExecutionStatusResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ResourceKeyTypeDef](./type_defs.md#resourcekeytypedef) 
2. See [:material-code-braces: DescribeRemediationExecutionStatusResponseTypeDef](./type_defs.md#describeremediationexecutionstatusresponsetypedef) 


```python
# describe_remediation_execution_status method usage example with argument unpacking

kwargs: DescribeRemediationExecutionStatusRequestRequestTypeDef = {  # (1)
    "ConfigRuleName": ...,
}

parent.describe_remediation_execution_status(**kwargs)
```

1. See [:material-code-braces: DescribeRemediationExecutionStatusRequestRequestTypeDef](./type_defs.md#describeremediationexecutionstatusrequestrequesttypedef) 

### describe\_retention\_configurations

Returns the details of one or more retention configurations.

Type annotations and code completion for `#!python session.client("config").describe_retention_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# describe_retention_configurations method definition

await def describe_retention_configurations(
    self,
    *,
    RetentionConfigurationNames: Sequence[str] = ...,
    NextToken: str = ...,
) -> DescribeRetentionConfigurationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRetentionConfigurationsResponseTypeDef](./type_defs.md#describeretentionconfigurationsresponsetypedef) 


```python
# describe_retention_configurations method usage example with argument unpacking

kwargs: DescribeRetentionConfigurationsRequestRequestTypeDef = {  # (1)
    "RetentionConfigurationNames": ...,
}

parent.describe_retention_configurations(**kwargs)
```

1. See [:material-code-braces: DescribeRetentionConfigurationsRequestRequestTypeDef](./type_defs.md#describeretentionconfigurationsrequestrequesttypedef) 

### disassociate\_resource\_types

Removes all resource types specified in the <code>ResourceTypes</code> list
from the <a
href="https://docs.aws.amazon.com/config/latest/APIReference/API_RecordingGroup.html">RecordingGroup</a>
of configuration recorder and excludes these resource types when recording.

Type annotations and code completion for `#!python session.client("config").disassociate_resource_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# disassociate_resource_types method definition

await def disassociate_resource_types(
    self,
    *,
    ConfigurationRecorderArn: str,
    ResourceTypes: Sequence[ResourceTypeType],  # (1)
) -> DisassociateResourceTypesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: DisassociateResourceTypesResponseTypeDef](./type_defs.md#disassociateresourcetypesresponsetypedef) 


```python
# disassociate_resource_types method usage example with argument unpacking

kwargs: DisassociateResourceTypesRequestRequestTypeDef = {  # (1)
    "ConfigurationRecorderArn": ...,
    "ResourceTypes": ...,
}

parent.disassociate_resource_types(**kwargs)
```

1. See [:material-code-braces: DisassociateResourceTypesRequestRequestTypeDef](./type_defs.md#disassociateresourcetypesrequestrequesttypedef) 

### get\_aggregate\_compliance\_details\_by\_config\_rule

Returns the evaluation results for the specified Config rule for a specific
resource in a rule.

Type annotations and code completion for `#!python session.client("config").get_aggregate_compliance_details_by_config_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# get_aggregate_compliance_details_by_config_rule method definition

await def get_aggregate_compliance_details_by_config_rule(
    self,
    *,
    ConfigurationAggregatorName: str,
    ConfigRuleName: str,
    AccountId: str,
    AwsRegion: str,
    ComplianceType: ComplianceTypeType = ...,  # (1)
    Limit: int = ...,
    NextToken: str = ...,
) -> GetAggregateComplianceDetailsByConfigRuleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: GetAggregateComplianceDetailsByConfigRuleResponseTypeDef](./type_defs.md#getaggregatecompliancedetailsbyconfigruleresponsetypedef) 


```python
# get_aggregate_compliance_details_by_config_rule method usage example with argument unpacking

kwargs: GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
    "ConfigRuleName": ...,
    "AccountId": ...,
    "AwsRegion": ...,
}

parent.get_aggregate_compliance_details_by_config_rule(**kwargs)
```

1. See [:material-code-braces: GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef](./type_defs.md#getaggregatecompliancedetailsbyconfigrulerequestrequesttypedef) 

### get\_aggregate\_config\_rule\_compliance\_summary

Returns the number of compliant and noncompliant rules for one or more accounts
and regions in an aggregator.

Type annotations and code completion for `#!python session.client("config").get_aggregate_config_rule_compliance_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# get_aggregate_config_rule_compliance_summary method definition

await def get_aggregate_config_rule_compliance_summary(
    self,
    *,
    ConfigurationAggregatorName: str,
    Filters: ConfigRuleComplianceSummaryFiltersTypeDef = ...,  # (1)
    GroupByKey: ConfigRuleComplianceSummaryGroupKeyType = ...,  # (2)
    Limit: int = ...,
    NextToken: str = ...,
) -> GetAggregateConfigRuleComplianceSummaryResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ConfigRuleComplianceSummaryFiltersTypeDef](./type_defs.md#configrulecompliancesummaryfilterstypedef) 
2. See [:material-code-brackets: ConfigRuleComplianceSummaryGroupKeyType](./literals.md#configrulecompliancesummarygroupkeytype) 
3. See [:material-code-braces: GetAggregateConfigRuleComplianceSummaryResponseTypeDef](./type_defs.md#getaggregateconfigrulecompliancesummaryresponsetypedef) 


```python
# get_aggregate_config_rule_compliance_summary method usage example with argument unpacking

kwargs: GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
}

parent.get_aggregate_config_rule_compliance_summary(**kwargs)
```

1. See [:material-code-braces: GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef](./type_defs.md#getaggregateconfigrulecompliancesummaryrequestrequesttypedef) 

### get\_aggregate\_conformance\_pack\_compliance\_summary

Returns the count of compliant and noncompliant conformance packs across all
Amazon Web Services accounts and Amazon Web Services Regions in an aggregator.

Type annotations and code completion for `#!python session.client("config").get_aggregate_conformance_pack_compliance_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# get_aggregate_conformance_pack_compliance_summary method definition

await def get_aggregate_conformance_pack_compliance_summary(
    self,
    *,
    ConfigurationAggregatorName: str,
    Filters: AggregateConformancePackComplianceSummaryFiltersTypeDef = ...,  # (1)
    GroupByKey: AggregateConformancePackComplianceSummaryGroupKeyType = ...,  # (2)
    Limit: int = ...,
    NextToken: str = ...,
) -> GetAggregateConformancePackComplianceSummaryResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AggregateConformancePackComplianceSummaryFiltersTypeDef](./type_defs.md#aggregateconformancepackcompliancesummaryfilterstypedef) 
2. See [:material-code-brackets: AggregateConformancePackComplianceSummaryGroupKeyType](./literals.md#aggregateconformancepackcompliancesummarygroupkeytype) 
3. See [:material-code-braces: GetAggregateConformancePackComplianceSummaryResponseTypeDef](./type_defs.md#getaggregateconformancepackcompliancesummaryresponsetypedef) 


```python
# get_aggregate_conformance_pack_compliance_summary method usage example with argument unpacking

kwargs: GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
}

parent.get_aggregate_conformance_pack_compliance_summary(**kwargs)
```

1. See [:material-code-braces: GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef](./type_defs.md#getaggregateconformancepackcompliancesummaryrequestrequesttypedef) 

### get\_aggregate\_discovered\_resource\_counts

Returns the resource counts across accounts and regions that are present in
your Config aggregator.

Type annotations and code completion for `#!python session.client("config").get_aggregate_discovered_resource_counts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# get_aggregate_discovered_resource_counts method definition

await def get_aggregate_discovered_resource_counts(
    self,
    *,
    ConfigurationAggregatorName: str,
    Filters: ResourceCountFiltersTypeDef = ...,  # (1)
    GroupByKey: ResourceCountGroupKeyType = ...,  # (2)
    Limit: int = ...,
    NextToken: str = ...,
) -> GetAggregateDiscoveredResourceCountsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourceCountFiltersTypeDef](./type_defs.md#resourcecountfilterstypedef) 
2. See [:material-code-brackets: ResourceCountGroupKeyType](./literals.md#resourcecountgroupkeytype) 
3. See [:material-code-braces: GetAggregateDiscoveredResourceCountsResponseTypeDef](./type_defs.md#getaggregatediscoveredresourcecountsresponsetypedef) 


```python
# get_aggregate_discovered_resource_counts method usage example with argument unpacking

kwargs: GetAggregateDiscoveredResourceCountsRequestRequestTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
}

parent.get_aggregate_discovered_resource_counts(**kwargs)
```

1. See [:material-code-braces: GetAggregateDiscoveredResourceCountsRequestRequestTypeDef](./type_defs.md#getaggregatediscoveredresourcecountsrequestrequesttypedef) 

### get\_aggregate\_resource\_config

Returns configuration item that is aggregated for your specific resource in a
specific source account and region.

Type annotations and code completion for `#!python session.client("config").get_aggregate_resource_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# get_aggregate_resource_config method definition

await def get_aggregate_resource_config(
    self,
    *,
    ConfigurationAggregatorName: str,
    ResourceIdentifier: AggregateResourceIdentifierTypeDef,  # (1)
) -> GetAggregateResourceConfigResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AggregateResourceIdentifierTypeDef](./type_defs.md#aggregateresourceidentifiertypedef) 
2. See [:material-code-braces: GetAggregateResourceConfigResponseTypeDef](./type_defs.md#getaggregateresourceconfigresponsetypedef) 


```python
# get_aggregate_resource_config method usage example with argument unpacking

kwargs: GetAggregateResourceConfigRequestRequestTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
    "ResourceIdentifier": ...,
}

parent.get_aggregate_resource_config(**kwargs)
```

1. See [:material-code-braces: GetAggregateResourceConfigRequestRequestTypeDef](./type_defs.md#getaggregateresourceconfigrequestrequesttypedef) 

### get\_compliance\_details\_by\_config\_rule

Returns the evaluation results for the specified Config rule.

Type annotations and code completion for `#!python session.client("config").get_compliance_details_by_config_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# get_compliance_details_by_config_rule method definition

await def get_compliance_details_by_config_rule(
    self,
    *,
    ConfigRuleName: str,
    ComplianceTypes: Sequence[ComplianceTypeType] = ...,  # (1)
    Limit: int = ...,
    NextToken: str = ...,
) -> GetComplianceDetailsByConfigRuleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: GetComplianceDetailsByConfigRuleResponseTypeDef](./type_defs.md#getcompliancedetailsbyconfigruleresponsetypedef) 


```python
# get_compliance_details_by_config_rule method usage example with argument unpacking

kwargs: GetComplianceDetailsByConfigRuleRequestRequestTypeDef = {  # (1)
    "ConfigRuleName": ...,
}

parent.get_compliance_details_by_config_rule(**kwargs)
```

1. See [:material-code-braces: GetComplianceDetailsByConfigRuleRequestRequestTypeDef](./type_defs.md#getcompliancedetailsbyconfigrulerequestrequesttypedef) 

### get\_compliance\_details\_by\_resource

Returns the evaluation results for the specified Amazon Web Services resource.

Type annotations and code completion for `#!python session.client("config").get_compliance_details_by_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# get_compliance_details_by_resource method definition

await def get_compliance_details_by_resource(
    self,
    *,
    ResourceType: str = ...,
    ResourceId: str = ...,
    ComplianceTypes: Sequence[ComplianceTypeType] = ...,  # (1)
    NextToken: str = ...,
    ResourceEvaluationId: str = ...,
) -> GetComplianceDetailsByResourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: GetComplianceDetailsByResourceResponseTypeDef](./type_defs.md#getcompliancedetailsbyresourceresponsetypedef) 


```python
# get_compliance_details_by_resource method usage example with argument unpacking

kwargs: GetComplianceDetailsByResourceRequestRequestTypeDef = {  # (1)
    "ResourceType": ...,
}

parent.get_compliance_details_by_resource(**kwargs)
```

1. See [:material-code-braces: GetComplianceDetailsByResourceRequestRequestTypeDef](./type_defs.md#getcompliancedetailsbyresourcerequestrequesttypedef) 

### get\_compliance\_summary\_by\_config\_rule

Returns the number of Config rules that are compliant and noncompliant, up to a
maximum of 25 for each.

Type annotations and code completion for `#!python session.client("config").get_compliance_summary_by_config_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# get_compliance_summary_by_config_rule method definition

await def get_compliance_summary_by_config_rule(
    self,
) -> GetComplianceSummaryByConfigRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetComplianceSummaryByConfigRuleResponseTypeDef](./type_defs.md#getcompliancesummarybyconfigruleresponsetypedef) 

### get\_compliance\_summary\_by\_resource\_type

Returns the number of resources that are compliant and the number that are
noncompliant.

Type annotations and code completion for `#!python session.client("config").get_compliance_summary_by_resource_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# get_compliance_summary_by_resource_type method definition

await def get_compliance_summary_by_resource_type(
    self,
    *,
    ResourceTypes: Sequence[str] = ...,
) -> GetComplianceSummaryByResourceTypeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetComplianceSummaryByResourceTypeResponseTypeDef](./type_defs.md#getcompliancesummarybyresourcetyperesponsetypedef) 


```python
# get_compliance_summary_by_resource_type method usage example with argument unpacking

kwargs: GetComplianceSummaryByResourceTypeRequestRequestTypeDef = {  # (1)
    "ResourceTypes": ...,
}

parent.get_compliance_summary_by_resource_type(**kwargs)
```

1. See [:material-code-braces: GetComplianceSummaryByResourceTypeRequestRequestTypeDef](./type_defs.md#getcompliancesummarybyresourcetyperequestrequesttypedef) 

### get\_conformance\_pack\_compliance\_details

Returns compliance details of a conformance pack for all Amazon Web Services
resources that are monitered by conformance pack.

Type annotations and code completion for `#!python session.client("config").get_conformance_pack_compliance_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# get_conformance_pack_compliance_details method definition

await def get_conformance_pack_compliance_details(
    self,
    *,
    ConformancePackName: str,
    Filters: ConformancePackEvaluationFiltersTypeDef = ...,  # (1)
    Limit: int = ...,
    NextToken: str = ...,
) -> GetConformancePackComplianceDetailsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConformancePackEvaluationFiltersTypeDef](./type_defs.md#conformancepackevaluationfilterstypedef) 
2. See [:material-code-braces: GetConformancePackComplianceDetailsResponseTypeDef](./type_defs.md#getconformancepackcompliancedetailsresponsetypedef) 


```python
# get_conformance_pack_compliance_details method usage example with argument unpacking

kwargs: GetConformancePackComplianceDetailsRequestRequestTypeDef = {  # (1)
    "ConformancePackName": ...,
}

parent.get_conformance_pack_compliance_details(**kwargs)
```

1. See [:material-code-braces: GetConformancePackComplianceDetailsRequestRequestTypeDef](./type_defs.md#getconformancepackcompliancedetailsrequestrequesttypedef) 

### get\_conformance\_pack\_compliance\_summary

Returns compliance details for the conformance pack based on the cumulative
compliance results of all the rules in that conformance pack.

Type annotations and code completion for `#!python session.client("config").get_conformance_pack_compliance_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# get_conformance_pack_compliance_summary method definition

await def get_conformance_pack_compliance_summary(
    self,
    *,
    ConformancePackNames: Sequence[str],
    Limit: int = ...,
    NextToken: str = ...,
) -> GetConformancePackComplianceSummaryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConformancePackComplianceSummaryResponseTypeDef](./type_defs.md#getconformancepackcompliancesummaryresponsetypedef) 


```python
# get_conformance_pack_compliance_summary method usage example with argument unpacking

kwargs: GetConformancePackComplianceSummaryRequestRequestTypeDef = {  # (1)
    "ConformancePackNames": ...,
}

parent.get_conformance_pack_compliance_summary(**kwargs)
```

1. See [:material-code-braces: GetConformancePackComplianceSummaryRequestRequestTypeDef](./type_defs.md#getconformancepackcompliancesummaryrequestrequesttypedef) 

### get\_custom\_rule\_policy

Returns the policy definition containing the logic for your Config Custom
Policy rule.

Type annotations and code completion for `#!python session.client("config").get_custom_rule_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# get_custom_rule_policy method definition

await def get_custom_rule_policy(
    self,
    *,
    ConfigRuleName: str = ...,
) -> GetCustomRulePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCustomRulePolicyResponseTypeDef](./type_defs.md#getcustomrulepolicyresponsetypedef) 


```python
# get_custom_rule_policy method usage example with argument unpacking

kwargs: GetCustomRulePolicyRequestRequestTypeDef = {  # (1)
    "ConfigRuleName": ...,
}

parent.get_custom_rule_policy(**kwargs)
```

1. See [:material-code-braces: GetCustomRulePolicyRequestRequestTypeDef](./type_defs.md#getcustomrulepolicyrequestrequesttypedef) 

### get\_discovered\_resource\_counts

Returns the resource types, the number of each resource type, and the total
number of resources that Config is recording in this region for your Amazon Web
Services account.

Type annotations and code completion for `#!python session.client("config").get_discovered_resource_counts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# get_discovered_resource_counts method definition

await def get_discovered_resource_counts(
    self,
    *,
    resourceTypes: Sequence[str] = ...,
    limit: int = ...,
    nextToken: str = ...,
) -> GetDiscoveredResourceCountsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDiscoveredResourceCountsResponseTypeDef](./type_defs.md#getdiscoveredresourcecountsresponsetypedef) 


```python
# get_discovered_resource_counts method usage example with argument unpacking

kwargs: GetDiscoveredResourceCountsRequestRequestTypeDef = {  # (1)
    "resourceTypes": ...,
}

parent.get_discovered_resource_counts(**kwargs)
```

1. See [:material-code-braces: GetDiscoveredResourceCountsRequestRequestTypeDef](./type_defs.md#getdiscoveredresourcecountsrequestrequesttypedef) 

### get\_organization\_config\_rule\_detailed\_status

Returns detailed status for each member account within an organization for a
given organization Config rule.

Type annotations and code completion for `#!python session.client("config").get_organization_config_rule_detailed_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# get_organization_config_rule_detailed_status method definition

await def get_organization_config_rule_detailed_status(
    self,
    *,
    OrganizationConfigRuleName: str,
    Filters: StatusDetailFiltersTypeDef = ...,  # (1)
    Limit: int = ...,
    NextToken: str = ...,
) -> GetOrganizationConfigRuleDetailedStatusResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StatusDetailFiltersTypeDef](./type_defs.md#statusdetailfilterstypedef) 
2. See [:material-code-braces: GetOrganizationConfigRuleDetailedStatusResponseTypeDef](./type_defs.md#getorganizationconfigruledetailedstatusresponsetypedef) 


```python
# get_organization_config_rule_detailed_status method usage example with argument unpacking

kwargs: GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef = {  # (1)
    "OrganizationConfigRuleName": ...,
}

parent.get_organization_config_rule_detailed_status(**kwargs)
```

1. See [:material-code-braces: GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef](./type_defs.md#getorganizationconfigruledetailedstatusrequestrequesttypedef) 

### get\_organization\_conformance\_pack\_detailed\_status

Returns detailed status for each member account within an organization for a
given organization conformance pack.

Type annotations and code completion for `#!python session.client("config").get_organization_conformance_pack_detailed_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# get_organization_conformance_pack_detailed_status method definition

await def get_organization_conformance_pack_detailed_status(
    self,
    *,
    OrganizationConformancePackName: str,
    Filters: OrganizationResourceDetailedStatusFiltersTypeDef = ...,  # (1)
    Limit: int = ...,
    NextToken: str = ...,
) -> GetOrganizationConformancePackDetailedStatusResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OrganizationResourceDetailedStatusFiltersTypeDef](./type_defs.md#organizationresourcedetailedstatusfilterstypedef) 
2. See [:material-code-braces: GetOrganizationConformancePackDetailedStatusResponseTypeDef](./type_defs.md#getorganizationconformancepackdetailedstatusresponsetypedef) 


```python
# get_organization_conformance_pack_detailed_status method usage example with argument unpacking

kwargs: GetOrganizationConformancePackDetailedStatusRequestRequestTypeDef = {  # (1)
    "OrganizationConformancePackName": ...,
}

parent.get_organization_conformance_pack_detailed_status(**kwargs)
```

1. See [:material-code-braces: GetOrganizationConformancePackDetailedStatusRequestRequestTypeDef](./type_defs.md#getorganizationconformancepackdetailedstatusrequestrequesttypedef) 

### get\_organization\_custom\_rule\_policy

Returns the policy definition containing the logic for your organization Config
Custom Policy rule.

Type annotations and code completion for `#!python session.client("config").get_organization_custom_rule_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# get_organization_custom_rule_policy method definition

await def get_organization_custom_rule_policy(
    self,
    *,
    OrganizationConfigRuleName: str,
) -> GetOrganizationCustomRulePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOrganizationCustomRulePolicyResponseTypeDef](./type_defs.md#getorganizationcustomrulepolicyresponsetypedef) 


```python
# get_organization_custom_rule_policy method usage example with argument unpacking

kwargs: GetOrganizationCustomRulePolicyRequestRequestTypeDef = {  # (1)
    "OrganizationConfigRuleName": ...,
}

parent.get_organization_custom_rule_policy(**kwargs)
```

1. See [:material-code-braces: GetOrganizationCustomRulePolicyRequestRequestTypeDef](./type_defs.md#getorganizationcustomrulepolicyrequestrequesttypedef) 

### get\_resource\_config\_history

For accurate reporting on the compliance status, you must record the
<code>AWS::Config::ResourceCompliance</code> resource type.

Type annotations and code completion for `#!python session.client("config").get_resource_config_history` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# get_resource_config_history method definition

await def get_resource_config_history(
    self,
    *,
    resourceType: ResourceTypeType,  # (1)
    resourceId: str,
    laterTime: TimestampTypeDef = ...,
    earlierTime: TimestampTypeDef = ...,
    chronologicalOrder: ChronologicalOrderType = ...,  # (2)
    limit: int = ...,
    nextToken: str = ...,
) -> GetResourceConfigHistoryResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: ChronologicalOrderType](./literals.md#chronologicalordertype) 
3. See [:material-code-braces: GetResourceConfigHistoryResponseTypeDef](./type_defs.md#getresourceconfighistoryresponsetypedef) 


```python
# get_resource_config_history method usage example with argument unpacking

kwargs: GetResourceConfigHistoryRequestRequestTypeDef = {  # (1)
    "resourceType": ...,
    "resourceId": ...,
}

parent.get_resource_config_history(**kwargs)
```

1. See [:material-code-braces: GetResourceConfigHistoryRequestRequestTypeDef](./type_defs.md#getresourceconfighistoryrequestrequesttypedef) 

### get\_resource\_evaluation\_summary

Returns a summary of resource evaluation for the specified resource evaluation
ID from the proactive rules that were run.

Type annotations and code completion for `#!python session.client("config").get_resource_evaluation_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# get_resource_evaluation_summary method definition

await def get_resource_evaluation_summary(
    self,
    *,
    ResourceEvaluationId: str,
) -> GetResourceEvaluationSummaryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResourceEvaluationSummaryResponseTypeDef](./type_defs.md#getresourceevaluationsummaryresponsetypedef) 


```python
# get_resource_evaluation_summary method usage example with argument unpacking

kwargs: GetResourceEvaluationSummaryRequestRequestTypeDef = {  # (1)
    "ResourceEvaluationId": ...,
}

parent.get_resource_evaluation_summary(**kwargs)
```

1. See [:material-code-braces: GetResourceEvaluationSummaryRequestRequestTypeDef](./type_defs.md#getresourceevaluationsummaryrequestrequesttypedef) 

### get\_stored\_query

Returns the details of a specific stored query.

Type annotations and code completion for `#!python session.client("config").get_stored_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# get_stored_query method definition

await def get_stored_query(
    self,
    *,
    QueryName: str,
) -> GetStoredQueryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStoredQueryResponseTypeDef](./type_defs.md#getstoredqueryresponsetypedef) 


```python
# get_stored_query method usage example with argument unpacking

kwargs: GetStoredQueryRequestRequestTypeDef = {  # (1)
    "QueryName": ...,
}

parent.get_stored_query(**kwargs)
```

1. See [:material-code-braces: GetStoredQueryRequestRequestTypeDef](./type_defs.md#getstoredqueryrequestrequesttypedef) 

### list\_aggregate\_discovered\_resources

Accepts a resource type and returns a list of resource identifiers that are
aggregated for a specific resource type across accounts and regions.

Type annotations and code completion for `#!python session.client("config").list_aggregate_discovered_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# list_aggregate_discovered_resources method definition

await def list_aggregate_discovered_resources(
    self,
    *,
    ConfigurationAggregatorName: str,
    ResourceType: ResourceTypeType,  # (1)
    Filters: ResourceFiltersTypeDef = ...,  # (2)
    Limit: int = ...,
    NextToken: str = ...,
) -> ListAggregateDiscoveredResourcesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ResourceFiltersTypeDef](./type_defs.md#resourcefilterstypedef) 
3. See [:material-code-braces: ListAggregateDiscoveredResourcesResponseTypeDef](./type_defs.md#listaggregatediscoveredresourcesresponsetypedef) 


```python
# list_aggregate_discovered_resources method usage example with argument unpacking

kwargs: ListAggregateDiscoveredResourcesRequestRequestTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
    "ResourceType": ...,
}

parent.list_aggregate_discovered_resources(**kwargs)
```

1. See [:material-code-braces: ListAggregateDiscoveredResourcesRequestRequestTypeDef](./type_defs.md#listaggregatediscoveredresourcesrequestrequesttypedef) 

### list\_configuration\_recorders

Returns a list of configuration recorders depending on the filters you specify.

Type annotations and code completion for `#!python session.client("config").list_configuration_recorders` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# list_configuration_recorders method definition

await def list_configuration_recorders(
    self,
    *,
    Filters: Sequence[ConfigurationRecorderFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListConfigurationRecordersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConfigurationRecorderFilterTypeDef](./type_defs.md#configurationrecorderfiltertypedef) 
2. See [:material-code-braces: ListConfigurationRecordersResponseTypeDef](./type_defs.md#listconfigurationrecordersresponsetypedef) 


```python
# list_configuration_recorders method usage example with argument unpacking

kwargs: ListConfigurationRecordersRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.list_configuration_recorders(**kwargs)
```

1. See [:material-code-braces: ListConfigurationRecordersRequestRequestTypeDef](./type_defs.md#listconfigurationrecordersrequestrequesttypedef) 

### list\_conformance\_pack\_compliance\_scores

Returns a list of conformance pack compliance scores.

Type annotations and code completion for `#!python session.client("config").list_conformance_pack_compliance_scores` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# list_conformance_pack_compliance_scores method definition

await def list_conformance_pack_compliance_scores(
    self,
    *,
    Filters: ConformancePackComplianceScoresFiltersTypeDef = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    SortBy: SortByType = ...,  # (3)
    Limit: int = ...,
    NextToken: str = ...,
) -> ListConformancePackComplianceScoresResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ConformancePackComplianceScoresFiltersTypeDef](./type_defs.md#conformancepackcompliancescoresfilterstypedef) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: SortByType](./literals.md#sortbytype) 
4. See [:material-code-braces: ListConformancePackComplianceScoresResponseTypeDef](./type_defs.md#listconformancepackcompliancescoresresponsetypedef) 


```python
# list_conformance_pack_compliance_scores method usage example with argument unpacking

kwargs: ListConformancePackComplianceScoresRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.list_conformance_pack_compliance_scores(**kwargs)
```

1. See [:material-code-braces: ListConformancePackComplianceScoresRequestRequestTypeDef](./type_defs.md#listconformancepackcompliancescoresrequestrequesttypedef) 

### list\_discovered\_resources

Accepts a resource type and returns a list of resource identifiers for the
resources of that type.

Type annotations and code completion for `#!python session.client("config").list_discovered_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# list_discovered_resources method definition

await def list_discovered_resources(
    self,
    *,
    resourceType: ResourceTypeType,  # (1)
    resourceIds: Sequence[str] = ...,
    resourceName: str = ...,
    limit: int = ...,
    includeDeletedResources: bool = ...,
    nextToken: str = ...,
) -> ListDiscoveredResourcesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ListDiscoveredResourcesResponseTypeDef](./type_defs.md#listdiscoveredresourcesresponsetypedef) 


```python
# list_discovered_resources method usage example with argument unpacking

kwargs: ListDiscoveredResourcesRequestRequestTypeDef = {  # (1)
    "resourceType": ...,
}

parent.list_discovered_resources(**kwargs)
```

1. See [:material-code-braces: ListDiscoveredResourcesRequestRequestTypeDef](./type_defs.md#listdiscoveredresourcesrequestrequesttypedef) 

### list\_resource\_evaluations

Returns a list of proactive resource evaluations.

Type annotations and code completion for `#!python session.client("config").list_resource_evaluations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# list_resource_evaluations method definition

await def list_resource_evaluations(
    self,
    *,
    Filters: ResourceEvaluationFiltersTypeDef = ...,  # (1)
    Limit: int = ...,
    NextToken: str = ...,
) -> ListResourceEvaluationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ResourceEvaluationFiltersTypeDef](./type_defs.md#resourceevaluationfilterstypedef) 
2. See [:material-code-braces: ListResourceEvaluationsResponseTypeDef](./type_defs.md#listresourceevaluationsresponsetypedef) 


```python
# list_resource_evaluations method usage example with argument unpacking

kwargs: ListResourceEvaluationsRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.list_resource_evaluations(**kwargs)
```

1. See [:material-code-braces: ListResourceEvaluationsRequestRequestTypeDef](./type_defs.md#listresourceevaluationsrequestrequesttypedef) 

### list\_stored\_queries

Lists the stored queries for a single Amazon Web Services account and a single
Amazon Web Services Region.

Type annotations and code completion for `#!python session.client("config").list_stored_queries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# list_stored_queries method definition

await def list_stored_queries(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListStoredQueriesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStoredQueriesResponseTypeDef](./type_defs.md#liststoredqueriesresponsetypedef) 


```python
# list_stored_queries method usage example with argument unpacking

kwargs: ListStoredQueriesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_stored_queries(**kwargs)
```

1. See [:material-code-braces: ListStoredQueriesRequestRequestTypeDef](./type_defs.md#liststoredqueriesrequestrequesttypedef) 

### list\_tags\_for\_resource

List the tags for Config resource.

Type annotations and code completion for `#!python session.client("config").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
    Limit: int = ...,
    NextToken: str = ...,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### put\_aggregation\_authorization

Authorizes the aggregator account and region to collect data from the source
account and region.

Type annotations and code completion for `#!python session.client("config").put_aggregation_authorization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# put_aggregation_authorization method definition

await def put_aggregation_authorization(
    self,
    *,
    AuthorizedAccountId: str,
    AuthorizedAwsRegion: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> PutAggregationAuthorizationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: PutAggregationAuthorizationResponseTypeDef](./type_defs.md#putaggregationauthorizationresponsetypedef) 


```python
# put_aggregation_authorization method usage example with argument unpacking

kwargs: PutAggregationAuthorizationRequestRequestTypeDef = {  # (1)
    "AuthorizedAccountId": ...,
    "AuthorizedAwsRegion": ...,
}

parent.put_aggregation_authorization(**kwargs)
```

1. See [:material-code-braces: PutAggregationAuthorizationRequestRequestTypeDef](./type_defs.md#putaggregationauthorizationrequestrequesttypedef) 

### put\_config\_rule

Adds or updates an Config rule to evaluate if your Amazon Web Services
resources comply with your desired configurations.

Type annotations and code completion for `#!python session.client("config").put_config_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# put_config_rule method definition

await def put_config_rule(
    self,
    *,
    ConfigRule: ConfigRuleTypeDef,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ConfigRuleTypeDef](./type_defs.md#configruletypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_config_rule method usage example with argument unpacking

kwargs: PutConfigRuleRequestRequestTypeDef = {  # (1)
    "ConfigRule": ...,
}

parent.put_config_rule(**kwargs)
```

1. See [:material-code-braces: PutConfigRuleRequestRequestTypeDef](./type_defs.md#putconfigrulerequestrequesttypedef) 

### put\_configuration\_aggregator

Creates and updates the configuration aggregator with the selected source
accounts and regions.

Type annotations and code completion for `#!python session.client("config").put_configuration_aggregator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# put_configuration_aggregator method definition

await def put_configuration_aggregator(
    self,
    *,
    ConfigurationAggregatorName: str,
    AccountAggregationSources: Sequence[AccountAggregationSourceUnionTypeDef] = ...,  # (1)
    OrganizationAggregationSource: OrganizationAggregationSourceTypeDef = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    AggregatorFilters: AggregatorFiltersTypeDef = ...,  # (4)
) -> PutConfigurationAggregatorResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: AccountAggregationSourceTypeDef](./type_defs.md#accountaggregationsourcetypedef) [:material-code-braces: AccountAggregationSourceOutputTypeDef](./type_defs.md#accountaggregationsourceoutputtypedef) 
2. See [:material-code-braces: OrganizationAggregationSourceTypeDef](./type_defs.md#organizationaggregationsourcetypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: AggregatorFiltersTypeDef](./type_defs.md#aggregatorfilterstypedef) 
5. See [:material-code-braces: PutConfigurationAggregatorResponseTypeDef](./type_defs.md#putconfigurationaggregatorresponsetypedef) 


```python
# put_configuration_aggregator method usage example with argument unpacking

kwargs: PutConfigurationAggregatorRequestRequestTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
}

parent.put_configuration_aggregator(**kwargs)
```

1. See [:material-code-braces: PutConfigurationAggregatorRequestRequestTypeDef](./type_defs.md#putconfigurationaggregatorrequestrequesttypedef) 

### put\_configuration\_recorder

Creates or updates the customer managed configuration recorder.

Type annotations and code completion for `#!python session.client("config").put_configuration_recorder` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# put_configuration_recorder method definition

await def put_configuration_recorder(
    self,
    *,
    ConfigurationRecorder: ConfigurationRecorderTypeDef,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ConfigurationRecorderTypeDef](./type_defs.md#configurationrecordertypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_configuration_recorder method usage example with argument unpacking

kwargs: PutConfigurationRecorderRequestRequestTypeDef = {  # (1)
    "ConfigurationRecorder": ...,
}

parent.put_configuration_recorder(**kwargs)
```

1. See [:material-code-braces: PutConfigurationRecorderRequestRequestTypeDef](./type_defs.md#putconfigurationrecorderrequestrequesttypedef) 

### put\_conformance\_pack

Creates or updates a conformance pack.

Type annotations and code completion for `#!python session.client("config").put_conformance_pack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# put_conformance_pack method definition

await def put_conformance_pack(
    self,
    *,
    ConformancePackName: str,
    TemplateS3Uri: str = ...,
    TemplateBody: str = ...,
    DeliveryS3Bucket: str = ...,
    DeliveryS3KeyPrefix: str = ...,
    ConformancePackInputParameters: Sequence[ConformancePackInputParameterTypeDef] = ...,  # (1)
    TemplateSSMDocumentDetails: TemplateSSMDocumentDetailsTypeDef = ...,  # (2)
) -> PutConformancePackResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ConformancePackInputParameterTypeDef](./type_defs.md#conformancepackinputparametertypedef) 
2. See [:material-code-braces: TemplateSSMDocumentDetailsTypeDef](./type_defs.md#templatessmdocumentdetailstypedef) 
3. See [:material-code-braces: PutConformancePackResponseTypeDef](./type_defs.md#putconformancepackresponsetypedef) 


```python
# put_conformance_pack method usage example with argument unpacking

kwargs: PutConformancePackRequestRequestTypeDef = {  # (1)
    "ConformancePackName": ...,
}

parent.put_conformance_pack(**kwargs)
```

1. See [:material-code-braces: PutConformancePackRequestRequestTypeDef](./type_defs.md#putconformancepackrequestrequesttypedef) 

### put\_delivery\_channel

Creates or updates a delivery channel to deliver configuration information and
other compliance information.

Type annotations and code completion for `#!python session.client("config").put_delivery_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# put_delivery_channel method definition

await def put_delivery_channel(
    self,
    *,
    DeliveryChannel: DeliveryChannelTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DeliveryChannelTypeDef](./type_defs.md#deliverychanneltypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_delivery_channel method usage example with argument unpacking

kwargs: PutDeliveryChannelRequestRequestTypeDef = {  # (1)
    "DeliveryChannel": ...,
}

parent.put_delivery_channel(**kwargs)
```

1. See [:material-code-braces: PutDeliveryChannelRequestRequestTypeDef](./type_defs.md#putdeliverychannelrequestrequesttypedef) 

### put\_evaluations

Used by an Lambda function to deliver evaluation results to Config.

Type annotations and code completion for `#!python session.client("config").put_evaluations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# put_evaluations method definition

await def put_evaluations(
    self,
    *,
    ResultToken: str,
    Evaluations: Sequence[EvaluationUnionTypeDef] = ...,  # (1)
    TestMode: bool = ...,
) -> PutEvaluationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EvaluationTypeDef](./type_defs.md#evaluationtypedef) [:material-code-braces: EvaluationOutputTypeDef](./type_defs.md#evaluationoutputtypedef) 
2. See [:material-code-braces: PutEvaluationsResponseTypeDef](./type_defs.md#putevaluationsresponsetypedef) 


```python
# put_evaluations method usage example with argument unpacking

kwargs: PutEvaluationsRequestRequestTypeDef = {  # (1)
    "ResultToken": ...,
}

parent.put_evaluations(**kwargs)
```

1. See [:material-code-braces: PutEvaluationsRequestRequestTypeDef](./type_defs.md#putevaluationsrequestrequesttypedef) 

### put\_external\_evaluation

Add or updates the evaluations for process checks.

Type annotations and code completion for `#!python session.client("config").put_external_evaluation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# put_external_evaluation method definition

await def put_external_evaluation(
    self,
    *,
    ConfigRuleName: str,
    ExternalEvaluation: ExternalEvaluationTypeDef,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: ExternalEvaluationTypeDef](./type_defs.md#externalevaluationtypedef) 


```python
# put_external_evaluation method usage example with argument unpacking

kwargs: PutExternalEvaluationRequestRequestTypeDef = {  # (1)
    "ConfigRuleName": ...,
    "ExternalEvaluation": ...,
}

parent.put_external_evaluation(**kwargs)
```

1. See [:material-code-braces: PutExternalEvaluationRequestRequestTypeDef](./type_defs.md#putexternalevaluationrequestrequesttypedef) 

### put\_organization\_config\_rule

Adds or updates an Config rule for your entire organization to evaluate if your
Amazon Web Services resources comply with your desired configurations.

Type annotations and code completion for `#!python session.client("config").put_organization_config_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# put_organization_config_rule method definition

await def put_organization_config_rule(
    self,
    *,
    OrganizationConfigRuleName: str,
    OrganizationManagedRuleMetadata: OrganizationManagedRuleMetadataTypeDef = ...,  # (1)
    OrganizationCustomRuleMetadata: OrganizationCustomRuleMetadataTypeDef = ...,  # (2)
    ExcludedAccounts: Sequence[str] = ...,
    OrganizationCustomPolicyRuleMetadata: OrganizationCustomPolicyRuleMetadataTypeDef = ...,  # (3)
) -> PutOrganizationConfigRuleResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: OrganizationManagedRuleMetadataTypeDef](./type_defs.md#organizationmanagedrulemetadatatypedef) 
2. See [:material-code-braces: OrganizationCustomRuleMetadataTypeDef](./type_defs.md#organizationcustomrulemetadatatypedef) 
3. See [:material-code-braces: OrganizationCustomPolicyRuleMetadataTypeDef](./type_defs.md#organizationcustompolicyrulemetadatatypedef) 
4. See [:material-code-braces: PutOrganizationConfigRuleResponseTypeDef](./type_defs.md#putorganizationconfigruleresponsetypedef) 


```python
# put_organization_config_rule method usage example with argument unpacking

kwargs: PutOrganizationConfigRuleRequestRequestTypeDef = {  # (1)
    "OrganizationConfigRuleName": ...,
}

parent.put_organization_config_rule(**kwargs)
```

1. See [:material-code-braces: PutOrganizationConfigRuleRequestRequestTypeDef](./type_defs.md#putorganizationconfigrulerequestrequesttypedef) 

### put\_organization\_conformance\_pack

Deploys conformance packs across member accounts in an Amazon Web Services
Organization.

Type annotations and code completion for `#!python session.client("config").put_organization_conformance_pack` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# put_organization_conformance_pack method definition

await def put_organization_conformance_pack(
    self,
    *,
    OrganizationConformancePackName: str,
    TemplateS3Uri: str = ...,
    TemplateBody: str = ...,
    DeliveryS3Bucket: str = ...,
    DeliveryS3KeyPrefix: str = ...,
    ConformancePackInputParameters: Sequence[ConformancePackInputParameterTypeDef] = ...,  # (1)
    ExcludedAccounts: Sequence[str] = ...,
) -> PutOrganizationConformancePackResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConformancePackInputParameterTypeDef](./type_defs.md#conformancepackinputparametertypedef) 
2. See [:material-code-braces: PutOrganizationConformancePackResponseTypeDef](./type_defs.md#putorganizationconformancepackresponsetypedef) 


```python
# put_organization_conformance_pack method usage example with argument unpacking

kwargs: PutOrganizationConformancePackRequestRequestTypeDef = {  # (1)
    "OrganizationConformancePackName": ...,
}

parent.put_organization_conformance_pack(**kwargs)
```

1. See [:material-code-braces: PutOrganizationConformancePackRequestRequestTypeDef](./type_defs.md#putorganizationconformancepackrequestrequesttypedef) 

### put\_remediation\_configurations

Adds or updates the remediation configuration with a specific Config rule with
the selected target or action.

Type annotations and code completion for `#!python session.client("config").put_remediation_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# put_remediation_configurations method definition

await def put_remediation_configurations(
    self,
    *,
    RemediationConfigurations: Sequence[RemediationConfigurationUnionTypeDef],  # (1)
) -> PutRemediationConfigurationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RemediationConfigurationTypeDef](./type_defs.md#remediationconfigurationtypedef) [:material-code-braces: RemediationConfigurationOutputTypeDef](./type_defs.md#remediationconfigurationoutputtypedef) 
2. See [:material-code-braces: PutRemediationConfigurationsResponseTypeDef](./type_defs.md#putremediationconfigurationsresponsetypedef) 


```python
# put_remediation_configurations method usage example with argument unpacking

kwargs: PutRemediationConfigurationsRequestRequestTypeDef = {  # (1)
    "RemediationConfigurations": ...,
}

parent.put_remediation_configurations(**kwargs)
```

1. See [:material-code-braces: PutRemediationConfigurationsRequestRequestTypeDef](./type_defs.md#putremediationconfigurationsrequestrequesttypedef) 

### put\_remediation\_exceptions

A remediation exception is when a specified resource is no longer considered
for auto-remediation.

Type annotations and code completion for `#!python session.client("config").put_remediation_exceptions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# put_remediation_exceptions method definition

await def put_remediation_exceptions(
    self,
    *,
    ConfigRuleName: str,
    ResourceKeys: Sequence[RemediationExceptionResourceKeyTypeDef],  # (1)
    Message: str = ...,
    ExpirationTime: TimestampTypeDef = ...,
) -> PutRemediationExceptionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RemediationExceptionResourceKeyTypeDef](./type_defs.md#remediationexceptionresourcekeytypedef) 
2. See [:material-code-braces: PutRemediationExceptionsResponseTypeDef](./type_defs.md#putremediationexceptionsresponsetypedef) 


```python
# put_remediation_exceptions method usage example with argument unpacking

kwargs: PutRemediationExceptionsRequestRequestTypeDef = {  # (1)
    "ConfigRuleName": ...,
    "ResourceKeys": ...,
}

parent.put_remediation_exceptions(**kwargs)
```

1. See [:material-code-braces: PutRemediationExceptionsRequestRequestTypeDef](./type_defs.md#putremediationexceptionsrequestrequesttypedef) 

### put\_resource\_config

Records the configuration state for the resource provided in the request.

Type annotations and code completion for `#!python session.client("config").put_resource_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# put_resource_config method definition

await def put_resource_config(
    self,
    *,
    ResourceType: str,
    SchemaVersionId: str,
    ResourceId: str,
    Configuration: str,
    ResourceName: str = ...,
    Tags: Mapping[str, str] = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_resource_config method usage example with argument unpacking

kwargs: PutResourceConfigRequestRequestTypeDef = {  # (1)
    "ResourceType": ...,
    "SchemaVersionId": ...,
    "ResourceId": ...,
    "Configuration": ...,
}

parent.put_resource_config(**kwargs)
```

1. See [:material-code-braces: PutResourceConfigRequestRequestTypeDef](./type_defs.md#putresourceconfigrequestrequesttypedef) 

### put\_retention\_configuration

Creates and updates the retention configuration with details about retention
period (number of days) that Config stores your historical information.

Type annotations and code completion for `#!python session.client("config").put_retention_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# put_retention_configuration method definition

await def put_retention_configuration(
    self,
    *,
    RetentionPeriodInDays: int,
) -> PutRetentionConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutRetentionConfigurationResponseTypeDef](./type_defs.md#putretentionconfigurationresponsetypedef) 


```python
# put_retention_configuration method usage example with argument unpacking

kwargs: PutRetentionConfigurationRequestRequestTypeDef = {  # (1)
    "RetentionPeriodInDays": ...,
}

parent.put_retention_configuration(**kwargs)
```

1. See [:material-code-braces: PutRetentionConfigurationRequestRequestTypeDef](./type_defs.md#putretentionconfigurationrequestrequesttypedef) 

### put\_service\_linked\_configuration\_recorder

Creates a service-linked configuration recorder that is linked to a specific
Amazon Web Services service based on the <code>ServicePrincipal</code> you
specify.

Type annotations and code completion for `#!python session.client("config").put_service_linked_configuration_recorder` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# put_service_linked_configuration_recorder method definition

await def put_service_linked_configuration_recorder(
    self,
    *,
    ServicePrincipal: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> PutServiceLinkedConfigurationRecorderResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: PutServiceLinkedConfigurationRecorderResponseTypeDef](./type_defs.md#putservicelinkedconfigurationrecorderresponsetypedef) 


```python
# put_service_linked_configuration_recorder method usage example with argument unpacking

kwargs: PutServiceLinkedConfigurationRecorderRequestRequestTypeDef = {  # (1)
    "ServicePrincipal": ...,
}

parent.put_service_linked_configuration_recorder(**kwargs)
```

1. See [:material-code-braces: PutServiceLinkedConfigurationRecorderRequestRequestTypeDef](./type_defs.md#putservicelinkedconfigurationrecorderrequestrequesttypedef) 

### put\_stored\_query

Saves a new query or updates an existing saved query.

Type annotations and code completion for `#!python session.client("config").put_stored_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# put_stored_query method definition

await def put_stored_query(
    self,
    *,
    StoredQuery: StoredQueryTypeDef,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> PutStoredQueryResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: StoredQueryTypeDef](./type_defs.md#storedquerytypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: PutStoredQueryResponseTypeDef](./type_defs.md#putstoredqueryresponsetypedef) 


```python
# put_stored_query method usage example with argument unpacking

kwargs: PutStoredQueryRequestRequestTypeDef = {  # (1)
    "StoredQuery": ...,
}

parent.put_stored_query(**kwargs)
```

1. See [:material-code-braces: PutStoredQueryRequestRequestTypeDef](./type_defs.md#putstoredqueryrequestrequesttypedef) 

### select\_aggregate\_resource\_config

Accepts a structured query language (SQL) SELECT command and an aggregator to
query configuration state of Amazon Web Services resources across multiple
accounts and regions, performs the corresponding search, and returns resource
configurations matching the properties.

Type annotations and code completion for `#!python session.client("config").select_aggregate_resource_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# select_aggregate_resource_config method definition

await def select_aggregate_resource_config(
    self,
    *,
    Expression: str,
    ConfigurationAggregatorName: str,
    Limit: int = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> SelectAggregateResourceConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SelectAggregateResourceConfigResponseTypeDef](./type_defs.md#selectaggregateresourceconfigresponsetypedef) 


```python
# select_aggregate_resource_config method usage example with argument unpacking

kwargs: SelectAggregateResourceConfigRequestRequestTypeDef = {  # (1)
    "Expression": ...,
    "ConfigurationAggregatorName": ...,
}

parent.select_aggregate_resource_config(**kwargs)
```

1. See [:material-code-braces: SelectAggregateResourceConfigRequestRequestTypeDef](./type_defs.md#selectaggregateresourceconfigrequestrequesttypedef) 

### select\_resource\_config

Accepts a structured query language (SQL) <code>SELECT</code> command, performs
the corresponding search, and returns resource configurations matching the
properties.

Type annotations and code completion for `#!python session.client("config").select_resource_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# select_resource_config method definition

await def select_resource_config(
    self,
    *,
    Expression: str,
    Limit: int = ...,
    NextToken: str = ...,
) -> SelectResourceConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SelectResourceConfigResponseTypeDef](./type_defs.md#selectresourceconfigresponsetypedef) 


```python
# select_resource_config method usage example with argument unpacking

kwargs: SelectResourceConfigRequestRequestTypeDef = {  # (1)
    "Expression": ...,
}

parent.select_resource_config(**kwargs)
```

1. See [:material-code-braces: SelectResourceConfigRequestRequestTypeDef](./type_defs.md#selectresourceconfigrequestrequesttypedef) 

### start\_config\_rules\_evaluation

Runs an on-demand evaluation for the specified Config rules against the last
known configuration state of the resources.

Type annotations and code completion for `#!python session.client("config").start_config_rules_evaluation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# start_config_rules_evaluation method definition

await def start_config_rules_evaluation(
    self,
    *,
    ConfigRuleNames: Sequence[str] = ...,
) -> dict[str, Any]:
    ...
```



```python
# start_config_rules_evaluation method usage example with argument unpacking

kwargs: StartConfigRulesEvaluationRequestRequestTypeDef = {  # (1)
    "ConfigRuleNames": ...,
}

parent.start_config_rules_evaluation(**kwargs)
```

1. See [:material-code-braces: StartConfigRulesEvaluationRequestRequestTypeDef](./type_defs.md#startconfigrulesevaluationrequestrequesttypedef) 

### start\_configuration\_recorder

Starts the customer managed configuration recorder.

Type annotations and code completion for `#!python session.client("config").start_configuration_recorder` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# start_configuration_recorder method definition

await def start_configuration_recorder(
    self,
    *,
    ConfigurationRecorderName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# start_configuration_recorder method usage example with argument unpacking

kwargs: StartConfigurationRecorderRequestRequestTypeDef = {  # (1)
    "ConfigurationRecorderName": ...,
}

parent.start_configuration_recorder(**kwargs)
```

1. See [:material-code-braces: StartConfigurationRecorderRequestRequestTypeDef](./type_defs.md#startconfigurationrecorderrequestrequesttypedef) 

### start\_remediation\_execution

Runs an on-demand remediation for the specified Config rules against the last
known remediation configuration.

Type annotations and code completion for `#!python session.client("config").start_remediation_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# start_remediation_execution method definition

await def start_remediation_execution(
    self,
    *,
    ConfigRuleName: str,
    ResourceKeys: Sequence[ResourceKeyTypeDef],  # (1)
) -> StartRemediationExecutionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ResourceKeyTypeDef](./type_defs.md#resourcekeytypedef) 
2. See [:material-code-braces: StartRemediationExecutionResponseTypeDef](./type_defs.md#startremediationexecutionresponsetypedef) 


```python
# start_remediation_execution method usage example with argument unpacking

kwargs: StartRemediationExecutionRequestRequestTypeDef = {  # (1)
    "ConfigRuleName": ...,
    "ResourceKeys": ...,
}

parent.start_remediation_execution(**kwargs)
```

1. See [:material-code-braces: StartRemediationExecutionRequestRequestTypeDef](./type_defs.md#startremediationexecutionrequestrequesttypedef) 

### start\_resource\_evaluation

Runs an on-demand evaluation for the specified resource to determine whether
the resource details will comply with configured Config rules.

Type annotations and code completion for `#!python session.client("config").start_resource_evaluation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# start_resource_evaluation method definition

await def start_resource_evaluation(
    self,
    *,
    ResourceDetails: ResourceDetailsTypeDef,  # (1)
    EvaluationMode: EvaluationModeType,  # (2)
    EvaluationContext: EvaluationContextTypeDef = ...,  # (3)
    EvaluationTimeout: int = ...,
    ClientToken: str = ...,
) -> StartResourceEvaluationResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef) 
2. See [:material-code-brackets: EvaluationModeType](./literals.md#evaluationmodetype) 
3. See [:material-code-braces: EvaluationContextTypeDef](./type_defs.md#evaluationcontexttypedef) 
4. See [:material-code-braces: StartResourceEvaluationResponseTypeDef](./type_defs.md#startresourceevaluationresponsetypedef) 


```python
# start_resource_evaluation method usage example with argument unpacking

kwargs: StartResourceEvaluationRequestRequestTypeDef = {  # (1)
    "ResourceDetails": ...,
    "EvaluationMode": ...,
}

parent.start_resource_evaluation(**kwargs)
```

1. See [:material-code-braces: StartResourceEvaluationRequestRequestTypeDef](./type_defs.md#startresourceevaluationrequestrequesttypedef) 

### stop\_configuration\_recorder

Stops the customer managed configuration recorder.

Type annotations and code completion for `#!python session.client("config").stop_configuration_recorder` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# stop_configuration_recorder method definition

await def stop_configuration_recorder(
    self,
    *,
    ConfigurationRecorderName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_configuration_recorder method usage example with argument unpacking

kwargs: StopConfigurationRecorderRequestRequestTypeDef = {  # (1)
    "ConfigurationRecorderName": ...,
}

parent.stop_configuration_recorder(**kwargs)
```

1. See [:material-code-braces: StopConfigurationRecorderRequestRequestTypeDef](./type_defs.md#stopconfigurationrecorderrequestrequesttypedef) 

### tag\_resource

Associates the specified tags to a resource with the specified
<code>ResourceArn</code>.

Type annotations and code completion for `#!python session.client("config").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Deletes specified tags from a resource.

Type annotations and code completion for `#!python session.client("config").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("config").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("config").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client)

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

Type annotations and code completion for `#!python session.client("config").get_paginator` method with overloads.

- `client.get_paginator("describe_aggregate_compliance_by_config_rules")` -> [DescribeAggregateComplianceByConfigRulesPaginator](./paginators.md#describeaggregatecompliancebyconfigrulespaginator)
- `client.get_paginator("describe_aggregate_compliance_by_conformance_packs")` -> [DescribeAggregateComplianceByConformancePacksPaginator](./paginators.md#describeaggregatecompliancebyconformancepackspaginator)
- `client.get_paginator("describe_aggregation_authorizations")` -> [DescribeAggregationAuthorizationsPaginator](./paginators.md#describeaggregationauthorizationspaginator)
- `client.get_paginator("describe_compliance_by_config_rule")` -> [DescribeComplianceByConfigRulePaginator](./paginators.md#describecompliancebyconfigrulepaginator)
- `client.get_paginator("describe_compliance_by_resource")` -> [DescribeComplianceByResourcePaginator](./paginators.md#describecompliancebyresourcepaginator)
- `client.get_paginator("describe_config_rule_evaluation_status")` -> [DescribeConfigRuleEvaluationStatusPaginator](./paginators.md#describeconfigruleevaluationstatuspaginator)
- `client.get_paginator("describe_config_rules")` -> [DescribeConfigRulesPaginator](./paginators.md#describeconfigrulespaginator)
- `client.get_paginator("describe_configuration_aggregator_sources_status")` -> [DescribeConfigurationAggregatorSourcesStatusPaginator](./paginators.md#describeconfigurationaggregatorsourcesstatuspaginator)
- `client.get_paginator("describe_configuration_aggregators")` -> [DescribeConfigurationAggregatorsPaginator](./paginators.md#describeconfigurationaggregatorspaginator)
- `client.get_paginator("describe_conformance_pack_status")` -> [DescribeConformancePackStatusPaginator](./paginators.md#describeconformancepackstatuspaginator)
- `client.get_paginator("describe_conformance_packs")` -> [DescribeConformancePacksPaginator](./paginators.md#describeconformancepackspaginator)
- `client.get_paginator("describe_organization_config_rule_statuses")` -> [DescribeOrganizationConfigRuleStatusesPaginator](./paginators.md#describeorganizationconfigrulestatusespaginator)
- `client.get_paginator("describe_organization_config_rules")` -> [DescribeOrganizationConfigRulesPaginator](./paginators.md#describeorganizationconfigrulespaginator)
- `client.get_paginator("describe_organization_conformance_pack_statuses")` -> [DescribeOrganizationConformancePackStatusesPaginator](./paginators.md#describeorganizationconformancepackstatusespaginator)
- `client.get_paginator("describe_organization_conformance_packs")` -> [DescribeOrganizationConformancePacksPaginator](./paginators.md#describeorganizationconformancepackspaginator)
- `client.get_paginator("describe_pending_aggregation_requests")` -> [DescribePendingAggregationRequestsPaginator](./paginators.md#describependingaggregationrequestspaginator)
- `client.get_paginator("describe_remediation_execution_status")` -> [DescribeRemediationExecutionStatusPaginator](./paginators.md#describeremediationexecutionstatuspaginator)
- `client.get_paginator("describe_retention_configurations")` -> [DescribeRetentionConfigurationsPaginator](./paginators.md#describeretentionconfigurationspaginator)
- `client.get_paginator("get_aggregate_compliance_details_by_config_rule")` -> [GetAggregateComplianceDetailsByConfigRulePaginator](./paginators.md#getaggregatecompliancedetailsbyconfigrulepaginator)
- `client.get_paginator("get_compliance_details_by_config_rule")` -> [GetComplianceDetailsByConfigRulePaginator](./paginators.md#getcompliancedetailsbyconfigrulepaginator)
- `client.get_paginator("get_compliance_details_by_resource")` -> [GetComplianceDetailsByResourcePaginator](./paginators.md#getcompliancedetailsbyresourcepaginator)
- `client.get_paginator("get_conformance_pack_compliance_summary")` -> [GetConformancePackComplianceSummaryPaginator](./paginators.md#getconformancepackcompliancesummarypaginator)
- `client.get_paginator("get_organization_config_rule_detailed_status")` -> [GetOrganizationConfigRuleDetailedStatusPaginator](./paginators.md#getorganizationconfigruledetailedstatuspaginator)
- `client.get_paginator("get_organization_conformance_pack_detailed_status")` -> [GetOrganizationConformancePackDetailedStatusPaginator](./paginators.md#getorganizationconformancepackdetailedstatuspaginator)
- `client.get_paginator("get_resource_config_history")` -> [GetResourceConfigHistoryPaginator](./paginators.md#getresourceconfighistorypaginator)
- `client.get_paginator("list_aggregate_discovered_resources")` -> [ListAggregateDiscoveredResourcesPaginator](./paginators.md#listaggregatediscoveredresourcespaginator)
- `client.get_paginator("list_configuration_recorders")` -> [ListConfigurationRecordersPaginator](./paginators.md#listconfigurationrecorderspaginator)
- `client.get_paginator("list_discovered_resources")` -> [ListDiscoveredResourcesPaginator](./paginators.md#listdiscoveredresourcespaginator)
- `client.get_paginator("list_resource_evaluations")` -> [ListResourceEvaluationsPaginator](./paginators.md#listresourceevaluationspaginator)
- `client.get_paginator("list_tags_for_resource")` -> [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
- `client.get_paginator("select_aggregate_resource_config")` -> [SelectAggregateResourceConfigPaginator](./paginators.md#selectaggregateresourceconfigpaginator)
- `client.get_paginator("select_resource_config")` -> [SelectResourceConfigPaginator](./paginators.md#selectresourceconfigpaginator)


