# Bedrock module

> [Index](../README.md) > Bedrock


!!! note ""

    Auto-generated documentation for [Bedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock)
    type annotations stubs module [types-aiobotocore-bedrock](https://pypi.org/project/types-aiobotocore-bedrock/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `Bedrock` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[bedrock]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[bedrock]'


# standalone installation
python -m pip install types-aiobotocore-bedrock
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-bedrock
```

## Usage

Code samples can be found in [Examples](./usage.md).

## BedrockClient

Type annotations and code completion for  `#!python session.client("bedrock")` as [BedrockClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client)

```python
# BedrockClient usage example

from aioboto3.session import Session

from types_aiobotocore_bedrock.client import BedrockClient


session = Session()
async with session.client("bedrock") as client:
    client: BedrockClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("bedrock").get_paginator("...")`.

```python
# ListCustomModelsPaginator usage example

from types_aiobotocore_bedrock.paginator import ListCustomModelsPaginator

def get_list_custom_models_paginator() -> ListCustomModelsPaginator:
    return client.get_paginator("list_custom_models"))
```

- [ListCustomModelsPaginator](./paginators.md#listcustommodelspaginator)
- [ListModelCustomizationJobsPaginator](./paginators.md#listmodelcustomizationjobspaginator)
- [ListProvisionedModelThroughputsPaginator](./paginators.md#listprovisionedmodelthroughputspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CommitmentDurationType usage example

from types_aiobotocore_bedrock.literals import CommitmentDurationType

def get_value() -> CommitmentDurationType:
    return "OneMonth"
```

- [CommitmentDurationType](./literals.md#commitmentdurationtype)
- [CustomizationTypeType](./literals.md#customizationtypetype)
- [FineTuningJobStatusType](./literals.md#finetuningjobstatustype)
- [FoundationModelLifecycleStatusType](./literals.md#foundationmodellifecyclestatustype)
- [InferenceTypeType](./literals.md#inferencetypetype)
- [ListCustomModelsPaginatorName](./literals.md#listcustommodelspaginatorname)
- [ListModelCustomizationJobsPaginatorName](./literals.md#listmodelcustomizationjobspaginatorname)
- [ListProvisionedModelThroughputsPaginatorName](./literals.md#listprovisionedmodelthroughputspaginatorname)
- [ModelCustomizationJobStatusType](./literals.md#modelcustomizationjobstatustype)
- [ModelCustomizationType](./literals.md#modelcustomizationtype)
- [ModelModalityType](./literals.md#modelmodalitytype)
- [ProvisionedModelStatusType](./literals.md#provisionedmodelstatustype)
- [SortByProvisionedModelsType](./literals.md#sortbyprovisionedmodelstype)
- [SortJobsByType](./literals.md#sortjobsbytype)
- [SortModelsByType](./literals.md#sortmodelsbytype)
- [SortOrderType](./literals.md#sortordertype)
- [BedrockServiceName](./literals.md#bedrockservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [S3ConfigTypeDef](./type_defs.md#s3configtypedef)
- [OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [TrainingDataConfigTypeDef](./type_defs.md#trainingdataconfigtypedef)
- [VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CustomModelSummaryTypeDef](./type_defs.md#custommodelsummarytypedef)
- [DeleteCustomModelRequestRequestTypeDef](./type_defs.md#deletecustommodelrequestrequesttypedef)
- [DeleteProvisionedModelThroughputRequestRequestTypeDef](./type_defs.md#deleteprovisionedmodelthroughputrequestrequesttypedef)
- [FoundationModelLifecycleTypeDef](./type_defs.md#foundationmodellifecycletypedef)
- [GetCustomModelRequestRequestTypeDef](./type_defs.md#getcustommodelrequestrequesttypedef)
- [TrainingMetricsTypeDef](./type_defs.md#trainingmetricstypedef)
- [ValidatorMetricTypeDef](./type_defs.md#validatormetrictypedef)
- [GetFoundationModelRequestRequestTypeDef](./type_defs.md#getfoundationmodelrequestrequesttypedef)
- [GetModelCustomizationJobRequestRequestTypeDef](./type_defs.md#getmodelcustomizationjobrequestrequesttypedef)
- [GetProvisionedModelThroughputRequestRequestTypeDef](./type_defs.md#getprovisionedmodelthroughputrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ListFoundationModelsRequestRequestTypeDef](./type_defs.md#listfoundationmodelsrequestrequesttypedef)
- [ModelCustomizationJobSummaryTypeDef](./type_defs.md#modelcustomizationjobsummarytypedef)
- [ProvisionedModelSummaryTypeDef](./type_defs.md#provisionedmodelsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [StopModelCustomizationJobRequestRequestTypeDef](./type_defs.md#stopmodelcustomizationjobrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateProvisionedModelThroughputRequestRequestTypeDef](./type_defs.md#updateprovisionedmodelthroughputrequestrequesttypedef)
- [ValidatorTypeDef](./type_defs.md#validatortypedef)
- [CloudWatchConfigTypeDef](./type_defs.md#cloudwatchconfigtypedef)
- [CreateProvisionedModelThroughputRequestRequestTypeDef](./type_defs.md#createprovisionedmodelthroughputrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateModelCustomizationJobResponseTypeDef](./type_defs.md#createmodelcustomizationjobresponsetypedef)
- [CreateProvisionedModelThroughputResponseTypeDef](./type_defs.md#createprovisionedmodelthroughputresponsetypedef)
- [GetProvisionedModelThroughputResponseTypeDef](./type_defs.md#getprovisionedmodelthroughputresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ListCustomModelsResponseTypeDef](./type_defs.md#listcustommodelsresponsetypedef)
- [FoundationModelDetailsTypeDef](./type_defs.md#foundationmodeldetailstypedef)
- [FoundationModelSummaryTypeDef](./type_defs.md#foundationmodelsummarytypedef)
- [ListCustomModelsRequestListCustomModelsPaginateTypeDef](./type_defs.md#listcustommodelsrequestlistcustommodelspaginatetypedef)
- [ListCustomModelsRequestRequestTypeDef](./type_defs.md#listcustommodelsrequestrequesttypedef)
- [ListModelCustomizationJobsRequestListModelCustomizationJobsPaginateTypeDef](./type_defs.md#listmodelcustomizationjobsrequestlistmodelcustomizationjobspaginatetypedef)
- [ListModelCustomizationJobsRequestRequestTypeDef](./type_defs.md#listmodelcustomizationjobsrequestrequesttypedef)
- [ListProvisionedModelThroughputsRequestListProvisionedModelThroughputsPaginateTypeDef](./type_defs.md#listprovisionedmodelthroughputsrequestlistprovisionedmodelthroughputspaginatetypedef)
- [ListProvisionedModelThroughputsRequestRequestTypeDef](./type_defs.md#listprovisionedmodelthroughputsrequestrequesttypedef)
- [ListModelCustomizationJobsResponseTypeDef](./type_defs.md#listmodelcustomizationjobsresponsetypedef)
- [ListProvisionedModelThroughputsResponseTypeDef](./type_defs.md#listprovisionedmodelthroughputsresponsetypedef)
- [ValidationDataConfigTypeDef](./type_defs.md#validationdataconfigtypedef)
- [LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef)
- [GetFoundationModelResponseTypeDef](./type_defs.md#getfoundationmodelresponsetypedef)
- [ListFoundationModelsResponseTypeDef](./type_defs.md#listfoundationmodelsresponsetypedef)
- [CreateModelCustomizationJobRequestRequestTypeDef](./type_defs.md#createmodelcustomizationjobrequestrequesttypedef)
- [GetCustomModelResponseTypeDef](./type_defs.md#getcustommodelresponsetypedef)
- [GetModelCustomizationJobResponseTypeDef](./type_defs.md#getmodelcustomizationjobresponsetypedef)
- [GetModelInvocationLoggingConfigurationResponseTypeDef](./type_defs.md#getmodelinvocationloggingconfigurationresponsetypedef)
- [PutModelInvocationLoggingConfigurationRequestRequestTypeDef](./type_defs.md#putmodelinvocationloggingconfigurationrequestrequesttypedef)

