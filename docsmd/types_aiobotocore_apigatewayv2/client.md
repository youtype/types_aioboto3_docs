# ApiGatewayV2Client

> [Index](../README.md) > [ApiGatewayV2](./README.md) > ApiGatewayV2Client

!!! note ""

    Auto-generated documentation for [ApiGatewayV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#apigatewayv2)
    type annotations stubs module [types-aiobotocore-apigatewayv2](https://pypi.org/project/types-aiobotocore-apigatewayv2/).

## ApiGatewayV2Client

Type annotations and code completion for `#!python session.client("apigatewayv2")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# ApiGatewayV2Client usage example

from aioboto3.session import Session
from types_aiobotocore_apigatewayv2.client import ApiGatewayV2Client

session = Session()
async with session.client("apigatewayv2") as client:
    client: ApiGatewayV2Client
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("apigatewayv2").exceptions` structure.

```python
# ApiGatewayV2Client.exceptions usage example

async with session.client("apigatewayv2") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.BadRequestException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.NotFoundException,
        client.exceptions.TooManyRequestsException,
    ) as e:
        print(e)
```

```python
# ApiGatewayV2Client.exceptions type checking example

from types_aiobotocore_apigatewayv2.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("apigatewayv2").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("apigatewayv2").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

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


### create\_api

Creates an Api resource.

Type annotations and code completion for `#!python session.client("apigatewayv2").create_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# create_api method definition

await def create_api(
    self,
    *,
    Name: str,
    ProtocolType: ProtocolTypeType,  # (1)
    ApiKeySelectionExpression: str = ...,
    CorsConfiguration: CorsUnionTypeDef = ...,  # (2)
    CredentialsArn: str = ...,
    Description: str = ...,
    DisableSchemaValidation: bool = ...,
    DisableExecuteApiEndpoint: bool = ...,
    RouteKey: str = ...,
    RouteSelectionExpression: str = ...,
    Tags: Mapping[str, str] = ...,
    Target: str = ...,
    Version: str = ...,
) -> CreateApiResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ProtocolTypeType](./literals.md#protocoltypetype)
2. See [:material-code-braces: CorsUnionTypeDef](#corsuniontypedef)
3. See [:material-code-braces: CreateApiResponseTypeDef](./type_defs.md#createapiresponsetypedef)


```python
# create_api method usage example with argument unpacking

kwargs: CreateApiRequestTypeDef = {  # (1)
    "Name": ...,
    "ProtocolType": ...,
}

parent.create_api(**kwargs)
```

1. See [:material-code-braces: CreateApiRequestTypeDef](./type_defs.md#createapirequesttypedef)

### create\_api\_mapping

Creates an API mapping.

Type annotations and code completion for `#!python session.client("apigatewayv2").create_api_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# create_api_mapping method definition

await def create_api_mapping(
    self,
    *,
    ApiId: str,
    DomainName: str,
    Stage: str,
    ApiMappingKey: str = ...,
) -> CreateApiMappingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateApiMappingResponseTypeDef](./type_defs.md#createapimappingresponsetypedef)


```python
# create_api_mapping method usage example with argument unpacking

kwargs: CreateApiMappingRequestTypeDef = {  # (1)
    "ApiId": ...,
    "DomainName": ...,
    "Stage": ...,
}

parent.create_api_mapping(**kwargs)
```

1. See [:material-code-braces: CreateApiMappingRequestTypeDef](./type_defs.md#createapimappingrequesttypedef)

### create\_authorizer

Creates an Authorizer for an API.

Type annotations and code completion for `#!python session.client("apigatewayv2").create_authorizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# create_authorizer method definition

await def create_authorizer(
    self,
    *,
    ApiId: str,
    AuthorizerType: AuthorizerTypeType,  # (1)
    IdentitySource: Sequence[str],
    Name: str,
    AuthorizerCredentialsArn: str = ...,
    AuthorizerPayloadFormatVersion: str = ...,
    AuthorizerResultTtlInSeconds: int = ...,
    AuthorizerUri: str = ...,
    EnableSimpleResponses: bool = ...,
    IdentityValidationExpression: str = ...,
    JwtConfiguration: JWTConfigurationUnionTypeDef = ...,  # (2)
) -> CreateAuthorizerResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AuthorizerTypeType](./literals.md#authorizertypetype)
2. See [:material-code-braces: JWTConfigurationUnionTypeDef](#jwtconfigurationuniontypedef)
3. See [:material-code-braces: CreateAuthorizerResponseTypeDef](./type_defs.md#createauthorizerresponsetypedef)


```python
# create_authorizer method usage example with argument unpacking

kwargs: CreateAuthorizerRequestTypeDef = {  # (1)
    "ApiId": ...,
    "AuthorizerType": ...,
    "IdentitySource": ...,
    "Name": ...,
}

parent.create_authorizer(**kwargs)
```

1. See [:material-code-braces: CreateAuthorizerRequestTypeDef](./type_defs.md#createauthorizerrequesttypedef)

### create\_deployment

Creates a Deployment for an API.

Type annotations and code completion for `#!python session.client("apigatewayv2").create_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# create_deployment method definition

await def create_deployment(
    self,
    *,
    ApiId: str,
    Description: str = ...,
    StageName: str = ...,
) -> CreateDeploymentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateDeploymentResponseTypeDef](./type_defs.md#createdeploymentresponsetypedef)


```python
# create_deployment method usage example with argument unpacking

kwargs: CreateDeploymentRequestTypeDef = {  # (1)
    "ApiId": ...,
}

parent.create_deployment(**kwargs)
```

1. See [:material-code-braces: CreateDeploymentRequestTypeDef](./type_defs.md#createdeploymentrequesttypedef)

### create\_domain\_name

Creates a domain name.

Type annotations and code completion for `#!python session.client("apigatewayv2").create_domain_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# create_domain_name method definition

await def create_domain_name(
    self,
    *,
    DomainName: str,
    DomainNameConfigurations: Sequence[DomainNameConfigurationUnionTypeDef] = ...,  # (1)
    MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...,  # (2)
    Tags: Mapping[str, str] = ...,
) -> CreateDomainNameResponseTypeDef:  # (3)
    ...
```

1. See `Sequence[DomainNameConfigurationUnionTypeDef]`
2. See [:material-code-braces: MutualTlsAuthenticationInputTypeDef](./type_defs.md#mutualtlsauthenticationinputtypedef)
3. See [:material-code-braces: CreateDomainNameResponseTypeDef](./type_defs.md#createdomainnameresponsetypedef)


```python
# create_domain_name method usage example with argument unpacking

kwargs: CreateDomainNameRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.create_domain_name(**kwargs)
```

1. See [:material-code-braces: CreateDomainNameRequestTypeDef](./type_defs.md#createdomainnamerequesttypedef)

### create\_integration

Creates an Integration.

Type annotations and code completion for `#!python session.client("apigatewayv2").create_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# create_integration method definition

await def create_integration(
    self,
    *,
    ApiId: str,
    IntegrationType: IntegrationTypeType,  # (1)
    ConnectionId: str = ...,
    ConnectionType: ConnectionTypeType = ...,  # (2)
    ContentHandlingStrategy: ContentHandlingStrategyType = ...,  # (3)
    CredentialsArn: str = ...,
    Description: str = ...,
    IntegrationMethod: str = ...,
    IntegrationSubtype: str = ...,
    IntegrationUri: str = ...,
    PassthroughBehavior: PassthroughBehaviorType = ...,  # (4)
    PayloadFormatVersion: str = ...,
    RequestParameters: Mapping[str, str] = ...,
    RequestTemplates: Mapping[str, str] = ...,
    ResponseParameters: Mapping[str, Mapping[str, str]] = ...,
    TemplateSelectionExpression: str = ...,
    TimeoutInMillis: int = ...,
    TlsConfig: TlsConfigInputTypeDef = ...,  # (5)
) -> CreateIntegrationResultTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype)
2. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype)
3. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype)
4. See [:material-code-brackets: PassthroughBehaviorType](./literals.md#passthroughbehaviortype)
5. See [:material-code-braces: TlsConfigInputTypeDef](./type_defs.md#tlsconfiginputtypedef)
6. See [:material-code-braces: CreateIntegrationResultTypeDef](./type_defs.md#createintegrationresulttypedef)


```python
# create_integration method usage example with argument unpacking

kwargs: CreateIntegrationRequestTypeDef = {  # (1)
    "ApiId": ...,
    "IntegrationType": ...,
}

parent.create_integration(**kwargs)
```

1. See [:material-code-braces: CreateIntegrationRequestTypeDef](./type_defs.md#createintegrationrequesttypedef)

### create\_integration\_response

Creates an IntegrationResponses.

Type annotations and code completion for `#!python session.client("apigatewayv2").create_integration_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# create_integration_response method definition

await def create_integration_response(
    self,
    *,
    ApiId: str,
    IntegrationId: str,
    IntegrationResponseKey: str,
    ContentHandlingStrategy: ContentHandlingStrategyType = ...,  # (1)
    ResponseParameters: Mapping[str, str] = ...,
    ResponseTemplates: Mapping[str, str] = ...,
    TemplateSelectionExpression: str = ...,
) -> CreateIntegrationResponseResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype)
2. See [:material-code-braces: CreateIntegrationResponseResponseTypeDef](./type_defs.md#createintegrationresponseresponsetypedef)


```python
# create_integration_response method usage example with argument unpacking

kwargs: CreateIntegrationResponseRequestTypeDef = {  # (1)
    "ApiId": ...,
    "IntegrationId": ...,
    "IntegrationResponseKey": ...,
}

parent.create_integration_response(**kwargs)
```

1. See [:material-code-braces: CreateIntegrationResponseRequestTypeDef](./type_defs.md#createintegrationresponserequesttypedef)

### create\_model

Creates a Model for an API.

Type annotations and code completion for `#!python session.client("apigatewayv2").create_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# create_model method definition

await def create_model(
    self,
    *,
    ApiId: str,
    Name: str,
    Schema: str,
    ContentType: str = ...,
    Description: str = ...,
) -> CreateModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateModelResponseTypeDef](./type_defs.md#createmodelresponsetypedef)


```python
# create_model method usage example with argument unpacking

kwargs: CreateModelRequestTypeDef = {  # (1)
    "ApiId": ...,
    "Name": ...,
    "Schema": ...,
}

parent.create_model(**kwargs)
```

1. See [:material-code-braces: CreateModelRequestTypeDef](./type_defs.md#createmodelrequesttypedef)

### create\_route

Creates a Route for an API.

Type annotations and code completion for `#!python session.client("apigatewayv2").create_route` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# create_route method definition

await def create_route(
    self,
    *,
    ApiId: str,
    RouteKey: str,
    ApiKeyRequired: bool = ...,
    AuthorizationScopes: Sequence[str] = ...,
    AuthorizationType: AuthorizationTypeType = ...,  # (1)
    AuthorizerId: str = ...,
    ModelSelectionExpression: str = ...,
    OperationName: str = ...,
    RequestModels: Mapping[str, str] = ...,
    RequestParameters: Mapping[str, ParameterConstraintsTypeDef] = ...,  # (2)
    RouteResponseSelectionExpression: str = ...,
    Target: str = ...,
) -> CreateRouteResultTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AuthorizationTypeType](./literals.md#authorizationtypetype)
2. See `Mapping[str, ParameterConstraintsTypeDef]`
3. See [:material-code-braces: CreateRouteResultTypeDef](./type_defs.md#createrouteresulttypedef)


```python
# create_route method usage example with argument unpacking

kwargs: CreateRouteRequestTypeDef = {  # (1)
    "ApiId": ...,
    "RouteKey": ...,
}

parent.create_route(**kwargs)
```

1. See [:material-code-braces: CreateRouteRequestTypeDef](./type_defs.md#createrouterequesttypedef)

### create\_route\_response

Creates a RouteResponse for a Route.

Type annotations and code completion for `#!python session.client("apigatewayv2").create_route_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# create_route_response method definition

await def create_route_response(
    self,
    *,
    ApiId: str,
    RouteId: str,
    RouteResponseKey: str,
    ModelSelectionExpression: str = ...,
    ResponseModels: Mapping[str, str] = ...,
    ResponseParameters: Mapping[str, ParameterConstraintsTypeDef] = ...,  # (1)
) -> CreateRouteResponseResponseTypeDef:  # (2)
    ...
```

1. See `Mapping[str, ParameterConstraintsTypeDef]`
2. See [:material-code-braces: CreateRouteResponseResponseTypeDef](./type_defs.md#createrouteresponseresponsetypedef)


```python
# create_route_response method usage example with argument unpacking

kwargs: CreateRouteResponseRequestTypeDef = {  # (1)
    "ApiId": ...,
    "RouteId": ...,
    "RouteResponseKey": ...,
}

parent.create_route_response(**kwargs)
```

1. See [:material-code-braces: CreateRouteResponseRequestTypeDef](./type_defs.md#createrouteresponserequesttypedef)

### create\_stage

Creates a Stage for an API.

Type annotations and code completion for `#!python session.client("apigatewayv2").create_stage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# create_stage method definition

await def create_stage(
    self,
    *,
    ApiId: str,
    StageName: str,
    AccessLogSettings: AccessLogSettingsTypeDef = ...,  # (1)
    AutoDeploy: bool = ...,
    ClientCertificateId: str = ...,
    DefaultRouteSettings: RouteSettingsTypeDef = ...,  # (2)
    DeploymentId: str = ...,
    Description: str = ...,
    RouteSettings: Mapping[str, RouteSettingsTypeDef] = ...,  # (3)
    StageVariables: Mapping[str, str] = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateStageResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: AccessLogSettingsTypeDef](./type_defs.md#accesslogsettingstypedef)
2. See [:material-code-braces: RouteSettingsTypeDef](./type_defs.md#routesettingstypedef)
3. See `Mapping[str, RouteSettingsTypeDef]`
4. See [:material-code-braces: CreateStageResponseTypeDef](./type_defs.md#createstageresponsetypedef)


```python
# create_stage method usage example with argument unpacking

kwargs: CreateStageRequestTypeDef = {  # (1)
    "ApiId": ...,
    "StageName": ...,
}

parent.create_stage(**kwargs)
```

1. See [:material-code-braces: CreateStageRequestTypeDef](./type_defs.md#createstagerequesttypedef)

### create\_vpc\_link

Creates a VPC link.

Type annotations and code completion for `#!python session.client("apigatewayv2").create_vpc_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# create_vpc_link method definition

await def create_vpc_link(
    self,
    *,
    Name: str,
    SubnetIds: Sequence[str],
    SecurityGroupIds: Sequence[str] = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateVpcLinkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateVpcLinkResponseTypeDef](./type_defs.md#createvpclinkresponsetypedef)


```python
# create_vpc_link method usage example with argument unpacking

kwargs: CreateVpcLinkRequestTypeDef = {  # (1)
    "Name": ...,
    "SubnetIds": ...,
}

parent.create_vpc_link(**kwargs)
```

1. See [:material-code-braces: CreateVpcLinkRequestTypeDef](./type_defs.md#createvpclinkrequesttypedef)

### delete\_access\_log\_settings

Deletes the AccessLogSettings for a Stage.

Type annotations and code completion for `#!python session.client("apigatewayv2").delete_access_log_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# delete_access_log_settings method definition

await def delete_access_log_settings(
    self,
    *,
    ApiId: str,
    StageName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_access_log_settings method usage example with argument unpacking

kwargs: DeleteAccessLogSettingsRequestTypeDef = {  # (1)
    "ApiId": ...,
    "StageName": ...,
}

parent.delete_access_log_settings(**kwargs)
```

1. See [:material-code-braces: DeleteAccessLogSettingsRequestTypeDef](./type_defs.md#deleteaccesslogsettingsrequesttypedef)

### delete\_api

Deletes an Api resource.

Type annotations and code completion for `#!python session.client("apigatewayv2").delete_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# delete_api method definition

await def delete_api(
    self,
    *,
    ApiId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_api method usage example with argument unpacking

kwargs: DeleteApiRequestTypeDef = {  # (1)
    "ApiId": ...,
}

parent.delete_api(**kwargs)
```

1. See [:material-code-braces: DeleteApiRequestTypeDef](./type_defs.md#deleteapirequesttypedef)

### delete\_api\_mapping

Deletes an API mapping.

Type annotations and code completion for `#!python session.client("apigatewayv2").delete_api_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# delete_api_mapping method definition

await def delete_api_mapping(
    self,
    *,
    ApiMappingId: str,
    DomainName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_api_mapping method usage example with argument unpacking

kwargs: DeleteApiMappingRequestTypeDef = {  # (1)
    "ApiMappingId": ...,
    "DomainName": ...,
}

parent.delete_api_mapping(**kwargs)
```

1. See [:material-code-braces: DeleteApiMappingRequestTypeDef](./type_defs.md#deleteapimappingrequesttypedef)

### delete\_authorizer

Deletes an Authorizer.

Type annotations and code completion for `#!python session.client("apigatewayv2").delete_authorizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# delete_authorizer method definition

await def delete_authorizer(
    self,
    *,
    ApiId: str,
    AuthorizerId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_authorizer method usage example with argument unpacking

kwargs: DeleteAuthorizerRequestTypeDef = {  # (1)
    "ApiId": ...,
    "AuthorizerId": ...,
}

parent.delete_authorizer(**kwargs)
```

1. See [:material-code-braces: DeleteAuthorizerRequestTypeDef](./type_defs.md#deleteauthorizerrequesttypedef)

### delete\_cors\_configuration

Deletes a CORS configuration.

Type annotations and code completion for `#!python session.client("apigatewayv2").delete_cors_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# delete_cors_configuration method definition

await def delete_cors_configuration(
    self,
    *,
    ApiId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_cors_configuration method usage example with argument unpacking

kwargs: DeleteCorsConfigurationRequestTypeDef = {  # (1)
    "ApiId": ...,
}

parent.delete_cors_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteCorsConfigurationRequestTypeDef](./type_defs.md#deletecorsconfigurationrequesttypedef)

### delete\_deployment

Deletes a Deployment.

Type annotations and code completion for `#!python session.client("apigatewayv2").delete_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# delete_deployment method definition

await def delete_deployment(
    self,
    *,
    ApiId: str,
    DeploymentId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_deployment method usage example with argument unpacking

kwargs: DeleteDeploymentRequestTypeDef = {  # (1)
    "ApiId": ...,
    "DeploymentId": ...,
}

parent.delete_deployment(**kwargs)
```

1. See [:material-code-braces: DeleteDeploymentRequestTypeDef](./type_defs.md#deletedeploymentrequesttypedef)

### delete\_domain\_name

Deletes a domain name.

Type annotations and code completion for `#!python session.client("apigatewayv2").delete_domain_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# delete_domain_name method definition

await def delete_domain_name(
    self,
    *,
    DomainName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_domain_name method usage example with argument unpacking

kwargs: DeleteDomainNameRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.delete_domain_name(**kwargs)
```

1. See [:material-code-braces: DeleteDomainNameRequestTypeDef](./type_defs.md#deletedomainnamerequesttypedef)

### delete\_integration

Deletes an Integration.

Type annotations and code completion for `#!python session.client("apigatewayv2").delete_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# delete_integration method definition

await def delete_integration(
    self,
    *,
    ApiId: str,
    IntegrationId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_integration method usage example with argument unpacking

kwargs: DeleteIntegrationRequestTypeDef = {  # (1)
    "ApiId": ...,
    "IntegrationId": ...,
}

parent.delete_integration(**kwargs)
```

1. See [:material-code-braces: DeleteIntegrationRequestTypeDef](./type_defs.md#deleteintegrationrequesttypedef)

### delete\_integration\_response

Deletes an IntegrationResponses.

Type annotations and code completion for `#!python session.client("apigatewayv2").delete_integration_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# delete_integration_response method definition

await def delete_integration_response(
    self,
    *,
    ApiId: str,
    IntegrationId: str,
    IntegrationResponseId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_integration_response method usage example with argument unpacking

kwargs: DeleteIntegrationResponseRequestTypeDef = {  # (1)
    "ApiId": ...,
    "IntegrationId": ...,
    "IntegrationResponseId": ...,
}

parent.delete_integration_response(**kwargs)
```

1. See [:material-code-braces: DeleteIntegrationResponseRequestTypeDef](./type_defs.md#deleteintegrationresponserequesttypedef)

### delete\_model

Deletes a Model.

Type annotations and code completion for `#!python session.client("apigatewayv2").delete_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# delete_model method definition

await def delete_model(
    self,
    *,
    ApiId: str,
    ModelId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_model method usage example with argument unpacking

kwargs: DeleteModelRequestTypeDef = {  # (1)
    "ApiId": ...,
    "ModelId": ...,
}

parent.delete_model(**kwargs)
```

1. See [:material-code-braces: DeleteModelRequestTypeDef](./type_defs.md#deletemodelrequesttypedef)

### delete\_route

Deletes a Route.

Type annotations and code completion for `#!python session.client("apigatewayv2").delete_route` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# delete_route method definition

await def delete_route(
    self,
    *,
    ApiId: str,
    RouteId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_route method usage example with argument unpacking

kwargs: DeleteRouteRequestTypeDef = {  # (1)
    "ApiId": ...,
    "RouteId": ...,
}

parent.delete_route(**kwargs)
```

1. See [:material-code-braces: DeleteRouteRequestTypeDef](./type_defs.md#deleterouterequesttypedef)

### delete\_route\_request\_parameter

Deletes a route request parameter.

Type annotations and code completion for `#!python session.client("apigatewayv2").delete_route_request_parameter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# delete_route_request_parameter method definition

await def delete_route_request_parameter(
    self,
    *,
    ApiId: str,
    RequestParameterKey: str,
    RouteId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_route_request_parameter method usage example with argument unpacking

kwargs: DeleteRouteRequestParameterRequestTypeDef = {  # (1)
    "ApiId": ...,
    "RequestParameterKey": ...,
    "RouteId": ...,
}

parent.delete_route_request_parameter(**kwargs)
```

1. See [:material-code-braces: DeleteRouteRequestParameterRequestTypeDef](./type_defs.md#deleterouterequestparameterrequesttypedef)

### delete\_route\_response

Deletes a RouteResponse.

Type annotations and code completion for `#!python session.client("apigatewayv2").delete_route_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# delete_route_response method definition

await def delete_route_response(
    self,
    *,
    ApiId: str,
    RouteId: str,
    RouteResponseId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_route_response method usage example with argument unpacking

kwargs: DeleteRouteResponseRequestTypeDef = {  # (1)
    "ApiId": ...,
    "RouteId": ...,
    "RouteResponseId": ...,
}

parent.delete_route_response(**kwargs)
```

1. See [:material-code-braces: DeleteRouteResponseRequestTypeDef](./type_defs.md#deleterouteresponserequesttypedef)

### delete\_route\_settings

Deletes the RouteSettings for a stage.

Type annotations and code completion for `#!python session.client("apigatewayv2").delete_route_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# delete_route_settings method definition

await def delete_route_settings(
    self,
    *,
    ApiId: str,
    RouteKey: str,
    StageName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_route_settings method usage example with argument unpacking

kwargs: DeleteRouteSettingsRequestTypeDef = {  # (1)
    "ApiId": ...,
    "RouteKey": ...,
    "StageName": ...,
}

parent.delete_route_settings(**kwargs)
```

1. See [:material-code-braces: DeleteRouteSettingsRequestTypeDef](./type_defs.md#deleteroutesettingsrequesttypedef)

### delete\_stage

Deletes a Stage.

Type annotations and code completion for `#!python session.client("apigatewayv2").delete_stage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# delete_stage method definition

await def delete_stage(
    self,
    *,
    ApiId: str,
    StageName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_stage method usage example with argument unpacking

kwargs: DeleteStageRequestTypeDef = {  # (1)
    "ApiId": ...,
    "StageName": ...,
}

parent.delete_stage(**kwargs)
```

1. See [:material-code-braces: DeleteStageRequestTypeDef](./type_defs.md#deletestagerequesttypedef)

### delete\_vpc\_link

Deletes a VPC link.

Type annotations and code completion for `#!python session.client("apigatewayv2").delete_vpc_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# delete_vpc_link method definition

await def delete_vpc_link(
    self,
    *,
    VpcLinkId: str,
) -> Dict[str, Any]:
    ...
```

```python
# delete_vpc_link method usage example with argument unpacking

kwargs: DeleteVpcLinkRequestTypeDef = {  # (1)
    "VpcLinkId": ...,
}

parent.delete_vpc_link(**kwargs)
```

1. See [:material-code-braces: DeleteVpcLinkRequestTypeDef](./type_defs.md#deletevpclinkrequesttypedef)

### export\_api



Type annotations and code completion for `#!python session.client("apigatewayv2").export_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# export_api method definition

await def export_api(
    self,
    *,
    ApiId: str,
    OutputType: JSONYAMLType,  # (1)
    Specification: OAS30Type,  # (2)
    ExportVersion: str = ...,
    IncludeExtensions: bool = ...,
    StageName: str = ...,
) -> ExportApiResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: JSONYAMLType](./literals.md#jsonyamltype)
2. See [:material-code-brackets: OAS30Type](./literals.md#oas30type)
3. See [:material-code-braces: ExportApiResponseTypeDef](./type_defs.md#exportapiresponsetypedef)


```python
# export_api method usage example with argument unpacking

kwargs: ExportApiRequestTypeDef = {  # (1)
    "ApiId": ...,
    "OutputType": ...,
    "Specification": ...,
}

parent.export_api(**kwargs)
```

1. See [:material-code-braces: ExportApiRequestTypeDef](./type_defs.md#exportapirequesttypedef)

### reset\_authorizers\_cache

Resets all authorizer cache entries on a stage.

Type annotations and code completion for `#!python session.client("apigatewayv2").reset_authorizers_cache` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# reset_authorizers_cache method definition

await def reset_authorizers_cache(
    self,
    *,
    ApiId: str,
    StageName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# reset_authorizers_cache method usage example with argument unpacking

kwargs: ResetAuthorizersCacheRequestTypeDef = {  # (1)
    "ApiId": ...,
    "StageName": ...,
}

parent.reset_authorizers_cache(**kwargs)
```

1. See [:material-code-braces: ResetAuthorizersCacheRequestTypeDef](./type_defs.md#resetauthorizerscacherequesttypedef)

### get\_api

Gets an Api resource.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_api method definition

await def get_api(
    self,
    *,
    ApiId: str,
) -> GetApiResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetApiResponseTypeDef](./type_defs.md#getapiresponsetypedef)


```python
# get_api method usage example with argument unpacking

kwargs: GetApiRequestTypeDef = {  # (1)
    "ApiId": ...,
}

parent.get_api(**kwargs)
```

1. See [:material-code-braces: GetApiRequestTypeDef](./type_defs.md#getapirequesttypedef)

### get\_api\_mapping

Gets an API mapping.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_api_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_api_mapping method definition

await def get_api_mapping(
    self,
    *,
    ApiMappingId: str,
    DomainName: str,
) -> GetApiMappingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetApiMappingResponseTypeDef](./type_defs.md#getapimappingresponsetypedef)


```python
# get_api_mapping method usage example with argument unpacking

kwargs: GetApiMappingRequestTypeDef = {  # (1)
    "ApiMappingId": ...,
    "DomainName": ...,
}

parent.get_api_mapping(**kwargs)
```

1. See [:material-code-braces: GetApiMappingRequestTypeDef](./type_defs.md#getapimappingrequesttypedef)

### get\_api\_mappings

Gets API mappings.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_api_mappings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_api_mappings method definition

await def get_api_mappings(
    self,
    *,
    DomainName: str,
    MaxResults: str = ...,
    NextToken: str = ...,
) -> GetApiMappingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetApiMappingsResponseTypeDef](./type_defs.md#getapimappingsresponsetypedef)


```python
# get_api_mappings method usage example with argument unpacking

kwargs: GetApiMappingsRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.get_api_mappings(**kwargs)
```

1. See [:material-code-braces: GetApiMappingsRequestTypeDef](./type_defs.md#getapimappingsrequesttypedef)

### get\_apis

Gets a collection of Api resources.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_apis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_apis method definition

await def get_apis(
    self,
    *,
    MaxResults: str = ...,
    NextToken: str = ...,
) -> GetApisResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetApisResponseTypeDef](./type_defs.md#getapisresponsetypedef)


```python
# get_apis method usage example with argument unpacking

kwargs: GetApisRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.get_apis(**kwargs)
```

1. See [:material-code-braces: GetApisRequestTypeDef](./type_defs.md#getapisrequesttypedef)

### get\_authorizer

Gets an Authorizer.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_authorizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_authorizer method definition

await def get_authorizer(
    self,
    *,
    ApiId: str,
    AuthorizerId: str,
) -> GetAuthorizerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAuthorizerResponseTypeDef](./type_defs.md#getauthorizerresponsetypedef)


```python
# get_authorizer method usage example with argument unpacking

kwargs: GetAuthorizerRequestTypeDef = {  # (1)
    "ApiId": ...,
    "AuthorizerId": ...,
}

parent.get_authorizer(**kwargs)
```

1. See [:material-code-braces: GetAuthorizerRequestTypeDef](./type_defs.md#getauthorizerrequesttypedef)

### get\_authorizers

Gets the Authorizers for an API.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_authorizers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_authorizers method definition

await def get_authorizers(
    self,
    *,
    ApiId: str,
    MaxResults: str = ...,
    NextToken: str = ...,
) -> GetAuthorizersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAuthorizersResponseTypeDef](./type_defs.md#getauthorizersresponsetypedef)


```python
# get_authorizers method usage example with argument unpacking

kwargs: GetAuthorizersRequestTypeDef = {  # (1)
    "ApiId": ...,
}

parent.get_authorizers(**kwargs)
```

1. See [:material-code-braces: GetAuthorizersRequestTypeDef](./type_defs.md#getauthorizersrequesttypedef)

### get\_deployment

Gets a Deployment.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_deployment method definition

await def get_deployment(
    self,
    *,
    ApiId: str,
    DeploymentId: str,
) -> GetDeploymentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeploymentResponseTypeDef](./type_defs.md#getdeploymentresponsetypedef)


```python
# get_deployment method usage example with argument unpacking

kwargs: GetDeploymentRequestTypeDef = {  # (1)
    "ApiId": ...,
    "DeploymentId": ...,
}

parent.get_deployment(**kwargs)
```

1. See [:material-code-braces: GetDeploymentRequestTypeDef](./type_defs.md#getdeploymentrequesttypedef)

### get\_deployments

Gets the Deployments for an API.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_deployments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_deployments method definition

await def get_deployments(
    self,
    *,
    ApiId: str,
    MaxResults: str = ...,
    NextToken: str = ...,
) -> GetDeploymentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeploymentsResponseTypeDef](./type_defs.md#getdeploymentsresponsetypedef)


```python
# get_deployments method usage example with argument unpacking

kwargs: GetDeploymentsRequestTypeDef = {  # (1)
    "ApiId": ...,
}

parent.get_deployments(**kwargs)
```

1. See [:material-code-braces: GetDeploymentsRequestTypeDef](./type_defs.md#getdeploymentsrequesttypedef)

### get\_domain\_name

Gets a domain name.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_domain_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_domain_name method definition

await def get_domain_name(
    self,
    *,
    DomainName: str,
) -> GetDomainNameResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDomainNameResponseTypeDef](./type_defs.md#getdomainnameresponsetypedef)


```python
# get_domain_name method usage example with argument unpacking

kwargs: GetDomainNameRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.get_domain_name(**kwargs)
```

1. See [:material-code-braces: GetDomainNameRequestTypeDef](./type_defs.md#getdomainnamerequesttypedef)

### get\_domain\_names

Gets the domain names for an AWS account.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_domain_names` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_domain_names method definition

await def get_domain_names(
    self,
    *,
    MaxResults: str = ...,
    NextToken: str = ...,
) -> GetDomainNamesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDomainNamesResponseTypeDef](./type_defs.md#getdomainnamesresponsetypedef)


```python
# get_domain_names method usage example with argument unpacking

kwargs: GetDomainNamesRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.get_domain_names(**kwargs)
```

1. See [:material-code-braces: GetDomainNamesRequestTypeDef](./type_defs.md#getdomainnamesrequesttypedef)

### get\_integration

Gets an Integration.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_integration method definition

await def get_integration(
    self,
    *,
    ApiId: str,
    IntegrationId: str,
) -> GetIntegrationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIntegrationResultTypeDef](./type_defs.md#getintegrationresulttypedef)


```python
# get_integration method usage example with argument unpacking

kwargs: GetIntegrationRequestTypeDef = {  # (1)
    "ApiId": ...,
    "IntegrationId": ...,
}

parent.get_integration(**kwargs)
```

1. See [:material-code-braces: GetIntegrationRequestTypeDef](./type_defs.md#getintegrationrequesttypedef)

### get\_integration\_response

Gets an IntegrationResponses.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_integration_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_integration_response method definition

await def get_integration_response(
    self,
    *,
    ApiId: str,
    IntegrationId: str,
    IntegrationResponseId: str,
) -> GetIntegrationResponseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIntegrationResponseResponseTypeDef](./type_defs.md#getintegrationresponseresponsetypedef)


```python
# get_integration_response method usage example with argument unpacking

kwargs: GetIntegrationResponseRequestTypeDef = {  # (1)
    "ApiId": ...,
    "IntegrationId": ...,
    "IntegrationResponseId": ...,
}

parent.get_integration_response(**kwargs)
```

1. See [:material-code-braces: GetIntegrationResponseRequestTypeDef](./type_defs.md#getintegrationresponserequesttypedef)

### get\_integration\_responses

Gets the IntegrationResponses for an Integration.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_integration_responses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_integration_responses method definition

await def get_integration_responses(
    self,
    *,
    ApiId: str,
    IntegrationId: str,
    MaxResults: str = ...,
    NextToken: str = ...,
) -> GetIntegrationResponsesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIntegrationResponsesResponseTypeDef](./type_defs.md#getintegrationresponsesresponsetypedef)


```python
# get_integration_responses method usage example with argument unpacking

kwargs: GetIntegrationResponsesRequestTypeDef = {  # (1)
    "ApiId": ...,
    "IntegrationId": ...,
}

parent.get_integration_responses(**kwargs)
```

1. See [:material-code-braces: GetIntegrationResponsesRequestTypeDef](./type_defs.md#getintegrationresponsesrequesttypedef)

### get\_integrations

Gets the Integrations for an API.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_integrations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_integrations method definition

await def get_integrations(
    self,
    *,
    ApiId: str,
    MaxResults: str = ...,
    NextToken: str = ...,
) -> GetIntegrationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIntegrationsResponseTypeDef](./type_defs.md#getintegrationsresponsetypedef)


```python
# get_integrations method usage example with argument unpacking

kwargs: GetIntegrationsRequestTypeDef = {  # (1)
    "ApiId": ...,
}

parent.get_integrations(**kwargs)
```

1. See [:material-code-braces: GetIntegrationsRequestTypeDef](./type_defs.md#getintegrationsrequesttypedef)

### get\_model

Gets a Model.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_model method definition

await def get_model(
    self,
    *,
    ApiId: str,
    ModelId: str,
) -> GetModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetModelResponseTypeDef](./type_defs.md#getmodelresponsetypedef)


```python
# get_model method usage example with argument unpacking

kwargs: GetModelRequestTypeDef = {  # (1)
    "ApiId": ...,
    "ModelId": ...,
}

parent.get_model(**kwargs)
```

1. See [:material-code-braces: GetModelRequestTypeDef](./type_defs.md#getmodelrequesttypedef)

### get\_model\_template

Gets a model template.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_model_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_model_template method definition

await def get_model_template(
    self,
    *,
    ApiId: str,
    ModelId: str,
) -> GetModelTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetModelTemplateResponseTypeDef](./type_defs.md#getmodeltemplateresponsetypedef)


```python
# get_model_template method usage example with argument unpacking

kwargs: GetModelTemplateRequestTypeDef = {  # (1)
    "ApiId": ...,
    "ModelId": ...,
}

parent.get_model_template(**kwargs)
```

1. See [:material-code-braces: GetModelTemplateRequestTypeDef](./type_defs.md#getmodeltemplaterequesttypedef)

### get\_models

Gets the Models for an API.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_models` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_models method definition

await def get_models(
    self,
    *,
    ApiId: str,
    MaxResults: str = ...,
    NextToken: str = ...,
) -> GetModelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetModelsResponseTypeDef](./type_defs.md#getmodelsresponsetypedef)


```python
# get_models method usage example with argument unpacking

kwargs: GetModelsRequestTypeDef = {  # (1)
    "ApiId": ...,
}

parent.get_models(**kwargs)
```

1. See [:material-code-braces: GetModelsRequestTypeDef](./type_defs.md#getmodelsrequesttypedef)

### get\_route

Gets a Route.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_route` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_route method definition

await def get_route(
    self,
    *,
    ApiId: str,
    RouteId: str,
) -> GetRouteResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRouteResultTypeDef](./type_defs.md#getrouteresulttypedef)


```python
# get_route method usage example with argument unpacking

kwargs: GetRouteRequestTypeDef = {  # (1)
    "ApiId": ...,
    "RouteId": ...,
}

parent.get_route(**kwargs)
```

1. See [:material-code-braces: GetRouteRequestTypeDef](./type_defs.md#getrouterequesttypedef)

### get\_route\_response

Gets a RouteResponse.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_route_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_route_response method definition

await def get_route_response(
    self,
    *,
    ApiId: str,
    RouteId: str,
    RouteResponseId: str,
) -> GetRouteResponseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRouteResponseResponseTypeDef](./type_defs.md#getrouteresponseresponsetypedef)


```python
# get_route_response method usage example with argument unpacking

kwargs: GetRouteResponseRequestTypeDef = {  # (1)
    "ApiId": ...,
    "RouteId": ...,
    "RouteResponseId": ...,
}

parent.get_route_response(**kwargs)
```

1. See [:material-code-braces: GetRouteResponseRequestTypeDef](./type_defs.md#getrouteresponserequesttypedef)

### get\_route\_responses

Gets the RouteResponses for a Route.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_route_responses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_route_responses method definition

await def get_route_responses(
    self,
    *,
    ApiId: str,
    RouteId: str,
    MaxResults: str = ...,
    NextToken: str = ...,
) -> GetRouteResponsesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRouteResponsesResponseTypeDef](./type_defs.md#getrouteresponsesresponsetypedef)


```python
# get_route_responses method usage example with argument unpacking

kwargs: GetRouteResponsesRequestTypeDef = {  # (1)
    "ApiId": ...,
    "RouteId": ...,
}

parent.get_route_responses(**kwargs)
```

1. See [:material-code-braces: GetRouteResponsesRequestTypeDef](./type_defs.md#getrouteresponsesrequesttypedef)

### get\_routes

Gets the Routes for an API.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_routes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_routes method definition

await def get_routes(
    self,
    *,
    ApiId: str,
    MaxResults: str = ...,
    NextToken: str = ...,
) -> GetRoutesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRoutesResponseTypeDef](./type_defs.md#getroutesresponsetypedef)


```python
# get_routes method usage example with argument unpacking

kwargs: GetRoutesRequestTypeDef = {  # (1)
    "ApiId": ...,
}

parent.get_routes(**kwargs)
```

1. See [:material-code-braces: GetRoutesRequestTypeDef](./type_defs.md#getroutesrequesttypedef)

### get\_stage

Gets a Stage.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_stage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_stage method definition

await def get_stage(
    self,
    *,
    ApiId: str,
    StageName: str,
) -> GetStageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStageResponseTypeDef](./type_defs.md#getstageresponsetypedef)


```python
# get_stage method usage example with argument unpacking

kwargs: GetStageRequestTypeDef = {  # (1)
    "ApiId": ...,
    "StageName": ...,
}

parent.get_stage(**kwargs)
```

1. See [:material-code-braces: GetStageRequestTypeDef](./type_defs.md#getstagerequesttypedef)

### get\_stages

Gets the Stages for an API.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_stages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_stages method definition

await def get_stages(
    self,
    *,
    ApiId: str,
    MaxResults: str = ...,
    NextToken: str = ...,
) -> GetStagesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStagesResponseTypeDef](./type_defs.md#getstagesresponsetypedef)


```python
# get_stages method usage example with argument unpacking

kwargs: GetStagesRequestTypeDef = {  # (1)
    "ApiId": ...,
}

parent.get_stages(**kwargs)
```

1. See [:material-code-braces: GetStagesRequestTypeDef](./type_defs.md#getstagesrequesttypedef)

### get\_tags

Gets a collection of Tag resources.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_tags method definition

await def get_tags(
    self,
    *,
    ResourceArn: str,
) -> GetTagsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTagsResponseTypeDef](./type_defs.md#gettagsresponsetypedef)


```python
# get_tags method usage example with argument unpacking

kwargs: GetTagsRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_tags(**kwargs)
```

1. See [:material-code-braces: GetTagsRequestTypeDef](./type_defs.md#gettagsrequesttypedef)

### get\_vpc\_link

Gets a VPC link.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_vpc_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_vpc_link method definition

await def get_vpc_link(
    self,
    *,
    VpcLinkId: str,
) -> GetVpcLinkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVpcLinkResponseTypeDef](./type_defs.md#getvpclinkresponsetypedef)


```python
# get_vpc_link method usage example with argument unpacking

kwargs: GetVpcLinkRequestTypeDef = {  # (1)
    "VpcLinkId": ...,
}

parent.get_vpc_link(**kwargs)
```

1. See [:material-code-braces: GetVpcLinkRequestTypeDef](./type_defs.md#getvpclinkrequesttypedef)

### get\_vpc\_links

Gets a collection of VPC links.

Type annotations and code completion for `#!python session.client("apigatewayv2").get_vpc_links` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# get_vpc_links method definition

await def get_vpc_links(
    self,
    *,
    MaxResults: str = ...,
    NextToken: str = ...,
) -> GetVpcLinksResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVpcLinksResponseTypeDef](./type_defs.md#getvpclinksresponsetypedef)


```python
# get_vpc_links method usage example with argument unpacking

kwargs: GetVpcLinksRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.get_vpc_links(**kwargs)
```

1. See [:material-code-braces: GetVpcLinksRequestTypeDef](./type_defs.md#getvpclinksrequesttypedef)

### import\_api

Imports an API.

Type annotations and code completion for `#!python session.client("apigatewayv2").import_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# import_api method definition

await def import_api(
    self,
    *,
    Body: str,
    Basepath: str = ...,
    FailOnWarnings: bool = ...,
) -> ImportApiResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ImportApiResponseTypeDef](./type_defs.md#importapiresponsetypedef)


```python
# import_api method usage example with argument unpacking

kwargs: ImportApiRequestTypeDef = {  # (1)
    "Body": ...,
}

parent.import_api(**kwargs)
```

1. See [:material-code-braces: ImportApiRequestTypeDef](./type_defs.md#importapirequesttypedef)

### reimport\_api

Puts an Api resource.

Type annotations and code completion for `#!python session.client("apigatewayv2").reimport_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# reimport_api method definition

await def reimport_api(
    self,
    *,
    ApiId: str,
    Body: str,
    Basepath: str = ...,
    FailOnWarnings: bool = ...,
) -> ReimportApiResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ReimportApiResponseTypeDef](./type_defs.md#reimportapiresponsetypedef)


```python
# reimport_api method usage example with argument unpacking

kwargs: ReimportApiRequestTypeDef = {  # (1)
    "ApiId": ...,
    "Body": ...,
}

parent.reimport_api(**kwargs)
```

1. See [:material-code-braces: ReimportApiRequestTypeDef](./type_defs.md#reimportapirequesttypedef)

### tag\_resource

Creates a new Tag resource to represent a tag.

Type annotations and code completion for `#!python session.client("apigatewayv2").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str] = ...,
) -> Dict[str, Any]:
    ...
```

```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)

### untag\_resource

Deletes a Tag.

Type annotations and code completion for `#!python session.client("apigatewayv2").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

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

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)

### update\_api

Updates an Api resource.

Type annotations and code completion for `#!python session.client("apigatewayv2").update_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# update_api method definition

await def update_api(
    self,
    *,
    ApiId: str,
    ApiKeySelectionExpression: str = ...,
    CorsConfiguration: CorsUnionTypeDef = ...,  # (1)
    CredentialsArn: str = ...,
    Description: str = ...,
    DisableSchemaValidation: bool = ...,
    DisableExecuteApiEndpoint: bool = ...,
    Name: str = ...,
    RouteKey: str = ...,
    RouteSelectionExpression: str = ...,
    Target: str = ...,
    Version: str = ...,
) -> UpdateApiResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CorsUnionTypeDef](#corsuniontypedef)
2. See [:material-code-braces: UpdateApiResponseTypeDef](./type_defs.md#updateapiresponsetypedef)


```python
# update_api method usage example with argument unpacking

kwargs: UpdateApiRequestTypeDef = {  # (1)
    "ApiId": ...,
}

parent.update_api(**kwargs)
```

1. See [:material-code-braces: UpdateApiRequestTypeDef](./type_defs.md#updateapirequesttypedef)

### update\_api\_mapping

The API mapping.

Type annotations and code completion for `#!python session.client("apigatewayv2").update_api_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# update_api_mapping method definition

await def update_api_mapping(
    self,
    *,
    ApiId: str,
    ApiMappingId: str,
    DomainName: str,
    ApiMappingKey: str = ...,
    Stage: str = ...,
) -> UpdateApiMappingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateApiMappingResponseTypeDef](./type_defs.md#updateapimappingresponsetypedef)


```python
# update_api_mapping method usage example with argument unpacking

kwargs: UpdateApiMappingRequestTypeDef = {  # (1)
    "ApiId": ...,
    "ApiMappingId": ...,
    "DomainName": ...,
}

parent.update_api_mapping(**kwargs)
```

1. See [:material-code-braces: UpdateApiMappingRequestTypeDef](./type_defs.md#updateapimappingrequesttypedef)

### update\_authorizer

Updates an Authorizer.

Type annotations and code completion for `#!python session.client("apigatewayv2").update_authorizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# update_authorizer method definition

await def update_authorizer(
    self,
    *,
    ApiId: str,
    AuthorizerId: str,
    AuthorizerCredentialsArn: str = ...,
    AuthorizerPayloadFormatVersion: str = ...,
    AuthorizerResultTtlInSeconds: int = ...,
    AuthorizerType: AuthorizerTypeType = ...,  # (1)
    AuthorizerUri: str = ...,
    EnableSimpleResponses: bool = ...,
    IdentitySource: Sequence[str] = ...,
    IdentityValidationExpression: str = ...,
    JwtConfiguration: JWTConfigurationUnionTypeDef = ...,  # (2)
    Name: str = ...,
) -> UpdateAuthorizerResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AuthorizerTypeType](./literals.md#authorizertypetype)
2. See [:material-code-braces: JWTConfigurationUnionTypeDef](#jwtconfigurationuniontypedef)
3. See [:material-code-braces: UpdateAuthorizerResponseTypeDef](./type_defs.md#updateauthorizerresponsetypedef)


```python
# update_authorizer method usage example with argument unpacking

kwargs: UpdateAuthorizerRequestTypeDef = {  # (1)
    "ApiId": ...,
    "AuthorizerId": ...,
}

parent.update_authorizer(**kwargs)
```

1. See [:material-code-braces: UpdateAuthorizerRequestTypeDef](./type_defs.md#updateauthorizerrequesttypedef)

### update\_deployment

Updates a Deployment.

Type annotations and code completion for `#!python session.client("apigatewayv2").update_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# update_deployment method definition

await def update_deployment(
    self,
    *,
    ApiId: str,
    DeploymentId: str,
    Description: str = ...,
) -> UpdateDeploymentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateDeploymentResponseTypeDef](./type_defs.md#updatedeploymentresponsetypedef)


```python
# update_deployment method usage example with argument unpacking

kwargs: UpdateDeploymentRequestTypeDef = {  # (1)
    "ApiId": ...,
    "DeploymentId": ...,
}

parent.update_deployment(**kwargs)
```

1. See [:material-code-braces: UpdateDeploymentRequestTypeDef](./type_defs.md#updatedeploymentrequesttypedef)

### update\_domain\_name

Updates a domain name.

Type annotations and code completion for `#!python session.client("apigatewayv2").update_domain_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# update_domain_name method definition

await def update_domain_name(
    self,
    *,
    DomainName: str,
    DomainNameConfigurations: Sequence[DomainNameConfigurationUnionTypeDef] = ...,  # (1)
    MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...,  # (2)
) -> UpdateDomainNameResponseTypeDef:  # (3)
    ...
```

1. See `Sequence[DomainNameConfigurationUnionTypeDef]`
2. See [:material-code-braces: MutualTlsAuthenticationInputTypeDef](./type_defs.md#mutualtlsauthenticationinputtypedef)
3. See [:material-code-braces: UpdateDomainNameResponseTypeDef](./type_defs.md#updatedomainnameresponsetypedef)


```python
# update_domain_name method usage example with argument unpacking

kwargs: UpdateDomainNameRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.update_domain_name(**kwargs)
```

1. See [:material-code-braces: UpdateDomainNameRequestTypeDef](./type_defs.md#updatedomainnamerequesttypedef)

### update\_integration

Updates an Integration.

Type annotations and code completion for `#!python session.client("apigatewayv2").update_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# update_integration method definition

await def update_integration(
    self,
    *,
    ApiId: str,
    IntegrationId: str,
    ConnectionId: str = ...,
    ConnectionType: ConnectionTypeType = ...,  # (1)
    ContentHandlingStrategy: ContentHandlingStrategyType = ...,  # (2)
    CredentialsArn: str = ...,
    Description: str = ...,
    IntegrationMethod: str = ...,
    IntegrationSubtype: str = ...,
    IntegrationType: IntegrationTypeType = ...,  # (3)
    IntegrationUri: str = ...,
    PassthroughBehavior: PassthroughBehaviorType = ...,  # (4)
    PayloadFormatVersion: str = ...,
    RequestParameters: Mapping[str, str] = ...,
    RequestTemplates: Mapping[str, str] = ...,
    ResponseParameters: Mapping[str, Mapping[str, str]] = ...,
    TemplateSelectionExpression: str = ...,
    TimeoutInMillis: int = ...,
    TlsConfig: TlsConfigInputTypeDef = ...,  # (5)
) -> UpdateIntegrationResultTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype)
2. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype)
3. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype)
4. See [:material-code-brackets: PassthroughBehaviorType](./literals.md#passthroughbehaviortype)
5. See [:material-code-braces: TlsConfigInputTypeDef](./type_defs.md#tlsconfiginputtypedef)
6. See [:material-code-braces: UpdateIntegrationResultTypeDef](./type_defs.md#updateintegrationresulttypedef)


```python
# update_integration method usage example with argument unpacking

kwargs: UpdateIntegrationRequestTypeDef = {  # (1)
    "ApiId": ...,
    "IntegrationId": ...,
}

parent.update_integration(**kwargs)
```

1. See [:material-code-braces: UpdateIntegrationRequestTypeDef](./type_defs.md#updateintegrationrequesttypedef)

### update\_integration\_response

Updates an IntegrationResponses.

Type annotations and code completion for `#!python session.client("apigatewayv2").update_integration_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# update_integration_response method definition

await def update_integration_response(
    self,
    *,
    ApiId: str,
    IntegrationId: str,
    IntegrationResponseId: str,
    ContentHandlingStrategy: ContentHandlingStrategyType = ...,  # (1)
    IntegrationResponseKey: str = ...,
    ResponseParameters: Mapping[str, str] = ...,
    ResponseTemplates: Mapping[str, str] = ...,
    TemplateSelectionExpression: str = ...,
) -> UpdateIntegrationResponseResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype)
2. See [:material-code-braces: UpdateIntegrationResponseResponseTypeDef](./type_defs.md#updateintegrationresponseresponsetypedef)


```python
# update_integration_response method usage example with argument unpacking

kwargs: UpdateIntegrationResponseRequestTypeDef = {  # (1)
    "ApiId": ...,
    "IntegrationId": ...,
    "IntegrationResponseId": ...,
}

parent.update_integration_response(**kwargs)
```

1. See [:material-code-braces: UpdateIntegrationResponseRequestTypeDef](./type_defs.md#updateintegrationresponserequesttypedef)

### update\_model

Updates a Model.

Type annotations and code completion for `#!python session.client("apigatewayv2").update_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# update_model method definition

await def update_model(
    self,
    *,
    ApiId: str,
    ModelId: str,
    ContentType: str = ...,
    Description: str = ...,
    Name: str = ...,
    Schema: str = ...,
) -> UpdateModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateModelResponseTypeDef](./type_defs.md#updatemodelresponsetypedef)


```python
# update_model method usage example with argument unpacking

kwargs: UpdateModelRequestTypeDef = {  # (1)
    "ApiId": ...,
    "ModelId": ...,
}

parent.update_model(**kwargs)
```

1. See [:material-code-braces: UpdateModelRequestTypeDef](./type_defs.md#updatemodelrequesttypedef)

### update\_route

Updates a Route.

Type annotations and code completion for `#!python session.client("apigatewayv2").update_route` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# update_route method definition

await def update_route(
    self,
    *,
    ApiId: str,
    RouteId: str,
    ApiKeyRequired: bool = ...,
    AuthorizationScopes: Sequence[str] = ...,
    AuthorizationType: AuthorizationTypeType = ...,  # (1)
    AuthorizerId: str = ...,
    ModelSelectionExpression: str = ...,
    OperationName: str = ...,
    RequestModels: Mapping[str, str] = ...,
    RequestParameters: Mapping[str, ParameterConstraintsTypeDef] = ...,  # (2)
    RouteKey: str = ...,
    RouteResponseSelectionExpression: str = ...,
    Target: str = ...,
) -> UpdateRouteResultTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AuthorizationTypeType](./literals.md#authorizationtypetype)
2. See `Mapping[str, ParameterConstraintsTypeDef]`
3. See [:material-code-braces: UpdateRouteResultTypeDef](./type_defs.md#updaterouteresulttypedef)


```python
# update_route method usage example with argument unpacking

kwargs: UpdateRouteRequestTypeDef = {  # (1)
    "ApiId": ...,
    "RouteId": ...,
}

parent.update_route(**kwargs)
```

1. See [:material-code-braces: UpdateRouteRequestTypeDef](./type_defs.md#updaterouterequesttypedef)

### update\_route\_response

Updates a RouteResponse.

Type annotations and code completion for `#!python session.client("apigatewayv2").update_route_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# update_route_response method definition

await def update_route_response(
    self,
    *,
    ApiId: str,
    RouteId: str,
    RouteResponseId: str,
    ModelSelectionExpression: str = ...,
    ResponseModels: Mapping[str, str] = ...,
    ResponseParameters: Mapping[str, ParameterConstraintsTypeDef] = ...,  # (1)
    RouteResponseKey: str = ...,
) -> UpdateRouteResponseResponseTypeDef:  # (2)
    ...
```

1. See `Mapping[str, ParameterConstraintsTypeDef]`
2. See [:material-code-braces: UpdateRouteResponseResponseTypeDef](./type_defs.md#updaterouteresponseresponsetypedef)


```python
# update_route_response method usage example with argument unpacking

kwargs: UpdateRouteResponseRequestTypeDef = {  # (1)
    "ApiId": ...,
    "RouteId": ...,
    "RouteResponseId": ...,
}

parent.update_route_response(**kwargs)
```

1. See [:material-code-braces: UpdateRouteResponseRequestTypeDef](./type_defs.md#updaterouteresponserequesttypedef)

### update\_stage

Updates a Stage.

Type annotations and code completion for `#!python session.client("apigatewayv2").update_stage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# update_stage method definition

await def update_stage(
    self,
    *,
    ApiId: str,
    StageName: str,
    AccessLogSettings: AccessLogSettingsTypeDef = ...,  # (1)
    AutoDeploy: bool = ...,
    ClientCertificateId: str = ...,
    DefaultRouteSettings: RouteSettingsTypeDef = ...,  # (2)
    DeploymentId: str = ...,
    Description: str = ...,
    RouteSettings: Mapping[str, RouteSettingsTypeDef] = ...,  # (3)
    StageVariables: Mapping[str, str] = ...,
) -> UpdateStageResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: AccessLogSettingsTypeDef](./type_defs.md#accesslogsettingstypedef)
2. See [:material-code-braces: RouteSettingsTypeDef](./type_defs.md#routesettingstypedef)
3. See `Mapping[str, RouteSettingsTypeDef]`
4. See [:material-code-braces: UpdateStageResponseTypeDef](./type_defs.md#updatestageresponsetypedef)


```python
# update_stage method usage example with argument unpacking

kwargs: UpdateStageRequestTypeDef = {  # (1)
    "ApiId": ...,
    "StageName": ...,
}

parent.update_stage(**kwargs)
```

1. See [:material-code-braces: UpdateStageRequestTypeDef](./type_defs.md#updatestagerequesttypedef)

### update\_vpc\_link

Updates a VPC link.

Type annotations and code completion for `#!python session.client("apigatewayv2").update_vpc_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# update_vpc_link method definition

await def update_vpc_link(
    self,
    *,
    VpcLinkId: str,
    Name: str = ...,
) -> UpdateVpcLinkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateVpcLinkResponseTypeDef](./type_defs.md#updatevpclinkresponsetypedef)


```python
# update_vpc_link method usage example with argument unpacking

kwargs: UpdateVpcLinkRequestTypeDef = {  # (1)
    "VpcLinkId": ...,
}

parent.update_vpc_link(**kwargs)
```

1. See [:material-code-braces: UpdateVpcLinkRequestTypeDef](./type_defs.md#updatevpclinkrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("apigatewayv2").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("apigatewayv2").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

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

Type annotations and code completion for `#!python session.client("apigatewayv2").get_paginator` method with overloads.

- `client.get_paginator("get_apis")` -> [GetApisPaginator](./paginators.md#getapispaginator)
- `client.get_paginator("get_authorizers")` -> [GetAuthorizersPaginator](./paginators.md#getauthorizerspaginator)
- `client.get_paginator("get_deployments")` -> [GetDeploymentsPaginator](./paginators.md#getdeploymentspaginator)
- `client.get_paginator("get_domain_names")` -> [GetDomainNamesPaginator](./paginators.md#getdomainnamespaginator)
- `client.get_paginator("get_integration_responses")` -> [GetIntegrationResponsesPaginator](./paginators.md#getintegrationresponsespaginator)
- `client.get_paginator("get_integrations")` -> [GetIntegrationsPaginator](./paginators.md#getintegrationspaginator)
- `client.get_paginator("get_models")` -> [GetModelsPaginator](./paginators.md#getmodelspaginator)
- `client.get_paginator("get_route_responses")` -> [GetRouteResponsesPaginator](./paginators.md#getrouteresponsespaginator)
- `client.get_paginator("get_routes")` -> [GetRoutesPaginator](./paginators.md#getroutespaginator)
- `client.get_paginator("get_stages")` -> [GetStagesPaginator](./paginators.md#getstagespaginator)



