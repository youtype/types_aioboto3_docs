# IoTSecureTunnelingClient

> [Index](../README.md) > [IoTSecureTunneling](./README.md) > IoTSecureTunnelingClient

!!! note ""

    Auto-generated documentation for [IoTSecureTunneling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
    type annotations stubs module [types-aiobotocore-iotsecuretunneling](https://pypi.org/project/types-aiobotocore-iotsecuretunneling/).

## IoTSecureTunnelingClient

Type annotations and code completion for `#!python session.client("iotsecuretunneling")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client)

```python title="Usage example"
from aioboto3.session import Session
from types_aiobotocore_iotsecuretunneling.client import IoTSecureTunnelingClient

session = Session()
async with session.client("iotsecuretunneling") as client:
    client: IoTSecureTunnelingClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("iotsecuretunneling").exceptions` structure.

```python title="Usage example"
async with session.client("iotsecuretunneling") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.LimitExceededException,
        client.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_iotsecuretunneling.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.client("iotsecuretunneling").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close\_tunnel

Closes a tunnel identified by the unique tunnel id.

Type annotations and code completion for `#!python session.client("iotsecuretunneling").close_tunnel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.close_tunnel)

```python title="Method definition"
await def close_tunnel(
    self,
    *,
    tunnelId: str,
    delete: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python title="Usage example with kwargs"
kwargs: CloseTunnelRequestRequestTypeDef = {  # (1)
    "tunnelId": ...,
}

parent.close_tunnel(**kwargs)
```

1. See [:material-code-braces: CloseTunnelRequestRequestTypeDef](./type_defs.md#closetunnelrequestrequesttypedef) 

### describe\_tunnel

Gets information about a tunnel identified by the unique tunnel id.

Type annotations and code completion for `#!python session.client("iotsecuretunneling").describe_tunnel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.describe_tunnel)

```python title="Method definition"
await def describe_tunnel(
    self,
    *,
    tunnelId: str,
) -> DescribeTunnelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTunnelResponseTypeDef](./type_defs.md#describetunnelresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTunnelRequestRequestTypeDef = {  # (1)
    "tunnelId": ...,
}

parent.describe_tunnel(**kwargs)
```

1. See [:material-code-braces: DescribeTunnelRequestRequestTypeDef](./type_defs.md#describetunnelrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.client("iotsecuretunneling").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.generate_presigned_url)

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


### list\_tags\_for\_resource

Lists the tags for the specified resource.

Type annotations and code completion for `#!python session.client("iotsecuretunneling").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.list_tags_for_resource)

```python title="Method definition"
await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_tunnels

List all tunnels for an AWS account.

Type annotations and code completion for `#!python session.client("iotsecuretunneling").list_tunnels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.list_tunnels)

```python title="Method definition"
await def list_tunnels(
    self,
    *,
    thingName: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListTunnelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTunnelsResponseTypeDef](./type_defs.md#listtunnelsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTunnelsRequestRequestTypeDef = {  # (1)
    "thingName": ...,
}

parent.list_tunnels(**kwargs)
```

1. See [:material-code-braces: ListTunnelsRequestRequestTypeDef](./type_defs.md#listtunnelsrequestrequesttypedef) 

### open\_tunnel

Creates a new tunnel, and returns two client access tokens for clients to use to
connect to the AWS IoT Secure Tunneling proxy server.

Type annotations and code completion for `#!python session.client("iotsecuretunneling").open_tunnel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.open_tunnel)

```python title="Method definition"
await def open_tunnel(
    self,
    *,
    description: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (1)
    destinationConfig: DestinationConfigTypeDef = ...,  # (2)
    timeoutConfig: TimeoutConfigTypeDef = ...,  # (3)
) -> OpenTunnelResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
3. See [:material-code-braces: TimeoutConfigTypeDef](./type_defs.md#timeoutconfigtypedef) 
4. See [:material-code-braces: OpenTunnelResponseTypeDef](./type_defs.md#opentunnelresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: OpenTunnelRequestRequestTypeDef = {  # (1)
    "description": ...,
}

parent.open_tunnel(**kwargs)
```

1. See [:material-code-braces: OpenTunnelRequestRequestTypeDef](./type_defs.md#opentunnelrequestrequesttypedef) 

### tag\_resource

A resource tag.

Type annotations and code completion for `#!python session.client("iotsecuretunneling").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.tag_resource)

```python title="Method definition"
await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python title="Usage example with kwargs"
kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes a tag from a resource.

Type annotations and code completion for `#!python session.client("iotsecuretunneling").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.untag_resource)

```python title="Method definition"
await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python title="Usage example with kwargs"
kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("iotsecuretunneling").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> IoTSecureTunnelingClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("iotsecuretunneling").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





