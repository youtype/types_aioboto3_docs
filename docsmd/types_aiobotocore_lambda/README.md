# Lambda module

> [Index](../README.md) > Lambda


!!! note ""

    Auto-generated documentation for [Lambda](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#lambda)
    type annotations stubs module [types-aiobotocore-lambda](https://pypi.org/project/types-aiobotocore-lambda/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `Lambda` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `Lambda` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[lambda]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[lambda]'

# standalone installation
python -m pip install types-aiobotocore-lambda
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-lambda
```

## Usage

Code samples can be found in [Examples](./usage.md).

## LambdaClient

Type annotations and code completion for  `#!python session.client("lambda")` as [LambdaClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client)

```python
# LambdaClient usage example

from aioboto3.session import Session

from types_aiobotocore_lambda.client import LambdaClient


session = Session()
async with session.client("lambda") as client:
    client: LambdaClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("lambda").get_paginator("...")`.

```python
# ListAliasesPaginator usage example

from types_aiobotocore_lambda.paginator import ListAliasesPaginator

def get_list_aliases_paginator() -> ListAliasesPaginator:
    return client.get_paginator("list_aliases"))
```

- [ListAliasesPaginator](./paginators.md#listaliasespaginator)
- [ListCodeSigningConfigsPaginator](./paginators.md#listcodesigningconfigspaginator)
- [ListEventSourceMappingsPaginator](./paginators.md#listeventsourcemappingspaginator)
- [ListFunctionEventInvokeConfigsPaginator](./paginators.md#listfunctioneventinvokeconfigspaginator)
- [ListFunctionUrlConfigsPaginator](./paginators.md#listfunctionurlconfigspaginator)
- [ListFunctionsByCodeSigningConfigPaginator](./paginators.md#listfunctionsbycodesigningconfigpaginator)
- [ListFunctionsPaginator](./paginators.md#listfunctionspaginator)
- [ListLayerVersionsPaginator](./paginators.md#listlayerversionspaginator)
- [ListLayersPaginator](./paginators.md#listlayerspaginator)
- [ListProvisionedConcurrencyConfigsPaginator](./paginators.md#listprovisionedconcurrencyconfigspaginator)
- [ListVersionsByFunctionPaginator](./paginators.md#listversionsbyfunctionpaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.client("lambda").get_waiter("...")`.

```python
# FunctionActiveV2Waiter usage example

from types_aiobotocore_lambda.waiter import FunctionActiveV2Waiter

def get_function_active_v2_waiter() -> FunctionActiveV2Waiter:
    return Session().client("lambda").get_waiter("function_active_v2")
```

- [FunctionActiveV2Waiter](./waiters.md#functionactivev2waiter)
- [FunctionActiveWaiter](./waiters.md#functionactivewaiter)
- [FunctionExistsWaiter](./waiters.md#functionexistswaiter)
- [FunctionUpdatedV2Waiter](./waiters.md#functionupdatedv2waiter)
- [FunctionUpdatedWaiter](./waiters.md#functionupdatedwaiter)
- [PublishedVersionActiveWaiter](./waiters.md#publishedversionactivewaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ApplicationLogLevelType usage example

from types_aiobotocore_lambda.literals import ApplicationLogLevelType

def get_value() -> ApplicationLogLevelType:
    return "DEBUG"
```

- [ApplicationLogLevelType](./literals.md#applicationlogleveltype)
- [ArchitectureType](./literals.md#architecturetype)
- [CodeSigningPolicyType](./literals.md#codesigningpolicytype)
- [EndPointTypeType](./literals.md#endpointtypetype)
- [EventSourceMappingMetricType](./literals.md#eventsourcemappingmetrictype)
- [EventSourcePositionType](./literals.md#eventsourcepositiontype)
- [FullDocumentType](./literals.md#fulldocumenttype)
- [FunctionActiveV2WaiterName](./literals.md#functionactivev2waitername)
- [FunctionActiveWaiterName](./literals.md#functionactivewaitername)
- [FunctionExistsWaiterName](./literals.md#functionexistswaitername)
- [FunctionResponseTypeType](./literals.md#functionresponsetypetype)
- [FunctionUpdatedV2WaiterName](./literals.md#functionupdatedv2waitername)
- [FunctionUpdatedWaiterName](./literals.md#functionupdatedwaitername)
- [FunctionUrlAuthTypeType](./literals.md#functionurlauthtypetype)
- [FunctionVersionType](./literals.md#functionversiontype)
- [InvocationTypeType](./literals.md#invocationtypetype)
- [InvokeModeType](./literals.md#invokemodetype)
- [LastUpdateStatusReasonCodeType](./literals.md#lastupdatestatusreasoncodetype)
- [LastUpdateStatusType](./literals.md#lastupdatestatustype)
- [ListAliasesPaginatorName](./literals.md#listaliasespaginatorname)
- [ListCodeSigningConfigsPaginatorName](./literals.md#listcodesigningconfigspaginatorname)
- [ListEventSourceMappingsPaginatorName](./literals.md#listeventsourcemappingspaginatorname)
- [ListFunctionEventInvokeConfigsPaginatorName](./literals.md#listfunctioneventinvokeconfigspaginatorname)
- [ListFunctionUrlConfigsPaginatorName](./literals.md#listfunctionurlconfigspaginatorname)
- [ListFunctionsByCodeSigningConfigPaginatorName](./literals.md#listfunctionsbycodesigningconfigpaginatorname)
- [ListFunctionsPaginatorName](./literals.md#listfunctionspaginatorname)
- [ListLayerVersionsPaginatorName](./literals.md#listlayerversionspaginatorname)
- [ListLayersPaginatorName](./literals.md#listlayerspaginatorname)
- [ListProvisionedConcurrencyConfigsPaginatorName](./literals.md#listprovisionedconcurrencyconfigspaginatorname)
- [ListVersionsByFunctionPaginatorName](./literals.md#listversionsbyfunctionpaginatorname)
- [LogFormatType](./literals.md#logformattype)
- [LogTypeType](./literals.md#logtypetype)
- [PackageTypeType](./literals.md#packagetypetype)
- [ProvisionedConcurrencyStatusEnumType](./literals.md#provisionedconcurrencystatusenumtype)
- [PublishedVersionActiveWaiterName](./literals.md#publishedversionactivewaitername)
- [RecursiveLoopType](./literals.md#recursivelooptype)
- [ResponseStreamingInvocationTypeType](./literals.md#responsestreaminginvocationtypetype)
- [RuntimeType](./literals.md#runtimetype)
- [SnapStartApplyOnType](./literals.md#snapstartapplyontype)
- [SnapStartOptimizationStatusType](./literals.md#snapstartoptimizationstatustype)
- [SourceAccessTypeType](./literals.md#sourceaccesstypetype)
- [StateReasonCodeType](./literals.md#statereasoncodetype)
- [StateType](./literals.md#statetype)
- [SystemLogLevelType](./literals.md#systemlogleveltype)
- [TracingModeType](./literals.md#tracingmodetype)
- [UpdateRuntimeOnType](./literals.md#updateruntimeontype)
- [LambdaServiceName](./literals.md#lambdaservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccountLimitTypeDef](./type_defs.md#accountlimittypedef)
- [AccountUsageTypeDef](./type_defs.md#accountusagetypedef)
- [AddLayerVersionPermissionRequestRequestTypeDef](./type_defs.md#addlayerversionpermissionrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AddPermissionRequestRequestTypeDef](./type_defs.md#addpermissionrequestrequesttypedef)
- [AliasRoutingConfigurationOutputTypeDef](./type_defs.md#aliasroutingconfigurationoutputtypedef)
- [AliasRoutingConfigurationTypeDef](./type_defs.md#aliasroutingconfigurationtypedef)
- [AllowedPublishersOutputTypeDef](./type_defs.md#allowedpublishersoutputtypedef)
- [AllowedPublishersTypeDef](./type_defs.md#allowedpublisherstypedef)
- [AmazonManagedKafkaEventSourceConfigTypeDef](./type_defs.md#amazonmanagedkafkaeventsourceconfigtypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CodeSigningPoliciesTypeDef](./type_defs.md#codesigningpoliciestypedef)
- [ConcurrencyTypeDef](./type_defs.md#concurrencytypedef)
- [CorsOutputTypeDef](./type_defs.md#corsoutputtypedef)
- [CorsTypeDef](./type_defs.md#corstypedef)
- [DocumentDBEventSourceConfigTypeDef](./type_defs.md#documentdbeventsourceconfigtypedef)
- [EventSourceMappingMetricsConfigTypeDef](./type_defs.md#eventsourcemappingmetricsconfigtypedef)
- [ProvisionedPollerConfigTypeDef](./type_defs.md#provisionedpollerconfigtypedef)
- [ScalingConfigTypeDef](./type_defs.md#scalingconfigtypedef)
- [SelfManagedEventSourceTypeDef](./type_defs.md#selfmanagedeventsourcetypedef)
- [SelfManagedKafkaEventSourceConfigTypeDef](./type_defs.md#selfmanagedkafkaeventsourceconfigtypedef)
- [SourceAccessConfigurationTypeDef](./type_defs.md#sourceaccessconfigurationtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [DeadLetterConfigTypeDef](./type_defs.md#deadletterconfigtypedef)
- [EnvironmentTypeDef](./type_defs.md#environmenttypedef)
- [EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef)
- [FileSystemConfigTypeDef](./type_defs.md#filesystemconfigtypedef)
- [ImageConfigTypeDef](./type_defs.md#imageconfigtypedef)
- [LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef)
- [SnapStartTypeDef](./type_defs.md#snapstarttypedef)
- [TracingConfigTypeDef](./type_defs.md#tracingconfigtypedef)
- [VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef)
- [DeleteAliasRequestRequestTypeDef](./type_defs.md#deletealiasrequestrequesttypedef)
- [DeleteCodeSigningConfigRequestRequestTypeDef](./type_defs.md#deletecodesigningconfigrequestrequesttypedef)
- [DeleteEventSourceMappingRequestRequestTypeDef](./type_defs.md#deleteeventsourcemappingrequestrequesttypedef)
- [DeleteFunctionCodeSigningConfigRequestRequestTypeDef](./type_defs.md#deletefunctioncodesigningconfigrequestrequesttypedef)
- [DeleteFunctionConcurrencyRequestRequestTypeDef](./type_defs.md#deletefunctionconcurrencyrequestrequesttypedef)
- [DeleteFunctionEventInvokeConfigRequestRequestTypeDef](./type_defs.md#deletefunctioneventinvokeconfigrequestrequesttypedef)
- [DeleteFunctionRequestRequestTypeDef](./type_defs.md#deletefunctionrequestrequesttypedef)
- [DeleteFunctionUrlConfigRequestRequestTypeDef](./type_defs.md#deletefunctionurlconfigrequestrequesttypedef)
- [DeleteLayerVersionRequestRequestTypeDef](./type_defs.md#deletelayerversionrequestrequesttypedef)
- [DeleteProvisionedConcurrencyConfigRequestRequestTypeDef](./type_defs.md#deleteprovisionedconcurrencyconfigrequestrequesttypedef)
- [OnFailureTypeDef](./type_defs.md#onfailuretypedef)
- [OnSuccessTypeDef](./type_defs.md#onsuccesstypedef)
- [EnvironmentErrorTypeDef](./type_defs.md#environmenterrortypedef)
- [EventSourceMappingMetricsConfigOutputTypeDef](./type_defs.md#eventsourcemappingmetricsconfigoutputtypedef)
- [FilterCriteriaErrorTypeDef](./type_defs.md#filtercriteriaerrortypedef)
- [SelfManagedEventSourceOutputTypeDef](./type_defs.md#selfmanagedeventsourceoutputtypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [FunctionCodeLocationTypeDef](./type_defs.md#functioncodelocationtypedef)
- [LayerTypeDef](./type_defs.md#layertypedef)
- [SnapStartResponseTypeDef](./type_defs.md#snapstartresponsetypedef)
- [TracingConfigResponseTypeDef](./type_defs.md#tracingconfigresponsetypedef)
- [VpcConfigResponseTypeDef](./type_defs.md#vpcconfigresponsetypedef)
- [GetAliasRequestRequestTypeDef](./type_defs.md#getaliasrequestrequesttypedef)
- [GetCodeSigningConfigRequestRequestTypeDef](./type_defs.md#getcodesigningconfigrequestrequesttypedef)
- [GetEventSourceMappingRequestRequestTypeDef](./type_defs.md#geteventsourcemappingrequestrequesttypedef)
- [GetFunctionCodeSigningConfigRequestRequestTypeDef](./type_defs.md#getfunctioncodesigningconfigrequestrequesttypedef)
- [GetFunctionConcurrencyRequestRequestTypeDef](./type_defs.md#getfunctionconcurrencyrequestrequesttypedef)
- [GetFunctionConfigurationRequestRequestTypeDef](./type_defs.md#getfunctionconfigurationrequestrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [GetFunctionEventInvokeConfigRequestRequestTypeDef](./type_defs.md#getfunctioneventinvokeconfigrequestrequesttypedef)
- [GetFunctionRecursionConfigRequestRequestTypeDef](./type_defs.md#getfunctionrecursionconfigrequestrequesttypedef)
- [GetFunctionRequestRequestTypeDef](./type_defs.md#getfunctionrequestrequesttypedef)
- [TagsErrorTypeDef](./type_defs.md#tagserrortypedef)
- [GetFunctionUrlConfigRequestRequestTypeDef](./type_defs.md#getfunctionurlconfigrequestrequesttypedef)
- [GetLayerVersionByArnRequestRequestTypeDef](./type_defs.md#getlayerversionbyarnrequestrequesttypedef)
- [GetLayerVersionPolicyRequestRequestTypeDef](./type_defs.md#getlayerversionpolicyrequestrequesttypedef)
- [GetLayerVersionRequestRequestTypeDef](./type_defs.md#getlayerversionrequestrequesttypedef)
- [LayerVersionContentOutputTypeDef](./type_defs.md#layerversioncontentoutputtypedef)
- [GetPolicyRequestRequestTypeDef](./type_defs.md#getpolicyrequestrequesttypedef)
- [GetProvisionedConcurrencyConfigRequestRequestTypeDef](./type_defs.md#getprovisionedconcurrencyconfigrequestrequesttypedef)
- [GetRuntimeManagementConfigRequestRequestTypeDef](./type_defs.md#getruntimemanagementconfigrequestrequesttypedef)
- [ImageConfigErrorTypeDef](./type_defs.md#imageconfigerrortypedef)
- [ImageConfigOutputTypeDef](./type_defs.md#imageconfigoutputtypedef)
- [InvokeResponseStreamUpdateTypeDef](./type_defs.md#invokeresponsestreamupdatetypedef)
- [InvokeWithResponseStreamCompleteEventTypeDef](./type_defs.md#invokewithresponsestreamcompleteeventtypedef)
- [LayerVersionsListItemTypeDef](./type_defs.md#layerversionslistitemtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAliasesRequestRequestTypeDef](./type_defs.md#listaliasesrequestrequesttypedef)
- [ListCodeSigningConfigsRequestRequestTypeDef](./type_defs.md#listcodesigningconfigsrequestrequesttypedef)
- [ListEventSourceMappingsRequestRequestTypeDef](./type_defs.md#listeventsourcemappingsrequestrequesttypedef)
- [ListFunctionEventInvokeConfigsRequestRequestTypeDef](./type_defs.md#listfunctioneventinvokeconfigsrequestrequesttypedef)
- [ListFunctionUrlConfigsRequestRequestTypeDef](./type_defs.md#listfunctionurlconfigsrequestrequesttypedef)
- [ListFunctionsByCodeSigningConfigRequestRequestTypeDef](./type_defs.md#listfunctionsbycodesigningconfigrequestrequesttypedef)
- [ListFunctionsRequestRequestTypeDef](./type_defs.md#listfunctionsrequestrequesttypedef)
- [ListLayerVersionsRequestRequestTypeDef](./type_defs.md#listlayerversionsrequestrequesttypedef)
- [ListLayersRequestRequestTypeDef](./type_defs.md#listlayersrequestrequesttypedef)
- [ListProvisionedConcurrencyConfigsRequestRequestTypeDef](./type_defs.md#listprovisionedconcurrencyconfigsrequestrequesttypedef)
- [ProvisionedConcurrencyConfigListItemTypeDef](./type_defs.md#provisionedconcurrencyconfiglistitemtypedef)
- [ListTagsRequestRequestTypeDef](./type_defs.md#listtagsrequestrequesttypedef)
- [ListVersionsByFunctionRequestRequestTypeDef](./type_defs.md#listversionsbyfunctionrequestrequesttypedef)
- [PublishVersionRequestRequestTypeDef](./type_defs.md#publishversionrequestrequesttypedef)
- [PutFunctionCodeSigningConfigRequestRequestTypeDef](./type_defs.md#putfunctioncodesigningconfigrequestrequesttypedef)
- [PutFunctionConcurrencyRequestRequestTypeDef](./type_defs.md#putfunctionconcurrencyrequestrequesttypedef)
- [PutFunctionRecursionConfigRequestRequestTypeDef](./type_defs.md#putfunctionrecursionconfigrequestrequesttypedef)
- [PutProvisionedConcurrencyConfigRequestRequestTypeDef](./type_defs.md#putprovisionedconcurrencyconfigrequestrequesttypedef)
- [PutRuntimeManagementConfigRequestRequestTypeDef](./type_defs.md#putruntimemanagementconfigrequestrequesttypedef)
- [RemoveLayerVersionPermissionRequestRequestTypeDef](./type_defs.md#removelayerversionpermissionrequestrequesttypedef)
- [RemovePermissionRequestRequestTypeDef](./type_defs.md#removepermissionrequestrequesttypedef)
- [RuntimeVersionErrorTypeDef](./type_defs.md#runtimeversionerrortypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [AddLayerVersionPermissionResponseTypeDef](./type_defs.md#addlayerversionpermissionresponsetypedef)
- [AddPermissionResponseTypeDef](./type_defs.md#addpermissionresponsetypedef)
- [ConcurrencyResponseTypeDef](./type_defs.md#concurrencyresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetAccountSettingsResponseTypeDef](./type_defs.md#getaccountsettingsresponsetypedef)
- [GetFunctionCodeSigningConfigResponseTypeDef](./type_defs.md#getfunctioncodesigningconfigresponsetypedef)
- [GetFunctionConcurrencyResponseTypeDef](./type_defs.md#getfunctionconcurrencyresponsetypedef)
- [GetFunctionRecursionConfigResponseTypeDef](./type_defs.md#getfunctionrecursionconfigresponsetypedef)
- [GetLayerVersionPolicyResponseTypeDef](./type_defs.md#getlayerversionpolicyresponsetypedef)
- [GetPolicyResponseTypeDef](./type_defs.md#getpolicyresponsetypedef)
- [GetProvisionedConcurrencyConfigResponseTypeDef](./type_defs.md#getprovisionedconcurrencyconfigresponsetypedef)
- [GetRuntimeManagementConfigResponseTypeDef](./type_defs.md#getruntimemanagementconfigresponsetypedef)
- [InvocationResponseTypeDef](./type_defs.md#invocationresponsetypedef)
- [InvokeAsyncResponseTypeDef](./type_defs.md#invokeasyncresponsetypedef)
- [ListFunctionsByCodeSigningConfigResponseTypeDef](./type_defs.md#listfunctionsbycodesigningconfigresponsetypedef)
- [ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef)
- [PutFunctionCodeSigningConfigResponseTypeDef](./type_defs.md#putfunctioncodesigningconfigresponsetypedef)
- [PutFunctionRecursionConfigResponseTypeDef](./type_defs.md#putfunctionrecursionconfigresponsetypedef)
- [PutProvisionedConcurrencyConfigResponseTypeDef](./type_defs.md#putprovisionedconcurrencyconfigresponsetypedef)
- [PutRuntimeManagementConfigResponseTypeDef](./type_defs.md#putruntimemanagementconfigresponsetypedef)
- [AliasConfigurationResponseTypeDef](./type_defs.md#aliasconfigurationresponsetypedef)
- [AliasConfigurationTypeDef](./type_defs.md#aliasconfigurationtypedef)
- [CreateAliasRequestRequestTypeDef](./type_defs.md#createaliasrequestrequesttypedef)
- [UpdateAliasRequestRequestTypeDef](./type_defs.md#updatealiasrequestrequesttypedef)
- [FunctionCodeTypeDef](./type_defs.md#functioncodetypedef)
- [InvocationRequestRequestTypeDef](./type_defs.md#invocationrequestrequesttypedef)
- [InvokeAsyncRequestRequestTypeDef](./type_defs.md#invokeasyncrequestrequesttypedef)
- [InvokeWithResponseStreamRequestRequestTypeDef](./type_defs.md#invokewithresponsestreamrequestrequesttypedef)
- [LayerVersionContentInputTypeDef](./type_defs.md#layerversioncontentinputtypedef)
- [UpdateFunctionCodeRequestRequestTypeDef](./type_defs.md#updatefunctioncoderequestrequesttypedef)
- [CodeSigningConfigTypeDef](./type_defs.md#codesigningconfigtypedef)
- [CreateCodeSigningConfigRequestRequestTypeDef](./type_defs.md#createcodesigningconfigrequestrequesttypedef)
- [UpdateCodeSigningConfigRequestRequestTypeDef](./type_defs.md#updatecodesigningconfigrequestrequesttypedef)
- [CreateFunctionUrlConfigResponseTypeDef](./type_defs.md#createfunctionurlconfigresponsetypedef)
- [FunctionUrlConfigTypeDef](./type_defs.md#functionurlconfigtypedef)
- [GetFunctionUrlConfigResponseTypeDef](./type_defs.md#getfunctionurlconfigresponsetypedef)
- [UpdateFunctionUrlConfigResponseTypeDef](./type_defs.md#updatefunctionurlconfigresponsetypedef)
- [CreateFunctionUrlConfigRequestRequestTypeDef](./type_defs.md#createfunctionurlconfigrequestrequesttypedef)
- [UpdateFunctionUrlConfigRequestRequestTypeDef](./type_defs.md#updatefunctionurlconfigrequestrequesttypedef)
- [UpdateFunctionConfigurationRequestRequestTypeDef](./type_defs.md#updatefunctionconfigurationrequestrequesttypedef)
- [DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef)
- [EnvironmentResponseTypeDef](./type_defs.md#environmentresponsetypedef)
- [FilterCriteriaOutputTypeDef](./type_defs.md#filtercriteriaoutputtypedef)
- [FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef)
- [GetFunctionConfigurationRequestWaitTypeDef](./type_defs.md#getfunctionconfigurationrequestwaittypedef)
- [GetFunctionRequestWaitTypeDef](./type_defs.md#getfunctionrequestwaittypedef)
- [GetLayerVersionResponseTypeDef](./type_defs.md#getlayerversionresponsetypedef)
- [PublishLayerVersionResponseTypeDef](./type_defs.md#publishlayerversionresponsetypedef)
- [ImageConfigResponseTypeDef](./type_defs.md#imageconfigresponsetypedef)
- [InvokeWithResponseStreamResponseEventTypeDef](./type_defs.md#invokewithresponsestreamresponseeventtypedef)
- [LayersListItemTypeDef](./type_defs.md#layerslistitemtypedef)
- [ListLayerVersionsResponseTypeDef](./type_defs.md#listlayerversionsresponsetypedef)
- [ListAliasesRequestPaginateTypeDef](./type_defs.md#listaliasesrequestpaginatetypedef)
- [ListCodeSigningConfigsRequestPaginateTypeDef](./type_defs.md#listcodesigningconfigsrequestpaginatetypedef)
- [ListEventSourceMappingsRequestPaginateTypeDef](./type_defs.md#listeventsourcemappingsrequestpaginatetypedef)
- [ListFunctionEventInvokeConfigsRequestPaginateTypeDef](./type_defs.md#listfunctioneventinvokeconfigsrequestpaginatetypedef)
- [ListFunctionUrlConfigsRequestPaginateTypeDef](./type_defs.md#listfunctionurlconfigsrequestpaginatetypedef)
- [ListFunctionsByCodeSigningConfigRequestPaginateTypeDef](./type_defs.md#listfunctionsbycodesigningconfigrequestpaginatetypedef)
- [ListFunctionsRequestPaginateTypeDef](./type_defs.md#listfunctionsrequestpaginatetypedef)
- [ListLayerVersionsRequestPaginateTypeDef](./type_defs.md#listlayerversionsrequestpaginatetypedef)
- [ListLayersRequestPaginateTypeDef](./type_defs.md#listlayersrequestpaginatetypedef)
- [ListProvisionedConcurrencyConfigsRequestPaginateTypeDef](./type_defs.md#listprovisionedconcurrencyconfigsrequestpaginatetypedef)
- [ListVersionsByFunctionRequestPaginateTypeDef](./type_defs.md#listversionsbyfunctionrequestpaginatetypedef)
- [ListProvisionedConcurrencyConfigsResponseTypeDef](./type_defs.md#listprovisionedconcurrencyconfigsresponsetypedef)
- [RuntimeVersionConfigTypeDef](./type_defs.md#runtimeversionconfigtypedef)
- [ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef)
- [CreateFunctionRequestRequestTypeDef](./type_defs.md#createfunctionrequestrequesttypedef)
- [PublishLayerVersionRequestRequestTypeDef](./type_defs.md#publishlayerversionrequestrequesttypedef)
- [CreateCodeSigningConfigResponseTypeDef](./type_defs.md#createcodesigningconfigresponsetypedef)
- [GetCodeSigningConfigResponseTypeDef](./type_defs.md#getcodesigningconfigresponsetypedef)
- [ListCodeSigningConfigsResponseTypeDef](./type_defs.md#listcodesigningconfigsresponsetypedef)
- [UpdateCodeSigningConfigResponseTypeDef](./type_defs.md#updatecodesigningconfigresponsetypedef)
- [ListFunctionUrlConfigsResponseTypeDef](./type_defs.md#listfunctionurlconfigsresponsetypedef)
- [FunctionEventInvokeConfigResponseTypeDef](./type_defs.md#functioneventinvokeconfigresponsetypedef)
- [FunctionEventInvokeConfigTypeDef](./type_defs.md#functioneventinvokeconfigtypedef)
- [PutFunctionEventInvokeConfigRequestRequestTypeDef](./type_defs.md#putfunctioneventinvokeconfigrequestrequesttypedef)
- [UpdateFunctionEventInvokeConfigRequestRequestTypeDef](./type_defs.md#updatefunctioneventinvokeconfigrequestrequesttypedef)
- [EventSourceMappingConfigurationResponseTypeDef](./type_defs.md#eventsourcemappingconfigurationresponsetypedef)
- [EventSourceMappingConfigurationTypeDef](./type_defs.md#eventsourcemappingconfigurationtypedef)
- [CreateEventSourceMappingRequestRequestTypeDef](./type_defs.md#createeventsourcemappingrequestrequesttypedef)
- [UpdateEventSourceMappingRequestRequestTypeDef](./type_defs.md#updateeventsourcemappingrequestrequesttypedef)
- [InvokeWithResponseStreamResponseTypeDef](./type_defs.md#invokewithresponsestreamresponsetypedef)
- [ListLayersResponseTypeDef](./type_defs.md#listlayersresponsetypedef)
- [FunctionConfigurationResponseTypeDef](./type_defs.md#functionconfigurationresponsetypedef)
- [FunctionConfigurationTypeDef](./type_defs.md#functionconfigurationtypedef)
- [ListFunctionEventInvokeConfigsResponseTypeDef](./type_defs.md#listfunctioneventinvokeconfigsresponsetypedef)
- [ListEventSourceMappingsResponseTypeDef](./type_defs.md#listeventsourcemappingsresponsetypedef)
- [GetFunctionResponseTypeDef](./type_defs.md#getfunctionresponsetypedef)
- [ListFunctionsResponseTypeDef](./type_defs.md#listfunctionsresponsetypedef)
- [ListVersionsByFunctionResponseTypeDef](./type_defs.md#listversionsbyfunctionresponsetypedef)
