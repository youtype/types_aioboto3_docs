# S3OutpostsClient

> [Index](../README.md) > [S3Outposts](./README.md) > S3OutpostsClient

!!! note ""

    Auto-generated documentation for [S3Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
    type annotations stubs module [types-aiobotocore-s3outposts](https://pypi.org/project/types-aiobotocore-s3outposts/).

## S3OutpostsClient

Type annotations and code completion for `#!python session.client("s3outposts")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client)

```python title="Usage example"
from aioboto3.session import Session
from types_aiobotocore_s3outposts.client import S3OutpostsClient

session = Session()
async with session.client("s3outposts") as client:
    client: S3OutpostsClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("s3outposts").exceptions` structure.

```python title="Usage example"
async with session.client("s3outposts") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_s3outposts.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.client("s3outposts").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.client("s3outposts").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client.close)

```python title="Method definition"
await def close(
    self,
) -> None:
    ...
```


### create\_endpoint

Creates an endpoint and associates it with the specified Outpost.

Type annotations and code completion for `#!python session.client("s3outposts").create_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client.create_endpoint)

```python title="Method definition"
await def create_endpoint(
    self,
    *,
    OutpostId: str,
    SubnetId: str,
    SecurityGroupId: str,
    AccessType: EndpointAccessTypeType = ...,  # (1)
    CustomerOwnedIpv4Pool: str = ...,
) -> CreateEndpointResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EndpointAccessTypeType](./literals.md#endpointaccesstypetype) 
2. See [:material-code-braces: CreateEndpointResultTypeDef](./type_defs.md#createendpointresulttypedef) 


```python title="Usage example with kwargs"
kwargs: CreateEndpointRequestRequestTypeDef = {  # (1)
    "OutpostId": ...,
    "SubnetId": ...,
    "SecurityGroupId": ...,
}

parent.create_endpoint(**kwargs)
```

1. See [:material-code-braces: CreateEndpointRequestRequestTypeDef](./type_defs.md#createendpointrequestrequesttypedef) 

### delete\_endpoint

Deletes an endpoint.

Type annotations and code completion for `#!python session.client("s3outposts").delete_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client.delete_endpoint)

```python title="Method definition"
await def delete_endpoint(
    self,
    *,
    EndpointId: str,
    OutpostId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python title="Usage example with kwargs"
kwargs: DeleteEndpointRequestRequestTypeDef = {  # (1)
    "EndpointId": ...,
    "OutpostId": ...,
}

parent.delete_endpoint(**kwargs)
```

1. See [:material-code-braces: DeleteEndpointRequestRequestTypeDef](./type_defs.md#deleteendpointrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.client("s3outposts").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client.generate_presigned_url)

```python title="Method definition"
await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### list\_endpoints

Lists endpoints associated with the specified Outpost.

Type annotations and code completion for `#!python session.client("s3outposts").list_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client.list_endpoints)

```python title="Method definition"
await def list_endpoints(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListEndpointsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEndpointsResultTypeDef](./type_defs.md#listendpointsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListEndpointsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_endpoints(**kwargs)
```

1. See [:material-code-braces: ListEndpointsRequestRequestTypeDef](./type_defs.md#listendpointsrequestrequesttypedef) 

### list\_shared\_endpoints

Lists all endpoints associated with an Outpost that has been shared by Amazon
Web Services Resource Access Manager (RAM).

Type annotations and code completion for `#!python session.client("s3outposts").list_shared_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client.list_shared_endpoints)

```python title="Method definition"
await def list_shared_endpoints(
    self,
    *,
    OutpostId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListSharedEndpointsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSharedEndpointsResultTypeDef](./type_defs.md#listsharedendpointsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListSharedEndpointsRequestRequestTypeDef = {  # (1)
    "OutpostId": ...,
}

parent.list_shared_endpoints(**kwargs)
```

1. See [:material-code-braces: ListSharedEndpointsRequestRequestTypeDef](./type_defs.md#listsharedendpointsrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("s3outposts").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> S3OutpostsClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("s3outposts").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("s3outposts").get_paginator` method with overloads.

- `client.get_paginator("list_endpoints")` -> [ListEndpointsPaginator](./paginators.md#listendpointspaginator)
- `client.get_paginator("list_shared_endpoints")` -> [ListSharedEndpointsPaginator](./paginators.md#listsharedendpointspaginator)



