# LambdaClient

> [Index](../README.md) > [Lambda](./README.md) > LambdaClient

!!! note ""

    Auto-generated documentation for [Lambda](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#lambda)
    type annotations stubs module [types-aiobotocore-lambda](https://pypi.org/project/types-aiobotocore-lambda/).

## LambdaClient

Type annotations and code completion for `#!python session.client("lambda")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# LambdaClient usage example

from aioboto3.session import Session
from types_aiobotocore_lambda.client import LambdaClient

session = Session()
async with session.client("lambda") as client:
    client: LambdaClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("lambda").exceptions` structure.

```python
# LambdaClient.exceptions usage example

async with session.client("lambda") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.CodeSigningConfigNotFoundException,
        client.exceptions.CodeStorageExceededException,
        client.exceptions.CodeVerificationFailedException,
        client.exceptions.EC2AccessDeniedException,
        client.exceptions.EC2ThrottledException,
        client.exceptions.EC2UnexpectedException,
        client.exceptions.EFSIOException,
        client.exceptions.EFSMountConnectivityException,
        client.exceptions.EFSMountFailureException,
        client.exceptions.EFSMountTimeoutException,
        client.exceptions.ENILimitReachedException,
        client.exceptions.InvalidCodeSignatureException,
        client.exceptions.InvalidParameterValueException,
        client.exceptions.InvalidRequestContentException,
        client.exceptions.InvalidRuntimeException,
        client.exceptions.InvalidSecurityGroupIDException,
        client.exceptions.InvalidSubnetIDException,
        client.exceptions.InvalidZipFileException,
        client.exceptions.KMSAccessDeniedException,
        client.exceptions.KMSDisabledException,
        client.exceptions.KMSInvalidStateException,
        client.exceptions.KMSNotFoundException,
        client.exceptions.PolicyLengthExceededException,
        client.exceptions.PreconditionFailedException,
        client.exceptions.ProvisionedConcurrencyConfigNotFoundException,
        client.exceptions.RecursiveInvocationException,
        client.exceptions.RequestTooLargeException,
        client.exceptions.ResourceConflictException,
        client.exceptions.ResourceInUseException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ResourceNotReadyException,
        client.exceptions.ServiceException,
        client.exceptions.SnapStartException,
        client.exceptions.SnapStartNotReadyException,
        client.exceptions.SnapStartTimeoutException,
        client.exceptions.SubnetIPAddressLimitReachedException,
        client.exceptions.TooManyRequestsException,
        client.exceptions.UnsupportedMediaTypeException,
    ) as e:
        print(e)
```

```python
# LambdaClient.exceptions type checking example

from types_aiobotocore_lambda.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("lambda").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("lambda").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

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


### add\_layer\_version\_permission

Adds permissions to the resource-based policy of a version of an <a
href="https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html">Lambda
layer</a>.

Type annotations and code completion for `#!python session.client("lambda").add_layer_version_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# add_layer_version_permission method definition

await def add_layer_version_permission(
    self,
    *,
    LayerName: str,
    VersionNumber: int,
    StatementId: str,
    Action: str,
    Principal: str,
    OrganizationId: str = ...,
    RevisionId: str = ...,
) -> AddLayerVersionPermissionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AddLayerVersionPermissionResponseTypeDef](./type_defs.md#addlayerversionpermissionresponsetypedef) 


```python
# add_layer_version_permission method usage example with argument unpacking

kwargs: AddLayerVersionPermissionRequestRequestTypeDef = {  # (1)
    "LayerName": ...,
    "VersionNumber": ...,
    "StatementId": ...,
    "Action": ...,
    "Principal": ...,
}

parent.add_layer_version_permission(**kwargs)
```

1. See [:material-code-braces: AddLayerVersionPermissionRequestRequestTypeDef](./type_defs.md#addlayerversionpermissionrequestrequesttypedef) 

### add\_permission

Grants a <a
href="https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_elements_principal.html#Principal_specifying">principal</a>
permission to use a function.

Type annotations and code completion for `#!python session.client("lambda").add_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# add_permission method definition

await def add_permission(
    self,
    *,
    FunctionName: str,
    StatementId: str,
    Action: str,
    Principal: str,
    SourceArn: str = ...,
    SourceAccount: str = ...,
    EventSourceToken: str = ...,
    Qualifier: str = ...,
    RevisionId: str = ...,
    PrincipalOrgID: str = ...,
    FunctionUrlAuthType: FunctionUrlAuthTypeType = ...,  # (1)
) -> AddPermissionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: FunctionUrlAuthTypeType](./literals.md#functionurlauthtypetype) 
2. See [:material-code-braces: AddPermissionResponseTypeDef](./type_defs.md#addpermissionresponsetypedef) 


```python
# add_permission method usage example with argument unpacking

kwargs: AddPermissionRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
    "StatementId": ...,
    "Action": ...,
    "Principal": ...,
}

parent.add_permission(**kwargs)
```

1. See [:material-code-braces: AddPermissionRequestRequestTypeDef](./type_defs.md#addpermissionrequestrequesttypedef) 

### create\_alias

Creates an <a
href="https://docs.aws.amazon.com/lambda/latest/dg/configuration-aliases.html">alias</a>
for a Lambda function version.

Type annotations and code completion for `#!python session.client("lambda").create_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# create_alias method definition

await def create_alias(
    self,
    *,
    FunctionName: str,
    Name: str,
    FunctionVersion: str,
    Description: str = ...,
    RoutingConfig: AliasRoutingConfigurationTypeDef = ...,  # (1)
) -> AliasConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AliasRoutingConfigurationTypeDef](./type_defs.md#aliasroutingconfigurationtypedef) 
2. See [:material-code-braces: AliasConfigurationResponseTypeDef](./type_defs.md#aliasconfigurationresponsetypedef) 


```python
# create_alias method usage example with argument unpacking

kwargs: CreateAliasRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
    "Name": ...,
    "FunctionVersion": ...,
}

parent.create_alias(**kwargs)
```

1. See [:material-code-braces: CreateAliasRequestRequestTypeDef](./type_defs.md#createaliasrequestrequesttypedef) 

### create\_code\_signing\_config

Creates a code signing configuration.

Type annotations and code completion for `#!python session.client("lambda").create_code_signing_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# create_code_signing_config method definition

await def create_code_signing_config(
    self,
    *,
    AllowedPublishers: AllowedPublishersTypeDef,  # (1)
    Description: str = ...,
    CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...,  # (2)
    Tags: Mapping[str, str] = ...,
) -> CreateCodeSigningConfigResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AllowedPublishersTypeDef](./type_defs.md#allowedpublisherstypedef) 
2. See [:material-code-braces: CodeSigningPoliciesTypeDef](./type_defs.md#codesigningpoliciestypedef) 
3. See [:material-code-braces: CreateCodeSigningConfigResponseTypeDef](./type_defs.md#createcodesigningconfigresponsetypedef) 


```python
# create_code_signing_config method usage example with argument unpacking

kwargs: CreateCodeSigningConfigRequestRequestTypeDef = {  # (1)
    "AllowedPublishers": ...,
}

parent.create_code_signing_config(**kwargs)
```

1. See [:material-code-braces: CreateCodeSigningConfigRequestRequestTypeDef](./type_defs.md#createcodesigningconfigrequestrequesttypedef) 

### create\_event\_source\_mapping

Creates a mapping between an event source and an Lambda function.

Type annotations and code completion for `#!python session.client("lambda").create_event_source_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# create_event_source_mapping method definition

await def create_event_source_mapping(
    self,
    *,
    FunctionName: str,
    EventSourceArn: str = ...,
    Enabled: bool = ...,
    BatchSize: int = ...,
    FilterCriteria: FilterCriteriaTypeDef = ...,  # (1)
    MaximumBatchingWindowInSeconds: int = ...,
    ParallelizationFactor: int = ...,
    StartingPosition: EventSourcePositionType = ...,  # (2)
    StartingPositionTimestamp: TimestampTypeDef = ...,
    DestinationConfig: DestinationConfigTypeDef = ...,  # (3)
    MaximumRecordAgeInSeconds: int = ...,
    BisectBatchOnFunctionError: bool = ...,
    MaximumRetryAttempts: int = ...,
    Tags: Mapping[str, str] = ...,
    TumblingWindowInSeconds: int = ...,
    Topics: Sequence[str] = ...,
    Queues: Sequence[str] = ...,
    SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,  # (4)
    SelfManagedEventSource: SelfManagedEventSourceTypeDef = ...,  # (5)
    FunctionResponseTypes: Sequence[FunctionResponseTypeType] = ...,  # (6)
    AmazonManagedKafkaEventSourceConfig: AmazonManagedKafkaEventSourceConfigTypeDef = ...,  # (7)
    SelfManagedKafkaEventSourceConfig: SelfManagedKafkaEventSourceConfigTypeDef = ...,  # (8)
    ScalingConfig: ScalingConfigTypeDef = ...,  # (9)
    DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...,  # (10)
    KMSKeyArn: str = ...,
    MetricsConfig: EventSourceMappingMetricsConfigTypeDef = ...,  # (11)
    ProvisionedPollerConfig: ProvisionedPollerConfigTypeDef = ...,  # (12)
) -> EventSourceMappingConfigurationResponseTypeDef:  # (13)
    ...
```

1. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
2. See [:material-code-brackets: EventSourcePositionType](./literals.md#eventsourcepositiontype) 
3. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
4. See [:material-code-braces: SourceAccessConfigurationTypeDef](./type_defs.md#sourceaccessconfigurationtypedef) 
5. See [:material-code-braces: SelfManagedEventSourceTypeDef](./type_defs.md#selfmanagedeventsourcetypedef) 
6. See [:material-code-brackets: FunctionResponseTypeType](./literals.md#functionresponsetypetype) 
7. See [:material-code-braces: AmazonManagedKafkaEventSourceConfigTypeDef](./type_defs.md#amazonmanagedkafkaeventsourceconfigtypedef) 
8. See [:material-code-braces: SelfManagedKafkaEventSourceConfigTypeDef](./type_defs.md#selfmanagedkafkaeventsourceconfigtypedef) 
9. See [:material-code-braces: ScalingConfigTypeDef](./type_defs.md#scalingconfigtypedef) 
10. See [:material-code-braces: DocumentDBEventSourceConfigTypeDef](./type_defs.md#documentdbeventsourceconfigtypedef) 
11. See [:material-code-braces: EventSourceMappingMetricsConfigTypeDef](./type_defs.md#eventsourcemappingmetricsconfigtypedef) 
12. See [:material-code-braces: ProvisionedPollerConfigTypeDef](./type_defs.md#provisionedpollerconfigtypedef) 
13. See [:material-code-braces: EventSourceMappingConfigurationResponseTypeDef](./type_defs.md#eventsourcemappingconfigurationresponsetypedef) 


```python
# create_event_source_mapping method usage example with argument unpacking

kwargs: CreateEventSourceMappingRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.create_event_source_mapping(**kwargs)
```

1. See [:material-code-braces: CreateEventSourceMappingRequestRequestTypeDef](./type_defs.md#createeventsourcemappingrequestrequesttypedef) 

### create\_function

Creates a Lambda function.

Type annotations and code completion for `#!python session.client("lambda").create_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# create_function method definition

await def create_function(
    self,
    *,
    FunctionName: str,
    Role: str,
    Code: FunctionCodeTypeDef,  # (1)
    Runtime: RuntimeType = ...,  # (2)
    Handler: str = ...,
    Description: str = ...,
    Timeout: int = ...,
    MemorySize: int = ...,
    Publish: bool = ...,
    VpcConfig: VpcConfigTypeDef = ...,  # (3)
    PackageType: PackageTypeType = ...,  # (4)
    DeadLetterConfig: DeadLetterConfigTypeDef = ...,  # (5)
    Environment: EnvironmentTypeDef = ...,  # (6)
    KMSKeyArn: str = ...,
    TracingConfig: TracingConfigTypeDef = ...,  # (7)
    Tags: Mapping[str, str] = ...,
    Layers: Sequence[str] = ...,
    FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,  # (8)
    ImageConfig: ImageConfigTypeDef = ...,  # (9)
    CodeSigningConfigArn: str = ...,
    Architectures: Sequence[ArchitectureType] = ...,  # (10)
    EphemeralStorage: EphemeralStorageTypeDef = ...,  # (11)
    SnapStart: SnapStartTypeDef = ...,  # (12)
    LoggingConfig: LoggingConfigTypeDef = ...,  # (13)
) -> FunctionConfigurationResponseTypeDef:  # (14)
    ...
```

1. See [:material-code-braces: FunctionCodeTypeDef](./type_defs.md#functioncodetypedef) 
2. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
3. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
4. See [:material-code-brackets: PackageTypeType](./literals.md#packagetypetype) 
5. See [:material-code-braces: DeadLetterConfigTypeDef](./type_defs.md#deadletterconfigtypedef) 
6. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
7. See [:material-code-braces: TracingConfigTypeDef](./type_defs.md#tracingconfigtypedef) 
8. See [:material-code-braces: FileSystemConfigTypeDef](./type_defs.md#filesystemconfigtypedef) 
9. See [:material-code-braces: ImageConfigTypeDef](./type_defs.md#imageconfigtypedef) 
10. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
11. See [:material-code-braces: EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef) 
12. See [:material-code-braces: SnapStartTypeDef](./type_defs.md#snapstarttypedef) 
13. See [:material-code-braces: LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef) 
14. See [:material-code-braces: FunctionConfigurationResponseTypeDef](./type_defs.md#functionconfigurationresponsetypedef) 


```python
# create_function method usage example with argument unpacking

kwargs: CreateFunctionRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
    "Role": ...,
    "Code": ...,
}

parent.create_function(**kwargs)
```

1. See [:material-code-braces: CreateFunctionRequestRequestTypeDef](./type_defs.md#createfunctionrequestrequesttypedef) 

### create\_function\_url\_config

Creates a Lambda function URL with the specified configuration parameters.

Type annotations and code completion for `#!python session.client("lambda").create_function_url_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# create_function_url_config method definition

await def create_function_url_config(
    self,
    *,
    FunctionName: str,
    AuthType: FunctionUrlAuthTypeType,  # (1)
    Qualifier: str = ...,
    Cors: CorsTypeDef = ...,  # (2)
    InvokeMode: InvokeModeType = ...,  # (3)
) -> CreateFunctionUrlConfigResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: FunctionUrlAuthTypeType](./literals.md#functionurlauthtypetype) 
2. See [:material-code-braces: CorsTypeDef](./type_defs.md#corstypedef) 
3. See [:material-code-brackets: InvokeModeType](./literals.md#invokemodetype) 
4. See [:material-code-braces: CreateFunctionUrlConfigResponseTypeDef](./type_defs.md#createfunctionurlconfigresponsetypedef) 


```python
# create_function_url_config method usage example with argument unpacking

kwargs: CreateFunctionUrlConfigRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
    "AuthType": ...,
}

parent.create_function_url_config(**kwargs)
```

1. See [:material-code-braces: CreateFunctionUrlConfigRequestRequestTypeDef](./type_defs.md#createfunctionurlconfigrequestrequesttypedef) 

### delete\_alias

Deletes a Lambda function <a
href="https://docs.aws.amazon.com/lambda/latest/dg/configuration-aliases.html">alias</a>.

Type annotations and code completion for `#!python session.client("lambda").delete_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# delete_alias method definition

await def delete_alias(
    self,
    *,
    FunctionName: str,
    Name: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_alias method usage example with argument unpacking

kwargs: DeleteAliasRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
    "Name": ...,
}

parent.delete_alias(**kwargs)
```

1. See [:material-code-braces: DeleteAliasRequestRequestTypeDef](./type_defs.md#deletealiasrequestrequesttypedef) 

### delete\_code\_signing\_config

Deletes the code signing configuration.

Type annotations and code completion for `#!python session.client("lambda").delete_code_signing_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# delete_code_signing_config method definition

await def delete_code_signing_config(
    self,
    *,
    CodeSigningConfigArn: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_code_signing_config method usage example with argument unpacking

kwargs: DeleteCodeSigningConfigRequestRequestTypeDef = {  # (1)
    "CodeSigningConfigArn": ...,
}

parent.delete_code_signing_config(**kwargs)
```

1. See [:material-code-braces: DeleteCodeSigningConfigRequestRequestTypeDef](./type_defs.md#deletecodesigningconfigrequestrequesttypedef) 

### delete\_event\_source\_mapping

Deletes an <a
href="https://docs.aws.amazon.com/lambda/latest/dg/intro-invocation-modes.html">event
source mapping</a>.

Type annotations and code completion for `#!python session.client("lambda").delete_event_source_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# delete_event_source_mapping method definition

await def delete_event_source_mapping(
    self,
    *,
    UUID: str,
) -> EventSourceMappingConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EventSourceMappingConfigurationResponseTypeDef](./type_defs.md#eventsourcemappingconfigurationresponsetypedef) 


```python
# delete_event_source_mapping method usage example with argument unpacking

kwargs: DeleteEventSourceMappingRequestRequestTypeDef = {  # (1)
    "UUID": ...,
}

parent.delete_event_source_mapping(**kwargs)
```

1. See [:material-code-braces: DeleteEventSourceMappingRequestRequestTypeDef](./type_defs.md#deleteeventsourcemappingrequestrequesttypedef) 

### delete\_function

Deletes a Lambda function.

Type annotations and code completion for `#!python session.client("lambda").delete_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# delete_function method definition

await def delete_function(
    self,
    *,
    FunctionName: str,
    Qualifier: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_function method usage example with argument unpacking

kwargs: DeleteFunctionRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.delete_function(**kwargs)
```

1. See [:material-code-braces: DeleteFunctionRequestRequestTypeDef](./type_defs.md#deletefunctionrequestrequesttypedef) 

### delete\_function\_code\_signing\_config

Removes the code signing configuration from the function.

Type annotations and code completion for `#!python session.client("lambda").delete_function_code_signing_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# delete_function_code_signing_config method definition

await def delete_function_code_signing_config(
    self,
    *,
    FunctionName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_function_code_signing_config method usage example with argument unpacking

kwargs: DeleteFunctionCodeSigningConfigRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.delete_function_code_signing_config(**kwargs)
```

1. See [:material-code-braces: DeleteFunctionCodeSigningConfigRequestRequestTypeDef](./type_defs.md#deletefunctioncodesigningconfigrequestrequesttypedef) 

### delete\_function\_concurrency

Removes a concurrent execution limit from a function.

Type annotations and code completion for `#!python session.client("lambda").delete_function_concurrency` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# delete_function_concurrency method definition

await def delete_function_concurrency(
    self,
    *,
    FunctionName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_function_concurrency method usage example with argument unpacking

kwargs: DeleteFunctionConcurrencyRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.delete_function_concurrency(**kwargs)
```

1. See [:material-code-braces: DeleteFunctionConcurrencyRequestRequestTypeDef](./type_defs.md#deletefunctionconcurrencyrequestrequesttypedef) 

### delete\_function\_event\_invoke\_config

Deletes the configuration for asynchronous invocation for a function, version,
or alias.

Type annotations and code completion for `#!python session.client("lambda").delete_function_event_invoke_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# delete_function_event_invoke_config method definition

await def delete_function_event_invoke_config(
    self,
    *,
    FunctionName: str,
    Qualifier: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_function_event_invoke_config method usage example with argument unpacking

kwargs: DeleteFunctionEventInvokeConfigRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.delete_function_event_invoke_config(**kwargs)
```

1. See [:material-code-braces: DeleteFunctionEventInvokeConfigRequestRequestTypeDef](./type_defs.md#deletefunctioneventinvokeconfigrequestrequesttypedef) 

### delete\_function\_url\_config

Deletes a Lambda function URL.

Type annotations and code completion for `#!python session.client("lambda").delete_function_url_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# delete_function_url_config method definition

await def delete_function_url_config(
    self,
    *,
    FunctionName: str,
    Qualifier: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_function_url_config method usage example with argument unpacking

kwargs: DeleteFunctionUrlConfigRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.delete_function_url_config(**kwargs)
```

1. See [:material-code-braces: DeleteFunctionUrlConfigRequestRequestTypeDef](./type_defs.md#deletefunctionurlconfigrequestrequesttypedef) 

### delete\_layer\_version

Deletes a version of an <a
href="https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html">Lambda
layer</a>.

Type annotations and code completion for `#!python session.client("lambda").delete_layer_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# delete_layer_version method definition

await def delete_layer_version(
    self,
    *,
    LayerName: str,
    VersionNumber: int,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_layer_version method usage example with argument unpacking

kwargs: DeleteLayerVersionRequestRequestTypeDef = {  # (1)
    "LayerName": ...,
    "VersionNumber": ...,
}

parent.delete_layer_version(**kwargs)
```

1. See [:material-code-braces: DeleteLayerVersionRequestRequestTypeDef](./type_defs.md#deletelayerversionrequestrequesttypedef) 

### delete\_provisioned\_concurrency\_config

Deletes the provisioned concurrency configuration for a function.

Type annotations and code completion for `#!python session.client("lambda").delete_provisioned_concurrency_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# delete_provisioned_concurrency_config method definition

await def delete_provisioned_concurrency_config(
    self,
    *,
    FunctionName: str,
    Qualifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_provisioned_concurrency_config method usage example with argument unpacking

kwargs: DeleteProvisionedConcurrencyConfigRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
    "Qualifier": ...,
}

parent.delete_provisioned_concurrency_config(**kwargs)
```

1. See [:material-code-braces: DeleteProvisionedConcurrencyConfigRequestRequestTypeDef](./type_defs.md#deleteprovisionedconcurrencyconfigrequestrequesttypedef) 

### get\_account\_settings

Retrieves details about your account's <a
href="https://docs.aws.amazon.com/lambda/latest/dg/limits.html">limits</a> and
usage in an Amazon Web Services Region.

Type annotations and code completion for `#!python session.client("lambda").get_account_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# get_account_settings method definition

await def get_account_settings(
    self,
) -> GetAccountSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccountSettingsResponseTypeDef](./type_defs.md#getaccountsettingsresponsetypedef) 

### get\_alias

Returns details about a Lambda function <a
href="https://docs.aws.amazon.com/lambda/latest/dg/configuration-aliases.html">alias</a>.

Type annotations and code completion for `#!python session.client("lambda").get_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# get_alias method definition

await def get_alias(
    self,
    *,
    FunctionName: str,
    Name: str,
) -> AliasConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AliasConfigurationResponseTypeDef](./type_defs.md#aliasconfigurationresponsetypedef) 


```python
# get_alias method usage example with argument unpacking

kwargs: GetAliasRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
    "Name": ...,
}

parent.get_alias(**kwargs)
```

1. See [:material-code-braces: GetAliasRequestRequestTypeDef](./type_defs.md#getaliasrequestrequesttypedef) 

### get\_code\_signing\_config

Returns information about the specified code signing configuration.

Type annotations and code completion for `#!python session.client("lambda").get_code_signing_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# get_code_signing_config method definition

await def get_code_signing_config(
    self,
    *,
    CodeSigningConfigArn: str,
) -> GetCodeSigningConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCodeSigningConfigResponseTypeDef](./type_defs.md#getcodesigningconfigresponsetypedef) 


```python
# get_code_signing_config method usage example with argument unpacking

kwargs: GetCodeSigningConfigRequestRequestTypeDef = {  # (1)
    "CodeSigningConfigArn": ...,
}

parent.get_code_signing_config(**kwargs)
```

1. See [:material-code-braces: GetCodeSigningConfigRequestRequestTypeDef](./type_defs.md#getcodesigningconfigrequestrequesttypedef) 

### get\_event\_source\_mapping

Returns details about an event source mapping.

Type annotations and code completion for `#!python session.client("lambda").get_event_source_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# get_event_source_mapping method definition

await def get_event_source_mapping(
    self,
    *,
    UUID: str,
) -> EventSourceMappingConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EventSourceMappingConfigurationResponseTypeDef](./type_defs.md#eventsourcemappingconfigurationresponsetypedef) 


```python
# get_event_source_mapping method usage example with argument unpacking

kwargs: GetEventSourceMappingRequestRequestTypeDef = {  # (1)
    "UUID": ...,
}

parent.get_event_source_mapping(**kwargs)
```

1. See [:material-code-braces: GetEventSourceMappingRequestRequestTypeDef](./type_defs.md#geteventsourcemappingrequestrequesttypedef) 

### get\_function

Returns information about the function or function version, with a link to
download the deployment package that's valid for 10 minutes.

Type annotations and code completion for `#!python session.client("lambda").get_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# get_function method definition

await def get_function(
    self,
    *,
    FunctionName: str,
    Qualifier: str = ...,
) -> GetFunctionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFunctionResponseTypeDef](./type_defs.md#getfunctionresponsetypedef) 


```python
# get_function method usage example with argument unpacking

kwargs: GetFunctionRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.get_function(**kwargs)
```

1. See [:material-code-braces: GetFunctionRequestRequestTypeDef](./type_defs.md#getfunctionrequestrequesttypedef) 

### get\_function\_code\_signing\_config

Returns the code signing configuration for the specified function.

Type annotations and code completion for `#!python session.client("lambda").get_function_code_signing_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# get_function_code_signing_config method definition

await def get_function_code_signing_config(
    self,
    *,
    FunctionName: str,
) -> GetFunctionCodeSigningConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFunctionCodeSigningConfigResponseTypeDef](./type_defs.md#getfunctioncodesigningconfigresponsetypedef) 


```python
# get_function_code_signing_config method usage example with argument unpacking

kwargs: GetFunctionCodeSigningConfigRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.get_function_code_signing_config(**kwargs)
```

1. See [:material-code-braces: GetFunctionCodeSigningConfigRequestRequestTypeDef](./type_defs.md#getfunctioncodesigningconfigrequestrequesttypedef) 

### get\_function\_concurrency

Returns details about the reserved concurrency configuration for a function.

Type annotations and code completion for `#!python session.client("lambda").get_function_concurrency` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# get_function_concurrency method definition

await def get_function_concurrency(
    self,
    *,
    FunctionName: str,
) -> GetFunctionConcurrencyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFunctionConcurrencyResponseTypeDef](./type_defs.md#getfunctionconcurrencyresponsetypedef) 


```python
# get_function_concurrency method usage example with argument unpacking

kwargs: GetFunctionConcurrencyRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.get_function_concurrency(**kwargs)
```

1. See [:material-code-braces: GetFunctionConcurrencyRequestRequestTypeDef](./type_defs.md#getfunctionconcurrencyrequestrequesttypedef) 

### get\_function\_configuration

Returns the version-specific settings of a Lambda function or version.

Type annotations and code completion for `#!python session.client("lambda").get_function_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# get_function_configuration method definition

await def get_function_configuration(
    self,
    *,
    FunctionName: str,
    Qualifier: str = ...,
) -> FunctionConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: FunctionConfigurationResponseTypeDef](./type_defs.md#functionconfigurationresponsetypedef) 


```python
# get_function_configuration method usage example with argument unpacking

kwargs: GetFunctionConfigurationRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.get_function_configuration(**kwargs)
```

1. See [:material-code-braces: GetFunctionConfigurationRequestRequestTypeDef](./type_defs.md#getfunctionconfigurationrequestrequesttypedef) 

### get\_function\_event\_invoke\_config

Retrieves the configuration for asynchronous invocation for a function,
version, or alias.

Type annotations and code completion for `#!python session.client("lambda").get_function_event_invoke_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# get_function_event_invoke_config method definition

await def get_function_event_invoke_config(
    self,
    *,
    FunctionName: str,
    Qualifier: str = ...,
) -> FunctionEventInvokeConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: FunctionEventInvokeConfigResponseTypeDef](./type_defs.md#functioneventinvokeconfigresponsetypedef) 


```python
# get_function_event_invoke_config method usage example with argument unpacking

kwargs: GetFunctionEventInvokeConfigRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.get_function_event_invoke_config(**kwargs)
```

1. See [:material-code-braces: GetFunctionEventInvokeConfigRequestRequestTypeDef](./type_defs.md#getfunctioneventinvokeconfigrequestrequesttypedef) 

### get\_function\_recursion\_config

Returns your function's <a
href="https://docs.aws.amazon.com/lambda/latest/dg/invocation-recursion.html">recursive
loop detection</a> configuration.

Type annotations and code completion for `#!python session.client("lambda").get_function_recursion_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# get_function_recursion_config method definition

await def get_function_recursion_config(
    self,
    *,
    FunctionName: str,
) -> GetFunctionRecursionConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFunctionRecursionConfigResponseTypeDef](./type_defs.md#getfunctionrecursionconfigresponsetypedef) 


```python
# get_function_recursion_config method usage example with argument unpacking

kwargs: GetFunctionRecursionConfigRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.get_function_recursion_config(**kwargs)
```

1. See [:material-code-braces: GetFunctionRecursionConfigRequestRequestTypeDef](./type_defs.md#getfunctionrecursionconfigrequestrequesttypedef) 

### get\_function\_url\_config

Returns details about a Lambda function URL.

Type annotations and code completion for `#!python session.client("lambda").get_function_url_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# get_function_url_config method definition

await def get_function_url_config(
    self,
    *,
    FunctionName: str,
    Qualifier: str = ...,
) -> GetFunctionUrlConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFunctionUrlConfigResponseTypeDef](./type_defs.md#getfunctionurlconfigresponsetypedef) 


```python
# get_function_url_config method usage example with argument unpacking

kwargs: GetFunctionUrlConfigRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.get_function_url_config(**kwargs)
```

1. See [:material-code-braces: GetFunctionUrlConfigRequestRequestTypeDef](./type_defs.md#getfunctionurlconfigrequestrequesttypedef) 

### get\_layer\_version

Returns information about a version of an <a
href="https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html">Lambda
layer</a>, with a link to download the layer archive that's valid for 10
minutes.

Type annotations and code completion for `#!python session.client("lambda").get_layer_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# get_layer_version method definition

await def get_layer_version(
    self,
    *,
    LayerName: str,
    VersionNumber: int,
) -> GetLayerVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLayerVersionResponseTypeDef](./type_defs.md#getlayerversionresponsetypedef) 


```python
# get_layer_version method usage example with argument unpacking

kwargs: GetLayerVersionRequestRequestTypeDef = {  # (1)
    "LayerName": ...,
    "VersionNumber": ...,
}

parent.get_layer_version(**kwargs)
```

1. See [:material-code-braces: GetLayerVersionRequestRequestTypeDef](./type_defs.md#getlayerversionrequestrequesttypedef) 

### get\_layer\_version\_by\_arn

Returns information about a version of an <a
href="https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html">Lambda
layer</a>, with a link to download the layer archive that's valid for 10
minutes.

Type annotations and code completion for `#!python session.client("lambda").get_layer_version_by_arn` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# get_layer_version_by_arn method definition

await def get_layer_version_by_arn(
    self,
    *,
    Arn: str,
) -> GetLayerVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLayerVersionResponseTypeDef](./type_defs.md#getlayerversionresponsetypedef) 


```python
# get_layer_version_by_arn method usage example with argument unpacking

kwargs: GetLayerVersionByArnRequestRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.get_layer_version_by_arn(**kwargs)
```

1. See [:material-code-braces: GetLayerVersionByArnRequestRequestTypeDef](./type_defs.md#getlayerversionbyarnrequestrequesttypedef) 

### get\_layer\_version\_policy

Returns the permission policy for a version of an <a
href="https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html">Lambda
layer</a>.

Type annotations and code completion for `#!python session.client("lambda").get_layer_version_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# get_layer_version_policy method definition

await def get_layer_version_policy(
    self,
    *,
    LayerName: str,
    VersionNumber: int,
) -> GetLayerVersionPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLayerVersionPolicyResponseTypeDef](./type_defs.md#getlayerversionpolicyresponsetypedef) 


```python
# get_layer_version_policy method usage example with argument unpacking

kwargs: GetLayerVersionPolicyRequestRequestTypeDef = {  # (1)
    "LayerName": ...,
    "VersionNumber": ...,
}

parent.get_layer_version_policy(**kwargs)
```

1. See [:material-code-braces: GetLayerVersionPolicyRequestRequestTypeDef](./type_defs.md#getlayerversionpolicyrequestrequesttypedef) 

### get\_policy

Returns the <a
href="https://docs.aws.amazon.com/lambda/latest/dg/access-control-resource-based.html">resource-based
IAM policy</a> for a function, version, or alias.

Type annotations and code completion for `#!python session.client("lambda").get_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# get_policy method definition

await def get_policy(
    self,
    *,
    FunctionName: str,
    Qualifier: str = ...,
) -> GetPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPolicyResponseTypeDef](./type_defs.md#getpolicyresponsetypedef) 


```python
# get_policy method usage example with argument unpacking

kwargs: GetPolicyRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.get_policy(**kwargs)
```

1. See [:material-code-braces: GetPolicyRequestRequestTypeDef](./type_defs.md#getpolicyrequestrequesttypedef) 

### get\_provisioned\_concurrency\_config

Retrieves the provisioned concurrency configuration for a function's alias or
version.

Type annotations and code completion for `#!python session.client("lambda").get_provisioned_concurrency_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# get_provisioned_concurrency_config method definition

await def get_provisioned_concurrency_config(
    self,
    *,
    FunctionName: str,
    Qualifier: str,
) -> GetProvisionedConcurrencyConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetProvisionedConcurrencyConfigResponseTypeDef](./type_defs.md#getprovisionedconcurrencyconfigresponsetypedef) 


```python
# get_provisioned_concurrency_config method usage example with argument unpacking

kwargs: GetProvisionedConcurrencyConfigRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
    "Qualifier": ...,
}

parent.get_provisioned_concurrency_config(**kwargs)
```

1. See [:material-code-braces: GetProvisionedConcurrencyConfigRequestRequestTypeDef](./type_defs.md#getprovisionedconcurrencyconfigrequestrequesttypedef) 

### get\_runtime\_management\_config

Retrieves the runtime management configuration for a function's version.

Type annotations and code completion for `#!python session.client("lambda").get_runtime_management_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# get_runtime_management_config method definition

await def get_runtime_management_config(
    self,
    *,
    FunctionName: str,
    Qualifier: str = ...,
) -> GetRuntimeManagementConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRuntimeManagementConfigResponseTypeDef](./type_defs.md#getruntimemanagementconfigresponsetypedef) 


```python
# get_runtime_management_config method usage example with argument unpacking

kwargs: GetRuntimeManagementConfigRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.get_runtime_management_config(**kwargs)
```

1. See [:material-code-braces: GetRuntimeManagementConfigRequestRequestTypeDef](./type_defs.md#getruntimemanagementconfigrequestrequesttypedef) 

### invoke

Invokes a Lambda function.

Type annotations and code completion for `#!python session.client("lambda").invoke` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# invoke method definition

await def invoke(
    self,
    *,
    FunctionName: str,
    InvocationType: InvocationTypeType = ...,  # (1)
    LogType: LogTypeType = ...,  # (2)
    ClientContext: str = ...,
    Payload: BlobTypeDef = ...,
    Qualifier: str = ...,
) -> InvocationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: InvocationTypeType](./literals.md#invocationtypetype) 
2. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
3. See [:material-code-braces: InvocationResponseTypeDef](./type_defs.md#invocationresponsetypedef) 


```python
# invoke method usage example with argument unpacking

kwargs: InvocationRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.invoke(**kwargs)
```

1. See [:material-code-braces: InvocationRequestRequestTypeDef](./type_defs.md#invocationrequestrequesttypedef) 

### invoke\_async

For asynchronous function invocation, use <a>Invoke</a>.

Type annotations and code completion for `#!python session.client("lambda").invoke_async` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# invoke_async method definition

await def invoke_async(
    self,
    *,
    FunctionName: str,
    InvokeArgs: BlobTypeDef,
) -> InvokeAsyncResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: InvokeAsyncResponseTypeDef](./type_defs.md#invokeasyncresponsetypedef) 


```python
# invoke_async method usage example with argument unpacking

kwargs: InvokeAsyncRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
    "InvokeArgs": ...,
}

parent.invoke_async(**kwargs)
```

1. See [:material-code-braces: InvokeAsyncRequestRequestTypeDef](./type_defs.md#invokeasyncrequestrequesttypedef) 

### invoke\_with\_response\_stream

Configure your Lambda functions to stream response payloads back to clients.

Type annotations and code completion for `#!python session.client("lambda").invoke_with_response_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# invoke_with_response_stream method definition

await def invoke_with_response_stream(
    self,
    *,
    FunctionName: str,
    InvocationType: ResponseStreamingInvocationTypeType = ...,  # (1)
    LogType: LogTypeType = ...,  # (2)
    ClientContext: str = ...,
    Qualifier: str = ...,
    Payload: BlobTypeDef = ...,
) -> InvokeWithResponseStreamResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ResponseStreamingInvocationTypeType](./literals.md#responsestreaminginvocationtypetype) 
2. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
3. See [:material-code-braces: InvokeWithResponseStreamResponseTypeDef](./type_defs.md#invokewithresponsestreamresponsetypedef) 


```python
# invoke_with_response_stream method usage example with argument unpacking

kwargs: InvokeWithResponseStreamRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.invoke_with_response_stream(**kwargs)
```

1. See [:material-code-braces: InvokeWithResponseStreamRequestRequestTypeDef](./type_defs.md#invokewithresponsestreamrequestrequesttypedef) 

### list\_aliases

Returns a list of <a
href="https://docs.aws.amazon.com/lambda/latest/dg/configuration-aliases.html">aliases</a>
for a Lambda function.

Type annotations and code completion for `#!python session.client("lambda").list_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# list_aliases method definition

await def list_aliases(
    self,
    *,
    FunctionName: str,
    FunctionVersion: str = ...,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListAliasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef) 


```python
# list_aliases method usage example with argument unpacking

kwargs: ListAliasesRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.list_aliases(**kwargs)
```

1. See [:material-code-braces: ListAliasesRequestRequestTypeDef](./type_defs.md#listaliasesrequestrequesttypedef) 

### list\_code\_signing\_configs

Returns a list of <a
href="https://docs.aws.amazon.com/lambda/latest/dg/configuring-codesigning.html">code
signing configurations</a>.

Type annotations and code completion for `#!python session.client("lambda").list_code_signing_configs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# list_code_signing_configs method definition

await def list_code_signing_configs(
    self,
    *,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListCodeSigningConfigsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCodeSigningConfigsResponseTypeDef](./type_defs.md#listcodesigningconfigsresponsetypedef) 


```python
# list_code_signing_configs method usage example with argument unpacking

kwargs: ListCodeSigningConfigsRequestRequestTypeDef = {  # (1)
    "Marker": ...,
}

parent.list_code_signing_configs(**kwargs)
```

1. See [:material-code-braces: ListCodeSigningConfigsRequestRequestTypeDef](./type_defs.md#listcodesigningconfigsrequestrequesttypedef) 

### list\_event\_source\_mappings

Lists event source mappings.

Type annotations and code completion for `#!python session.client("lambda").list_event_source_mappings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# list_event_source_mappings method definition

await def list_event_source_mappings(
    self,
    *,
    EventSourceArn: str = ...,
    FunctionName: str = ...,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListEventSourceMappingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEventSourceMappingsResponseTypeDef](./type_defs.md#listeventsourcemappingsresponsetypedef) 


```python
# list_event_source_mappings method usage example with argument unpacking

kwargs: ListEventSourceMappingsRequestRequestTypeDef = {  # (1)
    "EventSourceArn": ...,
}

parent.list_event_source_mappings(**kwargs)
```

1. See [:material-code-braces: ListEventSourceMappingsRequestRequestTypeDef](./type_defs.md#listeventsourcemappingsrequestrequesttypedef) 

### list\_function\_event\_invoke\_configs

Retrieves a list of configurations for asynchronous invocation for a function.

Type annotations and code completion for `#!python session.client("lambda").list_function_event_invoke_configs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# list_function_event_invoke_configs method definition

await def list_function_event_invoke_configs(
    self,
    *,
    FunctionName: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListFunctionEventInvokeConfigsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFunctionEventInvokeConfigsResponseTypeDef](./type_defs.md#listfunctioneventinvokeconfigsresponsetypedef) 


```python
# list_function_event_invoke_configs method usage example with argument unpacking

kwargs: ListFunctionEventInvokeConfigsRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.list_function_event_invoke_configs(**kwargs)
```

1. See [:material-code-braces: ListFunctionEventInvokeConfigsRequestRequestTypeDef](./type_defs.md#listfunctioneventinvokeconfigsrequestrequesttypedef) 

### list\_function\_url\_configs

Returns a list of Lambda function URLs for the specified function.

Type annotations and code completion for `#!python session.client("lambda").list_function_url_configs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# list_function_url_configs method definition

await def list_function_url_configs(
    self,
    *,
    FunctionName: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListFunctionUrlConfigsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFunctionUrlConfigsResponseTypeDef](./type_defs.md#listfunctionurlconfigsresponsetypedef) 


```python
# list_function_url_configs method usage example with argument unpacking

kwargs: ListFunctionUrlConfigsRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.list_function_url_configs(**kwargs)
```

1. See [:material-code-braces: ListFunctionUrlConfigsRequestRequestTypeDef](./type_defs.md#listfunctionurlconfigsrequestrequesttypedef) 

### list\_functions

Returns a list of Lambda functions, with the version-specific configuration of
each.

Type annotations and code completion for `#!python session.client("lambda").list_functions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# list_functions method definition

await def list_functions(
    self,
    *,
    MasterRegion: str = ...,
    FunctionVersion: FunctionVersionType = ...,  # (1)
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListFunctionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: FunctionVersionType](./literals.md#functionversiontype) 
2. See [:material-code-braces: ListFunctionsResponseTypeDef](./type_defs.md#listfunctionsresponsetypedef) 


```python
# list_functions method usage example with argument unpacking

kwargs: ListFunctionsRequestRequestTypeDef = {  # (1)
    "MasterRegion": ...,
}

parent.list_functions(**kwargs)
```

1. See [:material-code-braces: ListFunctionsRequestRequestTypeDef](./type_defs.md#listfunctionsrequestrequesttypedef) 

### list\_functions\_by\_code\_signing\_config

List the functions that use the specified code signing configuration.

Type annotations and code completion for `#!python session.client("lambda").list_functions_by_code_signing_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# list_functions_by_code_signing_config method definition

await def list_functions_by_code_signing_config(
    self,
    *,
    CodeSigningConfigArn: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListFunctionsByCodeSigningConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFunctionsByCodeSigningConfigResponseTypeDef](./type_defs.md#listfunctionsbycodesigningconfigresponsetypedef) 


```python
# list_functions_by_code_signing_config method usage example with argument unpacking

kwargs: ListFunctionsByCodeSigningConfigRequestRequestTypeDef = {  # (1)
    "CodeSigningConfigArn": ...,
}

parent.list_functions_by_code_signing_config(**kwargs)
```

1. See [:material-code-braces: ListFunctionsByCodeSigningConfigRequestRequestTypeDef](./type_defs.md#listfunctionsbycodesigningconfigrequestrequesttypedef) 

### list\_layer\_versions

Lists the versions of an <a
href="https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html">Lambda
layer</a>.

Type annotations and code completion for `#!python session.client("lambda").list_layer_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# list_layer_versions method definition

await def list_layer_versions(
    self,
    *,
    LayerName: str,
    CompatibleRuntime: RuntimeType = ...,  # (1)
    Marker: str = ...,
    MaxItems: int = ...,
    CompatibleArchitecture: ArchitectureType = ...,  # (2)
) -> ListLayerVersionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
2. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
3. See [:material-code-braces: ListLayerVersionsResponseTypeDef](./type_defs.md#listlayerversionsresponsetypedef) 


```python
# list_layer_versions method usage example with argument unpacking

kwargs: ListLayerVersionsRequestRequestTypeDef = {  # (1)
    "LayerName": ...,
}

parent.list_layer_versions(**kwargs)
```

1. See [:material-code-braces: ListLayerVersionsRequestRequestTypeDef](./type_defs.md#listlayerversionsrequestrequesttypedef) 

### list\_layers

Lists <a
href="https://docs.aws.amazon.com/lambda/latest/dg/invocation-layers.html">Lambda
layers</a> and shows information about the latest version of each.

Type annotations and code completion for `#!python session.client("lambda").list_layers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# list_layers method definition

await def list_layers(
    self,
    *,
    CompatibleRuntime: RuntimeType = ...,  # (1)
    Marker: str = ...,
    MaxItems: int = ...,
    CompatibleArchitecture: ArchitectureType = ...,  # (2)
) -> ListLayersResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
2. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
3. See [:material-code-braces: ListLayersResponseTypeDef](./type_defs.md#listlayersresponsetypedef) 


```python
# list_layers method usage example with argument unpacking

kwargs: ListLayersRequestRequestTypeDef = {  # (1)
    "CompatibleRuntime": ...,
}

parent.list_layers(**kwargs)
```

1. See [:material-code-braces: ListLayersRequestRequestTypeDef](./type_defs.md#listlayersrequestrequesttypedef) 

### list\_provisioned\_concurrency\_configs

Retrieves a list of provisioned concurrency configurations for a function.

Type annotations and code completion for `#!python session.client("lambda").list_provisioned_concurrency_configs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# list_provisioned_concurrency_configs method definition

await def list_provisioned_concurrency_configs(
    self,
    *,
    FunctionName: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListProvisionedConcurrencyConfigsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListProvisionedConcurrencyConfigsResponseTypeDef](./type_defs.md#listprovisionedconcurrencyconfigsresponsetypedef) 


```python
# list_provisioned_concurrency_configs method usage example with argument unpacking

kwargs: ListProvisionedConcurrencyConfigsRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.list_provisioned_concurrency_configs(**kwargs)
```

1. See [:material-code-braces: ListProvisionedConcurrencyConfigsRequestRequestTypeDef](./type_defs.md#listprovisionedconcurrencyconfigsrequestrequesttypedef) 

### list\_tags

Returns a function, event source mapping, or code signing configuration's <a
href="https://docs.aws.amazon.com/lambda/latest/dg/tagging.html">tags</a>.

Type annotations and code completion for `#!python session.client("lambda").list_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# list_tags method definition

await def list_tags(
    self,
    *,
    Resource: str,
) -> ListTagsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef) 


```python
# list_tags method usage example with argument unpacking

kwargs: ListTagsRequestRequestTypeDef = {  # (1)
    "Resource": ...,
}

parent.list_tags(**kwargs)
```

1. See [:material-code-braces: ListTagsRequestRequestTypeDef](./type_defs.md#listtagsrequestrequesttypedef) 

### list\_versions\_by\_function

Returns a list of <a
href="https://docs.aws.amazon.com/lambda/latest/dg/versioning-aliases.html">versions</a>,
with the version-specific configuration of each.

Type annotations and code completion for `#!python session.client("lambda").list_versions_by_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# list_versions_by_function method definition

await def list_versions_by_function(
    self,
    *,
    FunctionName: str,
    Marker: str = ...,
    MaxItems: int = ...,
) -> ListVersionsByFunctionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVersionsByFunctionResponseTypeDef](./type_defs.md#listversionsbyfunctionresponsetypedef) 


```python
# list_versions_by_function method usage example with argument unpacking

kwargs: ListVersionsByFunctionRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.list_versions_by_function(**kwargs)
```

1. See [:material-code-braces: ListVersionsByFunctionRequestRequestTypeDef](./type_defs.md#listversionsbyfunctionrequestrequesttypedef) 

### publish\_layer\_version

Creates an <a
href="https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html">Lambda
layer</a> from a ZIP archive.

Type annotations and code completion for `#!python session.client("lambda").publish_layer_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# publish_layer_version method definition

await def publish_layer_version(
    self,
    *,
    LayerName: str,
    Content: LayerVersionContentInputTypeDef,  # (1)
    Description: str = ...,
    CompatibleRuntimes: Sequence[RuntimeType] = ...,  # (2)
    LicenseInfo: str = ...,
    CompatibleArchitectures: Sequence[ArchitectureType] = ...,  # (3)
) -> PublishLayerVersionResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: LayerVersionContentInputTypeDef](./type_defs.md#layerversioncontentinputtypedef) 
2. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
3. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
4. See [:material-code-braces: PublishLayerVersionResponseTypeDef](./type_defs.md#publishlayerversionresponsetypedef) 


```python
# publish_layer_version method usage example with argument unpacking

kwargs: PublishLayerVersionRequestRequestTypeDef = {  # (1)
    "LayerName": ...,
    "Content": ...,
}

parent.publish_layer_version(**kwargs)
```

1. See [:material-code-braces: PublishLayerVersionRequestRequestTypeDef](./type_defs.md#publishlayerversionrequestrequesttypedef) 

### publish\_version

Creates a <a
href="https://docs.aws.amazon.com/lambda/latest/dg/versioning-aliases.html">version</a>
from the current code and configuration of a function.

Type annotations and code completion for `#!python session.client("lambda").publish_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# publish_version method definition

await def publish_version(
    self,
    *,
    FunctionName: str,
    CodeSha256: str = ...,
    Description: str = ...,
    RevisionId: str = ...,
) -> FunctionConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: FunctionConfigurationResponseTypeDef](./type_defs.md#functionconfigurationresponsetypedef) 


```python
# publish_version method usage example with argument unpacking

kwargs: PublishVersionRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.publish_version(**kwargs)
```

1. See [:material-code-braces: PublishVersionRequestRequestTypeDef](./type_defs.md#publishversionrequestrequesttypedef) 

### put\_function\_code\_signing\_config

Update the code signing configuration for the function.

Type annotations and code completion for `#!python session.client("lambda").put_function_code_signing_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# put_function_code_signing_config method definition

await def put_function_code_signing_config(
    self,
    *,
    CodeSigningConfigArn: str,
    FunctionName: str,
) -> PutFunctionCodeSigningConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutFunctionCodeSigningConfigResponseTypeDef](./type_defs.md#putfunctioncodesigningconfigresponsetypedef) 


```python
# put_function_code_signing_config method usage example with argument unpacking

kwargs: PutFunctionCodeSigningConfigRequestRequestTypeDef = {  # (1)
    "CodeSigningConfigArn": ...,
    "FunctionName": ...,
}

parent.put_function_code_signing_config(**kwargs)
```

1. See [:material-code-braces: PutFunctionCodeSigningConfigRequestRequestTypeDef](./type_defs.md#putfunctioncodesigningconfigrequestrequesttypedef) 

### put\_function\_concurrency

Sets the maximum number of simultaneous executions for a function, and reserves
capacity for that concurrency level.

Type annotations and code completion for `#!python session.client("lambda").put_function_concurrency` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# put_function_concurrency method definition

await def put_function_concurrency(
    self,
    *,
    FunctionName: str,
    ReservedConcurrentExecutions: int,
) -> ConcurrencyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ConcurrencyResponseTypeDef](./type_defs.md#concurrencyresponsetypedef) 


```python
# put_function_concurrency method usage example with argument unpacking

kwargs: PutFunctionConcurrencyRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
    "ReservedConcurrentExecutions": ...,
}

parent.put_function_concurrency(**kwargs)
```

1. See [:material-code-braces: PutFunctionConcurrencyRequestRequestTypeDef](./type_defs.md#putfunctionconcurrencyrequestrequesttypedef) 

### put\_function\_event\_invoke\_config

Configures options for <a
href="https://docs.aws.amazon.com/lambda/latest/dg/invocation-async.html">asynchronous
invocation</a> on a function, version, or alias.

Type annotations and code completion for `#!python session.client("lambda").put_function_event_invoke_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# put_function_event_invoke_config method definition

await def put_function_event_invoke_config(
    self,
    *,
    FunctionName: str,
    Qualifier: str = ...,
    MaximumRetryAttempts: int = ...,
    MaximumEventAgeInSeconds: int = ...,
    DestinationConfig: DestinationConfigTypeDef = ...,  # (1)
) -> FunctionEventInvokeConfigResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
2. See [:material-code-braces: FunctionEventInvokeConfigResponseTypeDef](./type_defs.md#functioneventinvokeconfigresponsetypedef) 


```python
# put_function_event_invoke_config method usage example with argument unpacking

kwargs: PutFunctionEventInvokeConfigRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.put_function_event_invoke_config(**kwargs)
```

1. See [:material-code-braces: PutFunctionEventInvokeConfigRequestRequestTypeDef](./type_defs.md#putfunctioneventinvokeconfigrequestrequesttypedef) 

### put\_function\_recursion\_config

Sets your function's <a
href="https://docs.aws.amazon.com/lambda/latest/dg/invocation-recursion.html">recursive
loop detection</a> configuration.

Type annotations and code completion for `#!python session.client("lambda").put_function_recursion_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# put_function_recursion_config method definition

await def put_function_recursion_config(
    self,
    *,
    FunctionName: str,
    RecursiveLoop: RecursiveLoopType,  # (1)
) -> PutFunctionRecursionConfigResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RecursiveLoopType](./literals.md#recursivelooptype) 
2. See [:material-code-braces: PutFunctionRecursionConfigResponseTypeDef](./type_defs.md#putfunctionrecursionconfigresponsetypedef) 


```python
# put_function_recursion_config method usage example with argument unpacking

kwargs: PutFunctionRecursionConfigRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
    "RecursiveLoop": ...,
}

parent.put_function_recursion_config(**kwargs)
```

1. See [:material-code-braces: PutFunctionRecursionConfigRequestRequestTypeDef](./type_defs.md#putfunctionrecursionconfigrequestrequesttypedef) 

### put\_provisioned\_concurrency\_config

Adds a provisioned concurrency configuration to a function's alias or version.

Type annotations and code completion for `#!python session.client("lambda").put_provisioned_concurrency_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# put_provisioned_concurrency_config method definition

await def put_provisioned_concurrency_config(
    self,
    *,
    FunctionName: str,
    Qualifier: str,
    ProvisionedConcurrentExecutions: int,
) -> PutProvisionedConcurrencyConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutProvisionedConcurrencyConfigResponseTypeDef](./type_defs.md#putprovisionedconcurrencyconfigresponsetypedef) 


```python
# put_provisioned_concurrency_config method usage example with argument unpacking

kwargs: PutProvisionedConcurrencyConfigRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
    "Qualifier": ...,
    "ProvisionedConcurrentExecutions": ...,
}

parent.put_provisioned_concurrency_config(**kwargs)
```

1. See [:material-code-braces: PutProvisionedConcurrencyConfigRequestRequestTypeDef](./type_defs.md#putprovisionedconcurrencyconfigrequestrequesttypedef) 

### put\_runtime\_management\_config

Sets the runtime management configuration for a function's version.

Type annotations and code completion for `#!python session.client("lambda").put_runtime_management_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# put_runtime_management_config method definition

await def put_runtime_management_config(
    self,
    *,
    FunctionName: str,
    UpdateRuntimeOn: UpdateRuntimeOnType,  # (1)
    Qualifier: str = ...,
    RuntimeVersionArn: str = ...,
) -> PutRuntimeManagementConfigResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: UpdateRuntimeOnType](./literals.md#updateruntimeontype) 
2. See [:material-code-braces: PutRuntimeManagementConfigResponseTypeDef](./type_defs.md#putruntimemanagementconfigresponsetypedef) 


```python
# put_runtime_management_config method usage example with argument unpacking

kwargs: PutRuntimeManagementConfigRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
    "UpdateRuntimeOn": ...,
}

parent.put_runtime_management_config(**kwargs)
```

1. See [:material-code-braces: PutRuntimeManagementConfigRequestRequestTypeDef](./type_defs.md#putruntimemanagementconfigrequestrequesttypedef) 

### remove\_layer\_version\_permission

Removes a statement from the permissions policy for a version of an <a
href="https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html">Lambda
layer</a>.

Type annotations and code completion for `#!python session.client("lambda").remove_layer_version_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# remove_layer_version_permission method definition

await def remove_layer_version_permission(
    self,
    *,
    LayerName: str,
    VersionNumber: int,
    StatementId: str,
    RevisionId: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# remove_layer_version_permission method usage example with argument unpacking

kwargs: RemoveLayerVersionPermissionRequestRequestTypeDef = {  # (1)
    "LayerName": ...,
    "VersionNumber": ...,
    "StatementId": ...,
}

parent.remove_layer_version_permission(**kwargs)
```

1. See [:material-code-braces: RemoveLayerVersionPermissionRequestRequestTypeDef](./type_defs.md#removelayerversionpermissionrequestrequesttypedef) 

### remove\_permission

Revokes function-use permission from an Amazon Web Services service or another
Amazon Web Services account.

Type annotations and code completion for `#!python session.client("lambda").remove_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# remove_permission method definition

await def remove_permission(
    self,
    *,
    FunctionName: str,
    StatementId: str,
    Qualifier: str = ...,
    RevisionId: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# remove_permission method usage example with argument unpacking

kwargs: RemovePermissionRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
    "StatementId": ...,
}

parent.remove_permission(**kwargs)
```

1. See [:material-code-braces: RemovePermissionRequestRequestTypeDef](./type_defs.md#removepermissionrequestrequesttypedef) 

### tag\_resource

Adds <a
href="https://docs.aws.amazon.com/lambda/latest/dg/tagging.html">tags</a> to a
function, event source mapping, or code signing configuration.

Type annotations and code completion for `#!python session.client("lambda").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    Resource: str,
    Tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "Resource": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes <a
href="https://docs.aws.amazon.com/lambda/latest/dg/tagging.html">tags</a> from
a function, event source mapping, or code signing configuration.

Type annotations and code completion for `#!python session.client("lambda").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    Resource: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "Resource": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_alias

Updates the configuration of a Lambda function <a
href="https://docs.aws.amazon.com/lambda/latest/dg/configuration-aliases.html">alias</a>.

Type annotations and code completion for `#!python session.client("lambda").update_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# update_alias method definition

await def update_alias(
    self,
    *,
    FunctionName: str,
    Name: str,
    FunctionVersion: str = ...,
    Description: str = ...,
    RoutingConfig: AliasRoutingConfigurationTypeDef = ...,  # (1)
    RevisionId: str = ...,
) -> AliasConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AliasRoutingConfigurationTypeDef](./type_defs.md#aliasroutingconfigurationtypedef) 
2. See [:material-code-braces: AliasConfigurationResponseTypeDef](./type_defs.md#aliasconfigurationresponsetypedef) 


```python
# update_alias method usage example with argument unpacking

kwargs: UpdateAliasRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
    "Name": ...,
}

parent.update_alias(**kwargs)
```

1. See [:material-code-braces: UpdateAliasRequestRequestTypeDef](./type_defs.md#updatealiasrequestrequesttypedef) 

### update\_code\_signing\_config

Update the code signing configuration.

Type annotations and code completion for `#!python session.client("lambda").update_code_signing_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# update_code_signing_config method definition

await def update_code_signing_config(
    self,
    *,
    CodeSigningConfigArn: str,
    Description: str = ...,
    AllowedPublishers: AllowedPublishersTypeDef = ...,  # (1)
    CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...,  # (2)
) -> UpdateCodeSigningConfigResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AllowedPublishersTypeDef](./type_defs.md#allowedpublisherstypedef) 
2. See [:material-code-braces: CodeSigningPoliciesTypeDef](./type_defs.md#codesigningpoliciestypedef) 
3. See [:material-code-braces: UpdateCodeSigningConfigResponseTypeDef](./type_defs.md#updatecodesigningconfigresponsetypedef) 


```python
# update_code_signing_config method usage example with argument unpacking

kwargs: UpdateCodeSigningConfigRequestRequestTypeDef = {  # (1)
    "CodeSigningConfigArn": ...,
}

parent.update_code_signing_config(**kwargs)
```

1. See [:material-code-braces: UpdateCodeSigningConfigRequestRequestTypeDef](./type_defs.md#updatecodesigningconfigrequestrequesttypedef) 

### update\_event\_source\_mapping

Updates an event source mapping.

Type annotations and code completion for `#!python session.client("lambda").update_event_source_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# update_event_source_mapping method definition

await def update_event_source_mapping(
    self,
    *,
    UUID: str,
    FunctionName: str = ...,
    Enabled: bool = ...,
    BatchSize: int = ...,
    FilterCriteria: FilterCriteriaTypeDef = ...,  # (1)
    MaximumBatchingWindowInSeconds: int = ...,
    DestinationConfig: DestinationConfigTypeDef = ...,  # (2)
    MaximumRecordAgeInSeconds: int = ...,
    BisectBatchOnFunctionError: bool = ...,
    MaximumRetryAttempts: int = ...,
    ParallelizationFactor: int = ...,
    SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,  # (3)
    TumblingWindowInSeconds: int = ...,
    FunctionResponseTypes: Sequence[FunctionResponseTypeType] = ...,  # (4)
    ScalingConfig: ScalingConfigTypeDef = ...,  # (5)
    DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...,  # (6)
    KMSKeyArn: str = ...,
    MetricsConfig: EventSourceMappingMetricsConfigTypeDef = ...,  # (7)
    ProvisionedPollerConfig: ProvisionedPollerConfigTypeDef = ...,  # (8)
) -> EventSourceMappingConfigurationResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
2. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
3. See [:material-code-braces: SourceAccessConfigurationTypeDef](./type_defs.md#sourceaccessconfigurationtypedef) 
4. See [:material-code-brackets: FunctionResponseTypeType](./literals.md#functionresponsetypetype) 
5. See [:material-code-braces: ScalingConfigTypeDef](./type_defs.md#scalingconfigtypedef) 
6. See [:material-code-braces: DocumentDBEventSourceConfigTypeDef](./type_defs.md#documentdbeventsourceconfigtypedef) 
7. See [:material-code-braces: EventSourceMappingMetricsConfigTypeDef](./type_defs.md#eventsourcemappingmetricsconfigtypedef) 
8. See [:material-code-braces: ProvisionedPollerConfigTypeDef](./type_defs.md#provisionedpollerconfigtypedef) 
9. See [:material-code-braces: EventSourceMappingConfigurationResponseTypeDef](./type_defs.md#eventsourcemappingconfigurationresponsetypedef) 


```python
# update_event_source_mapping method usage example with argument unpacking

kwargs: UpdateEventSourceMappingRequestRequestTypeDef = {  # (1)
    "UUID": ...,
}

parent.update_event_source_mapping(**kwargs)
```

1. See [:material-code-braces: UpdateEventSourceMappingRequestRequestTypeDef](./type_defs.md#updateeventsourcemappingrequestrequesttypedef) 

### update\_function\_code

Updates a Lambda function's code.

Type annotations and code completion for `#!python session.client("lambda").update_function_code` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# update_function_code method definition

await def update_function_code(
    self,
    *,
    FunctionName: str,
    ZipFile: BlobTypeDef = ...,
    S3Bucket: str = ...,
    S3Key: str = ...,
    S3ObjectVersion: str = ...,
    ImageUri: str = ...,
    Publish: bool = ...,
    DryRun: bool = ...,
    RevisionId: str = ...,
    Architectures: Sequence[ArchitectureType] = ...,  # (1)
    SourceKMSKeyArn: str = ...,
) -> FunctionConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
2. See [:material-code-braces: FunctionConfigurationResponseTypeDef](./type_defs.md#functionconfigurationresponsetypedef) 


```python
# update_function_code method usage example with argument unpacking

kwargs: UpdateFunctionCodeRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.update_function_code(**kwargs)
```

1. See [:material-code-braces: UpdateFunctionCodeRequestRequestTypeDef](./type_defs.md#updatefunctioncoderequestrequesttypedef) 

### update\_function\_configuration

Modify the version-specific settings of a Lambda function.

Type annotations and code completion for `#!python session.client("lambda").update_function_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# update_function_configuration method definition

await def update_function_configuration(
    self,
    *,
    FunctionName: str,
    Role: str = ...,
    Handler: str = ...,
    Description: str = ...,
    Timeout: int = ...,
    MemorySize: int = ...,
    VpcConfig: VpcConfigTypeDef = ...,  # (1)
    Environment: EnvironmentTypeDef = ...,  # (2)
    Runtime: RuntimeType = ...,  # (3)
    DeadLetterConfig: DeadLetterConfigTypeDef = ...,  # (4)
    KMSKeyArn: str = ...,
    TracingConfig: TracingConfigTypeDef = ...,  # (5)
    RevisionId: str = ...,
    Layers: Sequence[str] = ...,
    FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,  # (6)
    ImageConfig: ImageConfigTypeDef = ...,  # (7)
    EphemeralStorage: EphemeralStorageTypeDef = ...,  # (8)
    SnapStart: SnapStartTypeDef = ...,  # (9)
    LoggingConfig: LoggingConfigTypeDef = ...,  # (10)
) -> FunctionConfigurationResponseTypeDef:  # (11)
    ...
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
2. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
3. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
4. See [:material-code-braces: DeadLetterConfigTypeDef](./type_defs.md#deadletterconfigtypedef) 
5. See [:material-code-braces: TracingConfigTypeDef](./type_defs.md#tracingconfigtypedef) 
6. See [:material-code-braces: FileSystemConfigTypeDef](./type_defs.md#filesystemconfigtypedef) 
7. See [:material-code-braces: ImageConfigTypeDef](./type_defs.md#imageconfigtypedef) 
8. See [:material-code-braces: EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef) 
9. See [:material-code-braces: SnapStartTypeDef](./type_defs.md#snapstarttypedef) 
10. See [:material-code-braces: LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef) 
11. See [:material-code-braces: FunctionConfigurationResponseTypeDef](./type_defs.md#functionconfigurationresponsetypedef) 


```python
# update_function_configuration method usage example with argument unpacking

kwargs: UpdateFunctionConfigurationRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.update_function_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateFunctionConfigurationRequestRequestTypeDef](./type_defs.md#updatefunctionconfigurationrequestrequesttypedef) 

### update\_function\_event\_invoke\_config

Updates the configuration for asynchronous invocation for a function, version,
or alias.

Type annotations and code completion for `#!python session.client("lambda").update_function_event_invoke_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# update_function_event_invoke_config method definition

await def update_function_event_invoke_config(
    self,
    *,
    FunctionName: str,
    Qualifier: str = ...,
    MaximumRetryAttempts: int = ...,
    MaximumEventAgeInSeconds: int = ...,
    DestinationConfig: DestinationConfigTypeDef = ...,  # (1)
) -> FunctionEventInvokeConfigResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
2. See [:material-code-braces: FunctionEventInvokeConfigResponseTypeDef](./type_defs.md#functioneventinvokeconfigresponsetypedef) 


```python
# update_function_event_invoke_config method usage example with argument unpacking

kwargs: UpdateFunctionEventInvokeConfigRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.update_function_event_invoke_config(**kwargs)
```

1. See [:material-code-braces: UpdateFunctionEventInvokeConfigRequestRequestTypeDef](./type_defs.md#updatefunctioneventinvokeconfigrequestrequesttypedef) 

### update\_function\_url\_config

Updates the configuration for a Lambda function URL.

Type annotations and code completion for `#!python session.client("lambda").update_function_url_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# update_function_url_config method definition

await def update_function_url_config(
    self,
    *,
    FunctionName: str,
    Qualifier: str = ...,
    AuthType: FunctionUrlAuthTypeType = ...,  # (1)
    Cors: CorsTypeDef = ...,  # (2)
    InvokeMode: InvokeModeType = ...,  # (3)
) -> UpdateFunctionUrlConfigResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: FunctionUrlAuthTypeType](./literals.md#functionurlauthtypetype) 
2. See [:material-code-braces: CorsTypeDef](./type_defs.md#corstypedef) 
3. See [:material-code-brackets: InvokeModeType](./literals.md#invokemodetype) 
4. See [:material-code-braces: UpdateFunctionUrlConfigResponseTypeDef](./type_defs.md#updatefunctionurlconfigresponsetypedef) 


```python
# update_function_url_config method usage example with argument unpacking

kwargs: UpdateFunctionUrlConfigRequestRequestTypeDef = {  # (1)
    "FunctionName": ...,
}

parent.update_function_url_config(**kwargs)
```

1. See [:material-code-braces: UpdateFunctionUrlConfigRequestRequestTypeDef](./type_defs.md#updatefunctionurlconfigrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("lambda").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("lambda").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

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

Type annotations and code completion for `#!python session.client("lambda").get_paginator` method with overloads.

- `client.get_paginator("list_aliases")` -> [ListAliasesPaginator](./paginators.md#listaliasespaginator)
- `client.get_paginator("list_code_signing_configs")` -> [ListCodeSigningConfigsPaginator](./paginators.md#listcodesigningconfigspaginator)
- `client.get_paginator("list_event_source_mappings")` -> [ListEventSourceMappingsPaginator](./paginators.md#listeventsourcemappingspaginator)
- `client.get_paginator("list_function_event_invoke_configs")` -> [ListFunctionEventInvokeConfigsPaginator](./paginators.md#listfunctioneventinvokeconfigspaginator)
- `client.get_paginator("list_function_url_configs")` -> [ListFunctionUrlConfigsPaginator](./paginators.md#listfunctionurlconfigspaginator)
- `client.get_paginator("list_functions_by_code_signing_config")` -> [ListFunctionsByCodeSigningConfigPaginator](./paginators.md#listfunctionsbycodesigningconfigpaginator)
- `client.get_paginator("list_functions")` -> [ListFunctionsPaginator](./paginators.md#listfunctionspaginator)
- `client.get_paginator("list_layer_versions")` -> [ListLayerVersionsPaginator](./paginators.md#listlayerversionspaginator)
- `client.get_paginator("list_layers")` -> [ListLayersPaginator](./paginators.md#listlayerspaginator)
- `client.get_paginator("list_provisioned_concurrency_configs")` -> [ListProvisionedConcurrencyConfigsPaginator](./paginators.md#listprovisionedconcurrencyconfigspaginator)
- `client.get_paginator("list_versions_by_function")` -> [ListVersionsByFunctionPaginator](./paginators.md#listversionsbyfunctionpaginator)




### get_waiter

Type annotations and code completion for `#!python session.client("lambda").get_waiter` method with overloads.

- `client.get_waiter("function_active_v2")` -> [FunctionActiveV2Waiter](./waiters.md#functionactivev2waiter)
- `client.get_waiter("function_active")` -> [FunctionActiveWaiter](./waiters.md#functionactivewaiter)
- `client.get_waiter("function_exists")` -> [FunctionExistsWaiter](./waiters.md#functionexistswaiter)
- `client.get_waiter("function_updated_v2")` -> [FunctionUpdatedV2Waiter](./waiters.md#functionupdatedv2waiter)
- `client.get_waiter("function_updated")` -> [FunctionUpdatedWaiter](./waiters.md#functionupdatedwaiter)
- `client.get_waiter("published_version_active")` -> [PublishedVersionActiveWaiter](./waiters.md#publishedversionactivewaiter)
