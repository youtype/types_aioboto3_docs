# SQSClient

> [Index](../README.md) > [SQS](./README.md) > SQSClient

!!! note ""

    Auto-generated documentation for [SQS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#sqs)
    type annotations stubs module [types-aiobotocore-sqs](https://pypi.org/project/types-aiobotocore-sqs/).

## SQSClient

Type annotations and code completion for `#!python session.client("sqs")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# SQSClient usage example

from aioboto3.session import Session
from types_aiobotocore_sqs.client import SQSClient

session = Session()
async with session.client("sqs") as client:
    client: SQSClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("sqs").exceptions` structure.

```python
# SQSClient.exceptions usage example

async with session.client("sqs") as client:
    try:
        do_something(client)
    except (
            client.exceptions.BatchEntryIdsNotDistinct,
        client.exceptions.BatchRequestTooLong,
        client.exceptions.ClientError,
        client.exceptions.EmptyBatchRequest,
        client.exceptions.InvalidAddress,
        client.exceptions.InvalidAttributeName,
        client.exceptions.InvalidAttributeValue,
        client.exceptions.InvalidBatchEntryId,
        client.exceptions.InvalidIdFormat,
        client.exceptions.InvalidMessageContents,
        client.exceptions.InvalidSecurity,
        client.exceptions.KmsAccessDenied,
        client.exceptions.KmsDisabled,
        client.exceptions.KmsInvalidKeyUsage,
        client.exceptions.KmsInvalidState,
        client.exceptions.KmsNotFound,
        client.exceptions.KmsOptInRequired,
        client.exceptions.KmsThrottled,
        client.exceptions.MessageNotInflight,
        client.exceptions.OverLimit,
        client.exceptions.PurgeQueueInProgress,
        client.exceptions.QueueDeletedRecently,
        client.exceptions.QueueDoesNotExist,
        client.exceptions.QueueNameExists,
        client.exceptions.ReceiptHandleIsInvalid,
        client.exceptions.RequestThrottled,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.TooManyEntriesInBatchRequest,
        client.exceptions.UnsupportedOperation,
    ) as e:
        print(e)
```

```python
# SQSClient.exceptions type checking example

from types_aiobotocore_sqs.client import Exceptions

def handle_error(exc: Exceptions.BatchEntryIdsNotDistinct) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("sqs").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("sqs").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

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


### add\_permission

Adds a permission to a queue for a specific <a
href="https://docs.aws.amazon.com/general/latest/gr/glos-chap.html#P">principal</a>.

Type annotations and code completion for `#!python session.client("sqs").add_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# add_permission method definition

await def add_permission(
    self,
    *,
    QueueUrl: str,
    Label: str,
    AWSAccountIds: Sequence[str],
    Actions: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# add_permission method usage example with argument unpacking

kwargs: AddPermissionRequestRequestTypeDef = {  # (1)
    "QueueUrl": ...,
    "Label": ...,
    "AWSAccountIds": ...,
    "Actions": ...,
}

parent.add_permission(**kwargs)
```

1. See [:material-code-braces: AddPermissionRequestRequestTypeDef](./type_defs.md#addpermissionrequestrequesttypedef) 

### cancel\_message\_move\_task

Cancels a specified message movement task.

Type annotations and code completion for `#!python session.client("sqs").cancel_message_move_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# cancel_message_move_task method definition

await def cancel_message_move_task(
    self,
    *,
    TaskHandle: str,
) -> CancelMessageMoveTaskResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelMessageMoveTaskResultTypeDef](./type_defs.md#cancelmessagemovetaskresulttypedef) 


```python
# cancel_message_move_task method usage example with argument unpacking

kwargs: CancelMessageMoveTaskRequestRequestTypeDef = {  # (1)
    "TaskHandle": ...,
}

parent.cancel_message_move_task(**kwargs)
```

1. See [:material-code-braces: CancelMessageMoveTaskRequestRequestTypeDef](./type_defs.md#cancelmessagemovetaskrequestrequesttypedef) 

### change\_message\_visibility

Changes the visibility timeout of a specified message in a queue to a new value.

Type annotations and code completion for `#!python session.client("sqs").change_message_visibility` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# change_message_visibility method definition

await def change_message_visibility(
    self,
    *,
    QueueUrl: str,
    ReceiptHandle: str,
    VisibilityTimeout: int,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# change_message_visibility method usage example with argument unpacking

kwargs: ChangeMessageVisibilityRequestRequestTypeDef = {  # (1)
    "QueueUrl": ...,
    "ReceiptHandle": ...,
    "VisibilityTimeout": ...,
}

parent.change_message_visibility(**kwargs)
```

1. See [:material-code-braces: ChangeMessageVisibilityRequestRequestTypeDef](./type_defs.md#changemessagevisibilityrequestrequesttypedef) 

### change\_message\_visibility\_batch

Changes the visibility timeout of multiple messages.

Type annotations and code completion for `#!python session.client("sqs").change_message_visibility_batch` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# change_message_visibility_batch method definition

await def change_message_visibility_batch(
    self,
    *,
    QueueUrl: str,
    Entries: Sequence[ChangeMessageVisibilityBatchRequestEntryTypeDef],  # (1)
) -> ChangeMessageVisibilityBatchResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ChangeMessageVisibilityBatchRequestEntryTypeDef](./type_defs.md#changemessagevisibilitybatchrequestentrytypedef) 
2. See [:material-code-braces: ChangeMessageVisibilityBatchResultTypeDef](./type_defs.md#changemessagevisibilitybatchresulttypedef) 


```python
# change_message_visibility_batch method usage example with argument unpacking

kwargs: ChangeMessageVisibilityBatchRequestRequestTypeDef = {  # (1)
    "QueueUrl": ...,
    "Entries": ...,
}

parent.change_message_visibility_batch(**kwargs)
```

1. See [:material-code-braces: ChangeMessageVisibilityBatchRequestRequestTypeDef](./type_defs.md#changemessagevisibilitybatchrequestrequesttypedef) 

### create\_queue

Creates a new standard or FIFO queue.

Type annotations and code completion for `#!python session.client("sqs").create_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# create_queue method definition

await def create_queue(
    self,
    *,
    QueueName: str,
    Attributes: Mapping[QueueAttributeNameType, str] = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> CreateQueueResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: QueueAttributeNameType](./literals.md#queueattributenametype) 
2. See [:material-code-braces: CreateQueueResultTypeDef](./type_defs.md#createqueueresulttypedef) 


```python
# create_queue method usage example with argument unpacking

kwargs: CreateQueueRequestRequestTypeDef = {  # (1)
    "QueueName": ...,
}

parent.create_queue(**kwargs)
```

1. See [:material-code-braces: CreateQueueRequestRequestTypeDef](./type_defs.md#createqueuerequestrequesttypedef) 

### delete\_message

Deletes the specified message from the specified queue.

Type annotations and code completion for `#!python session.client("sqs").delete_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# delete_message method definition

await def delete_message(
    self,
    *,
    QueueUrl: str,
    ReceiptHandle: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_message method usage example with argument unpacking

kwargs: DeleteMessageRequestRequestTypeDef = {  # (1)
    "QueueUrl": ...,
    "ReceiptHandle": ...,
}

parent.delete_message(**kwargs)
```

1. See [:material-code-braces: DeleteMessageRequestRequestTypeDef](./type_defs.md#deletemessagerequestrequesttypedef) 

### delete\_message\_batch

Deletes up to ten messages from the specified queue.

Type annotations and code completion for `#!python session.client("sqs").delete_message_batch` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# delete_message_batch method definition

await def delete_message_batch(
    self,
    *,
    QueueUrl: str,
    Entries: Sequence[DeleteMessageBatchRequestEntryTypeDef],  # (1)
) -> DeleteMessageBatchResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DeleteMessageBatchRequestEntryTypeDef](./type_defs.md#deletemessagebatchrequestentrytypedef) 
2. See [:material-code-braces: DeleteMessageBatchResultTypeDef](./type_defs.md#deletemessagebatchresulttypedef) 


```python
# delete_message_batch method usage example with argument unpacking

kwargs: DeleteMessageBatchRequestRequestTypeDef = {  # (1)
    "QueueUrl": ...,
    "Entries": ...,
}

parent.delete_message_batch(**kwargs)
```

1. See [:material-code-braces: DeleteMessageBatchRequestRequestTypeDef](./type_defs.md#deletemessagebatchrequestrequesttypedef) 

### delete\_queue

Deletes the queue specified by the <code>QueueUrl</code>, regardless of the
queue's contents.

Type annotations and code completion for `#!python session.client("sqs").delete_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# delete_queue method definition

await def delete_queue(
    self,
    *,
    QueueUrl: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_queue method usage example with argument unpacking

kwargs: DeleteQueueRequestRequestTypeDef = {  # (1)
    "QueueUrl": ...,
}

parent.delete_queue(**kwargs)
```

1. See [:material-code-braces: DeleteQueueRequestRequestTypeDef](./type_defs.md#deletequeuerequestrequesttypedef) 

### get\_queue\_attributes

Gets attributes for the specified queue.

Type annotations and code completion for `#!python session.client("sqs").get_queue_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# get_queue_attributes method definition

await def get_queue_attributes(
    self,
    *,
    QueueUrl: str,
    AttributeNames: Sequence[QueueAttributeFilterType] = ...,  # (1)
) -> GetQueueAttributesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: QueueAttributeFilterType](./literals.md#queueattributefiltertype) 
2. See [:material-code-braces: GetQueueAttributesResultTypeDef](./type_defs.md#getqueueattributesresulttypedef) 


```python
# get_queue_attributes method usage example with argument unpacking

kwargs: GetQueueAttributesRequestRequestTypeDef = {  # (1)
    "QueueUrl": ...,
}

parent.get_queue_attributes(**kwargs)
```

1. See [:material-code-braces: GetQueueAttributesRequestRequestTypeDef](./type_defs.md#getqueueattributesrequestrequesttypedef) 

### get\_queue\_url

Returns the URL of an existing Amazon SQS queue.

Type annotations and code completion for `#!python session.client("sqs").get_queue_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# get_queue_url method definition

await def get_queue_url(
    self,
    *,
    QueueName: str,
    QueueOwnerAWSAccountId: str = ...,
) -> GetQueueUrlResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQueueUrlResultTypeDef](./type_defs.md#getqueueurlresulttypedef) 


```python
# get_queue_url method usage example with argument unpacking

kwargs: GetQueueUrlRequestRequestTypeDef = {  # (1)
    "QueueName": ...,
}

parent.get_queue_url(**kwargs)
```

1. See [:material-code-braces: GetQueueUrlRequestRequestTypeDef](./type_defs.md#getqueueurlrequestrequesttypedef) 

### list\_dead\_letter\_source\_queues

Returns a list of your queues that have the <code>RedrivePolicy</code> queue
attribute configured with a dead-letter queue.

Type annotations and code completion for `#!python session.client("sqs").list_dead_letter_source_queues` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# list_dead_letter_source_queues method definition

await def list_dead_letter_source_queues(
    self,
    *,
    QueueUrl: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDeadLetterSourceQueuesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDeadLetterSourceQueuesResultTypeDef](./type_defs.md#listdeadlettersourcequeuesresulttypedef) 


```python
# list_dead_letter_source_queues method usage example with argument unpacking

kwargs: ListDeadLetterSourceQueuesRequestRequestTypeDef = {  # (1)
    "QueueUrl": ...,
}

parent.list_dead_letter_source_queues(**kwargs)
```

1. See [:material-code-braces: ListDeadLetterSourceQueuesRequestRequestTypeDef](./type_defs.md#listdeadlettersourcequeuesrequestrequesttypedef) 

### list\_message\_move\_tasks

Gets the most recent message movement tasks (up to 10) under a specific source
queue.

Type annotations and code completion for `#!python session.client("sqs").list_message_move_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# list_message_move_tasks method definition

await def list_message_move_tasks(
    self,
    *,
    SourceArn: str,
    MaxResults: int = ...,
) -> ListMessageMoveTasksResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMessageMoveTasksResultTypeDef](./type_defs.md#listmessagemovetasksresulttypedef) 


```python
# list_message_move_tasks method usage example with argument unpacking

kwargs: ListMessageMoveTasksRequestRequestTypeDef = {  # (1)
    "SourceArn": ...,
}

parent.list_message_move_tasks(**kwargs)
```

1. See [:material-code-braces: ListMessageMoveTasksRequestRequestTypeDef](./type_defs.md#listmessagemovetasksrequestrequesttypedef) 

### list\_queue\_tags

List all cost allocation tags added to the specified Amazon SQS queue.

Type annotations and code completion for `#!python session.client("sqs").list_queue_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# list_queue_tags method definition

await def list_queue_tags(
    self,
    *,
    QueueUrl: str,
) -> ListQueueTagsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListQueueTagsResultTypeDef](./type_defs.md#listqueuetagsresulttypedef) 


```python
# list_queue_tags method usage example with argument unpacking

kwargs: ListQueueTagsRequestRequestTypeDef = {  # (1)
    "QueueUrl": ...,
}

parent.list_queue_tags(**kwargs)
```

1. See [:material-code-braces: ListQueueTagsRequestRequestTypeDef](./type_defs.md#listqueuetagsrequestrequesttypedef) 

### list\_queues

Returns a list of your queues in the current region.

Type annotations and code completion for `#!python session.client("sqs").list_queues` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# list_queues method definition

await def list_queues(
    self,
    *,
    QueueNamePrefix: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListQueuesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListQueuesResultTypeDef](./type_defs.md#listqueuesresulttypedef) 


```python
# list_queues method usage example with argument unpacking

kwargs: ListQueuesRequestRequestTypeDef = {  # (1)
    "QueueNamePrefix": ...,
}

parent.list_queues(**kwargs)
```

1. See [:material-code-braces: ListQueuesRequestRequestTypeDef](./type_defs.md#listqueuesrequestrequesttypedef) 

### purge\_queue

Deletes available messages in a queue (including in-flight messages) specified
by the <code>QueueURL</code> parameter.

Type annotations and code completion for `#!python session.client("sqs").purge_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# purge_queue method definition

await def purge_queue(
    self,
    *,
    QueueUrl: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# purge_queue method usage example with argument unpacking

kwargs: PurgeQueueRequestRequestTypeDef = {  # (1)
    "QueueUrl": ...,
}

parent.purge_queue(**kwargs)
```

1. See [:material-code-braces: PurgeQueueRequestRequestTypeDef](./type_defs.md#purgequeuerequestrequesttypedef) 

### receive\_message

Retrieves one or more messages (up to 10), from the specified queue.

Type annotations and code completion for `#!python session.client("sqs").receive_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# receive_message method definition

await def receive_message(
    self,
    *,
    QueueUrl: str,
    AttributeNames: Sequence[QueueAttributeFilterType] = ...,  # (1)
    MessageSystemAttributeNames: Sequence[MessageSystemAttributeNameType] = ...,  # (2)
    MessageAttributeNames: Sequence[str] = ...,
    MaxNumberOfMessages: int = ...,
    VisibilityTimeout: int = ...,
    WaitTimeSeconds: int = ...,
    ReceiveRequestAttemptId: str = ...,
) -> ReceiveMessageResultTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: QueueAttributeFilterType](./literals.md#queueattributefiltertype) 
2. See [:material-code-brackets: MessageSystemAttributeNameType](./literals.md#messagesystemattributenametype) 
3. See [:material-code-braces: ReceiveMessageResultTypeDef](./type_defs.md#receivemessageresulttypedef) 


```python
# receive_message method usage example with argument unpacking

kwargs: ReceiveMessageRequestRequestTypeDef = {  # (1)
    "QueueUrl": ...,
}

parent.receive_message(**kwargs)
```

1. See [:material-code-braces: ReceiveMessageRequestRequestTypeDef](./type_defs.md#receivemessagerequestrequesttypedef) 

### remove\_permission

Revokes any permissions in the queue policy that matches the specified
<code>Label</code> parameter.

Type annotations and code completion for `#!python session.client("sqs").remove_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# remove_permission method definition

await def remove_permission(
    self,
    *,
    QueueUrl: str,
    Label: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# remove_permission method usage example with argument unpacking

kwargs: RemovePermissionRequestRequestTypeDef = {  # (1)
    "QueueUrl": ...,
    "Label": ...,
}

parent.remove_permission(**kwargs)
```

1. See [:material-code-braces: RemovePermissionRequestRequestTypeDef](./type_defs.md#removepermissionrequestrequesttypedef) 

### send\_message

Delivers a message to the specified queue.

Type annotations and code completion for `#!python session.client("sqs").send_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# send_message method definition

await def send_message(
    self,
    *,
    QueueUrl: str,
    MessageBody: str,
    DelaySeconds: int = ...,
    MessageAttributes: Mapping[str, MessageAttributeValueUnionTypeDef] = ...,  # (1)
    MessageSystemAttributes: Mapping[MessageSystemAttributeNameForSendsType, MessageSystemAttributeValueTypeDef] = ...,  # (2)
    MessageDeduplicationId: str = ...,
    MessageGroupId: str = ...,
) -> SendMessageResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: MessageAttributeValueTypeDef](./type_defs.md#messageattributevaluetypedef) [:material-code-braces: MessageAttributeValueOutputTypeDef](./type_defs.md#messageattributevalueoutputtypedef) 
2. See [:material-code-brackets: MessageSystemAttributeNameForSendsType](./literals.md#messagesystemattributenameforsendstype) [:material-code-braces: MessageSystemAttributeValueTypeDef](./type_defs.md#messagesystemattributevaluetypedef) 
3. See [:material-code-braces: SendMessageResultTypeDef](./type_defs.md#sendmessageresulttypedef) 


```python
# send_message method usage example with argument unpacking

kwargs: SendMessageRequestRequestTypeDef = {  # (1)
    "QueueUrl": ...,
    "MessageBody": ...,
}

parent.send_message(**kwargs)
```

1. See [:material-code-braces: SendMessageRequestRequestTypeDef](./type_defs.md#sendmessagerequestrequesttypedef) 

### send\_message\_batch

You can use <code>SendMessageBatch</code> to send up to 10 messages to the
specified queue by assigning either identical or different values to each
message (or by not assigning values at all).

Type annotations and code completion for `#!python session.client("sqs").send_message_batch` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# send_message_batch method definition

await def send_message_batch(
    self,
    *,
    QueueUrl: str,
    Entries: Sequence[SendMessageBatchRequestEntryTypeDef],  # (1)
) -> SendMessageBatchResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SendMessageBatchRequestEntryTypeDef](./type_defs.md#sendmessagebatchrequestentrytypedef) 
2. See [:material-code-braces: SendMessageBatchResultTypeDef](./type_defs.md#sendmessagebatchresulttypedef) 


```python
# send_message_batch method usage example with argument unpacking

kwargs: SendMessageBatchRequestRequestTypeDef = {  # (1)
    "QueueUrl": ...,
    "Entries": ...,
}

parent.send_message_batch(**kwargs)
```

1. See [:material-code-braces: SendMessageBatchRequestRequestTypeDef](./type_defs.md#sendmessagebatchrequestrequesttypedef) 

### set\_queue\_attributes

Sets the value of one or more queue attributes, like a policy.

Type annotations and code completion for `#!python session.client("sqs").set_queue_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# set_queue_attributes method definition

await def set_queue_attributes(
    self,
    *,
    QueueUrl: str,
    Attributes: Mapping[QueueAttributeNameType, str],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: QueueAttributeNameType](./literals.md#queueattributenametype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# set_queue_attributes method usage example with argument unpacking

kwargs: SetQueueAttributesRequestRequestTypeDef = {  # (1)
    "QueueUrl": ...,
    "Attributes": ...,
}

parent.set_queue_attributes(**kwargs)
```

1. See [:material-code-braces: SetQueueAttributesRequestRequestTypeDef](./type_defs.md#setqueueattributesrequestrequesttypedef) 

### start\_message\_move\_task

Starts an asynchronous task to move messages from a specified source queue to a
specified destination queue.

Type annotations and code completion for `#!python session.client("sqs").start_message_move_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# start_message_move_task method definition

await def start_message_move_task(
    self,
    *,
    SourceArn: str,
    DestinationArn: str = ...,
    MaxNumberOfMessagesPerSecond: int = ...,
) -> StartMessageMoveTaskResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartMessageMoveTaskResultTypeDef](./type_defs.md#startmessagemovetaskresulttypedef) 


```python
# start_message_move_task method usage example with argument unpacking

kwargs: StartMessageMoveTaskRequestRequestTypeDef = {  # (1)
    "SourceArn": ...,
}

parent.start_message_move_task(**kwargs)
```

1. See [:material-code-braces: StartMessageMoveTaskRequestRequestTypeDef](./type_defs.md#startmessagemovetaskrequestrequesttypedef) 

### tag\_queue

Add cost allocation tags to the specified Amazon SQS queue.

Type annotations and code completion for `#!python session.client("sqs").tag_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# tag_queue method definition

await def tag_queue(
    self,
    *,
    QueueUrl: str,
    Tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_queue method usage example with argument unpacking

kwargs: TagQueueRequestRequestTypeDef = {  # (1)
    "QueueUrl": ...,
    "Tags": ...,
}

parent.tag_queue(**kwargs)
```

1. See [:material-code-braces: TagQueueRequestRequestTypeDef](./type_defs.md#tagqueuerequestrequesttypedef) 

### untag\_queue

Remove cost allocation tags from the specified Amazon SQS queue.

Type annotations and code completion for `#!python session.client("sqs").untag_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# untag_queue method definition

await def untag_queue(
    self,
    *,
    QueueUrl: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_queue method usage example with argument unpacking

kwargs: UntagQueueRequestRequestTypeDef = {  # (1)
    "QueueUrl": ...,
    "TagKeys": ...,
}

parent.untag_queue(**kwargs)
```

1. See [:material-code-braces: UntagQueueRequestRequestTypeDef](./type_defs.md#untagqueuerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("sqs").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("sqs").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)

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

Type annotations and code completion for `#!python session.client("sqs").get_paginator` method with overloads.

- `client.get_paginator("list_dead_letter_source_queues")` -> [ListDeadLetterSourceQueuesPaginator](./paginators.md#listdeadlettersourcequeuespaginator)
- `client.get_paginator("list_queues")` -> [ListQueuesPaginator](./paginators.md#listqueuespaginator)


