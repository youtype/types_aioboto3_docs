# S3OutpostsClient

> [Index](../README.md) > [S3Outposts](./README.md) > S3OutpostsClient

!!! note ""

    Auto-generated documentation for [S3Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#s3outposts)
    type annotations stubs module [types-aiobotocore-s3outposts](https://pypi.org/project/types-aiobotocore-s3outposts/).

## S3OutpostsClient

Type annotations and code completion for `#!python session.client("s3outposts")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client)

```python
# S3OutpostsClient usage example

from aioboto3.session import Session
from types_aiobotocore_s3outposts.client import S3OutpostsClient

session = Session()
async with session.client("s3outposts") as client:
    client: S3OutpostsClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("s3outposts").exceptions` structure.

```python
# S3OutpostsClient.exceptions usage example

async with session.client("s3outposts") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.OutpostOfflineException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# S3OutpostsClient.exceptions type checking example

from types_aiobotocore_s3outposts.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("s3outposts").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("s3outposts").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client)

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


### create\_endpoint

Creates an endpoint and associates it with the specified Outpost.

Type annotations and code completion for `#!python session.client("s3outposts").create_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client)

```python
# create_endpoint method definition

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


```python
# create_endpoint method usage example with argument unpacking

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client)

```python
# delete_endpoint method definition

await def delete_endpoint(
    self,
    *,
    EndpointId: str,
    OutpostId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_endpoint method usage example with argument unpacking

kwargs: DeleteEndpointRequestRequestTypeDef = {  # (1)
    "EndpointId": ...,
    "OutpostId": ...,
}

parent.delete_endpoint(**kwargs)
```

1. See [:material-code-braces: DeleteEndpointRequestRequestTypeDef](./type_defs.md#deleteendpointrequestrequesttypedef) 

### list\_endpoints

Lists endpoints associated with the specified Outpost.

Type annotations and code completion for `#!python session.client("s3outposts").list_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client)

```python
# list_endpoints method definition

await def list_endpoints(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListEndpointsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEndpointsResultTypeDef](./type_defs.md#listendpointsresulttypedef) 


```python
# list_endpoints method usage example with argument unpacking

kwargs: ListEndpointsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_endpoints(**kwargs)
```

1. See [:material-code-braces: ListEndpointsRequestRequestTypeDef](./type_defs.md#listendpointsrequestrequesttypedef) 

### list\_outposts\_with\_s3

Lists the Outposts with S3 on Outposts capacity for your Amazon Web Services
account.

Type annotations and code completion for `#!python session.client("s3outposts").list_outposts_with_s3` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client)

```python
# list_outposts_with_s3 method definition

await def list_outposts_with_s3(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListOutpostsWithS3ResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOutpostsWithS3ResultTypeDef](./type_defs.md#listoutpostswiths3resulttypedef) 


```python
# list_outposts_with_s3 method usage example with argument unpacking

kwargs: ListOutpostsWithS3RequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_outposts_with_s3(**kwargs)
```

1. See [:material-code-braces: ListOutpostsWithS3RequestRequestTypeDef](./type_defs.md#listoutpostswiths3requestrequesttypedef) 

### list\_shared\_endpoints

Lists all endpoints associated with an Outpost that has been shared by Amazon
Web Services Resource Access Manager (RAM).

Type annotations and code completion for `#!python session.client("s3outposts").list_shared_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client)

```python
# list_shared_endpoints method definition

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


```python
# list_shared_endpoints method usage example with argument unpacking

kwargs: ListSharedEndpointsRequestRequestTypeDef = {  # (1)
    "OutpostId": ...,
}

parent.list_shared_endpoints(**kwargs)
```

1. See [:material-code-braces: ListSharedEndpointsRequestRequestTypeDef](./type_defs.md#listsharedendpointsrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("s3outposts").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("s3outposts").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client)

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

Type annotations and code completion for `#!python session.client("s3outposts").get_paginator` method with overloads.

- `client.get_paginator("list_endpoints")` -> [ListEndpointsPaginator](./paginators.md#listendpointspaginator)
- `client.get_paginator("list_outposts_with_s3")` -> [ListOutpostsWithS3Paginator](./paginators.md#listoutpostswiths3paginator)
- `client.get_paginator("list_shared_endpoints")` -> [ListSharedEndpointsPaginator](./paginators.md#listsharedendpointspaginator)


