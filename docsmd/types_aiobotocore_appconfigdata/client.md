# AppConfigDataClient

> [Index](../README.md) > [AppConfigData](./README.md) > AppConfigDataClient

!!! note ""

    Auto-generated documentation for [AppConfigData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#appconfigdata)
    type annotations stubs module [types-aiobotocore-appconfigdata](https://pypi.org/project/types-aiobotocore-appconfigdata/).

## AppConfigDataClient

Type annotations and code completion for `#!python session.client("appconfigdata")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData.Client)

```python
# AppConfigDataClient usage example

from aioboto3.session import Session
from types_aiobotocore_appconfigdata.client import AppConfigDataClient

session = Session()
async with session.client("appconfigdata") as client:
    client: AppConfigDataClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("appconfigdata").exceptions` structure.

```python
# AppConfigDataClient.exceptions usage example

async with session.client("appconfigdata") as client:
    try:
        do_something(client)
    except (
            client.exceptions.BadRequestException,
        client.exceptions.ClientError,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ThrottlingException,
    ) as e:
        print(e)
```

```python
# AppConfigDataClient.exceptions type checking example

from types_aiobotocore_appconfigdata.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("appconfigdata").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("appconfigdata").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData.Client)

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


### get\_latest\_configuration

Retrieves the latest deployed configuration.

Type annotations and code completion for `#!python session.client("appconfigdata").get_latest_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData.Client)

```python
# get_latest_configuration method definition

await def get_latest_configuration(
    self,
    *,
    ConfigurationToken: str,
) -> GetLatestConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLatestConfigurationResponseTypeDef](./type_defs.md#getlatestconfigurationresponsetypedef) 


```python
# get_latest_configuration method usage example with argument unpacking

kwargs: GetLatestConfigurationRequestRequestTypeDef = {  # (1)
    "ConfigurationToken": ...,
}

parent.get_latest_configuration(**kwargs)
```

1. See [:material-code-braces: GetLatestConfigurationRequestRequestTypeDef](./type_defs.md#getlatestconfigurationrequestrequesttypedef) 

### start\_configuration\_session

Starts a configuration session used to retrieve a deployed configuration.

Type annotations and code completion for `#!python session.client("appconfigdata").start_configuration_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData.Client)

```python
# start_configuration_session method definition

await def start_configuration_session(
    self,
    *,
    ApplicationIdentifier: str,
    EnvironmentIdentifier: str,
    ConfigurationProfileIdentifier: str,
    RequiredMinimumPollIntervalInSeconds: int = ...,
) -> StartConfigurationSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartConfigurationSessionResponseTypeDef](./type_defs.md#startconfigurationsessionresponsetypedef) 


```python
# start_configuration_session method usage example with argument unpacking

kwargs: StartConfigurationSessionRequestRequestTypeDef = {  # (1)
    "ApplicationIdentifier": ...,
    "EnvironmentIdentifier": ...,
    "ConfigurationProfileIdentifier": ...,
}

parent.start_configuration_session(**kwargs)
```

1. See [:material-code-braces: StartConfigurationSessionRequestRequestTypeDef](./type_defs.md#startconfigurationsessionrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("appconfigdata").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("appconfigdata").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData.Client)

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




