# SQS module

> [Index](../README.md) > SQS


!!! note ""

    Auto-generated documentation for [SQS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#sqs)
    type annotations stubs module [types-aiobotocore-sqs](https://pypi.org/project/types-aiobotocore-sqs/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `SQS` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `SQS` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[sqs]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[sqs]'

# standalone installation
python -m pip install types-aiobotocore-sqs
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-sqs
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SQSClient

Type annotations and code completion for  `#!python session.client("sqs")` as [SQSClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# SQSClient usage example

from aioboto3.session import Session

from types_aiobotocore_sqs.client import SQSClient


session = Session()
async with session.client("sqs") as client:
    client: SQSClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("sqs").get_paginator("...")`.

```python
# ListDeadLetterSourceQueuesPaginator usage example

from types_aiobotocore_sqs.paginator import ListDeadLetterSourceQueuesPaginator

def get_list_dead_letter_source_queues_paginator() -> ListDeadLetterSourceQueuesPaginator:
    return client.get_paginator("list_dead_letter_source_queues"))
```

- [ListDeadLetterSourceQueuesPaginator](./paginators.md#listdeadlettersourcequeuespaginator)
- [ListQueuesPaginator](./paginators.md#listqueuespaginator)






## SQSServiceResource

Type annotations and code completion for `#!python session.resource("sqs")` as
[SQSServiceResource](./service_resource.md#sqsserviceresource)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs/service-resource/index.html)

```python
# SQSServiceResource usage example

from types_aiobotocore_sqs.service_resource import SQSServiceResource
```


### Collections

Type annotations and code completion for collections
from `#!python session.resource("sqs").*`.

```python
# ServiceResourceQueuesCollection usage example

from types_aiobotocore_sqs.service_resource import ServiceResourceQueuesCollection

def get_collection() -> ServiceResourceQueuesCollection:
    return resource.queues
```

- [ServiceResourceQueuesCollection](./service_resource.md#serviceresourcequeuescollection)





### Resources

Type annotations and code completion for additional resources
from `#!python session.resource("sqs").*`.

```python
# Message usage example

from types_aiobotocore_sqs.service_resource import Message

def get_resource() -> Message:
    return resource.Message(...)
```

- [Message](./service_resource.md#message)
- [Queue](./service_resource.md#queue)





## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ListDeadLetterSourceQueuesPaginatorName usage example

from types_aiobotocore_sqs.literals import ListDeadLetterSourceQueuesPaginatorName

def get_value() -> ListDeadLetterSourceQueuesPaginatorName:
    return "list_dead_letter_source_queues"
```

- [ListDeadLetterSourceQueuesPaginatorName](./literals.md#listdeadlettersourcequeuespaginatorname)
- [ListQueuesPaginatorName](./literals.md#listqueuespaginatorname)
- [MessageSystemAttributeNameForSendsType](./literals.md#messagesystemattributenameforsendstype)
- [MessageSystemAttributeNameType](./literals.md#messagesystemattributenametype)
- [QueueAttributeFilterType](./literals.md#queueattributefiltertype)
- [QueueAttributeNameType](./literals.md#queueattributenametype)
- [SQSServiceName](./literals.md#sqsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AddPermissionRequestQueueAddPermissionTypeDef](./type_defs.md#addpermissionrequestqueueaddpermissiontypedef)
- [AddPermissionRequestRequestTypeDef](./type_defs.md#addpermissionrequestrequesttypedef)
- [BatchResultErrorEntryTypeDef](./type_defs.md#batchresulterrorentrytypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CancelMessageMoveTaskRequestRequestTypeDef](./type_defs.md#cancelmessagemovetaskrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ChangeMessageVisibilityBatchRequestEntryTypeDef](./type_defs.md#changemessagevisibilitybatchrequestentrytypedef)
- [ChangeMessageVisibilityBatchResultEntryTypeDef](./type_defs.md#changemessagevisibilitybatchresultentrytypedef)
- [ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef](./type_defs.md#changemessagevisibilityrequestmessagechangevisibilitytypedef)
- [ChangeMessageVisibilityRequestRequestTypeDef](./type_defs.md#changemessagevisibilityrequestrequesttypedef)
- [CreateQueueRequestRequestTypeDef](./type_defs.md#createqueuerequestrequesttypedef)
- [CreateQueueRequestServiceResourceCreateQueueTypeDef](./type_defs.md#createqueuerequestserviceresourcecreatequeuetypedef)
- [DeleteMessageBatchRequestEntryTypeDef](./type_defs.md#deletemessagebatchrequestentrytypedef)
- [DeleteMessageBatchResultEntryTypeDef](./type_defs.md#deletemessagebatchresultentrytypedef)
- [DeleteMessageRequestRequestTypeDef](./type_defs.md#deletemessagerequestrequesttypedef)
- [DeleteQueueRequestRequestTypeDef](./type_defs.md#deletequeuerequestrequesttypedef)
- [GetQueueAttributesRequestRequestTypeDef](./type_defs.md#getqueueattributesrequestrequesttypedef)
- [GetQueueUrlRequestRequestTypeDef](./type_defs.md#getqueueurlrequestrequesttypedef)
- [GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef](./type_defs.md#getqueueurlrequestserviceresourcegetqueuebynametypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListDeadLetterSourceQueuesRequestRequestTypeDef](./type_defs.md#listdeadlettersourcequeuesrequestrequesttypedef)
- [ListMessageMoveTasksRequestRequestTypeDef](./type_defs.md#listmessagemovetasksrequestrequesttypedef)
- [ListMessageMoveTasksResultEntryTypeDef](./type_defs.md#listmessagemovetasksresultentrytypedef)
- [ListQueueTagsRequestRequestTypeDef](./type_defs.md#listqueuetagsrequestrequesttypedef)
- [ListQueuesRequestRequestTypeDef](./type_defs.md#listqueuesrequestrequesttypedef)
- [MessageAttributeValueOutputTypeDef](./type_defs.md#messageattributevalueoutputtypedef)
- [PurgeQueueRequestRequestTypeDef](./type_defs.md#purgequeuerequestrequesttypedef)
- [ReceiveMessageRequestQueueReceiveMessagesTypeDef](./type_defs.md#receivemessagerequestqueuereceivemessagestypedef)
- [ReceiveMessageRequestRequestTypeDef](./type_defs.md#receivemessagerequestrequesttypedef)
- [RemovePermissionRequestQueueRemovePermissionTypeDef](./type_defs.md#removepermissionrequestqueueremovepermissiontypedef)
- [RemovePermissionRequestRequestTypeDef](./type_defs.md#removepermissionrequestrequesttypedef)
- [SendMessageBatchResultEntryTypeDef](./type_defs.md#sendmessagebatchresultentrytypedef)
- [SetQueueAttributesRequestQueueSetAttributesTypeDef](./type_defs.md#setqueueattributesrequestqueuesetattributestypedef)
- [SetQueueAttributesRequestRequestTypeDef](./type_defs.md#setqueueattributesrequestrequesttypedef)
- [StartMessageMoveTaskRequestRequestTypeDef](./type_defs.md#startmessagemovetaskrequestrequesttypedef)
- [TagQueueRequestRequestTypeDef](./type_defs.md#tagqueuerequestrequesttypedef)
- [UntagQueueRequestRequestTypeDef](./type_defs.md#untagqueuerequestrequesttypedef)
- [MessageAttributeValueTypeDef](./type_defs.md#messageattributevaluetypedef)
- [MessageSystemAttributeValueTypeDef](./type_defs.md#messagesystemattributevaluetypedef)
- [CancelMessageMoveTaskResultTypeDef](./type_defs.md#cancelmessagemovetaskresulttypedef)
- [CreateQueueResultTypeDef](./type_defs.md#createqueueresulttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetQueueAttributesResultTypeDef](./type_defs.md#getqueueattributesresulttypedef)
- [GetQueueUrlResultTypeDef](./type_defs.md#getqueueurlresulttypedef)
- [ListDeadLetterSourceQueuesResultTypeDef](./type_defs.md#listdeadlettersourcequeuesresulttypedef)
- [ListQueueTagsResultTypeDef](./type_defs.md#listqueuetagsresulttypedef)
- [ListQueuesResultTypeDef](./type_defs.md#listqueuesresulttypedef)
- [SendMessageResultTypeDef](./type_defs.md#sendmessageresulttypedef)
- [StartMessageMoveTaskResultTypeDef](./type_defs.md#startmessagemovetaskresulttypedef)
- [ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef](./type_defs.md#changemessagevisibilitybatchrequestqueuechangemessagevisibilitybatchtypedef)
- [ChangeMessageVisibilityBatchRequestRequestTypeDef](./type_defs.md#changemessagevisibilitybatchrequestrequesttypedef)
- [ChangeMessageVisibilityBatchResultTypeDef](./type_defs.md#changemessagevisibilitybatchresulttypedef)
- [DeleteMessageBatchRequestQueueDeleteMessagesTypeDef](./type_defs.md#deletemessagebatchrequestqueuedeletemessagestypedef)
- [DeleteMessageBatchRequestRequestTypeDef](./type_defs.md#deletemessagebatchrequestrequesttypedef)
- [DeleteMessageBatchResultTypeDef](./type_defs.md#deletemessagebatchresulttypedef)
- [ListDeadLetterSourceQueuesRequestPaginateTypeDef](./type_defs.md#listdeadlettersourcequeuesrequestpaginatetypedef)
- [ListQueuesRequestPaginateTypeDef](./type_defs.md#listqueuesrequestpaginatetypedef)
- [ListMessageMoveTasksResultTypeDef](./type_defs.md#listmessagemovetasksresulttypedef)
- [MessageTypeDef](./type_defs.md#messagetypedef)
- [SendMessageBatchResultTypeDef](./type_defs.md#sendmessagebatchresulttypedef)
- [MessageAttributeValueUnionTypeDef](./type_defs.md#messageattributevalueuniontypedef)
- [SendMessageBatchRequestEntryTypeDef](./type_defs.md#sendmessagebatchrequestentrytypedef)
- [SendMessageRequestQueueSendMessageTypeDef](./type_defs.md#sendmessagerequestqueuesendmessagetypedef)
- [ReceiveMessageResultTypeDef](./type_defs.md#receivemessageresulttypedef)
- [SendMessageRequestRequestTypeDef](./type_defs.md#sendmessagerequestrequesttypedef)
- [SendMessageBatchRequestQueueSendMessagesTypeDef](./type_defs.md#sendmessagebatchrequestqueuesendmessagestypedef)
- [SendMessageBatchRequestRequestTypeDef](./type_defs.md#sendmessagebatchrequestrequesttypedef)
