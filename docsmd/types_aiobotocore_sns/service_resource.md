# SNSServiceResource

> [Index](../README.md) > [SNS](./README.md) > SNSServiceResource

!!! note ""

    Auto-generated documentation for [SNS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#sns)
    type annotations stubs module [types-aiobotocore-sns](https://pypi.org/project/types-aiobotocore-sns/).

## SNSServiceResource

Type annotations and code completion for `#!python session.resource("sns")`, included resources and collections.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/service-resource/index.html)

```python
# SNSServiceResource usage example

from aioboto3.session import Session
from types_aiobotocore_sns.service_resource import SNSServiceResource

session = Session()
async with session.resource("sns") as resource:
    resource: SNSServiceResource
```


## Attributes


- `meta`: `SNSResourceMeta`

- `platform_applications`: `ServiceResourcePlatformApplicationsCollection`

- `subscriptions`: `ServiceResourceSubscriptionsCollection`

- `topics`: `ServiceResourceTopicsCollection`




## Collections

### ServiceResourcePlatformApplicationsCollection

Provides access to [PlatformApplication](#platformapplication) resource.

Type annotations and code completion for `#!python session.resource("sns").platform_applications` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/service-resource/platform_applications.html#SNS.ServiceResource.platform_applications)

```python
# ServiceResourcePlatformApplicationsCollection usage example

from types_aiobotocore_sns.service_resource import ServiceResourcePlatformApplicationsCollection,

def get_collection() -> ServiceResourcePlatformApplicationsCollection:
    return session.resource("sns").platform_applications
```

### ServiceResourceSubscriptionsCollection

Provides access to [Subscription](#subscription) resource.

Type annotations and code completion for `#!python session.resource("sns").subscriptions` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/service-resource/subscriptions.html#SNS.ServiceResource.subscriptions)

```python
# ServiceResourceSubscriptionsCollection usage example

from types_aiobotocore_sns.service_resource import ServiceResourceSubscriptionsCollection,

def get_collection() -> ServiceResourceSubscriptionsCollection:
    return session.resource("sns").subscriptions
```

### ServiceResourceTopicsCollection

Provides access to [Topic](#topic) resource.

Type annotations and code completion for `#!python session.resource("sns").topics` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/service-resource/topics.html#SNS.ServiceResource.topics)

```python
# ServiceResourceTopicsCollection usage example

from types_aiobotocore_sns.service_resource import ServiceResourceTopicsCollection,

def get_collection() -> ServiceResourceTopicsCollection:
    return session.resource("sns").topics
```



## Methods

### SNSServiceResource.get\_available\_subresources method

Returns a list of all the available sub-resources for this resource.

Type annotations and code completion for `#!python session.resource("sns").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/service-resource/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


### SNSServiceResource.create\_platform\_application method

Creates a platform application object for one of the supported push
notification services, such as APNS and GCM (Firebase Cloud Messaging), to
which devices and mobile apps may register.

Type annotations and code completion for `#!python session.resource("sns").create_platform_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/service-resource/create_platform_application.html)

```python
# create_platform_application method definition

await def create_platform_application(
    self,
    *,
    Name: str,
    Platform: str,
    Attributes: Mapping[str, str],
) -> _PlatformApplication:
    ...
```



```python
# create_platform_application method usage example with argument unpacking

kwargs: CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef = {  # (1)
    "Name": ...,
    "Platform": ...,
    "Attributes": ...,
}

parent.create_platform_application(**kwargs)
```

1. See [:material-code-braces: CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef](./type_defs.md#createplatformapplicationinputserviceresourcecreateplatformapplicationtypedef) 

### SNSServiceResource.create\_topic method

Creates a topic to which notifications can be published.

Type annotations and code completion for `#!python session.resource("sns").create_topic` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/service-resource/create_topic.html)

```python
# create_topic method definition

await def create_topic(
    self,
    *,
    Name: str,
    Attributes: Mapping[str, str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    DataProtectionPolicy: str = ...,
) -> _Topic:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# create_topic method usage example with argument unpacking

kwargs: CreateTopicInputServiceResourceCreateTopicTypeDef = {  # (1)
    "Name": ...,
}

parent.create_topic(**kwargs)
```

1. See [:material-code-braces: CreateTopicInputServiceResourceCreateTopicTypeDef](./type_defs.md#createtopicinputserviceresourcecreatetopictypedef) 

### SNSServiceResource.PlatformApplication method

Creates a PlatformApplication resource.

Type annotations and code completion for `#!python session.resource("sns").PlatformApplication` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/service-resource/PlatformApplication.html)

```python
# PlatformApplication method definition

await def PlatformApplication(
    self,
    arn: str,
) -> _PlatformApplication:
    ...
```


### SNSServiceResource.PlatformEndpoint method

Creates a PlatformEndpoint resource.

Type annotations and code completion for `#!python session.resource("sns").PlatformEndpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/service-resource/PlatformEndpoint.html)

```python
# PlatformEndpoint method definition

await def PlatformEndpoint(
    self,
    arn: str,
) -> _PlatformEndpoint:
    ...
```


### SNSServiceResource.Subscription method

Creates a Subscription resource.

Type annotations and code completion for `#!python session.resource("sns").Subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/service-resource/Subscription.html)

```python
# Subscription method definition

await def Subscription(
    self,
    arn: str,
) -> _Subscription:
    ...
```


### SNSServiceResource.Topic method

Creates a Topic resource.

Type annotations and code completion for `#!python session.resource("sns").Topic` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/service-resource/Topic.html)

```python
# Topic method definition

await def Topic(
    self,
    arn: str,
) -> _Topic:
    ...
```




## PlatformApplication

Type annotations and code completion for `#!python session.resource("sns").PlatformApplication` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/platformapplication/index.html#SNS.PlatformApplication)

```python
# PlatformApplication usage example

from types_aiobotocore_sns.service_resource import PlatformApplication


async def get_resource() -> PlatformApplication:
    async with session.resource("sns") as resource:
        return await resource.PlatformApplication(...)
```


### PlatformApplication attributes


- `arn`: `str`
- `endpoints`: `PlatformApplicationEndpointsCollection`
- `attributes`: `Awaitable`[`dict`[`str`, `str`]]
- `meta`: `SNSResourceMeta`



### PlatformApplication collections


#### PlatformApplication.endpoints

Provides access to [PlatformEndpoint](#platformendpoint) resource.

Type annotations and code completion for `#!python session.resource("sns").PlatformApplication(...).endpoints` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/platformapplication/endpoints.html#SNS.PlatformApplication.endpoints)

```python
# PlatformApplicationEndpointsCollection usage example

from types_aiobotocore_sns.service_resource import PlatformApplicationEndpointsCollection,

def get_collection() -> PlatformApplicationEndpointsCollection:
    resource = session.resource("sns").PlatformApplication(...)
    return resource.endpoints
```




### PlatformApplication methods


#### PlatformApplication.get\_available\_subresources method

Returns a list of all the available sub-resources for this PlatformApplication.

Type annotations and code completion for `#!python aioboto3.resource("sns").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/platformapplication/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### PlatformApplication.create\_platform\_endpoint method

Creates an endpoint for a device and mobile app on one of the supported push
notification services, such as GCM (Firebase Cloud Messaging) and APNS.

Type annotations and code completion for `#!python aioboto3.resource("sns").create_platform_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/platformapplication/create_platform_endpoint.html)

```python
# create_platform_endpoint method definition

await def create_platform_endpoint(
    self,
    *,
    Token: str,
    CustomUserData: str = ...,
    Attributes: Mapping[str, str] = ...,
) -> _PlatformEndpoint:
    ...
```



```python
# create_platform_endpoint method usage example with argument unpacking

kwargs: CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef = {  # (1)
    "Token": ...,
}

parent.create_platform_endpoint(**kwargs)
```

1. See [:material-code-braces: CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef](./type_defs.md#createplatformendpointinputplatformapplicationcreateplatformendpointtypedef) 

#### PlatformApplication.delete method

Deletes a platform application object for one of the supported push
notification services, such as APNS and GCM (Firebase Cloud Messaging).

Type annotations and code completion for `#!python aioboto3.resource("sns").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/platformapplication/delete.html)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### PlatformApplication.set\_attributes method

Sets the attributes of the platform application object for the supported push
notification services, such as APNS and GCM (Firebase Cloud Messaging).

Type annotations and code completion for `#!python aioboto3.resource("sns").set_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/platformapplication/set_attributes.html)

```python
# set_attributes method definition

await def set_attributes(
    self,
    *,
    Attributes: Mapping[str, str],
) -> None:
    ...
```



```python
# set_attributes method usage example with argument unpacking

kwargs: SetPlatformApplicationAttributesInputPlatformApplicationSetAttributesTypeDef = {  # (1)
    "Attributes": ...,
}

parent.set_attributes(**kwargs)
```

1. See [:material-code-braces: SetPlatformApplicationAttributesInputPlatformApplicationSetAttributesTypeDef](./type_defs.md#setplatformapplicationattributesinputplatformapplicationsetattributestypedef) 

#### PlatformApplication.load method



Type annotations and code completion for `#!python aioboto3.resource("sns").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/platformapplication/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### PlatformApplication.reload method



Type annotations and code completion for `#!python aioboto3.resource("sns").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/platformapplication/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## PlatformEndpoint

Type annotations and code completion for `#!python session.resource("sns").PlatformEndpoint` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/platformendpoint/index.html#SNS.PlatformEndpoint)

```python
# PlatformEndpoint usage example

from types_aiobotocore_sns.service_resource import PlatformEndpoint


async def get_resource() -> PlatformEndpoint:
    async with session.resource("sns") as resource:
        return await resource.PlatformEndpoint(...)
```


### PlatformEndpoint attributes


- `arn`: `str`
- `attributes`: `Awaitable`[`dict`[`str`, `str`]]
- `meta`: `SNSResourceMeta`





### PlatformEndpoint methods


#### PlatformEndpoint.get\_available\_subresources method

Returns a list of all the available sub-resources for this PlatformEndpoint.

Type annotations and code completion for `#!python aioboto3.resource("sns").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/platformendpoint/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### PlatformEndpoint.delete method

Deletes the endpoint for a device and mobile app from Amazon SNS.

Type annotations and code completion for `#!python aioboto3.resource("sns").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/platformendpoint/delete.html)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### PlatformEndpoint.publish method

Sends a message to an Amazon SNS topic, a text message (SMS message) directly
to a phone number, or a message to a mobile platform endpoint (when you specify
the <code>TargetArn</code>).

Type annotations and code completion for `#!python aioboto3.resource("sns").publish` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/platformendpoint/publish.html)

```python
# publish method definition

await def publish(
    self,
    *,
    Message: str,
    TopicArn: str = ...,
    PhoneNumber: str = ...,
    Subject: str = ...,
    MessageStructure: str = ...,
    MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,  # (1)
    MessageDeduplicationId: str = ...,
    MessageGroupId: str = ...,
) -> PublishResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MessageAttributeValueTypeDef](./type_defs.md#messageattributevaluetypedef) 
2. See [:material-code-braces: PublishResponseTypeDef](./type_defs.md#publishresponsetypedef) 


```python
# publish method usage example with argument unpacking

kwargs: PublishInputPlatformEndpointPublishTypeDef = {  # (1)
    "Message": ...,
}

parent.publish(**kwargs)
```

1. See [:material-code-braces: PublishInputPlatformEndpointPublishTypeDef](./type_defs.md#publishinputplatformendpointpublishtypedef) 

#### PlatformEndpoint.set\_attributes method

Sets the attributes for an endpoint for a device on one of the supported push
notification services, such as GCM (Firebase Cloud Messaging) and APNS.

Type annotations and code completion for `#!python aioboto3.resource("sns").set_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/platformendpoint/set_attributes.html)

```python
# set_attributes method definition

await def set_attributes(
    self,
    *,
    Attributes: Mapping[str, str],
) -> None:
    ...
```



```python
# set_attributes method usage example with argument unpacking

kwargs: SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef = {  # (1)
    "Attributes": ...,
}

parent.set_attributes(**kwargs)
```

1. See [:material-code-braces: SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef](./type_defs.md#setendpointattributesinputplatformendpointsetattributestypedef) 

#### PlatformEndpoint.load method



Type annotations and code completion for `#!python aioboto3.resource("sns").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/platformendpoint/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### PlatformEndpoint.reload method



Type annotations and code completion for `#!python aioboto3.resource("sns").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/platformendpoint/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## Subscription

Type annotations and code completion for `#!python session.resource("sns").Subscription` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/subscription/index.html#SNS.Subscription)

```python
# Subscription usage example

from types_aiobotocore_sns.service_resource import Subscription


async def get_resource() -> Subscription:
    async with session.resource("sns") as resource:
        return await resource.Subscription(...)
```


### Subscription attributes


- `arn`: `str`
- `attributes`: `Awaitable`[`dict`[`str`, `str`]]
- `meta`: `SNSResourceMeta`





### Subscription methods


#### Subscription.get\_available\_subresources method

Returns a list of all the available sub-resources for this Subscription.

Type annotations and code completion for `#!python aioboto3.resource("sns").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/subscription/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Subscription.delete method

Deletes a subscription.

Type annotations and code completion for `#!python aioboto3.resource("sns").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/subscription/delete.html)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### Subscription.set\_attributes method

Allows a subscription owner to set an attribute of the subscription to a new
value.

Type annotations and code completion for `#!python aioboto3.resource("sns").set_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/subscription/set_attributes.html)

```python
# set_attributes method definition

await def set_attributes(
    self,
    *,
    AttributeName: str,
    AttributeValue: str = ...,
) -> None:
    ...
```



```python
# set_attributes method usage example with argument unpacking

kwargs: SetSubscriptionAttributesInputSubscriptionSetAttributesTypeDef = {  # (1)
    "AttributeName": ...,
}

parent.set_attributes(**kwargs)
```

1. See [:material-code-braces: SetSubscriptionAttributesInputSubscriptionSetAttributesTypeDef](./type_defs.md#setsubscriptionattributesinputsubscriptionsetattributestypedef) 

#### Subscription.load method



Type annotations and code completion for `#!python aioboto3.resource("sns").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/subscription/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### Subscription.reload method



Type annotations and code completion for `#!python aioboto3.resource("sns").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/subscription/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## Topic

Type annotations and code completion for `#!python session.resource("sns").Topic` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/topic/index.html#SNS.Topic)

```python
# Topic usage example

from types_aiobotocore_sns.service_resource import Topic


async def get_resource() -> Topic:
    async with session.resource("sns") as resource:
        return await resource.Topic(...)
```


### Topic attributes


- `arn`: `str`
- `subscriptions`: `TopicSubscriptionsCollection`
- `attributes`: `Awaitable`[`dict`[`str`, `str`]]
- `meta`: `SNSResourceMeta`



### Topic collections


#### Topic.subscriptions

Provides access to [Subscription](#subscription) resource.

Type annotations and code completion for `#!python session.resource("sns").Topic(...).subscriptions` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/topic/subscriptions.html#SNS.Topic.subscriptions)

```python
# TopicSubscriptionsCollection usage example

from types_aiobotocore_sns.service_resource import TopicSubscriptionsCollection,

def get_collection() -> TopicSubscriptionsCollection:
    resource = session.resource("sns").Topic(...)
    return resource.subscriptions
```




### Topic methods


#### Topic.get\_available\_subresources method

Returns a list of all the available sub-resources for this Topic.

Type annotations and code completion for `#!python aioboto3.resource("sns").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/topic/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Topic.add\_permission method

Adds a statement to a topic's access control policy, granting access for the
specified Amazon Web Services accounts to the specified actions.

Type annotations and code completion for `#!python aioboto3.resource("sns").add_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/topic/add_permission.html)

```python
# add_permission method definition

await def add_permission(
    self,
    *,
    Label: str,
    AWSAccountId: Sequence[str],
    ActionName: Sequence[str],
) -> None:
    ...
```



```python
# add_permission method usage example with argument unpacking

kwargs: AddPermissionInputTopicAddPermissionTypeDef = {  # (1)
    "Label": ...,
    "AWSAccountId": ...,
    "ActionName": ...,
}

parent.add_permission(**kwargs)
```

1. See [:material-code-braces: AddPermissionInputTopicAddPermissionTypeDef](./type_defs.md#addpermissioninputtopicaddpermissiontypedef) 

#### Topic.confirm\_subscription method

Verifies an endpoint owner's intent to receive messages by validating the token
sent to the endpoint by an earlier <code>Subscribe</code> action.

Type annotations and code completion for `#!python aioboto3.resource("sns").confirm_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/topic/confirm_subscription.html)

```python
# confirm_subscription method definition

await def confirm_subscription(
    self,
    *,
    Token: str,
    AuthenticateOnUnsubscribe: str = ...,
) -> _Subscription:
    ...
```



```python
# confirm_subscription method usage example with argument unpacking

kwargs: ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef = {  # (1)
    "Token": ...,
}

parent.confirm_subscription(**kwargs)
```

1. See [:material-code-braces: ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef](./type_defs.md#confirmsubscriptioninputtopicconfirmsubscriptiontypedef) 

#### Topic.delete method

Deletes a topic and all its subscriptions.

Type annotations and code completion for `#!python aioboto3.resource("sns").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/topic/delete.html)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### Topic.publish method

Sends a message to an Amazon SNS topic, a text message (SMS message) directly
to a phone number, or a message to a mobile platform endpoint (when you specify
the <code>TargetArn</code>).

Type annotations and code completion for `#!python aioboto3.resource("sns").publish` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/topic/publish.html)

```python
# publish method definition

await def publish(
    self,
    *,
    Message: str,
    TargetArn: str = ...,
    PhoneNumber: str = ...,
    Subject: str = ...,
    MessageStructure: str = ...,
    MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,  # (1)
    MessageDeduplicationId: str = ...,
    MessageGroupId: str = ...,
) -> PublishResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MessageAttributeValueTypeDef](./type_defs.md#messageattributevaluetypedef) 
2. See [:material-code-braces: PublishResponseTypeDef](./type_defs.md#publishresponsetypedef) 


```python
# publish method usage example with argument unpacking

kwargs: PublishInputTopicPublishTypeDef = {  # (1)
    "Message": ...,
}

parent.publish(**kwargs)
```

1. See [:material-code-braces: PublishInputTopicPublishTypeDef](./type_defs.md#publishinputtopicpublishtypedef) 

#### Topic.remove\_permission method

Removes a statement from a topic's access control policy.

Type annotations and code completion for `#!python aioboto3.resource("sns").remove_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/topic/remove_permission.html)

```python
# remove_permission method definition

await def remove_permission(
    self,
    *,
    Label: str,
) -> None:
    ...
```



```python
# remove_permission method usage example with argument unpacking

kwargs: RemovePermissionInputTopicRemovePermissionTypeDef = {  # (1)
    "Label": ...,
}

parent.remove_permission(**kwargs)
```

1. See [:material-code-braces: RemovePermissionInputTopicRemovePermissionTypeDef](./type_defs.md#removepermissioninputtopicremovepermissiontypedef) 

#### Topic.set\_attributes method

Allows a topic owner to set an attribute of the topic to a new value.

Type annotations and code completion for `#!python aioboto3.resource("sns").set_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/topic/set_attributes.html)

```python
# set_attributes method definition

await def set_attributes(
    self,
    *,
    AttributeName: str,
    AttributeValue: str = ...,
) -> None:
    ...
```



```python
# set_attributes method usage example with argument unpacking

kwargs: SetTopicAttributesInputTopicSetAttributesTypeDef = {  # (1)
    "AttributeName": ...,
}

parent.set_attributes(**kwargs)
```

1. See [:material-code-braces: SetTopicAttributesInputTopicSetAttributesTypeDef](./type_defs.md#settopicattributesinputtopicsetattributestypedef) 

#### Topic.subscribe method

Subscribes an endpoint to an Amazon SNS topic.

Type annotations and code completion for `#!python aioboto3.resource("sns").subscribe` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/topic/subscribe.html)

```python
# subscribe method definition

await def subscribe(
    self,
    *,
    Protocol: str,
    Endpoint: str = ...,
    Attributes: Mapping[str, str] = ...,
    ReturnSubscriptionArn: bool = ...,
) -> _Subscription:
    ...
```



```python
# subscribe method usage example with argument unpacking

kwargs: SubscribeInputTopicSubscribeTypeDef = {  # (1)
    "Protocol": ...,
}

parent.subscribe(**kwargs)
```

1. See [:material-code-braces: SubscribeInputTopicSubscribeTypeDef](./type_defs.md#subscribeinputtopicsubscribetypedef) 

#### Topic.load method



Type annotations and code completion for `#!python aioboto3.resource("sns").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/topic/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### Topic.reload method



Type annotations and code completion for `#!python aioboto3.resource("sns").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns/topic/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```



