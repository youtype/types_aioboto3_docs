# ApiGatewayManagementApiClient

> [Index](../README.md) > [ApiGatewayManagementApi](./README.md) > ApiGatewayManagementApiClient

!!! note ""

    Auto-generated documentation for [ApiGatewayManagementApi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#apigatewaymanagementapi)
    type annotations stubs module [types-aiobotocore-apigatewaymanagementapi](https://pypi.org/project/types-aiobotocore-apigatewaymanagementapi/).

## ApiGatewayManagementApiClient

Type annotations and code completion for `#!python session.client("apigatewaymanagementapi")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client)

```python
# ApiGatewayManagementApiClient usage example

from aioboto3.session import Session
from types_aiobotocore_apigatewaymanagementapi.client import ApiGatewayManagementApiClient

session = Session()
async with session.client("apigatewaymanagementapi") as client:
    client: ApiGatewayManagementApiClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("apigatewaymanagementapi").exceptions` structure.

```python
# ApiGatewayManagementApiClient.exceptions usage example

async with session.client("apigatewaymanagementapi") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.ForbiddenException,
        client.exceptions.GoneException,
        client.exceptions.LimitExceededException,
        client.exceptions.PayloadTooLargeException,
    ) as e:
        print(e)
```

```python
# ApiGatewayManagementApiClient.exceptions type checking example

from types_aiobotocore_apigatewaymanagementapi.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("apigatewaymanagementapi").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("apigatewaymanagementapi").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client)

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


### delete\_connection

Delete the connection with the provided id.

Type annotations and code completion for `#!python session.client("apigatewaymanagementapi").delete_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client)

```python
# delete_connection method definition

await def delete_connection(
    self,
    *,
    ConnectionId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# delete_connection method usage example with argument unpacking

kwargs: DeleteConnectionRequestTypeDef = {  # (1)
    "ConnectionId": ...,
}

parent.delete_connection(**kwargs)
```

1. See [:material-code-braces: DeleteConnectionRequestTypeDef](./type_defs.md#deleteconnectionrequesttypedef)

### get\_connection

Get information about the connection with the provided id.

Type annotations and code completion for `#!python session.client("apigatewaymanagementapi").get_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client)

```python
# get_connection method definition

await def get_connection(
    self,
    *,
    ConnectionId: str,
) -> GetConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConnectionResponseTypeDef](./type_defs.md#getconnectionresponsetypedef)


```python
# get_connection method usage example with argument unpacking

kwargs: GetConnectionRequestTypeDef = {  # (1)
    "ConnectionId": ...,
}

parent.get_connection(**kwargs)
```

1. See [:material-code-braces: GetConnectionRequestTypeDef](./type_defs.md#getconnectionrequesttypedef)

### post\_to\_connection

Sends the provided data to the specified connection.

Type annotations and code completion for `#!python session.client("apigatewaymanagementapi").post_to_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client)

```python
# post_to_connection method definition

await def post_to_connection(
    self,
    *,
    Data: BlobTypeDef,
    ConnectionId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# post_to_connection method usage example with argument unpacking

kwargs: PostToConnectionRequestTypeDef = {  # (1)
    "Data": ...,
    "ConnectionId": ...,
}

parent.post_to_connection(**kwargs)
```

1. See [:material-code-braces: PostToConnectionRequestTypeDef](./type_defs.md#posttoconnectionrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("apigatewaymanagementapi").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("apigatewaymanagementapi").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client)

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





