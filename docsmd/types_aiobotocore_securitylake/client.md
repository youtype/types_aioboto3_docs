# SecurityLakeClient

> [Index](../README.md) > [SecurityLake](./README.md) > SecurityLakeClient

!!! note ""

    Auto-generated documentation for [SecurityLake](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#securitylake)
    type annotations stubs module [types-aiobotocore-securitylake](https://pypi.org/project/types-aiobotocore-securitylake/).

## SecurityLakeClient

Type annotations and code completion for `#!python session.client("securitylake")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# SecurityLakeClient usage example

from aioboto3.session import Session
from types_aiobotocore_securitylake.client import SecurityLakeClient

session = Session()
async with session.client("securitylake") as client:
    client: SecurityLakeClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("securitylake").exceptions` structure.

```python
# SecurityLakeClient.exceptions usage example

async with session.client("securitylake") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.BadRequestException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ThrottlingException,
    ) as e:
        print(e)
```

```python
# SecurityLakeClient.exceptions type checking example

from types_aiobotocore_securitylake.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("securitylake").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("securitylake").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

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


### create\_aws\_log\_source

Adds a natively supported Amazon Web Services service as an Amazon Security
Lake source.

Type annotations and code completion for `#!python session.client("securitylake").create_aws_log_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# create_aws_log_source method definition

await def create_aws_log_source(
    self,
    *,
    sources: Sequence[AwsLogSourceConfigurationTypeDef],  # (1)
) -> CreateAwsLogSourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AwsLogSourceConfigurationTypeDef](./type_defs.md#awslogsourceconfigurationtypedef) 
2. See [:material-code-braces: CreateAwsLogSourceResponseTypeDef](./type_defs.md#createawslogsourceresponsetypedef) 


```python
# create_aws_log_source method usage example with argument unpacking

kwargs: CreateAwsLogSourceRequestRequestTypeDef = {  # (1)
    "sources": ...,
}

parent.create_aws_log_source(**kwargs)
```

1. See [:material-code-braces: CreateAwsLogSourceRequestRequestTypeDef](./type_defs.md#createawslogsourcerequestrequesttypedef) 

### create\_custom\_log\_source

Adds a third-party custom source in Amazon Security Lake, from the Amazon Web
Services Region where you want to create a custom source.

Type annotations and code completion for `#!python session.client("securitylake").create_custom_log_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# create_custom_log_source method definition

await def create_custom_log_source(
    self,
    *,
    configuration: CustomLogSourceConfigurationTypeDef,  # (1)
    sourceName: str,
    eventClasses: Sequence[str] = ...,
    sourceVersion: str = ...,
) -> CreateCustomLogSourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CustomLogSourceConfigurationTypeDef](./type_defs.md#customlogsourceconfigurationtypedef) 
2. See [:material-code-braces: CreateCustomLogSourceResponseTypeDef](./type_defs.md#createcustomlogsourceresponsetypedef) 


```python
# create_custom_log_source method usage example with argument unpacking

kwargs: CreateCustomLogSourceRequestRequestTypeDef = {  # (1)
    "configuration": ...,
    "sourceName": ...,
}

parent.create_custom_log_source(**kwargs)
```

1. See [:material-code-braces: CreateCustomLogSourceRequestRequestTypeDef](./type_defs.md#createcustomlogsourcerequestrequesttypedef) 

### create\_data\_lake

Initializes an Amazon Security Lake instance with the provided (or default)
configuration.

Type annotations and code completion for `#!python session.client("securitylake").create_data_lake` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# create_data_lake method definition

await def create_data_lake(
    self,
    *,
    configurations: Sequence[DataLakeConfigurationTypeDef],  # (1)
    metaStoreManagerRoleArn: str,
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateDataLakeResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DataLakeConfigurationTypeDef](./type_defs.md#datalakeconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateDataLakeResponseTypeDef](./type_defs.md#createdatalakeresponsetypedef) 


```python
# create_data_lake method usage example with argument unpacking

kwargs: CreateDataLakeRequestRequestTypeDef = {  # (1)
    "configurations": ...,
    "metaStoreManagerRoleArn": ...,
}

parent.create_data_lake(**kwargs)
```

1. See [:material-code-braces: CreateDataLakeRequestRequestTypeDef](./type_defs.md#createdatalakerequestrequesttypedef) 

### create\_data\_lake\_exception\_subscription

Creates the specified notification subscription in Amazon Security Lake for the
organization you specify.

Type annotations and code completion for `#!python session.client("securitylake").create_data_lake_exception_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# create_data_lake_exception_subscription method definition

await def create_data_lake_exception_subscription(
    self,
    *,
    notificationEndpoint: str,
    subscriptionProtocol: str,
    exceptionTimeToLive: int = ...,
) -> dict[str, Any]:
    ...
```



```python
# create_data_lake_exception_subscription method usage example with argument unpacking

kwargs: CreateDataLakeExceptionSubscriptionRequestRequestTypeDef = {  # (1)
    "notificationEndpoint": ...,
    "subscriptionProtocol": ...,
}

parent.create_data_lake_exception_subscription(**kwargs)
```

1. See [:material-code-braces: CreateDataLakeExceptionSubscriptionRequestRequestTypeDef](./type_defs.md#createdatalakeexceptionsubscriptionrequestrequesttypedef) 

### create\_data\_lake\_organization\_configuration

Automatically enables Amazon Security Lake for new member accounts in your
organization.

Type annotations and code completion for `#!python session.client("securitylake").create_data_lake_organization_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# create_data_lake_organization_configuration method definition

await def create_data_lake_organization_configuration(
    self,
    *,
    autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationUnionTypeDef] = ...,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: DataLakeAutoEnableNewAccountConfigurationTypeDef](./type_defs.md#datalakeautoenablenewaccountconfigurationtypedef) [:material-code-braces: DataLakeAutoEnableNewAccountConfigurationOutputTypeDef](./type_defs.md#datalakeautoenablenewaccountconfigurationoutputtypedef) 


```python
# create_data_lake_organization_configuration method usage example with argument unpacking

kwargs: CreateDataLakeOrganizationConfigurationRequestRequestTypeDef = {  # (1)
    "autoEnableNewAccount": ...,
}

parent.create_data_lake_organization_configuration(**kwargs)
```

1. See [:material-code-braces: CreateDataLakeOrganizationConfigurationRequestRequestTypeDef](./type_defs.md#createdatalakeorganizationconfigurationrequestrequesttypedef) 

### create\_subscriber

Creates a subscriber for accounts that are already enabled in Amazon Security
Lake.

Type annotations and code completion for `#!python session.client("securitylake").create_subscriber` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# create_subscriber method definition

await def create_subscriber(
    self,
    *,
    sources: Sequence[LogSourceResourceTypeDef],  # (1)
    subscriberIdentity: AwsIdentityTypeDef,  # (2)
    subscriberName: str,
    accessTypes: Sequence[AccessTypeType] = ...,  # (3)
    subscriberDescription: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateSubscriberResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: LogSourceResourceTypeDef](./type_defs.md#logsourceresourcetypedef) 
2. See [:material-code-braces: AwsIdentityTypeDef](./type_defs.md#awsidentitytypedef) 
3. See [:material-code-brackets: AccessTypeType](./literals.md#accesstypetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateSubscriberResponseTypeDef](./type_defs.md#createsubscriberresponsetypedef) 


```python
# create_subscriber method usage example with argument unpacking

kwargs: CreateSubscriberRequestRequestTypeDef = {  # (1)
    "sources": ...,
    "subscriberIdentity": ...,
    "subscriberName": ...,
}

parent.create_subscriber(**kwargs)
```

1. See [:material-code-braces: CreateSubscriberRequestRequestTypeDef](./type_defs.md#createsubscriberrequestrequesttypedef) 

### create\_subscriber\_notification

Notifies the subscriber when new data is written to the data lake for the
sources that the subscriber consumes in Security Lake.

Type annotations and code completion for `#!python session.client("securitylake").create_subscriber_notification` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# create_subscriber_notification method definition

await def create_subscriber_notification(
    self,
    *,
    configuration: NotificationConfigurationTypeDef,  # (1)
    subscriberId: str,
) -> CreateSubscriberNotificationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
2. See [:material-code-braces: CreateSubscriberNotificationResponseTypeDef](./type_defs.md#createsubscribernotificationresponsetypedef) 


```python
# create_subscriber_notification method usage example with argument unpacking

kwargs: CreateSubscriberNotificationRequestRequestTypeDef = {  # (1)
    "configuration": ...,
    "subscriberId": ...,
}

parent.create_subscriber_notification(**kwargs)
```

1. See [:material-code-braces: CreateSubscriberNotificationRequestRequestTypeDef](./type_defs.md#createsubscribernotificationrequestrequesttypedef) 

### delete\_aws\_log\_source

Removes a natively supported Amazon Web Services service as an Amazon Security
Lake source.

Type annotations and code completion for `#!python session.client("securitylake").delete_aws_log_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# delete_aws_log_source method definition

await def delete_aws_log_source(
    self,
    *,
    sources: Sequence[AwsLogSourceConfigurationTypeDef],  # (1)
) -> DeleteAwsLogSourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AwsLogSourceConfigurationTypeDef](./type_defs.md#awslogsourceconfigurationtypedef) 
2. See [:material-code-braces: DeleteAwsLogSourceResponseTypeDef](./type_defs.md#deleteawslogsourceresponsetypedef) 


```python
# delete_aws_log_source method usage example with argument unpacking

kwargs: DeleteAwsLogSourceRequestRequestTypeDef = {  # (1)
    "sources": ...,
}

parent.delete_aws_log_source(**kwargs)
```

1. See [:material-code-braces: DeleteAwsLogSourceRequestRequestTypeDef](./type_defs.md#deleteawslogsourcerequestrequesttypedef) 

### delete\_custom\_log\_source

Removes a custom log source from Amazon Security Lake, to stop sending data
from the custom source to Security Lake.

Type annotations and code completion for `#!python session.client("securitylake").delete_custom_log_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# delete_custom_log_source method definition

await def delete_custom_log_source(
    self,
    *,
    sourceName: str,
    sourceVersion: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_custom_log_source method usage example with argument unpacking

kwargs: DeleteCustomLogSourceRequestRequestTypeDef = {  # (1)
    "sourceName": ...,
}

parent.delete_custom_log_source(**kwargs)
```

1. See [:material-code-braces: DeleteCustomLogSourceRequestRequestTypeDef](./type_defs.md#deletecustomlogsourcerequestrequesttypedef) 

### delete\_data\_lake

When you disable Amazon Security Lake from your account, Security Lake is
disabled in all Amazon Web Services Regions and it stops collecting data from
your sources.

Type annotations and code completion for `#!python session.client("securitylake").delete_data_lake` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# delete_data_lake method definition

await def delete_data_lake(
    self,
    *,
    regions: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# delete_data_lake method usage example with argument unpacking

kwargs: DeleteDataLakeRequestRequestTypeDef = {  # (1)
    "regions": ...,
}

parent.delete_data_lake(**kwargs)
```

1. See [:material-code-braces: DeleteDataLakeRequestRequestTypeDef](./type_defs.md#deletedatalakerequestrequesttypedef) 

### delete\_data\_lake\_exception\_subscription

Deletes the specified notification subscription in Amazon Security Lake for the
organization you specify.

Type annotations and code completion for `#!python session.client("securitylake").delete_data_lake_exception_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# delete_data_lake_exception_subscription method definition

await def delete_data_lake_exception_subscription(
    self,
) -> dict[str, Any]:
    ...
```


### delete\_data\_lake\_organization\_configuration

Turns off automatic enablement of Amazon Security Lake for member accounts that
are added to an organization in Organizations.

Type annotations and code completion for `#!python session.client("securitylake").delete_data_lake_organization_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# delete_data_lake_organization_configuration method definition

await def delete_data_lake_organization_configuration(
    self,
    *,
    autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef] = ...,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: DataLakeAutoEnableNewAccountConfigurationTypeDef](./type_defs.md#datalakeautoenablenewaccountconfigurationtypedef) 


```python
# delete_data_lake_organization_configuration method usage example with argument unpacking

kwargs: DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef = {  # (1)
    "autoEnableNewAccount": ...,
}

parent.delete_data_lake_organization_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef](./type_defs.md#deletedatalakeorganizationconfigurationrequestrequesttypedef) 

### delete\_subscriber

Deletes the subscription permission and all notification settings for accounts
that are already enabled in Amazon Security Lake.

Type annotations and code completion for `#!python session.client("securitylake").delete_subscriber` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# delete_subscriber method definition

await def delete_subscriber(
    self,
    *,
    subscriberId: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_subscriber method usage example with argument unpacking

kwargs: DeleteSubscriberRequestRequestTypeDef = {  # (1)
    "subscriberId": ...,
}

parent.delete_subscriber(**kwargs)
```

1. See [:material-code-braces: DeleteSubscriberRequestRequestTypeDef](./type_defs.md#deletesubscriberrequestrequesttypedef) 

### delete\_subscriber\_notification

Deletes the specified subscription notification in Amazon Security Lake for the
organization you specify.

Type annotations and code completion for `#!python session.client("securitylake").delete_subscriber_notification` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# delete_subscriber_notification method definition

await def delete_subscriber_notification(
    self,
    *,
    subscriberId: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_subscriber_notification method usage example with argument unpacking

kwargs: DeleteSubscriberNotificationRequestRequestTypeDef = {  # (1)
    "subscriberId": ...,
}

parent.delete_subscriber_notification(**kwargs)
```

1. See [:material-code-braces: DeleteSubscriberNotificationRequestRequestTypeDef](./type_defs.md#deletesubscribernotificationrequestrequesttypedef) 

### deregister\_data\_lake\_delegated\_administrator

Deletes the Amazon Security Lake delegated administrator account for the
organization.

Type annotations and code completion for `#!python session.client("securitylake").deregister_data_lake_delegated_administrator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# deregister_data_lake_delegated_administrator method definition

await def deregister_data_lake_delegated_administrator(
    self,
) -> dict[str, Any]:
    ...
```


### get\_data\_lake\_exception\_subscription

Retrieves the protocol and endpoint that were provided when subscribing to
Amazon SNS topics for exception notifications.

Type annotations and code completion for `#!python session.client("securitylake").get_data_lake_exception_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# get_data_lake_exception_subscription method definition

await def get_data_lake_exception_subscription(
    self,
) -> GetDataLakeExceptionSubscriptionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataLakeExceptionSubscriptionResponseTypeDef](./type_defs.md#getdatalakeexceptionsubscriptionresponsetypedef) 

### get\_data\_lake\_organization\_configuration

Retrieves the configuration that will be automatically set up for accounts
added to the organization after the organization has onboarded to Amazon
Security Lake.

Type annotations and code completion for `#!python session.client("securitylake").get_data_lake_organization_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# get_data_lake_organization_configuration method definition

await def get_data_lake_organization_configuration(
    self,
) -> GetDataLakeOrganizationConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataLakeOrganizationConfigurationResponseTypeDef](./type_defs.md#getdatalakeorganizationconfigurationresponsetypedef) 

### get\_data\_lake\_sources

Retrieves a snapshot of the current Region, including whether Amazon Security
Lake is enabled for those accounts and which sources Security Lake is
collecting data from.

Type annotations and code completion for `#!python session.client("securitylake").get_data_lake_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# get_data_lake_sources method definition

await def get_data_lake_sources(
    self,
    *,
    accounts: Sequence[str] = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> GetDataLakeSourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataLakeSourcesResponseTypeDef](./type_defs.md#getdatalakesourcesresponsetypedef) 


```python
# get_data_lake_sources method usage example with argument unpacking

kwargs: GetDataLakeSourcesRequestRequestTypeDef = {  # (1)
    "accounts": ...,
}

parent.get_data_lake_sources(**kwargs)
```

1. See [:material-code-braces: GetDataLakeSourcesRequestRequestTypeDef](./type_defs.md#getdatalakesourcesrequestrequesttypedef) 

### get\_subscriber

Retrieves the subscription information for the specified subscription ID.

Type annotations and code completion for `#!python session.client("securitylake").get_subscriber` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# get_subscriber method definition

await def get_subscriber(
    self,
    *,
    subscriberId: str,
) -> GetSubscriberResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSubscriberResponseTypeDef](./type_defs.md#getsubscriberresponsetypedef) 


```python
# get_subscriber method usage example with argument unpacking

kwargs: GetSubscriberRequestRequestTypeDef = {  # (1)
    "subscriberId": ...,
}

parent.get_subscriber(**kwargs)
```

1. See [:material-code-braces: GetSubscriberRequestRequestTypeDef](./type_defs.md#getsubscriberrequestrequesttypedef) 

### list\_data\_lake\_exceptions

Lists the Amazon Security Lake exceptions that you can use to find the source
of problems and fix them.

Type annotations and code completion for `#!python session.client("securitylake").list_data_lake_exceptions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# list_data_lake_exceptions method definition

await def list_data_lake_exceptions(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    regions: Sequence[str] = ...,
) -> ListDataLakeExceptionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataLakeExceptionsResponseTypeDef](./type_defs.md#listdatalakeexceptionsresponsetypedef) 


```python
# list_data_lake_exceptions method usage example with argument unpacking

kwargs: ListDataLakeExceptionsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_data_lake_exceptions(**kwargs)
```

1. See [:material-code-braces: ListDataLakeExceptionsRequestRequestTypeDef](./type_defs.md#listdatalakeexceptionsrequestrequesttypedef) 

### list\_data\_lakes

Retrieves the Amazon Security Lake configuration object for the specified
Amazon Web Services Regions.

Type annotations and code completion for `#!python session.client("securitylake").list_data_lakes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# list_data_lakes method definition

await def list_data_lakes(
    self,
    *,
    regions: Sequence[str] = ...,
) -> ListDataLakesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataLakesResponseTypeDef](./type_defs.md#listdatalakesresponsetypedef) 


```python
# list_data_lakes method usage example with argument unpacking

kwargs: ListDataLakesRequestRequestTypeDef = {  # (1)
    "regions": ...,
}

parent.list_data_lakes(**kwargs)
```

1. See [:material-code-braces: ListDataLakesRequestRequestTypeDef](./type_defs.md#listdatalakesrequestrequesttypedef) 

### list\_log\_sources

Retrieves the log sources.

Type annotations and code completion for `#!python session.client("securitylake").list_log_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# list_log_sources method definition

await def list_log_sources(
    self,
    *,
    accounts: Sequence[str] = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    regions: Sequence[str] = ...,
    sources: Sequence[LogSourceResourceTypeDef] = ...,  # (1)
) -> ListLogSourcesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LogSourceResourceTypeDef](./type_defs.md#logsourceresourcetypedef) 
2. See [:material-code-braces: ListLogSourcesResponseTypeDef](./type_defs.md#listlogsourcesresponsetypedef) 


```python
# list_log_sources method usage example with argument unpacking

kwargs: ListLogSourcesRequestRequestTypeDef = {  # (1)
    "accounts": ...,
}

parent.list_log_sources(**kwargs)
```

1. See [:material-code-braces: ListLogSourcesRequestRequestTypeDef](./type_defs.md#listlogsourcesrequestrequesttypedef) 

### list\_subscribers

Lists all subscribers for the specific Amazon Security Lake account ID.

Type annotations and code completion for `#!python session.client("securitylake").list_subscribers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# list_subscribers method definition

await def list_subscribers(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSubscribersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSubscribersResponseTypeDef](./type_defs.md#listsubscribersresponsetypedef) 


```python
# list_subscribers method usage example with argument unpacking

kwargs: ListSubscribersRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_subscribers(**kwargs)
```

1. See [:material-code-braces: ListSubscribersRequestRequestTypeDef](./type_defs.md#listsubscribersrequestrequesttypedef) 

### list\_tags\_for\_resource

Retrieves the tags (keys and values) that are associated with an Amazon
Security Lake resource: a subscriber, or the data lake configuration for your
Amazon Web Services account in a particular Amazon Web Services Region.

Type annotations and code completion for `#!python session.client("securitylake").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### register\_data\_lake\_delegated\_administrator

Designates the Amazon Security Lake delegated administrator account for the
organization.

Type annotations and code completion for `#!python session.client("securitylake").register_data_lake_delegated_administrator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# register_data_lake_delegated_administrator method definition

await def register_data_lake_delegated_administrator(
    self,
    *,
    accountId: str,
) -> dict[str, Any]:
    ...
```



```python
# register_data_lake_delegated_administrator method usage example with argument unpacking

kwargs: RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef = {  # (1)
    "accountId": ...,
}

parent.register_data_lake_delegated_administrator(**kwargs)
```

1. See [:material-code-braces: RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef](./type_defs.md#registerdatalakedelegatedadministratorrequestrequesttypedef) 

### tag\_resource

Adds or updates one or more tags that are associated with an Amazon Security
Lake resource: a subscriber, or the data lake configuration for your Amazon Web
Services account in a particular Amazon Web Services Region.

Type annotations and code completion for `#!python session.client("securitylake").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes one or more tags (keys and values) from an Amazon Security Lake
resource: a subscriber, or the data lake configuration for your Amazon Web
Services account in a particular Amazon Web Services Region.

Type annotations and code completion for `#!python session.client("securitylake").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_data\_lake

You can use <code>UpdateDataLake</code> to specify where to store your security
data, how it should be encrypted at rest and for how long.

Type annotations and code completion for `#!python session.client("securitylake").update_data_lake` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# update_data_lake method definition

await def update_data_lake(
    self,
    *,
    configurations: Sequence[DataLakeConfigurationTypeDef],  # (1)
    metaStoreManagerRoleArn: str = ...,
) -> UpdateDataLakeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DataLakeConfigurationTypeDef](./type_defs.md#datalakeconfigurationtypedef) 
2. See [:material-code-braces: UpdateDataLakeResponseTypeDef](./type_defs.md#updatedatalakeresponsetypedef) 


```python
# update_data_lake method usage example with argument unpacking

kwargs: UpdateDataLakeRequestRequestTypeDef = {  # (1)
    "configurations": ...,
}

parent.update_data_lake(**kwargs)
```

1. See [:material-code-braces: UpdateDataLakeRequestRequestTypeDef](./type_defs.md#updatedatalakerequestrequesttypedef) 

### update\_data\_lake\_exception\_subscription

Updates the specified notification subscription in Amazon Security Lake for the
organization you specify.

Type annotations and code completion for `#!python session.client("securitylake").update_data_lake_exception_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# update_data_lake_exception_subscription method definition

await def update_data_lake_exception_subscription(
    self,
    *,
    notificationEndpoint: str,
    subscriptionProtocol: str,
    exceptionTimeToLive: int = ...,
) -> dict[str, Any]:
    ...
```



```python
# update_data_lake_exception_subscription method usage example with argument unpacking

kwargs: UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef = {  # (1)
    "notificationEndpoint": ...,
    "subscriptionProtocol": ...,
}

parent.update_data_lake_exception_subscription(**kwargs)
```

1. See [:material-code-braces: UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef](./type_defs.md#updatedatalakeexceptionsubscriptionrequestrequesttypedef) 

### update\_subscriber

Updates an existing subscription for the given Amazon Security Lake account ID.

Type annotations and code completion for `#!python session.client("securitylake").update_subscriber` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# update_subscriber method definition

await def update_subscriber(
    self,
    *,
    subscriberId: str,
    sources: Sequence[LogSourceResourceTypeDef] = ...,  # (1)
    subscriberDescription: str = ...,
    subscriberIdentity: AwsIdentityTypeDef = ...,  # (2)
    subscriberName: str = ...,
) -> UpdateSubscriberResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: LogSourceResourceTypeDef](./type_defs.md#logsourceresourcetypedef) 
2. See [:material-code-braces: AwsIdentityTypeDef](./type_defs.md#awsidentitytypedef) 
3. See [:material-code-braces: UpdateSubscriberResponseTypeDef](./type_defs.md#updatesubscriberresponsetypedef) 


```python
# update_subscriber method usage example with argument unpacking

kwargs: UpdateSubscriberRequestRequestTypeDef = {  # (1)
    "subscriberId": ...,
}

parent.update_subscriber(**kwargs)
```

1. See [:material-code-braces: UpdateSubscriberRequestRequestTypeDef](./type_defs.md#updatesubscriberrequestrequesttypedef) 

### update\_subscriber\_notification

Updates an existing notification method for the subscription (SQS or HTTPs
endpoint) or switches the notification subscription endpoint for a subscriber.

Type annotations and code completion for `#!python session.client("securitylake").update_subscriber_notification` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# update_subscriber_notification method definition

await def update_subscriber_notification(
    self,
    *,
    configuration: NotificationConfigurationTypeDef,  # (1)
    subscriberId: str,
) -> UpdateSubscriberNotificationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
2. See [:material-code-braces: UpdateSubscriberNotificationResponseTypeDef](./type_defs.md#updatesubscribernotificationresponsetypedef) 


```python
# update_subscriber_notification method usage example with argument unpacking

kwargs: UpdateSubscriberNotificationRequestRequestTypeDef = {  # (1)
    "configuration": ...,
    "subscriberId": ...,
}

parent.update_subscriber_notification(**kwargs)
```

1. See [:material-code-braces: UpdateSubscriberNotificationRequestRequestTypeDef](./type_defs.md#updatesubscribernotificationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("securitylake").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("securitylake").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

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

Type annotations and code completion for `#!python session.client("securitylake").get_paginator` method with overloads.

- `client.get_paginator("get_data_lake_sources")` -> [GetDataLakeSourcesPaginator](./paginators.md#getdatalakesourcespaginator)
- `client.get_paginator("list_data_lake_exceptions")` -> [ListDataLakeExceptionsPaginator](./paginators.md#listdatalakeexceptionspaginator)
- `client.get_paginator("list_log_sources")` -> [ListLogSourcesPaginator](./paginators.md#listlogsourcespaginator)
- `client.get_paginator("list_subscribers")` -> [ListSubscribersPaginator](./paginators.md#listsubscriberspaginator)


