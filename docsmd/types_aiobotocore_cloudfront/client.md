# CloudFrontClient

> [Index](../README.md) > [CloudFront](./README.md) > CloudFrontClient

!!! note ""

    Auto-generated documentation for [CloudFront](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#cloudfront)
    type annotations stubs module [types-aiobotocore-cloudfront](https://pypi.org/project/types-aiobotocore-cloudfront/).

## CloudFrontClient

Type annotations and code completion for `#!python session.client("cloudfront")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# CloudFrontClient usage example

from aioboto3.session import Session
from types_aiobotocore_cloudfront.client import CloudFrontClient

session = Session()
async with session.client("cloudfront") as client:
    client: CloudFrontClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("cloudfront").exceptions` structure.

```python
# CloudFrontClient.exceptions usage example

async with session.client("cloudfront") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDenied,
        client.exceptions.BatchTooLarge,
        client.exceptions.CNAMEAlreadyExists,
        client.exceptions.CachePolicyAlreadyExists,
        client.exceptions.CachePolicyInUse,
        client.exceptions.CannotChangeImmutablePublicKeyFields,
        client.exceptions.CannotDeleteEntityWhileInUse,
        client.exceptions.CannotUpdateEntityWhileInUse,
        client.exceptions.ClientError,
        client.exceptions.CloudFrontOriginAccessIdentityAlreadyExists,
        client.exceptions.CloudFrontOriginAccessIdentityInUse,
        client.exceptions.ContinuousDeploymentPolicyAlreadyExists,
        client.exceptions.ContinuousDeploymentPolicyInUse,
        client.exceptions.DistributionAlreadyExists,
        client.exceptions.DistributionNotDisabled,
        client.exceptions.EntityAlreadyExists,
        client.exceptions.EntityLimitExceeded,
        client.exceptions.EntityNotFound,
        client.exceptions.EntitySizeLimitExceeded,
        client.exceptions.FieldLevelEncryptionConfigAlreadyExists,
        client.exceptions.FieldLevelEncryptionConfigInUse,
        client.exceptions.FieldLevelEncryptionProfileAlreadyExists,
        client.exceptions.FieldLevelEncryptionProfileInUse,
        client.exceptions.FieldLevelEncryptionProfileSizeExceeded,
        client.exceptions.FunctionAlreadyExists,
        client.exceptions.FunctionInUse,
        client.exceptions.FunctionSizeLimitExceeded,
        client.exceptions.IllegalDelete,
        client.exceptions.IllegalFieldLevelEncryptionConfigAssociationWithCacheBehavior,
        client.exceptions.IllegalOriginAccessConfiguration,
        client.exceptions.IllegalUpdate,
        client.exceptions.InconsistentQuantities,
        client.exceptions.InvalidArgument,
        client.exceptions.InvalidDefaultRootObject,
        client.exceptions.InvalidDomainNameForOriginAccessControl,
        client.exceptions.InvalidErrorCode,
        client.exceptions.InvalidForwardCookies,
        client.exceptions.InvalidFunctionAssociation,
        client.exceptions.InvalidGeoRestrictionParameter,
        client.exceptions.InvalidHeadersForS3Origin,
        client.exceptions.InvalidIfMatchVersion,
        client.exceptions.InvalidLambdaFunctionAssociation,
        client.exceptions.InvalidLocationCode,
        client.exceptions.InvalidMinimumProtocolVersion,
        client.exceptions.InvalidOrigin,
        client.exceptions.InvalidOriginAccessControl,
        client.exceptions.InvalidOriginAccessIdentity,
        client.exceptions.InvalidOriginKeepaliveTimeout,
        client.exceptions.InvalidOriginReadTimeout,
        client.exceptions.InvalidProtocolSettings,
        client.exceptions.InvalidQueryStringParameters,
        client.exceptions.InvalidRelativePath,
        client.exceptions.InvalidRequiredProtocol,
        client.exceptions.InvalidResponseCode,
        client.exceptions.InvalidTTLOrder,
        client.exceptions.InvalidTagging,
        client.exceptions.InvalidViewerCertificate,
        client.exceptions.InvalidWebACLId,
        client.exceptions.KeyGroupAlreadyExists,
        client.exceptions.MissingBody,
        client.exceptions.MonitoringSubscriptionAlreadyExists,
        client.exceptions.NoSuchCachePolicy,
        client.exceptions.NoSuchCloudFrontOriginAccessIdentity,
        client.exceptions.NoSuchContinuousDeploymentPolicy,
        client.exceptions.NoSuchDistribution,
        client.exceptions.NoSuchFieldLevelEncryptionConfig,
        client.exceptions.NoSuchFieldLevelEncryptionProfile,
        client.exceptions.NoSuchFunctionExists,
        client.exceptions.NoSuchInvalidation,
        client.exceptions.NoSuchMonitoringSubscription,
        client.exceptions.NoSuchOrigin,
        client.exceptions.NoSuchOriginAccessControl,
        client.exceptions.NoSuchOriginRequestPolicy,
        client.exceptions.NoSuchPublicKey,
        client.exceptions.NoSuchRealtimeLogConfig,
        client.exceptions.NoSuchResource,
        client.exceptions.NoSuchResponseHeadersPolicy,
        client.exceptions.NoSuchStreamingDistribution,
        client.exceptions.OriginAccessControlAlreadyExists,
        client.exceptions.OriginAccessControlInUse,
        client.exceptions.OriginRequestPolicyAlreadyExists,
        client.exceptions.OriginRequestPolicyInUse,
        client.exceptions.PreconditionFailed,
        client.exceptions.PublicKeyAlreadyExists,
        client.exceptions.PublicKeyInUse,
        client.exceptions.QueryArgProfileEmpty,
        client.exceptions.RealtimeLogConfigAlreadyExists,
        client.exceptions.RealtimeLogConfigInUse,
        client.exceptions.RealtimeLogConfigOwnerMismatch,
        client.exceptions.ResourceInUse,
        client.exceptions.ResponseHeadersPolicyAlreadyExists,
        client.exceptions.ResponseHeadersPolicyInUse,
        client.exceptions.StagingDistributionInUse,
        client.exceptions.StreamingDistributionAlreadyExists,
        client.exceptions.StreamingDistributionNotDisabled,
        client.exceptions.TestFunctionFailed,
        client.exceptions.TooLongCSPInResponseHeadersPolicy,
        client.exceptions.TooManyCacheBehaviors,
        client.exceptions.TooManyCachePolicies,
        client.exceptions.TooManyCertificates,
        client.exceptions.TooManyCloudFrontOriginAccessIdentities,
        client.exceptions.TooManyContinuousDeploymentPolicies,
        client.exceptions.TooManyCookieNamesInWhiteList,
        client.exceptions.TooManyCookiesInCachePolicy,
        client.exceptions.TooManyCookiesInOriginRequestPolicy,
        client.exceptions.TooManyCustomHeadersInResponseHeadersPolicy,
        client.exceptions.TooManyDistributionCNAMEs,
        client.exceptions.TooManyDistributions,
        client.exceptions.TooManyDistributionsAssociatedToCachePolicy,
        client.exceptions.TooManyDistributionsAssociatedToFieldLevelEncryptionConfig,
        client.exceptions.TooManyDistributionsAssociatedToKeyGroup,
        client.exceptions.TooManyDistributionsAssociatedToOriginAccessControl,
        client.exceptions.TooManyDistributionsAssociatedToOriginRequestPolicy,
        client.exceptions.TooManyDistributionsAssociatedToResponseHeadersPolicy,
        client.exceptions.TooManyDistributionsWithFunctionAssociations,
        client.exceptions.TooManyDistributionsWithLambdaAssociations,
        client.exceptions.TooManyDistributionsWithSingleFunctionARN,
        client.exceptions.TooManyFieldLevelEncryptionConfigs,
        client.exceptions.TooManyFieldLevelEncryptionContentTypeProfiles,
        client.exceptions.TooManyFieldLevelEncryptionEncryptionEntities,
        client.exceptions.TooManyFieldLevelEncryptionFieldPatterns,
        client.exceptions.TooManyFieldLevelEncryptionProfiles,
        client.exceptions.TooManyFieldLevelEncryptionQueryArgProfiles,
        client.exceptions.TooManyFunctionAssociations,
        client.exceptions.TooManyFunctions,
        client.exceptions.TooManyHeadersInCachePolicy,
        client.exceptions.TooManyHeadersInForwardedValues,
        client.exceptions.TooManyHeadersInOriginRequestPolicy,
        client.exceptions.TooManyInvalidationsInProgress,
        client.exceptions.TooManyKeyGroups,
        client.exceptions.TooManyKeyGroupsAssociatedToDistribution,
        client.exceptions.TooManyLambdaFunctionAssociations,
        client.exceptions.TooManyOriginAccessControls,
        client.exceptions.TooManyOriginCustomHeaders,
        client.exceptions.TooManyOriginGroupsPerDistribution,
        client.exceptions.TooManyOriginRequestPolicies,
        client.exceptions.TooManyOrigins,
        client.exceptions.TooManyPublicKeys,
        client.exceptions.TooManyPublicKeysInKeyGroup,
        client.exceptions.TooManyQueryStringParameters,
        client.exceptions.TooManyQueryStringsInCachePolicy,
        client.exceptions.TooManyQueryStringsInOriginRequestPolicy,
        client.exceptions.TooManyRealtimeLogConfigs,
        client.exceptions.TooManyRemoveHeadersInResponseHeadersPolicy,
        client.exceptions.TooManyResponseHeadersPolicies,
        client.exceptions.TooManyStreamingDistributionCNAMEs,
        client.exceptions.TooManyStreamingDistributions,
        client.exceptions.TooManyTrustedSigners,
        client.exceptions.TrustedKeyGroupDoesNotExist,
        client.exceptions.TrustedSignerDoesNotExist,
        client.exceptions.UnsupportedOperation,
    ) as e:
        print(e)
```

```python
# CloudFrontClient.exceptions type checking example

from types_aiobotocore_cloudfront.client import Exceptions

def handle_error(exc: Exceptions.AccessDenied) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("cloudfront").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("cloudfront").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

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


### associate\_alias

Associates an alias (also known as a CNAME or an alternate domain name) with a
CloudFront distribution.

Type annotations and code completion for `#!python session.client("cloudfront").associate_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# associate_alias method definition

await def associate_alias(
    self,
    *,
    TargetDistributionId: str,
    Alias: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# associate_alias method usage example with argument unpacking

kwargs: AssociateAliasRequestTypeDef = {  # (1)
    "TargetDistributionId": ...,
    "Alias": ...,
}

parent.associate_alias(**kwargs)
```

1. See [:material-code-braces: AssociateAliasRequestTypeDef](./type_defs.md#associatealiasrequesttypedef)

### copy\_distribution

Creates a staging distribution using the configuration of the provided primary
distribution.

Type annotations and code completion for `#!python session.client("cloudfront").copy_distribution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# copy_distribution method definition

await def copy_distribution(
    self,
    *,
    PrimaryDistributionId: str,
    CallerReference: str,
    Staging: bool = ...,
    IfMatch: str = ...,
    Enabled: bool = ...,
) -> CopyDistributionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CopyDistributionResultTypeDef](./type_defs.md#copydistributionresulttypedef)


```python
# copy_distribution method usage example with argument unpacking

kwargs: CopyDistributionRequestTypeDef = {  # (1)
    "PrimaryDistributionId": ...,
    "CallerReference": ...,
}

parent.copy_distribution(**kwargs)
```

1. See [:material-code-braces: CopyDistributionRequestTypeDef](./type_defs.md#copydistributionrequesttypedef)

### create\_anycast\_ip\_list

Creates an Anycast static IP list.

Type annotations and code completion for `#!python session.client("cloudfront").create_anycast_ip_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_anycast_ip_list method definition

await def create_anycast_ip_list(
    self,
    *,
    Name: str,
    IpCount: int,
    Tags: TagsUnionTypeDef = ...,  # (1)
) -> CreateAnycastIpListResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagsUnionTypeDef](#tagsuniontypedef)
2. See [:material-code-braces: CreateAnycastIpListResultTypeDef](./type_defs.md#createanycastiplistresulttypedef)


```python
# create_anycast_ip_list method usage example with argument unpacking

kwargs: CreateAnycastIpListRequestTypeDef = {  # (1)
    "Name": ...,
    "IpCount": ...,
}

parent.create_anycast_ip_list(**kwargs)
```

1. See [:material-code-braces: CreateAnycastIpListRequestTypeDef](./type_defs.md#createanycastiplistrequesttypedef)

### create\_cache\_policy

Creates a cache policy.

Type annotations and code completion for `#!python session.client("cloudfront").create_cache_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_cache_policy method definition

await def create_cache_policy(
    self,
    *,
    CachePolicyConfig: CachePolicyConfigUnionTypeDef,  # (1)
) -> CreateCachePolicyResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CachePolicyConfigUnionTypeDef](#cachepolicyconfiguniontypedef)
2. See [:material-code-braces: CreateCachePolicyResultTypeDef](./type_defs.md#createcachepolicyresulttypedef)


```python
# create_cache_policy method usage example with argument unpacking

kwargs: CreateCachePolicyRequestTypeDef = {  # (1)
    "CachePolicyConfig": ...,
}

parent.create_cache_policy(**kwargs)
```

1. See [:material-code-braces: CreateCachePolicyRequestTypeDef](./type_defs.md#createcachepolicyrequesttypedef)

### create\_cloud\_front\_origin\_access\_identity

Creates a new origin access identity.

Type annotations and code completion for `#!python session.client("cloudfront").create_cloud_front_origin_access_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_cloud_front_origin_access_identity method definition

await def create_cloud_front_origin_access_identity(
    self,
    *,
    CloudFrontOriginAccessIdentityConfig: CloudFrontOriginAccessIdentityConfigTypeDef,  # (1)
) -> CreateCloudFrontOriginAccessIdentityResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CloudFrontOriginAccessIdentityConfigTypeDef](./type_defs.md#cloudfrontoriginaccessidentityconfigtypedef)
2. See [:material-code-braces: CreateCloudFrontOriginAccessIdentityResultTypeDef](./type_defs.md#createcloudfrontoriginaccessidentityresulttypedef)


```python
# create_cloud_front_origin_access_identity method usage example with argument unpacking

kwargs: CreateCloudFrontOriginAccessIdentityRequestTypeDef = {  # (1)
    "CloudFrontOriginAccessIdentityConfig": ...,
}

parent.create_cloud_front_origin_access_identity(**kwargs)
```

1. See [:material-code-braces: CreateCloudFrontOriginAccessIdentityRequestTypeDef](./type_defs.md#createcloudfrontoriginaccessidentityrequesttypedef)

### create\_continuous\_deployment\_policy

Creates a continuous deployment policy that distributes traffic for a custom
domain name to two different CloudFront distributions.

Type annotations and code completion for `#!python session.client("cloudfront").create_continuous_deployment_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_continuous_deployment_policy method definition

await def create_continuous_deployment_policy(
    self,
    *,
    ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigUnionTypeDef,  # (1)
) -> CreateContinuousDeploymentPolicyResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ContinuousDeploymentPolicyConfigUnionTypeDef](#continuousdeploymentpolicyconfiguniontypedef)
2. See [:material-code-braces: CreateContinuousDeploymentPolicyResultTypeDef](./type_defs.md#createcontinuousdeploymentpolicyresulttypedef)


```python
# create_continuous_deployment_policy method usage example with argument unpacking

kwargs: CreateContinuousDeploymentPolicyRequestTypeDef = {  # (1)
    "ContinuousDeploymentPolicyConfig": ...,
}

parent.create_continuous_deployment_policy(**kwargs)
```

1. See [:material-code-braces: CreateContinuousDeploymentPolicyRequestTypeDef](./type_defs.md#createcontinuousdeploymentpolicyrequesttypedef)

### create\_distribution

Creates a CloudFront distribution.

Type annotations and code completion for `#!python session.client("cloudfront").create_distribution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_distribution method definition

await def create_distribution(
    self,
    *,
    DistributionConfig: DistributionConfigUnionTypeDef,  # (1)
) -> CreateDistributionResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DistributionConfigUnionTypeDef](#distributionconfiguniontypedef)
2. See [:material-code-braces: CreateDistributionResultTypeDef](./type_defs.md#createdistributionresulttypedef)


```python
# create_distribution method usage example with argument unpacking

kwargs: CreateDistributionRequestTypeDef = {  # (1)
    "DistributionConfig": ...,
}

parent.create_distribution(**kwargs)
```

1. See [:material-code-braces: CreateDistributionRequestTypeDef](./type_defs.md#createdistributionrequesttypedef)

### create\_distribution\_with\_tags

Create a new distribution with tags.

Type annotations and code completion for `#!python session.client("cloudfront").create_distribution_with_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_distribution_with_tags method definition

await def create_distribution_with_tags(
    self,
    *,
    DistributionConfigWithTags: DistributionConfigWithTagsTypeDef,  # (1)
) -> CreateDistributionWithTagsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DistributionConfigWithTagsTypeDef](./type_defs.md#distributionconfigwithtagstypedef)
2. See [:material-code-braces: CreateDistributionWithTagsResultTypeDef](./type_defs.md#createdistributionwithtagsresulttypedef)


```python
# create_distribution_with_tags method usage example with argument unpacking

kwargs: CreateDistributionWithTagsRequestTypeDef = {  # (1)
    "DistributionConfigWithTags": ...,
}

parent.create_distribution_with_tags(**kwargs)
```

1. See [:material-code-braces: CreateDistributionWithTagsRequestTypeDef](./type_defs.md#createdistributionwithtagsrequesttypedef)

### create\_field\_level\_encryption\_config

Create a new field-level encryption configuration.

Type annotations and code completion for `#!python session.client("cloudfront").create_field_level_encryption_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_field_level_encryption_config method definition

await def create_field_level_encryption_config(
    self,
    *,
    FieldLevelEncryptionConfig: FieldLevelEncryptionConfigUnionTypeDef,  # (1)
) -> CreateFieldLevelEncryptionConfigResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FieldLevelEncryptionConfigUnionTypeDef](#fieldlevelencryptionconfiguniontypedef)
2. See [:material-code-braces: CreateFieldLevelEncryptionConfigResultTypeDef](./type_defs.md#createfieldlevelencryptionconfigresulttypedef)


```python
# create_field_level_encryption_config method usage example with argument unpacking

kwargs: CreateFieldLevelEncryptionConfigRequestTypeDef = {  # (1)
    "FieldLevelEncryptionConfig": ...,
}

parent.create_field_level_encryption_config(**kwargs)
```

1. See [:material-code-braces: CreateFieldLevelEncryptionConfigRequestTypeDef](./type_defs.md#createfieldlevelencryptionconfigrequesttypedef)

### create\_field\_level\_encryption\_profile

Create a field-level encryption profile.

Type annotations and code completion for `#!python session.client("cloudfront").create_field_level_encryption_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_field_level_encryption_profile method definition

await def create_field_level_encryption_profile(
    self,
    *,
    FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigUnionTypeDef,  # (1)
) -> CreateFieldLevelEncryptionProfileResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FieldLevelEncryptionProfileConfigUnionTypeDef](#fieldlevelencryptionprofileconfiguniontypedef)
2. See [:material-code-braces: CreateFieldLevelEncryptionProfileResultTypeDef](./type_defs.md#createfieldlevelencryptionprofileresulttypedef)


```python
# create_field_level_encryption_profile method usage example with argument unpacking

kwargs: CreateFieldLevelEncryptionProfileRequestTypeDef = {  # (1)
    "FieldLevelEncryptionProfileConfig": ...,
}

parent.create_field_level_encryption_profile(**kwargs)
```

1. See [:material-code-braces: CreateFieldLevelEncryptionProfileRequestTypeDef](./type_defs.md#createfieldlevelencryptionprofilerequesttypedef)

### create\_function

Creates a CloudFront function.

Type annotations and code completion for `#!python session.client("cloudfront").create_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_function method definition

await def create_function(
    self,
    *,
    Name: str,
    FunctionConfig: FunctionConfigUnionTypeDef,  # (1)
    FunctionCode: BlobTypeDef,
) -> CreateFunctionResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FunctionConfigUnionTypeDef](#functionconfiguniontypedef)
2. See [:material-code-braces: CreateFunctionResultTypeDef](./type_defs.md#createfunctionresulttypedef)


```python
# create_function method usage example with argument unpacking

kwargs: CreateFunctionRequestTypeDef = {  # (1)
    "Name": ...,
    "FunctionConfig": ...,
    "FunctionCode": ...,
}

parent.create_function(**kwargs)
```

1. See [:material-code-braces: CreateFunctionRequestTypeDef](./type_defs.md#createfunctionrequesttypedef)

### create\_invalidation

Create a new invalidation.

Type annotations and code completion for `#!python session.client("cloudfront").create_invalidation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_invalidation method definition

await def create_invalidation(
    self,
    *,
    DistributionId: str,
    InvalidationBatch: InvalidationBatchUnionTypeDef,  # (1)
) -> CreateInvalidationResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InvalidationBatchUnionTypeDef](#invalidationbatchuniontypedef)
2. See [:material-code-braces: CreateInvalidationResultTypeDef](./type_defs.md#createinvalidationresulttypedef)


```python
# create_invalidation method usage example with argument unpacking

kwargs: CreateInvalidationRequestTypeDef = {  # (1)
    "DistributionId": ...,
    "InvalidationBatch": ...,
}

parent.create_invalidation(**kwargs)
```

1. See [:material-code-braces: CreateInvalidationRequestTypeDef](./type_defs.md#createinvalidationrequesttypedef)

### create\_key\_group

Creates a key group that you can use with <a
href="https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/PrivateContent.html">CloudFront
signed URLs and signed cookies</a>.

Type annotations and code completion for `#!python session.client("cloudfront").create_key_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_key_group method definition

await def create_key_group(
    self,
    *,
    KeyGroupConfig: KeyGroupConfigUnionTypeDef,  # (1)
) -> CreateKeyGroupResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: KeyGroupConfigUnionTypeDef](#keygroupconfiguniontypedef)
2. See [:material-code-braces: CreateKeyGroupResultTypeDef](./type_defs.md#createkeygroupresulttypedef)


```python
# create_key_group method usage example with argument unpacking

kwargs: CreateKeyGroupRequestTypeDef = {  # (1)
    "KeyGroupConfig": ...,
}

parent.create_key_group(**kwargs)
```

1. See [:material-code-braces: CreateKeyGroupRequestTypeDef](./type_defs.md#createkeygrouprequesttypedef)

### create\_key\_value\_store

Specifies the key value store resource to add to your account.

Type annotations and code completion for `#!python session.client("cloudfront").create_key_value_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_key_value_store method definition

await def create_key_value_store(
    self,
    *,
    Name: str,
    Comment: str = ...,
    ImportSource: ImportSourceTypeDef = ...,  # (1)
) -> CreateKeyValueStoreResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ImportSourceTypeDef](./type_defs.md#importsourcetypedef)
2. See [:material-code-braces: CreateKeyValueStoreResultTypeDef](./type_defs.md#createkeyvaluestoreresulttypedef)


```python
# create_key_value_store method usage example with argument unpacking

kwargs: CreateKeyValueStoreRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_key_value_store(**kwargs)
```

1. See [:material-code-braces: CreateKeyValueStoreRequestTypeDef](./type_defs.md#createkeyvaluestorerequesttypedef)

### create\_monitoring\_subscription

Enables additional CloudWatch metrics for the specified CloudFront distribution.

Type annotations and code completion for `#!python session.client("cloudfront").create_monitoring_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_monitoring_subscription method definition

await def create_monitoring_subscription(
    self,
    *,
    DistributionId: str,
    MonitoringSubscription: MonitoringSubscriptionTypeDef,  # (1)
) -> CreateMonitoringSubscriptionResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MonitoringSubscriptionTypeDef](./type_defs.md#monitoringsubscriptiontypedef)
2. See [:material-code-braces: CreateMonitoringSubscriptionResultTypeDef](./type_defs.md#createmonitoringsubscriptionresulttypedef)


```python
# create_monitoring_subscription method usage example with argument unpacking

kwargs: CreateMonitoringSubscriptionRequestTypeDef = {  # (1)
    "DistributionId": ...,
    "MonitoringSubscription": ...,
}

parent.create_monitoring_subscription(**kwargs)
```

1. See [:material-code-braces: CreateMonitoringSubscriptionRequestTypeDef](./type_defs.md#createmonitoringsubscriptionrequesttypedef)

### create\_origin\_access\_control

Creates a new origin access control in CloudFront.

Type annotations and code completion for `#!python session.client("cloudfront").create_origin_access_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_origin_access_control method definition

await def create_origin_access_control(
    self,
    *,
    OriginAccessControlConfig: OriginAccessControlConfigTypeDef,  # (1)
) -> CreateOriginAccessControlResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OriginAccessControlConfigTypeDef](./type_defs.md#originaccesscontrolconfigtypedef)
2. See [:material-code-braces: CreateOriginAccessControlResultTypeDef](./type_defs.md#createoriginaccesscontrolresulttypedef)


```python
# create_origin_access_control method usage example with argument unpacking

kwargs: CreateOriginAccessControlRequestTypeDef = {  # (1)
    "OriginAccessControlConfig": ...,
}

parent.create_origin_access_control(**kwargs)
```

1. See [:material-code-braces: CreateOriginAccessControlRequestTypeDef](./type_defs.md#createoriginaccesscontrolrequesttypedef)

### create\_origin\_request\_policy

Creates an origin request policy.

Type annotations and code completion for `#!python session.client("cloudfront").create_origin_request_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_origin_request_policy method definition

await def create_origin_request_policy(
    self,
    *,
    OriginRequestPolicyConfig: OriginRequestPolicyConfigUnionTypeDef,  # (1)
) -> CreateOriginRequestPolicyResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OriginRequestPolicyConfigUnionTypeDef](#originrequestpolicyconfiguniontypedef)
2. See [:material-code-braces: CreateOriginRequestPolicyResultTypeDef](./type_defs.md#createoriginrequestpolicyresulttypedef)


```python
# create_origin_request_policy method usage example with argument unpacking

kwargs: CreateOriginRequestPolicyRequestTypeDef = {  # (1)
    "OriginRequestPolicyConfig": ...,
}

parent.create_origin_request_policy(**kwargs)
```

1. See [:material-code-braces: CreateOriginRequestPolicyRequestTypeDef](./type_defs.md#createoriginrequestpolicyrequesttypedef)

### create\_public\_key

Uploads a public key to CloudFront that you can use with <a
href="https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/PrivateContent.html">signed
URLs and signed cookies</a>, or with <a
href="https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/field-level-encryption....

Type annotations and code completion for `#!python session.client("cloudfront").create_public_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_public_key method definition

await def create_public_key(
    self,
    *,
    PublicKeyConfig: PublicKeyConfigTypeDef,  # (1)
) -> CreatePublicKeyResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PublicKeyConfigTypeDef](./type_defs.md#publickeyconfigtypedef)
2. See [:material-code-braces: CreatePublicKeyResultTypeDef](./type_defs.md#createpublickeyresulttypedef)


```python
# create_public_key method usage example with argument unpacking

kwargs: CreatePublicKeyRequestTypeDef = {  # (1)
    "PublicKeyConfig": ...,
}

parent.create_public_key(**kwargs)
```

1. See [:material-code-braces: CreatePublicKeyRequestTypeDef](./type_defs.md#createpublickeyrequesttypedef)

### create\_realtime\_log\_config

Creates a real-time log configuration.

Type annotations and code completion for `#!python session.client("cloudfront").create_realtime_log_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_realtime_log_config method definition

await def create_realtime_log_config(
    self,
    *,
    EndPoints: Sequence[EndPointTypeDef],  # (1)
    Fields: Sequence[str],
    Name: str,
    SamplingRate: int,
) -> CreateRealtimeLogConfigResultTypeDef:  # (2)
    ...
```

1. See `Sequence[EndPointTypeDef]`
2. See [:material-code-braces: CreateRealtimeLogConfigResultTypeDef](./type_defs.md#createrealtimelogconfigresulttypedef)


```python
# create_realtime_log_config method usage example with argument unpacking

kwargs: CreateRealtimeLogConfigRequestTypeDef = {  # (1)
    "EndPoints": ...,
    "Fields": ...,
    "Name": ...,
    "SamplingRate": ...,
}

parent.create_realtime_log_config(**kwargs)
```

1. See [:material-code-braces: CreateRealtimeLogConfigRequestTypeDef](./type_defs.md#createrealtimelogconfigrequesttypedef)

### create\_response\_headers\_policy

Creates a response headers policy.

Type annotations and code completion for `#!python session.client("cloudfront").create_response_headers_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_response_headers_policy method definition

await def create_response_headers_policy(
    self,
    *,
    ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigUnionTypeDef,  # (1)
) -> CreateResponseHeadersPolicyResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ResponseHeadersPolicyConfigUnionTypeDef](#responseheaderspolicyconfiguniontypedef)
2. See [:material-code-braces: CreateResponseHeadersPolicyResultTypeDef](./type_defs.md#createresponseheaderspolicyresulttypedef)


```python
# create_response_headers_policy method usage example with argument unpacking

kwargs: CreateResponseHeadersPolicyRequestTypeDef = {  # (1)
    "ResponseHeadersPolicyConfig": ...,
}

parent.create_response_headers_policy(**kwargs)
```

1. See [:material-code-braces: CreateResponseHeadersPolicyRequestTypeDef](./type_defs.md#createresponseheaderspolicyrequesttypedef)

### create\_streaming\_distribution

This API is deprecated.

Type annotations and code completion for `#!python session.client("cloudfront").create_streaming_distribution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_streaming_distribution method definition

await def create_streaming_distribution(
    self,
    *,
    StreamingDistributionConfig: StreamingDistributionConfigUnionTypeDef,  # (1)
) -> CreateStreamingDistributionResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StreamingDistributionConfigUnionTypeDef](#streamingdistributionconfiguniontypedef)
2. See [:material-code-braces: CreateStreamingDistributionResultTypeDef](./type_defs.md#createstreamingdistributionresulttypedef)


```python
# create_streaming_distribution method usage example with argument unpacking

kwargs: CreateStreamingDistributionRequestTypeDef = {  # (1)
    "StreamingDistributionConfig": ...,
}

parent.create_streaming_distribution(**kwargs)
```

1. See [:material-code-braces: CreateStreamingDistributionRequestTypeDef](./type_defs.md#createstreamingdistributionrequesttypedef)

### create\_streaming\_distribution\_with\_tags

This API is deprecated.

Type annotations and code completion for `#!python session.client("cloudfront").create_streaming_distribution_with_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_streaming_distribution_with_tags method definition

await def create_streaming_distribution_with_tags(
    self,
    *,
    StreamingDistributionConfigWithTags: StreamingDistributionConfigWithTagsTypeDef,  # (1)
) -> CreateStreamingDistributionWithTagsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StreamingDistributionConfigWithTagsTypeDef](./type_defs.md#streamingdistributionconfigwithtagstypedef)
2. See [:material-code-braces: CreateStreamingDistributionWithTagsResultTypeDef](./type_defs.md#createstreamingdistributionwithtagsresulttypedef)


```python
# create_streaming_distribution_with_tags method usage example with argument unpacking

kwargs: CreateStreamingDistributionWithTagsRequestTypeDef = {  # (1)
    "StreamingDistributionConfigWithTags": ...,
}

parent.create_streaming_distribution_with_tags(**kwargs)
```

1. See [:material-code-braces: CreateStreamingDistributionWithTagsRequestTypeDef](./type_defs.md#createstreamingdistributionwithtagsrequesttypedef)

### create\_vpc\_origin

Create an Amazon CloudFront VPC origin.

Type annotations and code completion for `#!python session.client("cloudfront").create_vpc_origin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# create_vpc_origin method definition

await def create_vpc_origin(
    self,
    *,
    VpcOriginEndpointConfig: VpcOriginEndpointConfigUnionTypeDef,  # (1)
    Tags: TagsUnionTypeDef = ...,  # (2)
) -> CreateVpcOriginResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: VpcOriginEndpointConfigUnionTypeDef](#vpcoriginendpointconfiguniontypedef)
2. See [:material-code-braces: TagsUnionTypeDef](#tagsuniontypedef)
3. See [:material-code-braces: CreateVpcOriginResultTypeDef](./type_defs.md#createvpcoriginresulttypedef)


```python
# create_vpc_origin method usage example with argument unpacking

kwargs: CreateVpcOriginRequestTypeDef = {  # (1)
    "VpcOriginEndpointConfig": ...,
}

parent.create_vpc_origin(**kwargs)
```

1. See [:material-code-braces: CreateVpcOriginRequestTypeDef](./type_defs.md#createvpcoriginrequesttypedef)

### delete\_anycast\_ip\_list

Deletes an Anycast static IP list.

Type annotations and code completion for `#!python session.client("cloudfront").delete_anycast_ip_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# delete_anycast_ip_list method definition

await def delete_anycast_ip_list(
    self,
    *,
    Id: str,
    IfMatch: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_anycast_ip_list method usage example with argument unpacking

kwargs: DeleteAnycastIpListRequestTypeDef = {  # (1)
    "Id": ...,
    "IfMatch": ...,
}

parent.delete_anycast_ip_list(**kwargs)
```

1. See [:material-code-braces: DeleteAnycastIpListRequestTypeDef](./type_defs.md#deleteanycastiplistrequesttypedef)

### delete\_cache\_policy

Deletes a cache policy.

Type annotations and code completion for `#!python session.client("cloudfront").delete_cache_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# delete_cache_policy method definition

await def delete_cache_policy(
    self,
    *,
    Id: str,
    IfMatch: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_cache_policy method usage example with argument unpacking

kwargs: DeleteCachePolicyRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_cache_policy(**kwargs)
```

1. See [:material-code-braces: DeleteCachePolicyRequestTypeDef](./type_defs.md#deletecachepolicyrequesttypedef)

### delete\_cloud\_front\_origin\_access\_identity

Delete an origin access identity.

Type annotations and code completion for `#!python session.client("cloudfront").delete_cloud_front_origin_access_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# delete_cloud_front_origin_access_identity method definition

await def delete_cloud_front_origin_access_identity(
    self,
    *,
    Id: str,
    IfMatch: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_cloud_front_origin_access_identity method usage example with argument unpacking

kwargs: DeleteCloudFrontOriginAccessIdentityRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_cloud_front_origin_access_identity(**kwargs)
```

1. See [:material-code-braces: DeleteCloudFrontOriginAccessIdentityRequestTypeDef](./type_defs.md#deletecloudfrontoriginaccessidentityrequesttypedef)

### delete\_continuous\_deployment\_policy

Deletes a continuous deployment policy.

Type annotations and code completion for `#!python session.client("cloudfront").delete_continuous_deployment_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# delete_continuous_deployment_policy method definition

await def delete_continuous_deployment_policy(
    self,
    *,
    Id: str,
    IfMatch: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_continuous_deployment_policy method usage example with argument unpacking

kwargs: DeleteContinuousDeploymentPolicyRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_continuous_deployment_policy(**kwargs)
```

1. See [:material-code-braces: DeleteContinuousDeploymentPolicyRequestTypeDef](./type_defs.md#deletecontinuousdeploymentpolicyrequesttypedef)

### delete\_distribution

Delete a distribution.

Type annotations and code completion for `#!python session.client("cloudfront").delete_distribution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# delete_distribution method definition

await def delete_distribution(
    self,
    *,
    Id: str,
    IfMatch: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_distribution method usage example with argument unpacking

kwargs: DeleteDistributionRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_distribution(**kwargs)
```

1. See [:material-code-braces: DeleteDistributionRequestTypeDef](./type_defs.md#deletedistributionrequesttypedef)

### delete\_field\_level\_encryption\_config

Remove a field-level encryption configuration.

Type annotations and code completion for `#!python session.client("cloudfront").delete_field_level_encryption_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# delete_field_level_encryption_config method definition

await def delete_field_level_encryption_config(
    self,
    *,
    Id: str,
    IfMatch: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_field_level_encryption_config method usage example with argument unpacking

kwargs: DeleteFieldLevelEncryptionConfigRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_field_level_encryption_config(**kwargs)
```

1. See [:material-code-braces: DeleteFieldLevelEncryptionConfigRequestTypeDef](./type_defs.md#deletefieldlevelencryptionconfigrequesttypedef)

### delete\_field\_level\_encryption\_profile

Remove a field-level encryption profile.

Type annotations and code completion for `#!python session.client("cloudfront").delete_field_level_encryption_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# delete_field_level_encryption_profile method definition

await def delete_field_level_encryption_profile(
    self,
    *,
    Id: str,
    IfMatch: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_field_level_encryption_profile method usage example with argument unpacking

kwargs: DeleteFieldLevelEncryptionProfileRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_field_level_encryption_profile(**kwargs)
```

1. See [:material-code-braces: DeleteFieldLevelEncryptionProfileRequestTypeDef](./type_defs.md#deletefieldlevelencryptionprofilerequesttypedef)

### delete\_function

Deletes a CloudFront function.

Type annotations and code completion for `#!python session.client("cloudfront").delete_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# delete_function method definition

await def delete_function(
    self,
    *,
    Name: str,
    IfMatch: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_function method usage example with argument unpacking

kwargs: DeleteFunctionRequestTypeDef = {  # (1)
    "Name": ...,
    "IfMatch": ...,
}

parent.delete_function(**kwargs)
```

1. See [:material-code-braces: DeleteFunctionRequestTypeDef](./type_defs.md#deletefunctionrequesttypedef)

### delete\_key\_group

Deletes a key group.

Type annotations and code completion for `#!python session.client("cloudfront").delete_key_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# delete_key_group method definition

await def delete_key_group(
    self,
    *,
    Id: str,
    IfMatch: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_key_group method usage example with argument unpacking

kwargs: DeleteKeyGroupRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_key_group(**kwargs)
```

1. See [:material-code-braces: DeleteKeyGroupRequestTypeDef](./type_defs.md#deletekeygrouprequesttypedef)

### delete\_key\_value\_store

Specifies the key value store to delete.

Type annotations and code completion for `#!python session.client("cloudfront").delete_key_value_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# delete_key_value_store method definition

await def delete_key_value_store(
    self,
    *,
    Name: str,
    IfMatch: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_key_value_store method usage example with argument unpacking

kwargs: DeleteKeyValueStoreRequestTypeDef = {  # (1)
    "Name": ...,
    "IfMatch": ...,
}

parent.delete_key_value_store(**kwargs)
```

1. See [:material-code-braces: DeleteKeyValueStoreRequestTypeDef](./type_defs.md#deletekeyvaluestorerequesttypedef)

### delete\_monitoring\_subscription

Disables additional CloudWatch metrics for the specified CloudFront
distribution.

Type annotations and code completion for `#!python session.client("cloudfront").delete_monitoring_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# delete_monitoring_subscription method definition

await def delete_monitoring_subscription(
    self,
    *,
    DistributionId: str,
) -> Dict[str, Any]:
    ...
```

```python
# delete_monitoring_subscription method usage example with argument unpacking

kwargs: DeleteMonitoringSubscriptionRequestTypeDef = {  # (1)
    "DistributionId": ...,
}

parent.delete_monitoring_subscription(**kwargs)
```

1. See [:material-code-braces: DeleteMonitoringSubscriptionRequestTypeDef](./type_defs.md#deletemonitoringsubscriptionrequesttypedef)

### delete\_origin\_access\_control

Deletes a CloudFront origin access control.

Type annotations and code completion for `#!python session.client("cloudfront").delete_origin_access_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# delete_origin_access_control method definition

await def delete_origin_access_control(
    self,
    *,
    Id: str,
    IfMatch: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_origin_access_control method usage example with argument unpacking

kwargs: DeleteOriginAccessControlRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_origin_access_control(**kwargs)
```

1. See [:material-code-braces: DeleteOriginAccessControlRequestTypeDef](./type_defs.md#deleteoriginaccesscontrolrequesttypedef)

### delete\_origin\_request\_policy

Deletes an origin request policy.

Type annotations and code completion for `#!python session.client("cloudfront").delete_origin_request_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# delete_origin_request_policy method definition

await def delete_origin_request_policy(
    self,
    *,
    Id: str,
    IfMatch: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_origin_request_policy method usage example with argument unpacking

kwargs: DeleteOriginRequestPolicyRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_origin_request_policy(**kwargs)
```

1. See [:material-code-braces: DeleteOriginRequestPolicyRequestTypeDef](./type_defs.md#deleteoriginrequestpolicyrequesttypedef)

### delete\_public\_key

Remove a public key you previously added to CloudFront.

Type annotations and code completion for `#!python session.client("cloudfront").delete_public_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# delete_public_key method definition

await def delete_public_key(
    self,
    *,
    Id: str,
    IfMatch: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_public_key method usage example with argument unpacking

kwargs: DeletePublicKeyRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_public_key(**kwargs)
```

1. See [:material-code-braces: DeletePublicKeyRequestTypeDef](./type_defs.md#deletepublickeyrequesttypedef)

### delete\_realtime\_log\_config

Deletes a real-time log configuration.

Type annotations and code completion for `#!python session.client("cloudfront").delete_realtime_log_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# delete_realtime_log_config method definition

await def delete_realtime_log_config(
    self,
    *,
    Name: str = ...,
    ARN: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_realtime_log_config method usage example with argument unpacking

kwargs: DeleteRealtimeLogConfigRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_realtime_log_config(**kwargs)
```

1. See [:material-code-braces: DeleteRealtimeLogConfigRequestTypeDef](./type_defs.md#deleterealtimelogconfigrequesttypedef)

### delete\_response\_headers\_policy

Deletes a response headers policy.

Type annotations and code completion for `#!python session.client("cloudfront").delete_response_headers_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# delete_response_headers_policy method definition

await def delete_response_headers_policy(
    self,
    *,
    Id: str,
    IfMatch: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_response_headers_policy method usage example with argument unpacking

kwargs: DeleteResponseHeadersPolicyRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_response_headers_policy(**kwargs)
```

1. See [:material-code-braces: DeleteResponseHeadersPolicyRequestTypeDef](./type_defs.md#deleteresponseheaderspolicyrequesttypedef)

### delete\_streaming\_distribution

Delete a streaming distribution.

Type annotations and code completion for `#!python session.client("cloudfront").delete_streaming_distribution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# delete_streaming_distribution method definition

await def delete_streaming_distribution(
    self,
    *,
    Id: str,
    IfMatch: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_streaming_distribution method usage example with argument unpacking

kwargs: DeleteStreamingDistributionRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_streaming_distribution(**kwargs)
```

1. See [:material-code-braces: DeleteStreamingDistributionRequestTypeDef](./type_defs.md#deletestreamingdistributionrequesttypedef)

### delete\_vpc\_origin

Delete an Amazon CloudFront VPC origin.

Type annotations and code completion for `#!python session.client("cloudfront").delete_vpc_origin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# delete_vpc_origin method definition

await def delete_vpc_origin(
    self,
    *,
    Id: str,
    IfMatch: str,
) -> DeleteVpcOriginResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteVpcOriginResultTypeDef](./type_defs.md#deletevpcoriginresulttypedef)


```python
# delete_vpc_origin method usage example with argument unpacking

kwargs: DeleteVpcOriginRequestTypeDef = {  # (1)
    "Id": ...,
    "IfMatch": ...,
}

parent.delete_vpc_origin(**kwargs)
```

1. See [:material-code-braces: DeleteVpcOriginRequestTypeDef](./type_defs.md#deletevpcoriginrequesttypedef)

### describe\_function

Gets configuration information and metadata about a CloudFront function, but
not the function's code.

Type annotations and code completion for `#!python session.client("cloudfront").describe_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# describe_function method definition

await def describe_function(
    self,
    *,
    Name: str,
    Stage: FunctionStageType = ...,  # (1)
) -> DescribeFunctionResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: FunctionStageType](./literals.md#functionstagetype)
2. See [:material-code-braces: DescribeFunctionResultTypeDef](./type_defs.md#describefunctionresulttypedef)


```python
# describe_function method usage example with argument unpacking

kwargs: DescribeFunctionRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.describe_function(**kwargs)
```

1. See [:material-code-braces: DescribeFunctionRequestTypeDef](./type_defs.md#describefunctionrequesttypedef)

### describe\_key\_value\_store

Specifies the key value store and its configuration.

Type annotations and code completion for `#!python session.client("cloudfront").describe_key_value_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# describe_key_value_store method definition

await def describe_key_value_store(
    self,
    *,
    Name: str,
) -> DescribeKeyValueStoreResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeKeyValueStoreResultTypeDef](./type_defs.md#describekeyvaluestoreresulttypedef)


```python
# describe_key_value_store method usage example with argument unpacking

kwargs: DescribeKeyValueStoreRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.describe_key_value_store(**kwargs)
```

1. See [:material-code-braces: DescribeKeyValueStoreRequestTypeDef](./type_defs.md#describekeyvaluestorerequesttypedef)

### get\_anycast\_ip\_list

Gets an Anycast static IP list.

Type annotations and code completion for `#!python session.client("cloudfront").get_anycast_ip_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_anycast_ip_list method definition

await def get_anycast_ip_list(
    self,
    *,
    Id: str,
) -> GetAnycastIpListResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAnycastIpListResultTypeDef](./type_defs.md#getanycastiplistresulttypedef)


```python
# get_anycast_ip_list method usage example with argument unpacking

kwargs: GetAnycastIpListRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_anycast_ip_list(**kwargs)
```

1. See [:material-code-braces: GetAnycastIpListRequestTypeDef](./type_defs.md#getanycastiplistrequesttypedef)

### get\_cache\_policy

Gets a cache policy, including the following metadata:.

Type annotations and code completion for `#!python session.client("cloudfront").get_cache_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_cache_policy method definition

await def get_cache_policy(
    self,
    *,
    Id: str,
) -> GetCachePolicyResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCachePolicyResultTypeDef](./type_defs.md#getcachepolicyresulttypedef)


```python
# get_cache_policy method usage example with argument unpacking

kwargs: GetCachePolicyRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_cache_policy(**kwargs)
```

1. See [:material-code-braces: GetCachePolicyRequestTypeDef](./type_defs.md#getcachepolicyrequesttypedef)

### get\_cache\_policy\_config

Gets a cache policy configuration.

Type annotations and code completion for `#!python session.client("cloudfront").get_cache_policy_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_cache_policy_config method definition

await def get_cache_policy_config(
    self,
    *,
    Id: str,
) -> GetCachePolicyConfigResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCachePolicyConfigResultTypeDef](./type_defs.md#getcachepolicyconfigresulttypedef)


```python
# get_cache_policy_config method usage example with argument unpacking

kwargs: GetCachePolicyConfigRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_cache_policy_config(**kwargs)
```

1. See [:material-code-braces: GetCachePolicyConfigRequestTypeDef](./type_defs.md#getcachepolicyconfigrequesttypedef)

### get\_cloud\_front\_origin\_access\_identity

Get the information about an origin access identity.

Type annotations and code completion for `#!python session.client("cloudfront").get_cloud_front_origin_access_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_cloud_front_origin_access_identity method definition

await def get_cloud_front_origin_access_identity(
    self,
    *,
    Id: str,
) -> GetCloudFrontOriginAccessIdentityResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCloudFrontOriginAccessIdentityResultTypeDef](./type_defs.md#getcloudfrontoriginaccessidentityresulttypedef)


```python
# get_cloud_front_origin_access_identity method usage example with argument unpacking

kwargs: GetCloudFrontOriginAccessIdentityRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_cloud_front_origin_access_identity(**kwargs)
```

1. See [:material-code-braces: GetCloudFrontOriginAccessIdentityRequestTypeDef](./type_defs.md#getcloudfrontoriginaccessidentityrequesttypedef)

### get\_cloud\_front\_origin\_access\_identity\_config

Get the configuration information about an origin access identity.

Type annotations and code completion for `#!python session.client("cloudfront").get_cloud_front_origin_access_identity_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_cloud_front_origin_access_identity_config method definition

await def get_cloud_front_origin_access_identity_config(
    self,
    *,
    Id: str,
) -> GetCloudFrontOriginAccessIdentityConfigResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCloudFrontOriginAccessIdentityConfigResultTypeDef](./type_defs.md#getcloudfrontoriginaccessidentityconfigresulttypedef)


```python
# get_cloud_front_origin_access_identity_config method usage example with argument unpacking

kwargs: GetCloudFrontOriginAccessIdentityConfigRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_cloud_front_origin_access_identity_config(**kwargs)
```

1. See [:material-code-braces: GetCloudFrontOriginAccessIdentityConfigRequestTypeDef](./type_defs.md#getcloudfrontoriginaccessidentityconfigrequesttypedef)

### get\_continuous\_deployment\_policy

Gets a continuous deployment policy, including metadata (the policy's
identifier and the date and time when the policy was last modified).

Type annotations and code completion for `#!python session.client("cloudfront").get_continuous_deployment_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_continuous_deployment_policy method definition

await def get_continuous_deployment_policy(
    self,
    *,
    Id: str,
) -> GetContinuousDeploymentPolicyResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetContinuousDeploymentPolicyResultTypeDef](./type_defs.md#getcontinuousdeploymentpolicyresulttypedef)


```python
# get_continuous_deployment_policy method usage example with argument unpacking

kwargs: GetContinuousDeploymentPolicyRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_continuous_deployment_policy(**kwargs)
```

1. See [:material-code-braces: GetContinuousDeploymentPolicyRequestTypeDef](./type_defs.md#getcontinuousdeploymentpolicyrequesttypedef)

### get\_continuous\_deployment\_policy\_config

Gets configuration information about a continuous deployment policy.

Type annotations and code completion for `#!python session.client("cloudfront").get_continuous_deployment_policy_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_continuous_deployment_policy_config method definition

await def get_continuous_deployment_policy_config(
    self,
    *,
    Id: str,
) -> GetContinuousDeploymentPolicyConfigResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetContinuousDeploymentPolicyConfigResultTypeDef](./type_defs.md#getcontinuousdeploymentpolicyconfigresulttypedef)


```python
# get_continuous_deployment_policy_config method usage example with argument unpacking

kwargs: GetContinuousDeploymentPolicyConfigRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_continuous_deployment_policy_config(**kwargs)
```

1. See [:material-code-braces: GetContinuousDeploymentPolicyConfigRequestTypeDef](./type_defs.md#getcontinuousdeploymentpolicyconfigrequesttypedef)

### get\_distribution

Get the information about a distribution.

Type annotations and code completion for `#!python session.client("cloudfront").get_distribution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_distribution method definition

await def get_distribution(
    self,
    *,
    Id: str,
) -> GetDistributionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDistributionResultTypeDef](./type_defs.md#getdistributionresulttypedef)


```python
# get_distribution method usage example with argument unpacking

kwargs: GetDistributionRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_distribution(**kwargs)
```

1. See [:material-code-braces: GetDistributionRequestTypeDef](./type_defs.md#getdistributionrequesttypedef)

### get\_distribution\_config

Get the configuration information about a distribution.

Type annotations and code completion for `#!python session.client("cloudfront").get_distribution_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_distribution_config method definition

await def get_distribution_config(
    self,
    *,
    Id: str,
) -> GetDistributionConfigResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDistributionConfigResultTypeDef](./type_defs.md#getdistributionconfigresulttypedef)


```python
# get_distribution_config method usage example with argument unpacking

kwargs: GetDistributionConfigRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_distribution_config(**kwargs)
```

1. See [:material-code-braces: GetDistributionConfigRequestTypeDef](./type_defs.md#getdistributionconfigrequesttypedef)

### get\_field\_level\_encryption

Get the field-level encryption configuration information.

Type annotations and code completion for `#!python session.client("cloudfront").get_field_level_encryption` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_field_level_encryption method definition

await def get_field_level_encryption(
    self,
    *,
    Id: str,
) -> GetFieldLevelEncryptionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFieldLevelEncryptionResultTypeDef](./type_defs.md#getfieldlevelencryptionresulttypedef)


```python
# get_field_level_encryption method usage example with argument unpacking

kwargs: GetFieldLevelEncryptionRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_field_level_encryption(**kwargs)
```

1. See [:material-code-braces: GetFieldLevelEncryptionRequestTypeDef](./type_defs.md#getfieldlevelencryptionrequesttypedef)

### get\_field\_level\_encryption\_config

Get the field-level encryption configuration information.

Type annotations and code completion for `#!python session.client("cloudfront").get_field_level_encryption_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_field_level_encryption_config method definition

await def get_field_level_encryption_config(
    self,
    *,
    Id: str,
) -> GetFieldLevelEncryptionConfigResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFieldLevelEncryptionConfigResultTypeDef](./type_defs.md#getfieldlevelencryptionconfigresulttypedef)


```python
# get_field_level_encryption_config method usage example with argument unpacking

kwargs: GetFieldLevelEncryptionConfigRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_field_level_encryption_config(**kwargs)
```

1. See [:material-code-braces: GetFieldLevelEncryptionConfigRequestTypeDef](./type_defs.md#getfieldlevelencryptionconfigrequesttypedef)

### get\_field\_level\_encryption\_profile

Get the field-level encryption profile information.

Type annotations and code completion for `#!python session.client("cloudfront").get_field_level_encryption_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_field_level_encryption_profile method definition

await def get_field_level_encryption_profile(
    self,
    *,
    Id: str,
) -> GetFieldLevelEncryptionProfileResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFieldLevelEncryptionProfileResultTypeDef](./type_defs.md#getfieldlevelencryptionprofileresulttypedef)


```python
# get_field_level_encryption_profile method usage example with argument unpacking

kwargs: GetFieldLevelEncryptionProfileRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_field_level_encryption_profile(**kwargs)
```

1. See [:material-code-braces: GetFieldLevelEncryptionProfileRequestTypeDef](./type_defs.md#getfieldlevelencryptionprofilerequesttypedef)

### get\_field\_level\_encryption\_profile\_config

Get the field-level encryption profile configuration information.

Type annotations and code completion for `#!python session.client("cloudfront").get_field_level_encryption_profile_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_field_level_encryption_profile_config method definition

await def get_field_level_encryption_profile_config(
    self,
    *,
    Id: str,
) -> GetFieldLevelEncryptionProfileConfigResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFieldLevelEncryptionProfileConfigResultTypeDef](./type_defs.md#getfieldlevelencryptionprofileconfigresulttypedef)


```python
# get_field_level_encryption_profile_config method usage example with argument unpacking

kwargs: GetFieldLevelEncryptionProfileConfigRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_field_level_encryption_profile_config(**kwargs)
```

1. See [:material-code-braces: GetFieldLevelEncryptionProfileConfigRequestTypeDef](./type_defs.md#getfieldlevelencryptionprofileconfigrequesttypedef)

### get\_function

Gets the code of a CloudFront function.

Type annotations and code completion for `#!python session.client("cloudfront").get_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_function method definition

await def get_function(
    self,
    *,
    Name: str,
    Stage: FunctionStageType = ...,  # (1)
) -> GetFunctionResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: FunctionStageType](./literals.md#functionstagetype)
2. See [:material-code-braces: GetFunctionResultTypeDef](./type_defs.md#getfunctionresulttypedef)


```python
# get_function method usage example with argument unpacking

kwargs: GetFunctionRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_function(**kwargs)
```

1. See [:material-code-braces: GetFunctionRequestTypeDef](./type_defs.md#getfunctionrequesttypedef)

### get\_invalidation

Get the information about an invalidation.

Type annotations and code completion for `#!python session.client("cloudfront").get_invalidation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_invalidation method definition

await def get_invalidation(
    self,
    *,
    DistributionId: str,
    Id: str,
) -> GetInvalidationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInvalidationResultTypeDef](./type_defs.md#getinvalidationresulttypedef)


```python
# get_invalidation method usage example with argument unpacking

kwargs: GetInvalidationRequestTypeDef = {  # (1)
    "DistributionId": ...,
    "Id": ...,
}

parent.get_invalidation(**kwargs)
```

1. See [:material-code-braces: GetInvalidationRequestTypeDef](./type_defs.md#getinvalidationrequesttypedef)

### get\_key\_group

Gets a key group, including the date and time when the key group was last
modified.

Type annotations and code completion for `#!python session.client("cloudfront").get_key_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_key_group method definition

await def get_key_group(
    self,
    *,
    Id: str,
) -> GetKeyGroupResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetKeyGroupResultTypeDef](./type_defs.md#getkeygroupresulttypedef)


```python
# get_key_group method usage example with argument unpacking

kwargs: GetKeyGroupRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_key_group(**kwargs)
```

1. See [:material-code-braces: GetKeyGroupRequestTypeDef](./type_defs.md#getkeygrouprequesttypedef)

### get\_key\_group\_config

Gets a key group configuration.

Type annotations and code completion for `#!python session.client("cloudfront").get_key_group_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_key_group_config method definition

await def get_key_group_config(
    self,
    *,
    Id: str,
) -> GetKeyGroupConfigResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetKeyGroupConfigResultTypeDef](./type_defs.md#getkeygroupconfigresulttypedef)


```python
# get_key_group_config method usage example with argument unpacking

kwargs: GetKeyGroupConfigRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_key_group_config(**kwargs)
```

1. See [:material-code-braces: GetKeyGroupConfigRequestTypeDef](./type_defs.md#getkeygroupconfigrequesttypedef)

### get\_monitoring\_subscription

Gets information about whether additional CloudWatch metrics are enabled for
the specified CloudFront distribution.

Type annotations and code completion for `#!python session.client("cloudfront").get_monitoring_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_monitoring_subscription method definition

await def get_monitoring_subscription(
    self,
    *,
    DistributionId: str,
) -> GetMonitoringSubscriptionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMonitoringSubscriptionResultTypeDef](./type_defs.md#getmonitoringsubscriptionresulttypedef)


```python
# get_monitoring_subscription method usage example with argument unpacking

kwargs: GetMonitoringSubscriptionRequestTypeDef = {  # (1)
    "DistributionId": ...,
}

parent.get_monitoring_subscription(**kwargs)
```

1. See [:material-code-braces: GetMonitoringSubscriptionRequestTypeDef](./type_defs.md#getmonitoringsubscriptionrequesttypedef)

### get\_origin\_access\_control

Gets a CloudFront origin access control, including its unique identifier.

Type annotations and code completion for `#!python session.client("cloudfront").get_origin_access_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_origin_access_control method definition

await def get_origin_access_control(
    self,
    *,
    Id: str,
) -> GetOriginAccessControlResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOriginAccessControlResultTypeDef](./type_defs.md#getoriginaccesscontrolresulttypedef)


```python
# get_origin_access_control method usage example with argument unpacking

kwargs: GetOriginAccessControlRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_origin_access_control(**kwargs)
```

1. See [:material-code-braces: GetOriginAccessControlRequestTypeDef](./type_defs.md#getoriginaccesscontrolrequesttypedef)

### get\_origin\_access\_control\_config

Gets a CloudFront origin access control configuration.

Type annotations and code completion for `#!python session.client("cloudfront").get_origin_access_control_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_origin_access_control_config method definition

await def get_origin_access_control_config(
    self,
    *,
    Id: str,
) -> GetOriginAccessControlConfigResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOriginAccessControlConfigResultTypeDef](./type_defs.md#getoriginaccesscontrolconfigresulttypedef)


```python
# get_origin_access_control_config method usage example with argument unpacking

kwargs: GetOriginAccessControlConfigRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_origin_access_control_config(**kwargs)
```

1. See [:material-code-braces: GetOriginAccessControlConfigRequestTypeDef](./type_defs.md#getoriginaccesscontrolconfigrequesttypedef)

### get\_origin\_request\_policy

Gets an origin request policy, including the following metadata:.

Type annotations and code completion for `#!python session.client("cloudfront").get_origin_request_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_origin_request_policy method definition

await def get_origin_request_policy(
    self,
    *,
    Id: str,
) -> GetOriginRequestPolicyResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOriginRequestPolicyResultTypeDef](./type_defs.md#getoriginrequestpolicyresulttypedef)


```python
# get_origin_request_policy method usage example with argument unpacking

kwargs: GetOriginRequestPolicyRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_origin_request_policy(**kwargs)
```

1. See [:material-code-braces: GetOriginRequestPolicyRequestTypeDef](./type_defs.md#getoriginrequestpolicyrequesttypedef)

### get\_origin\_request\_policy\_config

Gets an origin request policy configuration.

Type annotations and code completion for `#!python session.client("cloudfront").get_origin_request_policy_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_origin_request_policy_config method definition

await def get_origin_request_policy_config(
    self,
    *,
    Id: str,
) -> GetOriginRequestPolicyConfigResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOriginRequestPolicyConfigResultTypeDef](./type_defs.md#getoriginrequestpolicyconfigresulttypedef)


```python
# get_origin_request_policy_config method usage example with argument unpacking

kwargs: GetOriginRequestPolicyConfigRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_origin_request_policy_config(**kwargs)
```

1. See [:material-code-braces: GetOriginRequestPolicyConfigRequestTypeDef](./type_defs.md#getoriginrequestpolicyconfigrequesttypedef)

### get\_public\_key

Gets a public key.

Type annotations and code completion for `#!python session.client("cloudfront").get_public_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_public_key method definition

await def get_public_key(
    self,
    *,
    Id: str,
) -> GetPublicKeyResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPublicKeyResultTypeDef](./type_defs.md#getpublickeyresulttypedef)


```python
# get_public_key method usage example with argument unpacking

kwargs: GetPublicKeyRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_public_key(**kwargs)
```

1. See [:material-code-braces: GetPublicKeyRequestTypeDef](./type_defs.md#getpublickeyrequesttypedef)

### get\_public\_key\_config

Gets a public key configuration.

Type annotations and code completion for `#!python session.client("cloudfront").get_public_key_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_public_key_config method definition

await def get_public_key_config(
    self,
    *,
    Id: str,
) -> GetPublicKeyConfigResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPublicKeyConfigResultTypeDef](./type_defs.md#getpublickeyconfigresulttypedef)


```python
# get_public_key_config method usage example with argument unpacking

kwargs: GetPublicKeyConfigRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_public_key_config(**kwargs)
```

1. See [:material-code-braces: GetPublicKeyConfigRequestTypeDef](./type_defs.md#getpublickeyconfigrequesttypedef)

### get\_realtime\_log\_config

Gets a real-time log configuration.

Type annotations and code completion for `#!python session.client("cloudfront").get_realtime_log_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_realtime_log_config method definition

await def get_realtime_log_config(
    self,
    *,
    Name: str = ...,
    ARN: str = ...,
) -> GetRealtimeLogConfigResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRealtimeLogConfigResultTypeDef](./type_defs.md#getrealtimelogconfigresulttypedef)


```python
# get_realtime_log_config method usage example with argument unpacking

kwargs: GetRealtimeLogConfigRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_realtime_log_config(**kwargs)
```

1. See [:material-code-braces: GetRealtimeLogConfigRequestTypeDef](./type_defs.md#getrealtimelogconfigrequesttypedef)

### get\_response\_headers\_policy

Gets a response headers policy, including metadata (the policy's identifier and
the date and time when the policy was last modified).

Type annotations and code completion for `#!python session.client("cloudfront").get_response_headers_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_response_headers_policy method definition

await def get_response_headers_policy(
    self,
    *,
    Id: str,
) -> GetResponseHeadersPolicyResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResponseHeadersPolicyResultTypeDef](./type_defs.md#getresponseheaderspolicyresulttypedef)


```python
# get_response_headers_policy method usage example with argument unpacking

kwargs: GetResponseHeadersPolicyRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_response_headers_policy(**kwargs)
```

1. See [:material-code-braces: GetResponseHeadersPolicyRequestTypeDef](./type_defs.md#getresponseheaderspolicyrequesttypedef)

### get\_response\_headers\_policy\_config

Gets a response headers policy configuration.

Type annotations and code completion for `#!python session.client("cloudfront").get_response_headers_policy_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_response_headers_policy_config method definition

await def get_response_headers_policy_config(
    self,
    *,
    Id: str,
) -> GetResponseHeadersPolicyConfigResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResponseHeadersPolicyConfigResultTypeDef](./type_defs.md#getresponseheaderspolicyconfigresulttypedef)


```python
# get_response_headers_policy_config method usage example with argument unpacking

kwargs: GetResponseHeadersPolicyConfigRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_response_headers_policy_config(**kwargs)
```

1. See [:material-code-braces: GetResponseHeadersPolicyConfigRequestTypeDef](./type_defs.md#getresponseheaderspolicyconfigrequesttypedef)

### get\_streaming\_distribution

Gets information about a specified RTMP distribution, including the
distribution configuration.

Type annotations and code completion for `#!python session.client("cloudfront").get_streaming_distribution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_streaming_distribution method definition

await def get_streaming_distribution(
    self,
    *,
    Id: str,
) -> GetStreamingDistributionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStreamingDistributionResultTypeDef](./type_defs.md#getstreamingdistributionresulttypedef)


```python
# get_streaming_distribution method usage example with argument unpacking

kwargs: GetStreamingDistributionRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_streaming_distribution(**kwargs)
```

1. See [:material-code-braces: GetStreamingDistributionRequestTypeDef](./type_defs.md#getstreamingdistributionrequesttypedef)

### get\_streaming\_distribution\_config

Get the configuration information about a streaming distribution.

Type annotations and code completion for `#!python session.client("cloudfront").get_streaming_distribution_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_streaming_distribution_config method definition

await def get_streaming_distribution_config(
    self,
    *,
    Id: str,
) -> GetStreamingDistributionConfigResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStreamingDistributionConfigResultTypeDef](./type_defs.md#getstreamingdistributionconfigresulttypedef)


```python
# get_streaming_distribution_config method usage example with argument unpacking

kwargs: GetStreamingDistributionConfigRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_streaming_distribution_config(**kwargs)
```

1. See [:material-code-braces: GetStreamingDistributionConfigRequestTypeDef](./type_defs.md#getstreamingdistributionconfigrequesttypedef)

### get\_vpc\_origin

Get the details of an Amazon CloudFront VPC origin.

Type annotations and code completion for `#!python session.client("cloudfront").get_vpc_origin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# get_vpc_origin method definition

await def get_vpc_origin(
    self,
    *,
    Id: str,
) -> GetVpcOriginResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVpcOriginResultTypeDef](./type_defs.md#getvpcoriginresulttypedef)


```python
# get_vpc_origin method usage example with argument unpacking

kwargs: GetVpcOriginRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_vpc_origin(**kwargs)
```

1. See [:material-code-braces: GetVpcOriginRequestTypeDef](./type_defs.md#getvpcoriginrequesttypedef)

### list\_anycast\_ip\_lists

Lists your Anycast static IP lists.

Type annotations and code completion for `#!python session.client("cloudfront").list_anycast_ip_lists` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_anycast_ip_lists method definition

await def list_anycast_ip_lists(
    self,
    *,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListAnycastIpListsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAnycastIpListsResultTypeDef](./type_defs.md#listanycastiplistsresulttypedef)


```python
# list_anycast_ip_lists method usage example with argument unpacking

kwargs: ListAnycastIpListsRequestTypeDef = {  # (1)
    "Marker": ...,
}

parent.list_anycast_ip_lists(**kwargs)
```

1. See [:material-code-braces: ListAnycastIpListsRequestTypeDef](./type_defs.md#listanycastiplistsrequesttypedef)

### list\_cache\_policies

Gets a list of cache policies.

Type annotations and code completion for `#!python session.client("cloudfront").list_cache_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_cache_policies method definition

await def list_cache_policies(
    self,
    *,
    Type: CachePolicyTypeType = ...,  # (1)
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListCachePoliciesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: CachePolicyTypeType](./literals.md#cachepolicytypetype)
2. See [:material-code-braces: ListCachePoliciesResultTypeDef](./type_defs.md#listcachepoliciesresulttypedef)


```python
# list_cache_policies method usage example with argument unpacking

kwargs: ListCachePoliciesRequestTypeDef = {  # (1)
    "Type": ...,
}

parent.list_cache_policies(**kwargs)
```

1. See [:material-code-braces: ListCachePoliciesRequestTypeDef](./type_defs.md#listcachepoliciesrequesttypedef)

### list\_cloud\_front\_origin\_access\_identities

Lists origin access identities.

Type annotations and code completion for `#!python session.client("cloudfront").list_cloud_front_origin_access_identities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_cloud_front_origin_access_identities method definition

await def list_cloud_front_origin_access_identities(
    self,
    *,
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListCloudFrontOriginAccessIdentitiesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCloudFrontOriginAccessIdentitiesResultTypeDef](./type_defs.md#listcloudfrontoriginaccessidentitiesresulttypedef)


```python
# list_cloud_front_origin_access_identities method usage example with argument unpacking

kwargs: ListCloudFrontOriginAccessIdentitiesRequestTypeDef = {  # (1)
    "Marker": ...,
}

parent.list_cloud_front_origin_access_identities(**kwargs)
```

1. See [:material-code-braces: ListCloudFrontOriginAccessIdentitiesRequestTypeDef](./type_defs.md#listcloudfrontoriginaccessidentitiesrequesttypedef)

### list\_conflicting\_aliases

Gets a list of aliases (also called CNAMEs or alternate domain names) that
conflict or overlap with the provided alias, and the associated CloudFront
distributions and Amazon Web Services accounts for each conflicting alias.

Type annotations and code completion for `#!python session.client("cloudfront").list_conflicting_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_conflicting_aliases method definition

await def list_conflicting_aliases(
    self,
    *,
    DistributionId: str,
    Alias: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListConflictingAliasesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListConflictingAliasesResultTypeDef](./type_defs.md#listconflictingaliasesresulttypedef)


```python
# list_conflicting_aliases method usage example with argument unpacking

kwargs: ListConflictingAliasesRequestTypeDef = {  # (1)
    "DistributionId": ...,
    "Alias": ...,
}

parent.list_conflicting_aliases(**kwargs)
```

1. See [:material-code-braces: ListConflictingAliasesRequestTypeDef](./type_defs.md#listconflictingaliasesrequesttypedef)

### list\_continuous\_deployment\_policies

Gets a list of the continuous deployment policies in your Amazon Web Services
account.

Type annotations and code completion for `#!python session.client("cloudfront").list_continuous_deployment_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_continuous_deployment_policies method definition

await def list_continuous_deployment_policies(
    self,
    *,
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListContinuousDeploymentPoliciesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListContinuousDeploymentPoliciesResultTypeDef](./type_defs.md#listcontinuousdeploymentpoliciesresulttypedef)


```python
# list_continuous_deployment_policies method usage example with argument unpacking

kwargs: ListContinuousDeploymentPoliciesRequestTypeDef = {  # (1)
    "Marker": ...,
}

parent.list_continuous_deployment_policies(**kwargs)
```

1. See [:material-code-braces: ListContinuousDeploymentPoliciesRequestTypeDef](./type_defs.md#listcontinuousdeploymentpoliciesrequesttypedef)

### list\_distributions

List CloudFront distributions.

Type annotations and code completion for `#!python session.client("cloudfront").list_distributions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_distributions method definition

await def list_distributions(
    self,
    *,
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListDistributionsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDistributionsResultTypeDef](./type_defs.md#listdistributionsresulttypedef)


```python
# list_distributions method usage example with argument unpacking

kwargs: ListDistributionsRequestTypeDef = {  # (1)
    "Marker": ...,
}

parent.list_distributions(**kwargs)
```

1. See [:material-code-braces: ListDistributionsRequestTypeDef](./type_defs.md#listdistributionsrequesttypedef)

### list\_distributions\_by\_anycast\_ip\_list\_id

Lists the distributions in your account that are associated with the specified
<code>AnycastIpListId</code>.

Type annotations and code completion for `#!python session.client("cloudfront").list_distributions_by_anycast_ip_list_id` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_distributions_by_anycast_ip_list_id method definition

await def list_distributions_by_anycast_ip_list_id(
    self,
    *,
    AnycastIpListId: str,
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListDistributionsByAnycastIpListIdResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDistributionsByAnycastIpListIdResultTypeDef](./type_defs.md#listdistributionsbyanycastiplistidresulttypedef)


```python
# list_distributions_by_anycast_ip_list_id method usage example with argument unpacking

kwargs: ListDistributionsByAnycastIpListIdRequestTypeDef = {  # (1)
    "AnycastIpListId": ...,
}

parent.list_distributions_by_anycast_ip_list_id(**kwargs)
```

1. See [:material-code-braces: ListDistributionsByAnycastIpListIdRequestTypeDef](./type_defs.md#listdistributionsbyanycastiplistidrequesttypedef)

### list\_distributions\_by\_cache\_policy\_id

Gets a list of distribution IDs for distributions that have a cache behavior
that's associated with the specified cache policy.

Type annotations and code completion for `#!python session.client("cloudfront").list_distributions_by_cache_policy_id` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_distributions_by_cache_policy_id method definition

await def list_distributions_by_cache_policy_id(
    self,
    *,
    CachePolicyId: str,
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListDistributionsByCachePolicyIdResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDistributionsByCachePolicyIdResultTypeDef](./type_defs.md#listdistributionsbycachepolicyidresulttypedef)


```python
# list_distributions_by_cache_policy_id method usage example with argument unpacking

kwargs: ListDistributionsByCachePolicyIdRequestTypeDef = {  # (1)
    "CachePolicyId": ...,
}

parent.list_distributions_by_cache_policy_id(**kwargs)
```

1. See [:material-code-braces: ListDistributionsByCachePolicyIdRequestTypeDef](./type_defs.md#listdistributionsbycachepolicyidrequesttypedef)

### list\_distributions\_by\_key\_group

Gets a list of distribution IDs for distributions that have a cache behavior
that references the specified key group.

Type annotations and code completion for `#!python session.client("cloudfront").list_distributions_by_key_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_distributions_by_key_group method definition

await def list_distributions_by_key_group(
    self,
    *,
    KeyGroupId: str,
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListDistributionsByKeyGroupResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDistributionsByKeyGroupResultTypeDef](./type_defs.md#listdistributionsbykeygroupresulttypedef)


```python
# list_distributions_by_key_group method usage example with argument unpacking

kwargs: ListDistributionsByKeyGroupRequestTypeDef = {  # (1)
    "KeyGroupId": ...,
}

parent.list_distributions_by_key_group(**kwargs)
```

1. See [:material-code-braces: ListDistributionsByKeyGroupRequestTypeDef](./type_defs.md#listdistributionsbykeygrouprequesttypedef)

### list\_distributions\_by\_origin\_request\_policy\_id

Gets a list of distribution IDs for distributions that have a cache behavior
that's associated with the specified origin request policy.

Type annotations and code completion for `#!python session.client("cloudfront").list_distributions_by_origin_request_policy_id` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_distributions_by_origin_request_policy_id method definition

await def list_distributions_by_origin_request_policy_id(
    self,
    *,
    OriginRequestPolicyId: str,
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListDistributionsByOriginRequestPolicyIdResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDistributionsByOriginRequestPolicyIdResultTypeDef](./type_defs.md#listdistributionsbyoriginrequestpolicyidresulttypedef)


```python
# list_distributions_by_origin_request_policy_id method usage example with argument unpacking

kwargs: ListDistributionsByOriginRequestPolicyIdRequestTypeDef = {  # (1)
    "OriginRequestPolicyId": ...,
}

parent.list_distributions_by_origin_request_policy_id(**kwargs)
```

1. See [:material-code-braces: ListDistributionsByOriginRequestPolicyIdRequestTypeDef](./type_defs.md#listdistributionsbyoriginrequestpolicyidrequesttypedef)

### list\_distributions\_by\_realtime\_log\_config

Gets a list of distributions that have a cache behavior that's associated with
the specified real-time log configuration.

Type annotations and code completion for `#!python session.client("cloudfront").list_distributions_by_realtime_log_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_distributions_by_realtime_log_config method definition

await def list_distributions_by_realtime_log_config(
    self,
    *,
    Marker: str = ...,
    MaxItems: str = ...,
    RealtimeLogConfigName: str = ...,
    RealtimeLogConfigArn: str = ...,
) -> ListDistributionsByRealtimeLogConfigResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDistributionsByRealtimeLogConfigResultTypeDef](./type_defs.md#listdistributionsbyrealtimelogconfigresulttypedef)


```python
# list_distributions_by_realtime_log_config method usage example with argument unpacking

kwargs: ListDistributionsByRealtimeLogConfigRequestTypeDef = {  # (1)
    "Marker": ...,
}

parent.list_distributions_by_realtime_log_config(**kwargs)
```

1. See [:material-code-braces: ListDistributionsByRealtimeLogConfigRequestTypeDef](./type_defs.md#listdistributionsbyrealtimelogconfigrequesttypedef)

### list\_distributions\_by\_response\_headers\_policy\_id

Gets a list of distribution IDs for distributions that have a cache behavior
that's associated with the specified response headers policy.

Type annotations and code completion for `#!python session.client("cloudfront").list_distributions_by_response_headers_policy_id` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_distributions_by_response_headers_policy_id method definition

await def list_distributions_by_response_headers_policy_id(
    self,
    *,
    ResponseHeadersPolicyId: str,
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListDistributionsByResponseHeadersPolicyIdResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDistributionsByResponseHeadersPolicyIdResultTypeDef](./type_defs.md#listdistributionsbyresponseheaderspolicyidresulttypedef)


```python
# list_distributions_by_response_headers_policy_id method usage example with argument unpacking

kwargs: ListDistributionsByResponseHeadersPolicyIdRequestTypeDef = {  # (1)
    "ResponseHeadersPolicyId": ...,
}

parent.list_distributions_by_response_headers_policy_id(**kwargs)
```

1. See [:material-code-braces: ListDistributionsByResponseHeadersPolicyIdRequestTypeDef](./type_defs.md#listdistributionsbyresponseheaderspolicyidrequesttypedef)

### list\_distributions\_by\_vpc\_origin\_id

List CloudFront distributions by their VPC origin ID.

Type annotations and code completion for `#!python session.client("cloudfront").list_distributions_by_vpc_origin_id` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_distributions_by_vpc_origin_id method definition

await def list_distributions_by_vpc_origin_id(
    self,
    *,
    VpcOriginId: str,
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListDistributionsByVpcOriginIdResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDistributionsByVpcOriginIdResultTypeDef](./type_defs.md#listdistributionsbyvpcoriginidresulttypedef)


```python
# list_distributions_by_vpc_origin_id method usage example with argument unpacking

kwargs: ListDistributionsByVpcOriginIdRequestTypeDef = {  # (1)
    "VpcOriginId": ...,
}

parent.list_distributions_by_vpc_origin_id(**kwargs)
```

1. See [:material-code-braces: ListDistributionsByVpcOriginIdRequestTypeDef](./type_defs.md#listdistributionsbyvpcoriginidrequesttypedef)

### list\_distributions\_by\_web\_acl\_id

List the distributions that are associated with a specified WAF web ACL.

Type annotations and code completion for `#!python session.client("cloudfront").list_distributions_by_web_acl_id` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_distributions_by_web_acl_id method definition

await def list_distributions_by_web_acl_id(
    self,
    *,
    WebACLId: str,
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListDistributionsByWebACLIdResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDistributionsByWebACLIdResultTypeDef](./type_defs.md#listdistributionsbywebaclidresulttypedef)


```python
# list_distributions_by_web_acl_id method usage example with argument unpacking

kwargs: ListDistributionsByWebACLIdRequestTypeDef = {  # (1)
    "WebACLId": ...,
}

parent.list_distributions_by_web_acl_id(**kwargs)
```

1. See [:material-code-braces: ListDistributionsByWebACLIdRequestTypeDef](./type_defs.md#listdistributionsbywebaclidrequesttypedef)

### list\_field\_level\_encryption\_configs

List all field-level encryption configurations that have been created in
CloudFront for this account.

Type annotations and code completion for `#!python session.client("cloudfront").list_field_level_encryption_configs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_field_level_encryption_configs method definition

await def list_field_level_encryption_configs(
    self,
    *,
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListFieldLevelEncryptionConfigsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFieldLevelEncryptionConfigsResultTypeDef](./type_defs.md#listfieldlevelencryptionconfigsresulttypedef)


```python
# list_field_level_encryption_configs method usage example with argument unpacking

kwargs: ListFieldLevelEncryptionConfigsRequestTypeDef = {  # (1)
    "Marker": ...,
}

parent.list_field_level_encryption_configs(**kwargs)
```

1. See [:material-code-braces: ListFieldLevelEncryptionConfigsRequestTypeDef](./type_defs.md#listfieldlevelencryptionconfigsrequesttypedef)

### list\_field\_level\_encryption\_profiles

Request a list of field-level encryption profiles that have been created in
CloudFront for this account.

Type annotations and code completion for `#!python session.client("cloudfront").list_field_level_encryption_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_field_level_encryption_profiles method definition

await def list_field_level_encryption_profiles(
    self,
    *,
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListFieldLevelEncryptionProfilesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFieldLevelEncryptionProfilesResultTypeDef](./type_defs.md#listfieldlevelencryptionprofilesresulttypedef)


```python
# list_field_level_encryption_profiles method usage example with argument unpacking

kwargs: ListFieldLevelEncryptionProfilesRequestTypeDef = {  # (1)
    "Marker": ...,
}

parent.list_field_level_encryption_profiles(**kwargs)
```

1. See [:material-code-braces: ListFieldLevelEncryptionProfilesRequestTypeDef](./type_defs.md#listfieldlevelencryptionprofilesrequesttypedef)

### list\_functions

Gets a list of all CloudFront functions in your Amazon Web Services account.

Type annotations and code completion for `#!python session.client("cloudfront").list_functions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_functions method definition

await def list_functions(
    self,
    *,
    Marker: str = ...,
    MaxItems: str = ...,
    Stage: FunctionStageType = ...,  # (1)
) -> ListFunctionsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: FunctionStageType](./literals.md#functionstagetype)
2. See [:material-code-braces: ListFunctionsResultTypeDef](./type_defs.md#listfunctionsresulttypedef)


```python
# list_functions method usage example with argument unpacking

kwargs: ListFunctionsRequestTypeDef = {  # (1)
    "Marker": ...,
}

parent.list_functions(**kwargs)
```

1. See [:material-code-braces: ListFunctionsRequestTypeDef](./type_defs.md#listfunctionsrequesttypedef)

### list\_invalidations

Lists invalidation batches.

Type annotations and code completion for `#!python session.client("cloudfront").list_invalidations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_invalidations method definition

await def list_invalidations(
    self,
    *,
    DistributionId: str,
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListInvalidationsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListInvalidationsResultTypeDef](./type_defs.md#listinvalidationsresulttypedef)


```python
# list_invalidations method usage example with argument unpacking

kwargs: ListInvalidationsRequestTypeDef = {  # (1)
    "DistributionId": ...,
}

parent.list_invalidations(**kwargs)
```

1. See [:material-code-braces: ListInvalidationsRequestTypeDef](./type_defs.md#listinvalidationsrequesttypedef)

### list\_key\_groups

Gets a list of key groups.

Type annotations and code completion for `#!python session.client("cloudfront").list_key_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_key_groups method definition

await def list_key_groups(
    self,
    *,
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListKeyGroupsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListKeyGroupsResultTypeDef](./type_defs.md#listkeygroupsresulttypedef)


```python
# list_key_groups method usage example with argument unpacking

kwargs: ListKeyGroupsRequestTypeDef = {  # (1)
    "Marker": ...,
}

parent.list_key_groups(**kwargs)
```

1. See [:material-code-braces: ListKeyGroupsRequestTypeDef](./type_defs.md#listkeygroupsrequesttypedef)

### list\_key\_value\_stores

Specifies the key value stores to list.

Type annotations and code completion for `#!python session.client("cloudfront").list_key_value_stores` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_key_value_stores method definition

await def list_key_value_stores(
    self,
    *,
    Marker: str = ...,
    MaxItems: str = ...,
    Status: str = ...,
) -> ListKeyValueStoresResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListKeyValueStoresResultTypeDef](./type_defs.md#listkeyvaluestoresresulttypedef)


```python
# list_key_value_stores method usage example with argument unpacking

kwargs: ListKeyValueStoresRequestTypeDef = {  # (1)
    "Marker": ...,
}

parent.list_key_value_stores(**kwargs)
```

1. See [:material-code-braces: ListKeyValueStoresRequestTypeDef](./type_defs.md#listkeyvaluestoresrequesttypedef)

### list\_origin\_access\_controls

Gets the list of CloudFront origin access controls (OACs) in this Amazon Web
Services account.

Type annotations and code completion for `#!python session.client("cloudfront").list_origin_access_controls` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_origin_access_controls method definition

await def list_origin_access_controls(
    self,
    *,
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListOriginAccessControlsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOriginAccessControlsResultTypeDef](./type_defs.md#listoriginaccesscontrolsresulttypedef)


```python
# list_origin_access_controls method usage example with argument unpacking

kwargs: ListOriginAccessControlsRequestTypeDef = {  # (1)
    "Marker": ...,
}

parent.list_origin_access_controls(**kwargs)
```

1. See [:material-code-braces: ListOriginAccessControlsRequestTypeDef](./type_defs.md#listoriginaccesscontrolsrequesttypedef)

### list\_origin\_request\_policies

Gets a list of origin request policies.

Type annotations and code completion for `#!python session.client("cloudfront").list_origin_request_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_origin_request_policies method definition

await def list_origin_request_policies(
    self,
    *,
    Type: OriginRequestPolicyTypeType = ...,  # (1)
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListOriginRequestPoliciesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OriginRequestPolicyTypeType](./literals.md#originrequestpolicytypetype)
2. See [:material-code-braces: ListOriginRequestPoliciesResultTypeDef](./type_defs.md#listoriginrequestpoliciesresulttypedef)


```python
# list_origin_request_policies method usage example with argument unpacking

kwargs: ListOriginRequestPoliciesRequestTypeDef = {  # (1)
    "Type": ...,
}

parent.list_origin_request_policies(**kwargs)
```

1. See [:material-code-braces: ListOriginRequestPoliciesRequestTypeDef](./type_defs.md#listoriginrequestpoliciesrequesttypedef)

### list\_public\_keys

List all public keys that have been added to CloudFront for this account.

Type annotations and code completion for `#!python session.client("cloudfront").list_public_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_public_keys method definition

await def list_public_keys(
    self,
    *,
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListPublicKeysResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPublicKeysResultTypeDef](./type_defs.md#listpublickeysresulttypedef)


```python
# list_public_keys method usage example with argument unpacking

kwargs: ListPublicKeysRequestTypeDef = {  # (1)
    "Marker": ...,
}

parent.list_public_keys(**kwargs)
```

1. See [:material-code-braces: ListPublicKeysRequestTypeDef](./type_defs.md#listpublickeysrequesttypedef)

### list\_realtime\_log\_configs

Gets a list of real-time log configurations.

Type annotations and code completion for `#!python session.client("cloudfront").list_realtime_log_configs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_realtime_log_configs method definition

await def list_realtime_log_configs(
    self,
    *,
    MaxItems: str = ...,
    Marker: str = ...,
) -> ListRealtimeLogConfigsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRealtimeLogConfigsResultTypeDef](./type_defs.md#listrealtimelogconfigsresulttypedef)


```python
# list_realtime_log_configs method usage example with argument unpacking

kwargs: ListRealtimeLogConfigsRequestTypeDef = {  # (1)
    "MaxItems": ...,
}

parent.list_realtime_log_configs(**kwargs)
```

1. See [:material-code-braces: ListRealtimeLogConfigsRequestTypeDef](./type_defs.md#listrealtimelogconfigsrequesttypedef)

### list\_response\_headers\_policies

Gets a list of response headers policies.

Type annotations and code completion for `#!python session.client("cloudfront").list_response_headers_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_response_headers_policies method definition

await def list_response_headers_policies(
    self,
    *,
    Type: ResponseHeadersPolicyTypeType = ...,  # (1)
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListResponseHeadersPoliciesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResponseHeadersPolicyTypeType](./literals.md#responseheaderspolicytypetype)
2. See [:material-code-braces: ListResponseHeadersPoliciesResultTypeDef](./type_defs.md#listresponseheaderspoliciesresulttypedef)


```python
# list_response_headers_policies method usage example with argument unpacking

kwargs: ListResponseHeadersPoliciesRequestTypeDef = {  # (1)
    "Type": ...,
}

parent.list_response_headers_policies(**kwargs)
```

1. See [:material-code-braces: ListResponseHeadersPoliciesRequestTypeDef](./type_defs.md#listresponseheaderspoliciesrequesttypedef)

### list\_streaming\_distributions

List streaming distributions.

Type annotations and code completion for `#!python session.client("cloudfront").list_streaming_distributions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_streaming_distributions method definition

await def list_streaming_distributions(
    self,
    *,
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListStreamingDistributionsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStreamingDistributionsResultTypeDef](./type_defs.md#liststreamingdistributionsresulttypedef)


```python
# list_streaming_distributions method usage example with argument unpacking

kwargs: ListStreamingDistributionsRequestTypeDef = {  # (1)
    "Marker": ...,
}

parent.list_streaming_distributions(**kwargs)
```

1. See [:material-code-braces: ListStreamingDistributionsRequestTypeDef](./type_defs.md#liststreamingdistributionsrequesttypedef)

### list\_tags\_for\_resource

List tags for a CloudFront resource.

Type annotations and code completion for `#!python session.client("cloudfront").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    Resource: str,
) -> ListTagsForResourceResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef)


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "Resource": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)

### list\_vpc\_origins

List the CloudFront VPC origins in your account.

Type annotations and code completion for `#!python session.client("cloudfront").list_vpc_origins` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# list_vpc_origins method definition

await def list_vpc_origins(
    self,
    *,
    Marker: str = ...,
    MaxItems: str = ...,
) -> ListVpcOriginsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVpcOriginsResultTypeDef](./type_defs.md#listvpcoriginsresulttypedef)


```python
# list_vpc_origins method usage example with argument unpacking

kwargs: ListVpcOriginsRequestTypeDef = {  # (1)
    "Marker": ...,
}

parent.list_vpc_origins(**kwargs)
```

1. See [:material-code-braces: ListVpcOriginsRequestTypeDef](./type_defs.md#listvpcoriginsrequesttypedef)

### publish\_function

Publishes a CloudFront function by copying the function code from the
<code>DEVELOPMENT</code> stage to <code>LIVE</code>.

Type annotations and code completion for `#!python session.client("cloudfront").publish_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# publish_function method definition

await def publish_function(
    self,
    *,
    Name: str,
    IfMatch: str,
) -> PublishFunctionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PublishFunctionResultTypeDef](./type_defs.md#publishfunctionresulttypedef)


```python
# publish_function method usage example with argument unpacking

kwargs: PublishFunctionRequestTypeDef = {  # (1)
    "Name": ...,
    "IfMatch": ...,
}

parent.publish_function(**kwargs)
```

1. See [:material-code-braces: PublishFunctionRequestTypeDef](./type_defs.md#publishfunctionrequesttypedef)

### tag\_resource

Add tags to a CloudFront resource.

Type annotations and code completion for `#!python session.client("cloudfront").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    Resource: str,
    Tags: TagsUnionTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagsUnionTypeDef](#tagsuniontypedef)
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "Resource": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)

### test\_function

Tests a CloudFront function.

Type annotations and code completion for `#!python session.client("cloudfront").test_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# test_function method definition

await def test_function(
    self,
    *,
    Name: str,
    IfMatch: str,
    EventObject: BlobTypeDef,
    Stage: FunctionStageType = ...,  # (1)
) -> TestFunctionResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: FunctionStageType](./literals.md#functionstagetype)
2. See [:material-code-braces: TestFunctionResultTypeDef](./type_defs.md#testfunctionresulttypedef)


```python
# test_function method usage example with argument unpacking

kwargs: TestFunctionRequestTypeDef = {  # (1)
    "Name": ...,
    "IfMatch": ...,
    "EventObject": ...,
}

parent.test_function(**kwargs)
```

1. See [:material-code-braces: TestFunctionRequestTypeDef](./type_defs.md#testfunctionrequesttypedef)

### untag\_resource

Remove tags from a CloudFront resource.

Type annotations and code completion for `#!python session.client("cloudfront").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    Resource: str,
    TagKeys: TagKeysTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagKeysTypeDef](./type_defs.md#tagkeystypedef)
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "Resource": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)

### update\_cache\_policy

Updates a cache policy configuration.

Type annotations and code completion for `#!python session.client("cloudfront").update_cache_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# update_cache_policy method definition

await def update_cache_policy(
    self,
    *,
    CachePolicyConfig: CachePolicyConfigUnionTypeDef,  # (1)
    Id: str,
    IfMatch: str = ...,
) -> UpdateCachePolicyResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CachePolicyConfigUnionTypeDef](#cachepolicyconfiguniontypedef)
2. See [:material-code-braces: UpdateCachePolicyResultTypeDef](./type_defs.md#updatecachepolicyresulttypedef)


```python
# update_cache_policy method usage example with argument unpacking

kwargs: UpdateCachePolicyRequestTypeDef = {  # (1)
    "CachePolicyConfig": ...,
    "Id": ...,
}

parent.update_cache_policy(**kwargs)
```

1. See [:material-code-braces: UpdateCachePolicyRequestTypeDef](./type_defs.md#updatecachepolicyrequesttypedef)

### update\_cloud\_front\_origin\_access\_identity

Update an origin access identity.

Type annotations and code completion for `#!python session.client("cloudfront").update_cloud_front_origin_access_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# update_cloud_front_origin_access_identity method definition

await def update_cloud_front_origin_access_identity(
    self,
    *,
    CloudFrontOriginAccessIdentityConfig: CloudFrontOriginAccessIdentityConfigTypeDef,  # (1)
    Id: str,
    IfMatch: str = ...,
) -> UpdateCloudFrontOriginAccessIdentityResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CloudFrontOriginAccessIdentityConfigTypeDef](./type_defs.md#cloudfrontoriginaccessidentityconfigtypedef)
2. See [:material-code-braces: UpdateCloudFrontOriginAccessIdentityResultTypeDef](./type_defs.md#updatecloudfrontoriginaccessidentityresulttypedef)


```python
# update_cloud_front_origin_access_identity method usage example with argument unpacking

kwargs: UpdateCloudFrontOriginAccessIdentityRequestTypeDef = {  # (1)
    "CloudFrontOriginAccessIdentityConfig": ...,
    "Id": ...,
}

parent.update_cloud_front_origin_access_identity(**kwargs)
```

1. See [:material-code-braces: UpdateCloudFrontOriginAccessIdentityRequestTypeDef](./type_defs.md#updatecloudfrontoriginaccessidentityrequesttypedef)

### update\_continuous\_deployment\_policy

Updates a continuous deployment policy.

Type annotations and code completion for `#!python session.client("cloudfront").update_continuous_deployment_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# update_continuous_deployment_policy method definition

await def update_continuous_deployment_policy(
    self,
    *,
    ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigUnionTypeDef,  # (1)
    Id: str,
    IfMatch: str = ...,
) -> UpdateContinuousDeploymentPolicyResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ContinuousDeploymentPolicyConfigUnionTypeDef](#continuousdeploymentpolicyconfiguniontypedef)
2. See [:material-code-braces: UpdateContinuousDeploymentPolicyResultTypeDef](./type_defs.md#updatecontinuousdeploymentpolicyresulttypedef)


```python
# update_continuous_deployment_policy method usage example with argument unpacking

kwargs: UpdateContinuousDeploymentPolicyRequestTypeDef = {  # (1)
    "ContinuousDeploymentPolicyConfig": ...,
    "Id": ...,
}

parent.update_continuous_deployment_policy(**kwargs)
```

1. See [:material-code-braces: UpdateContinuousDeploymentPolicyRequestTypeDef](./type_defs.md#updatecontinuousdeploymentpolicyrequesttypedef)

### update\_distribution

Updates the configuration for a CloudFront distribution.

Type annotations and code completion for `#!python session.client("cloudfront").update_distribution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# update_distribution method definition

await def update_distribution(
    self,
    *,
    DistributionConfig: DistributionConfigUnionTypeDef,  # (1)
    Id: str,
    IfMatch: str = ...,
) -> UpdateDistributionResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DistributionConfigUnionTypeDef](#distributionconfiguniontypedef)
2. See [:material-code-braces: UpdateDistributionResultTypeDef](./type_defs.md#updatedistributionresulttypedef)


```python
# update_distribution method usage example with argument unpacking

kwargs: UpdateDistributionRequestTypeDef = {  # (1)
    "DistributionConfig": ...,
    "Id": ...,
}

parent.update_distribution(**kwargs)
```

1. See [:material-code-braces: UpdateDistributionRequestTypeDef](./type_defs.md#updatedistributionrequesttypedef)

### update\_distribution\_with\_staging\_config

Copies the staging distribution's configuration to its corresponding primary
distribution.

Type annotations and code completion for `#!python session.client("cloudfront").update_distribution_with_staging_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# update_distribution_with_staging_config method definition

await def update_distribution_with_staging_config(
    self,
    *,
    Id: str,
    StagingDistributionId: str = ...,
    IfMatch: str = ...,
) -> UpdateDistributionWithStagingConfigResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateDistributionWithStagingConfigResultTypeDef](./type_defs.md#updatedistributionwithstagingconfigresulttypedef)


```python
# update_distribution_with_staging_config method usage example with argument unpacking

kwargs: UpdateDistributionWithStagingConfigRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.update_distribution_with_staging_config(**kwargs)
```

1. See [:material-code-braces: UpdateDistributionWithStagingConfigRequestTypeDef](./type_defs.md#updatedistributionwithstagingconfigrequesttypedef)

### update\_field\_level\_encryption\_config

Update a field-level encryption configuration.

Type annotations and code completion for `#!python session.client("cloudfront").update_field_level_encryption_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# update_field_level_encryption_config method definition

await def update_field_level_encryption_config(
    self,
    *,
    FieldLevelEncryptionConfig: FieldLevelEncryptionConfigUnionTypeDef,  # (1)
    Id: str,
    IfMatch: str = ...,
) -> UpdateFieldLevelEncryptionConfigResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FieldLevelEncryptionConfigUnionTypeDef](#fieldlevelencryptionconfiguniontypedef)
2. See [:material-code-braces: UpdateFieldLevelEncryptionConfigResultTypeDef](./type_defs.md#updatefieldlevelencryptionconfigresulttypedef)


```python
# update_field_level_encryption_config method usage example with argument unpacking

kwargs: UpdateFieldLevelEncryptionConfigRequestTypeDef = {  # (1)
    "FieldLevelEncryptionConfig": ...,
    "Id": ...,
}

parent.update_field_level_encryption_config(**kwargs)
```

1. See [:material-code-braces: UpdateFieldLevelEncryptionConfigRequestTypeDef](./type_defs.md#updatefieldlevelencryptionconfigrequesttypedef)

### update\_field\_level\_encryption\_profile

Update a field-level encryption profile.

Type annotations and code completion for `#!python session.client("cloudfront").update_field_level_encryption_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# update_field_level_encryption_profile method definition

await def update_field_level_encryption_profile(
    self,
    *,
    FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigUnionTypeDef,  # (1)
    Id: str,
    IfMatch: str = ...,
) -> UpdateFieldLevelEncryptionProfileResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FieldLevelEncryptionProfileConfigUnionTypeDef](#fieldlevelencryptionprofileconfiguniontypedef)
2. See [:material-code-braces: UpdateFieldLevelEncryptionProfileResultTypeDef](./type_defs.md#updatefieldlevelencryptionprofileresulttypedef)


```python
# update_field_level_encryption_profile method usage example with argument unpacking

kwargs: UpdateFieldLevelEncryptionProfileRequestTypeDef = {  # (1)
    "FieldLevelEncryptionProfileConfig": ...,
    "Id": ...,
}

parent.update_field_level_encryption_profile(**kwargs)
```

1. See [:material-code-braces: UpdateFieldLevelEncryptionProfileRequestTypeDef](./type_defs.md#updatefieldlevelencryptionprofilerequesttypedef)

### update\_function

Updates a CloudFront function.

Type annotations and code completion for `#!python session.client("cloudfront").update_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# update_function method definition

await def update_function(
    self,
    *,
    Name: str,
    IfMatch: str,
    FunctionConfig: FunctionConfigUnionTypeDef,  # (1)
    FunctionCode: BlobTypeDef,
) -> UpdateFunctionResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FunctionConfigUnionTypeDef](#functionconfiguniontypedef)
2. See [:material-code-braces: UpdateFunctionResultTypeDef](./type_defs.md#updatefunctionresulttypedef)


```python
# update_function method usage example with argument unpacking

kwargs: UpdateFunctionRequestTypeDef = {  # (1)
    "Name": ...,
    "IfMatch": ...,
    "FunctionConfig": ...,
    "FunctionCode": ...,
}

parent.update_function(**kwargs)
```

1. See [:material-code-braces: UpdateFunctionRequestTypeDef](./type_defs.md#updatefunctionrequesttypedef)

### update\_key\_group

Updates a key group.

Type annotations and code completion for `#!python session.client("cloudfront").update_key_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# update_key_group method definition

await def update_key_group(
    self,
    *,
    KeyGroupConfig: KeyGroupConfigUnionTypeDef,  # (1)
    Id: str,
    IfMatch: str = ...,
) -> UpdateKeyGroupResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: KeyGroupConfigUnionTypeDef](#keygroupconfiguniontypedef)
2. See [:material-code-braces: UpdateKeyGroupResultTypeDef](./type_defs.md#updatekeygroupresulttypedef)


```python
# update_key_group method usage example with argument unpacking

kwargs: UpdateKeyGroupRequestTypeDef = {  # (1)
    "KeyGroupConfig": ...,
    "Id": ...,
}

parent.update_key_group(**kwargs)
```

1. See [:material-code-braces: UpdateKeyGroupRequestTypeDef](./type_defs.md#updatekeygrouprequesttypedef)

### update\_key\_value\_store

Specifies the key value store to update.

Type annotations and code completion for `#!python session.client("cloudfront").update_key_value_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# update_key_value_store method definition

await def update_key_value_store(
    self,
    *,
    Name: str,
    Comment: str,
    IfMatch: str,
) -> UpdateKeyValueStoreResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateKeyValueStoreResultTypeDef](./type_defs.md#updatekeyvaluestoreresulttypedef)


```python
# update_key_value_store method usage example with argument unpacking

kwargs: UpdateKeyValueStoreRequestTypeDef = {  # (1)
    "Name": ...,
    "Comment": ...,
    "IfMatch": ...,
}

parent.update_key_value_store(**kwargs)
```

1. See [:material-code-braces: UpdateKeyValueStoreRequestTypeDef](./type_defs.md#updatekeyvaluestorerequesttypedef)

### update\_origin\_access\_control

Updates a CloudFront origin access control.

Type annotations and code completion for `#!python session.client("cloudfront").update_origin_access_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# update_origin_access_control method definition

await def update_origin_access_control(
    self,
    *,
    OriginAccessControlConfig: OriginAccessControlConfigTypeDef,  # (1)
    Id: str,
    IfMatch: str = ...,
) -> UpdateOriginAccessControlResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OriginAccessControlConfigTypeDef](./type_defs.md#originaccesscontrolconfigtypedef)
2. See [:material-code-braces: UpdateOriginAccessControlResultTypeDef](./type_defs.md#updateoriginaccesscontrolresulttypedef)


```python
# update_origin_access_control method usage example with argument unpacking

kwargs: UpdateOriginAccessControlRequestTypeDef = {  # (1)
    "OriginAccessControlConfig": ...,
    "Id": ...,
}

parent.update_origin_access_control(**kwargs)
```

1. See [:material-code-braces: UpdateOriginAccessControlRequestTypeDef](./type_defs.md#updateoriginaccesscontrolrequesttypedef)

### update\_origin\_request\_policy

Updates an origin request policy configuration.

Type annotations and code completion for `#!python session.client("cloudfront").update_origin_request_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# update_origin_request_policy method definition

await def update_origin_request_policy(
    self,
    *,
    OriginRequestPolicyConfig: OriginRequestPolicyConfigUnionTypeDef,  # (1)
    Id: str,
    IfMatch: str = ...,
) -> UpdateOriginRequestPolicyResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OriginRequestPolicyConfigUnionTypeDef](#originrequestpolicyconfiguniontypedef)
2. See [:material-code-braces: UpdateOriginRequestPolicyResultTypeDef](./type_defs.md#updateoriginrequestpolicyresulttypedef)


```python
# update_origin_request_policy method usage example with argument unpacking

kwargs: UpdateOriginRequestPolicyRequestTypeDef = {  # (1)
    "OriginRequestPolicyConfig": ...,
    "Id": ...,
}

parent.update_origin_request_policy(**kwargs)
```

1. See [:material-code-braces: UpdateOriginRequestPolicyRequestTypeDef](./type_defs.md#updateoriginrequestpolicyrequesttypedef)

### update\_public\_key

Update public key information.

Type annotations and code completion for `#!python session.client("cloudfront").update_public_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# update_public_key method definition

await def update_public_key(
    self,
    *,
    PublicKeyConfig: PublicKeyConfigTypeDef,  # (1)
    Id: str,
    IfMatch: str = ...,
) -> UpdatePublicKeyResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PublicKeyConfigTypeDef](./type_defs.md#publickeyconfigtypedef)
2. See [:material-code-braces: UpdatePublicKeyResultTypeDef](./type_defs.md#updatepublickeyresulttypedef)


```python
# update_public_key method usage example with argument unpacking

kwargs: UpdatePublicKeyRequestTypeDef = {  # (1)
    "PublicKeyConfig": ...,
    "Id": ...,
}

parent.update_public_key(**kwargs)
```

1. See [:material-code-braces: UpdatePublicKeyRequestTypeDef](./type_defs.md#updatepublickeyrequesttypedef)

### update\_realtime\_log\_config

Updates a real-time log configuration.

Type annotations and code completion for `#!python session.client("cloudfront").update_realtime_log_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# update_realtime_log_config method definition

await def update_realtime_log_config(
    self,
    *,
    EndPoints: Sequence[EndPointTypeDef] = ...,  # (1)
    Fields: Sequence[str] = ...,
    Name: str = ...,
    ARN: str = ...,
    SamplingRate: int = ...,
) -> UpdateRealtimeLogConfigResultTypeDef:  # (2)
    ...
```

1. See `Sequence[EndPointTypeDef]`
2. See [:material-code-braces: UpdateRealtimeLogConfigResultTypeDef](./type_defs.md#updaterealtimelogconfigresulttypedef)


```python
# update_realtime_log_config method usage example with argument unpacking

kwargs: UpdateRealtimeLogConfigRequestTypeDef = {  # (1)
    "EndPoints": ...,
}

parent.update_realtime_log_config(**kwargs)
```

1. See [:material-code-braces: UpdateRealtimeLogConfigRequestTypeDef](./type_defs.md#updaterealtimelogconfigrequesttypedef)

### update\_response\_headers\_policy

Updates a response headers policy.

Type annotations and code completion for `#!python session.client("cloudfront").update_response_headers_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# update_response_headers_policy method definition

await def update_response_headers_policy(
    self,
    *,
    ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigUnionTypeDef,  # (1)
    Id: str,
    IfMatch: str = ...,
) -> UpdateResponseHeadersPolicyResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ResponseHeadersPolicyConfigUnionTypeDef](#responseheaderspolicyconfiguniontypedef)
2. See [:material-code-braces: UpdateResponseHeadersPolicyResultTypeDef](./type_defs.md#updateresponseheaderspolicyresulttypedef)


```python
# update_response_headers_policy method usage example with argument unpacking

kwargs: UpdateResponseHeadersPolicyRequestTypeDef = {  # (1)
    "ResponseHeadersPolicyConfig": ...,
    "Id": ...,
}

parent.update_response_headers_policy(**kwargs)
```

1. See [:material-code-braces: UpdateResponseHeadersPolicyRequestTypeDef](./type_defs.md#updateresponseheaderspolicyrequesttypedef)

### update\_streaming\_distribution

Update a streaming distribution.

Type annotations and code completion for `#!python session.client("cloudfront").update_streaming_distribution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# update_streaming_distribution method definition

await def update_streaming_distribution(
    self,
    *,
    StreamingDistributionConfig: StreamingDistributionConfigUnionTypeDef,  # (1)
    Id: str,
    IfMatch: str = ...,
) -> UpdateStreamingDistributionResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StreamingDistributionConfigUnionTypeDef](#streamingdistributionconfiguniontypedef)
2. See [:material-code-braces: UpdateStreamingDistributionResultTypeDef](./type_defs.md#updatestreamingdistributionresulttypedef)


```python
# update_streaming_distribution method usage example with argument unpacking

kwargs: UpdateStreamingDistributionRequestTypeDef = {  # (1)
    "StreamingDistributionConfig": ...,
    "Id": ...,
}

parent.update_streaming_distribution(**kwargs)
```

1. See [:material-code-braces: UpdateStreamingDistributionRequestTypeDef](./type_defs.md#updatestreamingdistributionrequesttypedef)

### update\_vpc\_origin

Update an Amazon CloudFront VPC origin in your account.

Type annotations and code completion for `#!python session.client("cloudfront").update_vpc_origin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# update_vpc_origin method definition

await def update_vpc_origin(
    self,
    *,
    VpcOriginEndpointConfig: VpcOriginEndpointConfigUnionTypeDef,  # (1)
    Id: str,
    IfMatch: str,
) -> UpdateVpcOriginResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VpcOriginEndpointConfigUnionTypeDef](#vpcoriginendpointconfiguniontypedef)
2. See [:material-code-braces: UpdateVpcOriginResultTypeDef](./type_defs.md#updatevpcoriginresulttypedef)


```python
# update_vpc_origin method usage example with argument unpacking

kwargs: UpdateVpcOriginRequestTypeDef = {  # (1)
    "VpcOriginEndpointConfig": ...,
    "Id": ...,
    "IfMatch": ...,
}

parent.update_vpc_origin(**kwargs)
```

1. See [:material-code-braces: UpdateVpcOriginRequestTypeDef](./type_defs.md#updatevpcoriginrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("cloudfront").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("cloudfront").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("cloudfront").get_paginator` method with overloads.

- `client.get_paginator("list_cloud_front_origin_access_identities")` -> [ListCloudFrontOriginAccessIdentitiesPaginator](./paginators.md#listcloudfrontoriginaccessidentitiespaginator)
- `client.get_paginator("list_distributions")` -> [ListDistributionsPaginator](./paginators.md#listdistributionspaginator)
- `client.get_paginator("list_invalidations")` -> [ListInvalidationsPaginator](./paginators.md#listinvalidationspaginator)
- `client.get_paginator("list_key_value_stores")` -> [ListKeyValueStoresPaginator](./paginators.md#listkeyvaluestorespaginator)
- `client.get_paginator("list_public_keys")` -> [ListPublicKeysPaginator](./paginators.md#listpublickeyspaginator)
- `client.get_paginator("list_streaming_distributions")` -> [ListStreamingDistributionsPaginator](./paginators.md#liststreamingdistributionspaginator)




### get_waiter

Type annotations and code completion for `#!python session.client("cloudfront").get_waiter` method with overloads.

- `client.get_waiter("distribution_deployed")` -> [DistributionDeployedWaiter](./waiters.md#distributiondeployedwaiter)
- `client.get_waiter("invalidation_completed")` -> [InvalidationCompletedWaiter](./waiters.md#invalidationcompletedwaiter)
- `client.get_waiter("streaming_distribution_deployed")` -> [StreamingDistributionDeployedWaiter](./waiters.md#streamingdistributiondeployedwaiter)

