# ComputeOptimizerClient

> [Index](../README.md) > [ComputeOptimizer](./README.md) > ComputeOptimizerClient

!!! note ""

    Auto-generated documentation for [ComputeOptimizer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#computeoptimizer)
    type annotations stubs module [types-aiobotocore-compute-optimizer](https://pypi.org/project/types-aiobotocore-compute-optimizer/).

## ComputeOptimizerClient

Type annotations and code completion for `#!python session.client("compute-optimizer")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# ComputeOptimizerClient usage example

from aioboto3.session import Session
from types_aiobotocore_compute_optimizer.client import ComputeOptimizerClient

session = Session()
async with session.client("compute-optimizer") as client:
    client: ComputeOptimizerClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("compute-optimizer").exceptions` structure.

```python
# ComputeOptimizerClient.exceptions usage example

async with session.client("compute-optimizer") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.InternalServerException,
        client.exceptions.InvalidParameterValueException,
        client.exceptions.LimitExceededException,
        client.exceptions.MissingAuthenticationToken,
        client.exceptions.OptInRequiredException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceUnavailableException,
        client.exceptions.ThrottlingException,
    ) as e:
        print(e)
```

```python
# ComputeOptimizerClient.exceptions type checking example

from types_aiobotocore_compute_optimizer.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("compute-optimizer").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("compute-optimizer").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

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


### delete\_recommendation\_preferences

Deletes a recommendation preference, such as enhanced infrastructure metrics.

Type annotations and code completion for `#!python session.client("compute-optimizer").delete_recommendation_preferences` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# delete_recommendation_preferences method definition

await def delete_recommendation_preferences(
    self,
    *,
    resourceType: ResourceTypeType,  # (1)
    recommendationPreferenceNames: Sequence[RecommendationPreferenceNameType],  # (2)
    scope: ScopeTypeDef = ...,  # (3)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: RecommendationPreferenceNameType](./literals.md#recommendationpreferencenametype) 
3. See [:material-code-braces: ScopeTypeDef](./type_defs.md#scopetypedef) 


```python
# delete_recommendation_preferences method usage example with argument unpacking

kwargs: DeleteRecommendationPreferencesRequestRequestTypeDef = {  # (1)
    "resourceType": ...,
    "recommendationPreferenceNames": ...,
}

parent.delete_recommendation_preferences(**kwargs)
```

1. See [:material-code-braces: DeleteRecommendationPreferencesRequestRequestTypeDef](./type_defs.md#deleterecommendationpreferencesrequestrequesttypedef) 

### describe\_recommendation\_export\_jobs

Describes recommendation export jobs created in the last seven days.

Type annotations and code completion for `#!python session.client("compute-optimizer").describe_recommendation_export_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# describe_recommendation_export_jobs method definition

await def describe_recommendation_export_jobs(
    self,
    *,
    jobIds: Sequence[str] = ...,
    filters: Sequence[JobFilterTypeDef] = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> DescribeRecommendationExportJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: JobFilterTypeDef](./type_defs.md#jobfiltertypedef) 
2. See [:material-code-braces: DescribeRecommendationExportJobsResponseTypeDef](./type_defs.md#describerecommendationexportjobsresponsetypedef) 


```python
# describe_recommendation_export_jobs method usage example with argument unpacking

kwargs: DescribeRecommendationExportJobsRequestRequestTypeDef = {  # (1)
    "jobIds": ...,
}

parent.describe_recommendation_export_jobs(**kwargs)
```

1. See [:material-code-braces: DescribeRecommendationExportJobsRequestRequestTypeDef](./type_defs.md#describerecommendationexportjobsrequestrequesttypedef) 

### export\_auto\_scaling\_group\_recommendations

Exports optimization recommendations for Auto Scaling groups.

Type annotations and code completion for `#!python session.client("compute-optimizer").export_auto_scaling_group_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# export_auto_scaling_group_recommendations method definition

await def export_auto_scaling_group_recommendations(
    self,
    *,
    s3DestinationConfig: S3DestinationConfigTypeDef,  # (1)
    accountIds: Sequence[str] = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (2)
    fieldsToExport: Sequence[ExportableAutoScalingGroupFieldType] = ...,  # (3)
    fileFormat: FileFormatType = ...,  # (4)
    includeMemberAccounts: bool = ...,
    recommendationPreferences: RecommendationPreferencesTypeDef = ...,  # (5)
) -> ExportAutoScalingGroupRecommendationsResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-brackets: ExportableAutoScalingGroupFieldType](./literals.md#exportableautoscalinggroupfieldtype) 
4. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
5. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
6. See [:material-code-braces: ExportAutoScalingGroupRecommendationsResponseTypeDef](./type_defs.md#exportautoscalinggrouprecommendationsresponsetypedef) 


```python
# export_auto_scaling_group_recommendations method usage example with argument unpacking

kwargs: ExportAutoScalingGroupRecommendationsRequestRequestTypeDef = {  # (1)
    "s3DestinationConfig": ...,
}

parent.export_auto_scaling_group_recommendations(**kwargs)
```

1. See [:material-code-braces: ExportAutoScalingGroupRecommendationsRequestRequestTypeDef](./type_defs.md#exportautoscalinggrouprecommendationsrequestrequesttypedef) 

### export\_ebs\_volume\_recommendations

Exports optimization recommendations for Amazon EBS volumes.

Type annotations and code completion for `#!python session.client("compute-optimizer").export_ebs_volume_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# export_ebs_volume_recommendations method definition

await def export_ebs_volume_recommendations(
    self,
    *,
    s3DestinationConfig: S3DestinationConfigTypeDef,  # (1)
    accountIds: Sequence[str] = ...,
    filters: Sequence[EBSFilterTypeDef] = ...,  # (2)
    fieldsToExport: Sequence[ExportableVolumeFieldType] = ...,  # (3)
    fileFormat: FileFormatType = ...,  # (4)
    includeMemberAccounts: bool = ...,
) -> ExportEBSVolumeRecommendationsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
2. See [:material-code-braces: EBSFilterTypeDef](./type_defs.md#ebsfiltertypedef) 
3. See [:material-code-brackets: ExportableVolumeFieldType](./literals.md#exportablevolumefieldtype) 
4. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
5. See [:material-code-braces: ExportEBSVolumeRecommendationsResponseTypeDef](./type_defs.md#exportebsvolumerecommendationsresponsetypedef) 


```python
# export_ebs_volume_recommendations method usage example with argument unpacking

kwargs: ExportEBSVolumeRecommendationsRequestRequestTypeDef = {  # (1)
    "s3DestinationConfig": ...,
}

parent.export_ebs_volume_recommendations(**kwargs)
```

1. See [:material-code-braces: ExportEBSVolumeRecommendationsRequestRequestTypeDef](./type_defs.md#exportebsvolumerecommendationsrequestrequesttypedef) 

### export\_ec2\_instance\_recommendations

Exports optimization recommendations for Amazon EC2 instances.

Type annotations and code completion for `#!python session.client("compute-optimizer").export_ec2_instance_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# export_ec2_instance_recommendations method definition

await def export_ec2_instance_recommendations(
    self,
    *,
    s3DestinationConfig: S3DestinationConfigTypeDef,  # (1)
    accountIds: Sequence[str] = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (2)
    fieldsToExport: Sequence[ExportableInstanceFieldType] = ...,  # (3)
    fileFormat: FileFormatType = ...,  # (4)
    includeMemberAccounts: bool = ...,
    recommendationPreferences: RecommendationPreferencesTypeDef = ...,  # (5)
) -> ExportEC2InstanceRecommendationsResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-brackets: ExportableInstanceFieldType](./literals.md#exportableinstancefieldtype) 
4. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
5. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
6. See [:material-code-braces: ExportEC2InstanceRecommendationsResponseTypeDef](./type_defs.md#exportec2instancerecommendationsresponsetypedef) 


```python
# export_ec2_instance_recommendations method usage example with argument unpacking

kwargs: ExportEC2InstanceRecommendationsRequestRequestTypeDef = {  # (1)
    "s3DestinationConfig": ...,
}

parent.export_ec2_instance_recommendations(**kwargs)
```

1. See [:material-code-braces: ExportEC2InstanceRecommendationsRequestRequestTypeDef](./type_defs.md#exportec2instancerecommendationsrequestrequesttypedef) 

### export\_ecs\_service\_recommendations

Exports optimization recommendations for Amazon ECS services on Fargate.

Type annotations and code completion for `#!python session.client("compute-optimizer").export_ecs_service_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# export_ecs_service_recommendations method definition

await def export_ecs_service_recommendations(
    self,
    *,
    s3DestinationConfig: S3DestinationConfigTypeDef,  # (1)
    accountIds: Sequence[str] = ...,
    filters: Sequence[ECSServiceRecommendationFilterTypeDef] = ...,  # (2)
    fieldsToExport: Sequence[ExportableECSServiceFieldType] = ...,  # (3)
    fileFormat: FileFormatType = ...,  # (4)
    includeMemberAccounts: bool = ...,
) -> ExportECSServiceRecommendationsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
2. See [:material-code-braces: ECSServiceRecommendationFilterTypeDef](./type_defs.md#ecsservicerecommendationfiltertypedef) 
3. See [:material-code-brackets: ExportableECSServiceFieldType](./literals.md#exportableecsservicefieldtype) 
4. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
5. See [:material-code-braces: ExportECSServiceRecommendationsResponseTypeDef](./type_defs.md#exportecsservicerecommendationsresponsetypedef) 


```python
# export_ecs_service_recommendations method usage example with argument unpacking

kwargs: ExportECSServiceRecommendationsRequestRequestTypeDef = {  # (1)
    "s3DestinationConfig": ...,
}

parent.export_ecs_service_recommendations(**kwargs)
```

1. See [:material-code-braces: ExportECSServiceRecommendationsRequestRequestTypeDef](./type_defs.md#exportecsservicerecommendationsrequestrequesttypedef) 

### export\_idle\_recommendations

Export optimization recommendations for your idle resources.

Type annotations and code completion for `#!python session.client("compute-optimizer").export_idle_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# export_idle_recommendations method definition

await def export_idle_recommendations(
    self,
    *,
    s3DestinationConfig: S3DestinationConfigTypeDef,  # (1)
    accountIds: Sequence[str] = ...,
    filters: Sequence[IdleRecommendationFilterTypeDef] = ...,  # (2)
    fieldsToExport: Sequence[ExportableIdleFieldType] = ...,  # (3)
    fileFormat: FileFormatType = ...,  # (4)
    includeMemberAccounts: bool = ...,
) -> ExportIdleRecommendationsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
2. See [:material-code-braces: IdleRecommendationFilterTypeDef](./type_defs.md#idlerecommendationfiltertypedef) 
3. See [:material-code-brackets: ExportableIdleFieldType](./literals.md#exportableidlefieldtype) 
4. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
5. See [:material-code-braces: ExportIdleRecommendationsResponseTypeDef](./type_defs.md#exportidlerecommendationsresponsetypedef) 


```python
# export_idle_recommendations method usage example with argument unpacking

kwargs: ExportIdleRecommendationsRequestRequestTypeDef = {  # (1)
    "s3DestinationConfig": ...,
}

parent.export_idle_recommendations(**kwargs)
```

1. See [:material-code-braces: ExportIdleRecommendationsRequestRequestTypeDef](./type_defs.md#exportidlerecommendationsrequestrequesttypedef) 

### export\_lambda\_function\_recommendations

Exports optimization recommendations for Lambda functions.

Type annotations and code completion for `#!python session.client("compute-optimizer").export_lambda_function_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# export_lambda_function_recommendations method definition

await def export_lambda_function_recommendations(
    self,
    *,
    s3DestinationConfig: S3DestinationConfigTypeDef,  # (1)
    accountIds: Sequence[str] = ...,
    filters: Sequence[LambdaFunctionRecommendationFilterTypeDef] = ...,  # (2)
    fieldsToExport: Sequence[ExportableLambdaFunctionFieldType] = ...,  # (3)
    fileFormat: FileFormatType = ...,  # (4)
    includeMemberAccounts: bool = ...,
) -> ExportLambdaFunctionRecommendationsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
2. See [:material-code-braces: LambdaFunctionRecommendationFilterTypeDef](./type_defs.md#lambdafunctionrecommendationfiltertypedef) 
3. See [:material-code-brackets: ExportableLambdaFunctionFieldType](./literals.md#exportablelambdafunctionfieldtype) 
4. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
5. See [:material-code-braces: ExportLambdaFunctionRecommendationsResponseTypeDef](./type_defs.md#exportlambdafunctionrecommendationsresponsetypedef) 


```python
# export_lambda_function_recommendations method usage example with argument unpacking

kwargs: ExportLambdaFunctionRecommendationsRequestRequestTypeDef = {  # (1)
    "s3DestinationConfig": ...,
}

parent.export_lambda_function_recommendations(**kwargs)
```

1. See [:material-code-braces: ExportLambdaFunctionRecommendationsRequestRequestTypeDef](./type_defs.md#exportlambdafunctionrecommendationsrequestrequesttypedef) 

### export\_license\_recommendations

Export optimization recommendations for your licenses.

Type annotations and code completion for `#!python session.client("compute-optimizer").export_license_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# export_license_recommendations method definition

await def export_license_recommendations(
    self,
    *,
    s3DestinationConfig: S3DestinationConfigTypeDef,  # (1)
    accountIds: Sequence[str] = ...,
    filters: Sequence[LicenseRecommendationFilterTypeDef] = ...,  # (2)
    fieldsToExport: Sequence[ExportableLicenseFieldType] = ...,  # (3)
    fileFormat: FileFormatType = ...,  # (4)
    includeMemberAccounts: bool = ...,
) -> ExportLicenseRecommendationsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
2. See [:material-code-braces: LicenseRecommendationFilterTypeDef](./type_defs.md#licenserecommendationfiltertypedef) 
3. See [:material-code-brackets: ExportableLicenseFieldType](./literals.md#exportablelicensefieldtype) 
4. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
5. See [:material-code-braces: ExportLicenseRecommendationsResponseTypeDef](./type_defs.md#exportlicenserecommendationsresponsetypedef) 


```python
# export_license_recommendations method usage example with argument unpacking

kwargs: ExportLicenseRecommendationsRequestRequestTypeDef = {  # (1)
    "s3DestinationConfig": ...,
}

parent.export_license_recommendations(**kwargs)
```

1. See [:material-code-braces: ExportLicenseRecommendationsRequestRequestTypeDef](./type_defs.md#exportlicenserecommendationsrequestrequesttypedef) 

### export\_rds\_database\_recommendations

Export optimization recommendations for your Amazon Relational Database Service
(Amazon RDS).

Type annotations and code completion for `#!python session.client("compute-optimizer").export_rds_database_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# export_rds_database_recommendations method definition

await def export_rds_database_recommendations(
    self,
    *,
    s3DestinationConfig: S3DestinationConfigTypeDef,  # (1)
    accountIds: Sequence[str] = ...,
    filters: Sequence[RDSDBRecommendationFilterTypeDef] = ...,  # (2)
    fieldsToExport: Sequence[ExportableRDSDBFieldType] = ...,  # (3)
    fileFormat: FileFormatType = ...,  # (4)
    includeMemberAccounts: bool = ...,
    recommendationPreferences: RecommendationPreferencesTypeDef = ...,  # (5)
) -> ExportRDSDatabaseRecommendationsResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
2. See [:material-code-braces: RDSDBRecommendationFilterTypeDef](./type_defs.md#rdsdbrecommendationfiltertypedef) 
3. See [:material-code-brackets: ExportableRDSDBFieldType](./literals.md#exportablerdsdbfieldtype) 
4. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
5. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
6. See [:material-code-braces: ExportRDSDatabaseRecommendationsResponseTypeDef](./type_defs.md#exportrdsdatabaserecommendationsresponsetypedef) 


```python
# export_rds_database_recommendations method usage example with argument unpacking

kwargs: ExportRDSDatabaseRecommendationsRequestRequestTypeDef = {  # (1)
    "s3DestinationConfig": ...,
}

parent.export_rds_database_recommendations(**kwargs)
```

1. See [:material-code-braces: ExportRDSDatabaseRecommendationsRequestRequestTypeDef](./type_defs.md#exportrdsdatabaserecommendationsrequestrequesttypedef) 

### get\_auto\_scaling\_group\_recommendations

Returns Auto Scaling group recommendations.

Type annotations and code completion for `#!python session.client("compute-optimizer").get_auto_scaling_group_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# get_auto_scaling_group_recommendations method definition

await def get_auto_scaling_group_recommendations(
    self,
    *,
    accountIds: Sequence[str] = ...,
    autoScalingGroupArns: Sequence[str] = ...,
    nextToken: str = ...,
    maxResults: int = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    recommendationPreferences: RecommendationPreferencesTypeDef = ...,  # (2)
) -> GetAutoScalingGroupRecommendationsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
3. See [:material-code-braces: GetAutoScalingGroupRecommendationsResponseTypeDef](./type_defs.md#getautoscalinggrouprecommendationsresponsetypedef) 


```python
# get_auto_scaling_group_recommendations method usage example with argument unpacking

kwargs: GetAutoScalingGroupRecommendationsRequestRequestTypeDef = {  # (1)
    "accountIds": ...,
}

parent.get_auto_scaling_group_recommendations(**kwargs)
```

1. See [:material-code-braces: GetAutoScalingGroupRecommendationsRequestRequestTypeDef](./type_defs.md#getautoscalinggrouprecommendationsrequestrequesttypedef) 

### get\_ebs\_volume\_recommendations

Returns Amazon Elastic Block Store (Amazon EBS) volume recommendations.

Type annotations and code completion for `#!python session.client("compute-optimizer").get_ebs_volume_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# get_ebs_volume_recommendations method definition

await def get_ebs_volume_recommendations(
    self,
    *,
    volumeArns: Sequence[str] = ...,
    nextToken: str = ...,
    maxResults: int = ...,
    filters: Sequence[EBSFilterTypeDef] = ...,  # (1)
    accountIds: Sequence[str] = ...,
) -> GetEBSVolumeRecommendationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EBSFilterTypeDef](./type_defs.md#ebsfiltertypedef) 
2. See [:material-code-braces: GetEBSVolumeRecommendationsResponseTypeDef](./type_defs.md#getebsvolumerecommendationsresponsetypedef) 


```python
# get_ebs_volume_recommendations method usage example with argument unpacking

kwargs: GetEBSVolumeRecommendationsRequestRequestTypeDef = {  # (1)
    "volumeArns": ...,
}

parent.get_ebs_volume_recommendations(**kwargs)
```

1. See [:material-code-braces: GetEBSVolumeRecommendationsRequestRequestTypeDef](./type_defs.md#getebsvolumerecommendationsrequestrequesttypedef) 

### get\_ec2\_instance\_recommendations

Returns Amazon EC2 instance recommendations.

Type annotations and code completion for `#!python session.client("compute-optimizer").get_ec2_instance_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# get_ec2_instance_recommendations method definition

await def get_ec2_instance_recommendations(
    self,
    *,
    instanceArns: Sequence[str] = ...,
    nextToken: str = ...,
    maxResults: int = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    accountIds: Sequence[str] = ...,
    recommendationPreferences: RecommendationPreferencesTypeDef = ...,  # (2)
) -> GetEC2InstanceRecommendationsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
3. See [:material-code-braces: GetEC2InstanceRecommendationsResponseTypeDef](./type_defs.md#getec2instancerecommendationsresponsetypedef) 


```python
# get_ec2_instance_recommendations method usage example with argument unpacking

kwargs: GetEC2InstanceRecommendationsRequestRequestTypeDef = {  # (1)
    "instanceArns": ...,
}

parent.get_ec2_instance_recommendations(**kwargs)
```

1. See [:material-code-braces: GetEC2InstanceRecommendationsRequestRequestTypeDef](./type_defs.md#getec2instancerecommendationsrequestrequesttypedef) 

### get\_ec2\_recommendation\_projected\_metrics

Returns the projected utilization metrics of Amazon EC2 instance
recommendations.

Type annotations and code completion for `#!python session.client("compute-optimizer").get_ec2_recommendation_projected_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# get_ec2_recommendation_projected_metrics method definition

await def get_ec2_recommendation_projected_metrics(
    self,
    *,
    instanceArn: str,
    stat: MetricStatisticType,  # (1)
    period: int,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    recommendationPreferences: RecommendationPreferencesTypeDef = ...,  # (2)
) -> GetEC2RecommendationProjectedMetricsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
2. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
3. See [:material-code-braces: GetEC2RecommendationProjectedMetricsResponseTypeDef](./type_defs.md#getec2recommendationprojectedmetricsresponsetypedef) 


```python
# get_ec2_recommendation_projected_metrics method usage example with argument unpacking

kwargs: GetEC2RecommendationProjectedMetricsRequestRequestTypeDef = {  # (1)
    "instanceArn": ...,
    "stat": ...,
    "period": ...,
    "startTime": ...,
    "endTime": ...,
}

parent.get_ec2_recommendation_projected_metrics(**kwargs)
```

1. See [:material-code-braces: GetEC2RecommendationProjectedMetricsRequestRequestTypeDef](./type_defs.md#getec2recommendationprojectedmetricsrequestrequesttypedef) 

### get\_ecs\_service\_recommendation\_projected\_metrics

Returns the projected metrics of Amazon ECS service recommendations.

Type annotations and code completion for `#!python session.client("compute-optimizer").get_ecs_service_recommendation_projected_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# get_ecs_service_recommendation_projected_metrics method definition

await def get_ecs_service_recommendation_projected_metrics(
    self,
    *,
    serviceArn: str,
    stat: MetricStatisticType,  # (1)
    period: int,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
) -> GetECSServiceRecommendationProjectedMetricsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
2. See [:material-code-braces: GetECSServiceRecommendationProjectedMetricsResponseTypeDef](./type_defs.md#getecsservicerecommendationprojectedmetricsresponsetypedef) 


```python
# get_ecs_service_recommendation_projected_metrics method usage example with argument unpacking

kwargs: GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef = {  # (1)
    "serviceArn": ...,
    "stat": ...,
    "period": ...,
    "startTime": ...,
    "endTime": ...,
}

parent.get_ecs_service_recommendation_projected_metrics(**kwargs)
```

1. See [:material-code-braces: GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef](./type_defs.md#getecsservicerecommendationprojectedmetricsrequestrequesttypedef) 

### get\_ecs\_service\_recommendations

Returns Amazon ECS service recommendations.

Type annotations and code completion for `#!python session.client("compute-optimizer").get_ecs_service_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# get_ecs_service_recommendations method definition

await def get_ecs_service_recommendations(
    self,
    *,
    serviceArns: Sequence[str] = ...,
    nextToken: str = ...,
    maxResults: int = ...,
    filters: Sequence[ECSServiceRecommendationFilterTypeDef] = ...,  # (1)
    accountIds: Sequence[str] = ...,
) -> GetECSServiceRecommendationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ECSServiceRecommendationFilterTypeDef](./type_defs.md#ecsservicerecommendationfiltertypedef) 
2. See [:material-code-braces: GetECSServiceRecommendationsResponseTypeDef](./type_defs.md#getecsservicerecommendationsresponsetypedef) 


```python
# get_ecs_service_recommendations method usage example with argument unpacking

kwargs: GetECSServiceRecommendationsRequestRequestTypeDef = {  # (1)
    "serviceArns": ...,
}

parent.get_ecs_service_recommendations(**kwargs)
```

1. See [:material-code-braces: GetECSServiceRecommendationsRequestRequestTypeDef](./type_defs.md#getecsservicerecommendationsrequestrequesttypedef) 

### get\_effective\_recommendation\_preferences

Returns the recommendation preferences that are in effect for a given resource,
such as enhanced infrastructure metrics.

Type annotations and code completion for `#!python session.client("compute-optimizer").get_effective_recommendation_preferences` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# get_effective_recommendation_preferences method definition

await def get_effective_recommendation_preferences(
    self,
    *,
    resourceArn: str,
) -> GetEffectiveRecommendationPreferencesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEffectiveRecommendationPreferencesResponseTypeDef](./type_defs.md#geteffectiverecommendationpreferencesresponsetypedef) 


```python
# get_effective_recommendation_preferences method usage example with argument unpacking

kwargs: GetEffectiveRecommendationPreferencesRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.get_effective_recommendation_preferences(**kwargs)
```

1. See [:material-code-braces: GetEffectiveRecommendationPreferencesRequestRequestTypeDef](./type_defs.md#geteffectiverecommendationpreferencesrequestrequesttypedef) 

### get\_enrollment\_status

Returns the enrollment (opt in) status of an account to the Compute Optimizer
service.

Type annotations and code completion for `#!python session.client("compute-optimizer").get_enrollment_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# get_enrollment_status method definition

await def get_enrollment_status(
    self,
) -> GetEnrollmentStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEnrollmentStatusResponseTypeDef](./type_defs.md#getenrollmentstatusresponsetypedef) 

### get\_enrollment\_statuses\_for\_organization

Returns the Compute Optimizer enrollment (opt-in) status of organization member
accounts, if your account is an organization management account.

Type annotations and code completion for `#!python session.client("compute-optimizer").get_enrollment_statuses_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# get_enrollment_statuses_for_organization method definition

await def get_enrollment_statuses_for_organization(
    self,
    *,
    filters: Sequence[EnrollmentFilterTypeDef] = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> GetEnrollmentStatusesForOrganizationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EnrollmentFilterTypeDef](./type_defs.md#enrollmentfiltertypedef) 
2. See [:material-code-braces: GetEnrollmentStatusesForOrganizationResponseTypeDef](./type_defs.md#getenrollmentstatusesfororganizationresponsetypedef) 


```python
# get_enrollment_statuses_for_organization method usage example with argument unpacking

kwargs: GetEnrollmentStatusesForOrganizationRequestRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.get_enrollment_statuses_for_organization(**kwargs)
```

1. See [:material-code-braces: GetEnrollmentStatusesForOrganizationRequestRequestTypeDef](./type_defs.md#getenrollmentstatusesfororganizationrequestrequesttypedef) 

### get\_idle\_recommendations

Returns idle resource recommendations.

Type annotations and code completion for `#!python session.client("compute-optimizer").get_idle_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# get_idle_recommendations method definition

await def get_idle_recommendations(
    self,
    *,
    resourceArns: Sequence[str] = ...,
    nextToken: str = ...,
    maxResults: int = ...,
    filters: Sequence[IdleRecommendationFilterTypeDef] = ...,  # (1)
    accountIds: Sequence[str] = ...,
    orderBy: OrderByTypeDef = ...,  # (2)
) -> GetIdleRecommendationsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: IdleRecommendationFilterTypeDef](./type_defs.md#idlerecommendationfiltertypedef) 
2. See [:material-code-braces: OrderByTypeDef](./type_defs.md#orderbytypedef) 
3. See [:material-code-braces: GetIdleRecommendationsResponseTypeDef](./type_defs.md#getidlerecommendationsresponsetypedef) 


```python
# get_idle_recommendations method usage example with argument unpacking

kwargs: GetIdleRecommendationsRequestRequestTypeDef = {  # (1)
    "resourceArns": ...,
}

parent.get_idle_recommendations(**kwargs)
```

1. See [:material-code-braces: GetIdleRecommendationsRequestRequestTypeDef](./type_defs.md#getidlerecommendationsrequestrequesttypedef) 

### get\_lambda\_function\_recommendations

Returns Lambda function recommendations.

Type annotations and code completion for `#!python session.client("compute-optimizer").get_lambda_function_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# get_lambda_function_recommendations method definition

await def get_lambda_function_recommendations(
    self,
    *,
    functionArns: Sequence[str] = ...,
    accountIds: Sequence[str] = ...,
    filters: Sequence[LambdaFunctionRecommendationFilterTypeDef] = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> GetLambdaFunctionRecommendationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LambdaFunctionRecommendationFilterTypeDef](./type_defs.md#lambdafunctionrecommendationfiltertypedef) 
2. See [:material-code-braces: GetLambdaFunctionRecommendationsResponseTypeDef](./type_defs.md#getlambdafunctionrecommendationsresponsetypedef) 


```python
# get_lambda_function_recommendations method usage example with argument unpacking

kwargs: GetLambdaFunctionRecommendationsRequestRequestTypeDef = {  # (1)
    "functionArns": ...,
}

parent.get_lambda_function_recommendations(**kwargs)
```

1. See [:material-code-braces: GetLambdaFunctionRecommendationsRequestRequestTypeDef](./type_defs.md#getlambdafunctionrecommendationsrequestrequesttypedef) 

### get\_license\_recommendations

Returns license recommendations for Amazon EC2 instances that run on a specific
license.

Type annotations and code completion for `#!python session.client("compute-optimizer").get_license_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# get_license_recommendations method definition

await def get_license_recommendations(
    self,
    *,
    resourceArns: Sequence[str] = ...,
    nextToken: str = ...,
    maxResults: int = ...,
    filters: Sequence[LicenseRecommendationFilterTypeDef] = ...,  # (1)
    accountIds: Sequence[str] = ...,
) -> GetLicenseRecommendationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LicenseRecommendationFilterTypeDef](./type_defs.md#licenserecommendationfiltertypedef) 
2. See [:material-code-braces: GetLicenseRecommendationsResponseTypeDef](./type_defs.md#getlicenserecommendationsresponsetypedef) 


```python
# get_license_recommendations method usage example with argument unpacking

kwargs: GetLicenseRecommendationsRequestRequestTypeDef = {  # (1)
    "resourceArns": ...,
}

parent.get_license_recommendations(**kwargs)
```

1. See [:material-code-braces: GetLicenseRecommendationsRequestRequestTypeDef](./type_defs.md#getlicenserecommendationsrequestrequesttypedef) 

### get\_rds\_database\_recommendation\_projected\_metrics

Returns the projected metrics of Amazon RDS recommendations.

Type annotations and code completion for `#!python session.client("compute-optimizer").get_rds_database_recommendation_projected_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# get_rds_database_recommendation_projected_metrics method definition

await def get_rds_database_recommendation_projected_metrics(
    self,
    *,
    resourceArn: str,
    stat: MetricStatisticType,  # (1)
    period: int,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    recommendationPreferences: RecommendationPreferencesTypeDef = ...,  # (2)
) -> GetRDSDatabaseRecommendationProjectedMetricsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
2. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
3. See [:material-code-braces: GetRDSDatabaseRecommendationProjectedMetricsResponseTypeDef](./type_defs.md#getrdsdatabaserecommendationprojectedmetricsresponsetypedef) 


```python
# get_rds_database_recommendation_projected_metrics method usage example with argument unpacking

kwargs: GetRDSDatabaseRecommendationProjectedMetricsRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "stat": ...,
    "period": ...,
    "startTime": ...,
    "endTime": ...,
}

parent.get_rds_database_recommendation_projected_metrics(**kwargs)
```

1. See [:material-code-braces: GetRDSDatabaseRecommendationProjectedMetricsRequestRequestTypeDef](./type_defs.md#getrdsdatabaserecommendationprojectedmetricsrequestrequesttypedef) 

### get\_rds\_database\_recommendations

Returns Amazon RDS recommendations.

Type annotations and code completion for `#!python session.client("compute-optimizer").get_rds_database_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# get_rds_database_recommendations method definition

await def get_rds_database_recommendations(
    self,
    *,
    resourceArns: Sequence[str] = ...,
    nextToken: str = ...,
    maxResults: int = ...,
    filters: Sequence[RDSDBRecommendationFilterTypeDef] = ...,  # (1)
    accountIds: Sequence[str] = ...,
    recommendationPreferences: RecommendationPreferencesTypeDef = ...,  # (2)
) -> GetRDSDatabaseRecommendationsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RDSDBRecommendationFilterTypeDef](./type_defs.md#rdsdbrecommendationfiltertypedef) 
2. See [:material-code-braces: RecommendationPreferencesTypeDef](./type_defs.md#recommendationpreferencestypedef) 
3. See [:material-code-braces: GetRDSDatabaseRecommendationsResponseTypeDef](./type_defs.md#getrdsdatabaserecommendationsresponsetypedef) 


```python
# get_rds_database_recommendations method usage example with argument unpacking

kwargs: GetRDSDatabaseRecommendationsRequestRequestTypeDef = {  # (1)
    "resourceArns": ...,
}

parent.get_rds_database_recommendations(**kwargs)
```

1. See [:material-code-braces: GetRDSDatabaseRecommendationsRequestRequestTypeDef](./type_defs.md#getrdsdatabaserecommendationsrequestrequesttypedef) 

### get\_recommendation\_preferences

Returns existing recommendation preferences, such as enhanced infrastructure
metrics.

Type annotations and code completion for `#!python session.client("compute-optimizer").get_recommendation_preferences` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# get_recommendation_preferences method definition

await def get_recommendation_preferences(
    self,
    *,
    resourceType: ResourceTypeType,  # (1)
    scope: ScopeTypeDef = ...,  # (2)
    nextToken: str = ...,
    maxResults: int = ...,
) -> GetRecommendationPreferencesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ScopeTypeDef](./type_defs.md#scopetypedef) 
3. See [:material-code-braces: GetRecommendationPreferencesResponseTypeDef](./type_defs.md#getrecommendationpreferencesresponsetypedef) 


```python
# get_recommendation_preferences method usage example with argument unpacking

kwargs: GetRecommendationPreferencesRequestRequestTypeDef = {  # (1)
    "resourceType": ...,
}

parent.get_recommendation_preferences(**kwargs)
```

1. See [:material-code-braces: GetRecommendationPreferencesRequestRequestTypeDef](./type_defs.md#getrecommendationpreferencesrequestrequesttypedef) 

### get\_recommendation\_summaries

Returns the optimization findings for an account.

Type annotations and code completion for `#!python session.client("compute-optimizer").get_recommendation_summaries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# get_recommendation_summaries method definition

await def get_recommendation_summaries(
    self,
    *,
    accountIds: Sequence[str] = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> GetRecommendationSummariesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRecommendationSummariesResponseTypeDef](./type_defs.md#getrecommendationsummariesresponsetypedef) 


```python
# get_recommendation_summaries method usage example with argument unpacking

kwargs: GetRecommendationSummariesRequestRequestTypeDef = {  # (1)
    "accountIds": ...,
}

parent.get_recommendation_summaries(**kwargs)
```

1. See [:material-code-braces: GetRecommendationSummariesRequestRequestTypeDef](./type_defs.md#getrecommendationsummariesrequestrequesttypedef) 

### put\_recommendation\_preferences

Creates a new recommendation preference or updates an existing recommendation
preference, such as enhanced infrastructure metrics.

Type annotations and code completion for `#!python session.client("compute-optimizer").put_recommendation_preferences` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# put_recommendation_preferences method definition

await def put_recommendation_preferences(
    self,
    *,
    resourceType: ResourceTypeType,  # (1)
    scope: ScopeTypeDef = ...,  # (2)
    enhancedInfrastructureMetrics: EnhancedInfrastructureMetricsType = ...,  # (3)
    inferredWorkloadTypes: InferredWorkloadTypesPreferenceType = ...,  # (4)
    externalMetricsPreference: ExternalMetricsPreferenceTypeDef = ...,  # (5)
    lookBackPeriod: LookBackPeriodPreferenceType = ...,  # (6)
    utilizationPreferences: Sequence[UtilizationPreferenceTypeDef] = ...,  # (7)
    preferredResources: Sequence[PreferredResourceTypeDef] = ...,  # (8)
    savingsEstimationMode: SavingsEstimationModeType = ...,  # (9)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ScopeTypeDef](./type_defs.md#scopetypedef) 
3. See [:material-code-brackets: EnhancedInfrastructureMetricsType](./literals.md#enhancedinfrastructuremetricstype) 
4. See [:material-code-brackets: InferredWorkloadTypesPreferenceType](./literals.md#inferredworkloadtypespreferencetype) 
5. See [:material-code-braces: ExternalMetricsPreferenceTypeDef](./type_defs.md#externalmetricspreferencetypedef) 
6. See [:material-code-brackets: LookBackPeriodPreferenceType](./literals.md#lookbackperiodpreferencetype) 
7. See [:material-code-braces: UtilizationPreferenceTypeDef](./type_defs.md#utilizationpreferencetypedef) 
8. See [:material-code-braces: PreferredResourceTypeDef](./type_defs.md#preferredresourcetypedef) 
9. See [:material-code-brackets: SavingsEstimationModeType](./literals.md#savingsestimationmodetype) 


```python
# put_recommendation_preferences method usage example with argument unpacking

kwargs: PutRecommendationPreferencesRequestRequestTypeDef = {  # (1)
    "resourceType": ...,
}

parent.put_recommendation_preferences(**kwargs)
```

1. See [:material-code-braces: PutRecommendationPreferencesRequestRequestTypeDef](./type_defs.md#putrecommendationpreferencesrequestrequesttypedef) 

### update\_enrollment\_status

Updates the enrollment (opt in and opt out) status of an account to the Compute
Optimizer service.

Type annotations and code completion for `#!python session.client("compute-optimizer").update_enrollment_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# update_enrollment_status method definition

await def update_enrollment_status(
    self,
    *,
    status: StatusType,  # (1)
    includeMemberAccounts: bool = ...,
) -> UpdateEnrollmentStatusResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: UpdateEnrollmentStatusResponseTypeDef](./type_defs.md#updateenrollmentstatusresponsetypedef) 


```python
# update_enrollment_status method usage example with argument unpacking

kwargs: UpdateEnrollmentStatusRequestRequestTypeDef = {  # (1)
    "status": ...,
}

parent.update_enrollment_status(**kwargs)
```

1. See [:material-code-braces: UpdateEnrollmentStatusRequestRequestTypeDef](./type_defs.md#updateenrollmentstatusrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("compute-optimizer").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("compute-optimizer").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)

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

Type annotations and code completion for `#!python session.client("compute-optimizer").get_paginator` method with overloads.

- `client.get_paginator("describe_recommendation_export_jobs")` -> [DescribeRecommendationExportJobsPaginator](./paginators.md#describerecommendationexportjobspaginator)
- `client.get_paginator("get_enrollment_statuses_for_organization")` -> [GetEnrollmentStatusesForOrganizationPaginator](./paginators.md#getenrollmentstatusesfororganizationpaginator)
- `client.get_paginator("get_lambda_function_recommendations")` -> [GetLambdaFunctionRecommendationsPaginator](./paginators.md#getlambdafunctionrecommendationspaginator)
- `client.get_paginator("get_recommendation_preferences")` -> [GetRecommendationPreferencesPaginator](./paginators.md#getrecommendationpreferencespaginator)
- `client.get_paginator("get_recommendation_summaries")` -> [GetRecommendationSummariesPaginator](./paginators.md#getrecommendationsummariespaginator)


