# SupportAppClient

> [Index](../README.md) > [SupportApp](./README.md) > SupportAppClient

!!! note ""

    Auto-generated documentation for [SupportApp](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#supportapp)
    type annotations stubs module [types-aiobotocore-support-app](https://pypi.org/project/types-aiobotocore-support-app/).

## SupportAppClient

Type annotations and code completion for `#!python session.client("support-app")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp.Client)

```python
# SupportAppClient usage example

from aioboto3.session import Session
from types_aiobotocore_support_app.client import SupportAppClient

session = Session()
async with session.client("support-app") as client:
    client: SupportAppClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("support-app").exceptions` structure.

```python
# SupportAppClient.exceptions usage example

async with session.client("support-app") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# SupportAppClient.exceptions type checking example

from types_aiobotocore_support_app.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("support-app").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("support-app").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp.Client)

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


### create\_slack\_channel\_configuration

Creates a Slack channel configuration for your Amazon Web Services account.

Type annotations and code completion for `#!python session.client("support-app").create_slack_channel_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp.Client)

```python
# create_slack_channel_configuration method definition

await def create_slack_channel_configuration(
    self,
    *,
    channelId: str,
    channelRoleArn: str,
    notifyOnCaseSeverity: NotificationSeverityLevelType,  # (1)
    teamId: str,
    channelName: str = ...,
    notifyOnAddCorrespondenceToCase: bool = ...,
    notifyOnCreateOrReopenCase: bool = ...,
    notifyOnResolveCase: bool = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: NotificationSeverityLevelType](./literals.md#notificationseverityleveltype) 


```python
# create_slack_channel_configuration method usage example with argument unpacking

kwargs: CreateSlackChannelConfigurationRequestRequestTypeDef = {  # (1)
    "channelId": ...,
    "channelRoleArn": ...,
    "notifyOnCaseSeverity": ...,
    "teamId": ...,
}

parent.create_slack_channel_configuration(**kwargs)
```

1. See [:material-code-braces: CreateSlackChannelConfigurationRequestRequestTypeDef](./type_defs.md#createslackchannelconfigurationrequestrequesttypedef) 

### delete\_account\_alias

Deletes an alias for an Amazon Web Services account ID.

Type annotations and code completion for `#!python session.client("support-app").delete_account_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp.Client)

```python
# delete_account_alias method definition

await def delete_account_alias(
    self,
) -> dict[str, Any]:
    ...
```


### delete\_slack\_channel\_configuration

Deletes a Slack channel configuration from your Amazon Web Services account.

Type annotations and code completion for `#!python session.client("support-app").delete_slack_channel_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp.Client)

```python
# delete_slack_channel_configuration method definition

await def delete_slack_channel_configuration(
    self,
    *,
    channelId: str,
    teamId: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_slack_channel_configuration method usage example with argument unpacking

kwargs: DeleteSlackChannelConfigurationRequestRequestTypeDef = {  # (1)
    "channelId": ...,
    "teamId": ...,
}

parent.delete_slack_channel_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteSlackChannelConfigurationRequestRequestTypeDef](./type_defs.md#deleteslackchannelconfigurationrequestrequesttypedef) 

### delete\_slack\_workspace\_configuration

Deletes a Slack workspace configuration from your Amazon Web Services account.

Type annotations and code completion for `#!python session.client("support-app").delete_slack_workspace_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp.Client)

```python
# delete_slack_workspace_configuration method definition

await def delete_slack_workspace_configuration(
    self,
    *,
    teamId: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_slack_workspace_configuration method usage example with argument unpacking

kwargs: DeleteSlackWorkspaceConfigurationRequestRequestTypeDef = {  # (1)
    "teamId": ...,
}

parent.delete_slack_workspace_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteSlackWorkspaceConfigurationRequestRequestTypeDef](./type_defs.md#deleteslackworkspaceconfigurationrequestrequesttypedef) 

### get\_account\_alias

Retrieves the alias from an Amazon Web Services account ID.

Type annotations and code completion for `#!python session.client("support-app").get_account_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp.Client)

```python
# get_account_alias method definition

await def get_account_alias(
    self,
) -> GetAccountAliasResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccountAliasResultTypeDef](./type_defs.md#getaccountaliasresulttypedef) 

### list\_slack\_channel\_configurations

Lists the Slack channel configurations for an Amazon Web Services account.

Type annotations and code completion for `#!python session.client("support-app").list_slack_channel_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp.Client)

```python
# list_slack_channel_configurations method definition

await def list_slack_channel_configurations(
    self,
    *,
    nextToken: str = ...,
) -> ListSlackChannelConfigurationsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSlackChannelConfigurationsResultTypeDef](./type_defs.md#listslackchannelconfigurationsresulttypedef) 


```python
# list_slack_channel_configurations method usage example with argument unpacking

kwargs: ListSlackChannelConfigurationsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_slack_channel_configurations(**kwargs)
```

1. See [:material-code-braces: ListSlackChannelConfigurationsRequestRequestTypeDef](./type_defs.md#listslackchannelconfigurationsrequestrequesttypedef) 

### list\_slack\_workspace\_configurations

Lists the Slack workspace configurations for an Amazon Web Services account.

Type annotations and code completion for `#!python session.client("support-app").list_slack_workspace_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp.Client)

```python
# list_slack_workspace_configurations method definition

await def list_slack_workspace_configurations(
    self,
    *,
    nextToken: str = ...,
) -> ListSlackWorkspaceConfigurationsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSlackWorkspaceConfigurationsResultTypeDef](./type_defs.md#listslackworkspaceconfigurationsresulttypedef) 


```python
# list_slack_workspace_configurations method usage example with argument unpacking

kwargs: ListSlackWorkspaceConfigurationsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_slack_workspace_configurations(**kwargs)
```

1. See [:material-code-braces: ListSlackWorkspaceConfigurationsRequestRequestTypeDef](./type_defs.md#listslackworkspaceconfigurationsrequestrequesttypedef) 

### put\_account\_alias

Creates or updates an individual alias for each Amazon Web Services account ID.

Type annotations and code completion for `#!python session.client("support-app").put_account_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp.Client)

```python
# put_account_alias method definition

await def put_account_alias(
    self,
    *,
    accountAlias: str,
) -> dict[str, Any]:
    ...
```



```python
# put_account_alias method usage example with argument unpacking

kwargs: PutAccountAliasRequestRequestTypeDef = {  # (1)
    "accountAlias": ...,
}

parent.put_account_alias(**kwargs)
```

1. See [:material-code-braces: PutAccountAliasRequestRequestTypeDef](./type_defs.md#putaccountaliasrequestrequesttypedef) 

### register\_slack\_workspace\_for\_organization

Registers a Slack workspace for your Amazon Web Services account.

Type annotations and code completion for `#!python session.client("support-app").register_slack_workspace_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp.Client)

```python
# register_slack_workspace_for_organization method definition

await def register_slack_workspace_for_organization(
    self,
    *,
    teamId: str,
) -> RegisterSlackWorkspaceForOrganizationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RegisterSlackWorkspaceForOrganizationResultTypeDef](./type_defs.md#registerslackworkspacefororganizationresulttypedef) 


```python
# register_slack_workspace_for_organization method usage example with argument unpacking

kwargs: RegisterSlackWorkspaceForOrganizationRequestRequestTypeDef = {  # (1)
    "teamId": ...,
}

parent.register_slack_workspace_for_organization(**kwargs)
```

1. See [:material-code-braces: RegisterSlackWorkspaceForOrganizationRequestRequestTypeDef](./type_defs.md#registerslackworkspacefororganizationrequestrequesttypedef) 

### update\_slack\_channel\_configuration

Updates the configuration for a Slack channel, such as case update
notifications.

Type annotations and code completion for `#!python session.client("support-app").update_slack_channel_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp.Client)

```python
# update_slack_channel_configuration method definition

await def update_slack_channel_configuration(
    self,
    *,
    channelId: str,
    teamId: str,
    channelName: str = ...,
    channelRoleArn: str = ...,
    notifyOnAddCorrespondenceToCase: bool = ...,
    notifyOnCaseSeverity: NotificationSeverityLevelType = ...,  # (1)
    notifyOnCreateOrReopenCase: bool = ...,
    notifyOnResolveCase: bool = ...,
) -> UpdateSlackChannelConfigurationResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: NotificationSeverityLevelType](./literals.md#notificationseverityleveltype) 
2. See [:material-code-braces: UpdateSlackChannelConfigurationResultTypeDef](./type_defs.md#updateslackchannelconfigurationresulttypedef) 


```python
# update_slack_channel_configuration method usage example with argument unpacking

kwargs: UpdateSlackChannelConfigurationRequestRequestTypeDef = {  # (1)
    "channelId": ...,
    "teamId": ...,
}

parent.update_slack_channel_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateSlackChannelConfigurationRequestRequestTypeDef](./type_defs.md#updateslackchannelconfigurationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("support-app").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("support-app").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp.Client)

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




