# AppMeshClient

> [Index](../README.md) > [AppMesh](./README.md) > AppMeshClient

!!! note ""

    Auto-generated documentation for [AppMesh](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#appmesh)
    type annotations stubs module [types-aiobotocore-appmesh](https://pypi.org/project/types-aiobotocore-appmesh/).

## AppMeshClient

Type annotations and code completion for `#!python session.client("appmesh")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# AppMeshClient usage example

from aioboto3.session import Session
from types_aiobotocore_appmesh.client import AppMeshClient

session = Session()
async with session.client("appmesh") as client:
    client: AppMeshClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("appmesh").exceptions` structure.

```python
# AppMeshClient.exceptions usage example

async with session.client("appmesh") as client:
    try:
        do_something(client)
    except (
            client.exceptions.BadRequestException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.ForbiddenException,
        client.exceptions.InternalServerErrorException,
        client.exceptions.LimitExceededException,
        client.exceptions.NotFoundException,
        client.exceptions.ResourceInUseException,
        client.exceptions.ServiceUnavailableException,
        client.exceptions.TooManyRequestsException,
        client.exceptions.TooManyTagsException,
    ) as e:
        print(e)
```

```python
# AppMeshClient.exceptions type checking example

from types_aiobotocore_appmesh.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("appmesh").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("appmesh").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

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


### create\_gateway\_route

Creates a gateway route.

Type annotations and code completion for `#!python session.client("appmesh").create_gateway_route` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# create_gateway_route method definition

await def create_gateway_route(
    self,
    *,
    gatewayRouteName: str,
    meshName: str,
    spec: GatewayRouteSpecTypeDef,  # (1)
    virtualGatewayName: str,
    clientToken: str = ...,
    meshOwner: str = ...,
    tags: Sequence[TagRefTypeDef] = ...,  # (2)
) -> CreateGatewayRouteOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: GatewayRouteSpecTypeDef](./type_defs.md#gatewayroutespectypedef) 
2. See [:material-code-braces: TagRefTypeDef](./type_defs.md#tagreftypedef) 
3. See [:material-code-braces: CreateGatewayRouteOutputTypeDef](./type_defs.md#creategatewayrouteoutputtypedef) 


```python
# create_gateway_route method usage example with argument unpacking

kwargs: CreateGatewayRouteInputRequestTypeDef = {  # (1)
    "gatewayRouteName": ...,
    "meshName": ...,
    "spec": ...,
    "virtualGatewayName": ...,
}

parent.create_gateway_route(**kwargs)
```

1. See [:material-code-braces: CreateGatewayRouteInputRequestTypeDef](./type_defs.md#creategatewayrouteinputrequesttypedef) 

### create\_mesh

Creates a service mesh.

Type annotations and code completion for `#!python session.client("appmesh").create_mesh` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# create_mesh method definition

await def create_mesh(
    self,
    *,
    meshName: str,
    clientToken: str = ...,
    spec: MeshSpecTypeDef = ...,  # (1)
    tags: Sequence[TagRefTypeDef] = ...,  # (2)
) -> CreateMeshOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: MeshSpecTypeDef](./type_defs.md#meshspectypedef) 
2. See [:material-code-braces: TagRefTypeDef](./type_defs.md#tagreftypedef) 
3. See [:material-code-braces: CreateMeshOutputTypeDef](./type_defs.md#createmeshoutputtypedef) 


```python
# create_mesh method usage example with argument unpacking

kwargs: CreateMeshInputRequestTypeDef = {  # (1)
    "meshName": ...,
}

parent.create_mesh(**kwargs)
```

1. See [:material-code-braces: CreateMeshInputRequestTypeDef](./type_defs.md#createmeshinputrequesttypedef) 

### create\_route

Creates a route that is associated with a virtual router.

Type annotations and code completion for `#!python session.client("appmesh").create_route` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# create_route method definition

await def create_route(
    self,
    *,
    meshName: str,
    routeName: str,
    spec: RouteSpecTypeDef,  # (1)
    virtualRouterName: str,
    clientToken: str = ...,
    meshOwner: str = ...,
    tags: Sequence[TagRefTypeDef] = ...,  # (2)
) -> CreateRouteOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RouteSpecTypeDef](./type_defs.md#routespectypedef) 
2. See [:material-code-braces: TagRefTypeDef](./type_defs.md#tagreftypedef) 
3. See [:material-code-braces: CreateRouteOutputTypeDef](./type_defs.md#createrouteoutputtypedef) 


```python
# create_route method usage example with argument unpacking

kwargs: CreateRouteInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "routeName": ...,
    "spec": ...,
    "virtualRouterName": ...,
}

parent.create_route(**kwargs)
```

1. See [:material-code-braces: CreateRouteInputRequestTypeDef](./type_defs.md#createrouteinputrequesttypedef) 

### create\_virtual\_gateway

Creates a virtual gateway.

Type annotations and code completion for `#!python session.client("appmesh").create_virtual_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# create_virtual_gateway method definition

await def create_virtual_gateway(
    self,
    *,
    meshName: str,
    spec: VirtualGatewaySpecTypeDef,  # (1)
    virtualGatewayName: str,
    clientToken: str = ...,
    meshOwner: str = ...,
    tags: Sequence[TagRefTypeDef] = ...,  # (2)
) -> CreateVirtualGatewayOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: VirtualGatewaySpecTypeDef](./type_defs.md#virtualgatewayspectypedef) 
2. See [:material-code-braces: TagRefTypeDef](./type_defs.md#tagreftypedef) 
3. See [:material-code-braces: CreateVirtualGatewayOutputTypeDef](./type_defs.md#createvirtualgatewayoutputtypedef) 


```python
# create_virtual_gateway method usage example with argument unpacking

kwargs: CreateVirtualGatewayInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "spec": ...,
    "virtualGatewayName": ...,
}

parent.create_virtual_gateway(**kwargs)
```

1. See [:material-code-braces: CreateVirtualGatewayInputRequestTypeDef](./type_defs.md#createvirtualgatewayinputrequesttypedef) 

### create\_virtual\_node

Creates a virtual node within a service mesh.

Type annotations and code completion for `#!python session.client("appmesh").create_virtual_node` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# create_virtual_node method definition

await def create_virtual_node(
    self,
    *,
    meshName: str,
    spec: VirtualNodeSpecTypeDef,  # (1)
    virtualNodeName: str,
    clientToken: str = ...,
    meshOwner: str = ...,
    tags: Sequence[TagRefTypeDef] = ...,  # (2)
) -> CreateVirtualNodeOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: VirtualNodeSpecTypeDef](./type_defs.md#virtualnodespectypedef) 
2. See [:material-code-braces: TagRefTypeDef](./type_defs.md#tagreftypedef) 
3. See [:material-code-braces: CreateVirtualNodeOutputTypeDef](./type_defs.md#createvirtualnodeoutputtypedef) 


```python
# create_virtual_node method usage example with argument unpacking

kwargs: CreateVirtualNodeInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "spec": ...,
    "virtualNodeName": ...,
}

parent.create_virtual_node(**kwargs)
```

1. See [:material-code-braces: CreateVirtualNodeInputRequestTypeDef](./type_defs.md#createvirtualnodeinputrequesttypedef) 

### create\_virtual\_router

Creates a virtual router within a service mesh.

Type annotations and code completion for `#!python session.client("appmesh").create_virtual_router` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# create_virtual_router method definition

await def create_virtual_router(
    self,
    *,
    meshName: str,
    spec: VirtualRouterSpecTypeDef,  # (1)
    virtualRouterName: str,
    clientToken: str = ...,
    meshOwner: str = ...,
    tags: Sequence[TagRefTypeDef] = ...,  # (2)
) -> CreateVirtualRouterOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: VirtualRouterSpecTypeDef](./type_defs.md#virtualrouterspectypedef) 
2. See [:material-code-braces: TagRefTypeDef](./type_defs.md#tagreftypedef) 
3. See [:material-code-braces: CreateVirtualRouterOutputTypeDef](./type_defs.md#createvirtualrouteroutputtypedef) 


```python
# create_virtual_router method usage example with argument unpacking

kwargs: CreateVirtualRouterInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "spec": ...,
    "virtualRouterName": ...,
}

parent.create_virtual_router(**kwargs)
```

1. See [:material-code-braces: CreateVirtualRouterInputRequestTypeDef](./type_defs.md#createvirtualrouterinputrequesttypedef) 

### create\_virtual\_service

Creates a virtual service within a service mesh.

Type annotations and code completion for `#!python session.client("appmesh").create_virtual_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# create_virtual_service method definition

await def create_virtual_service(
    self,
    *,
    meshName: str,
    spec: VirtualServiceSpecTypeDef,  # (1)
    virtualServiceName: str,
    clientToken: str = ...,
    meshOwner: str = ...,
    tags: Sequence[TagRefTypeDef] = ...,  # (2)
) -> CreateVirtualServiceOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: VirtualServiceSpecTypeDef](./type_defs.md#virtualservicespectypedef) 
2. See [:material-code-braces: TagRefTypeDef](./type_defs.md#tagreftypedef) 
3. See [:material-code-braces: CreateVirtualServiceOutputTypeDef](./type_defs.md#createvirtualserviceoutputtypedef) 


```python
# create_virtual_service method usage example with argument unpacking

kwargs: CreateVirtualServiceInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "spec": ...,
    "virtualServiceName": ...,
}

parent.create_virtual_service(**kwargs)
```

1. See [:material-code-braces: CreateVirtualServiceInputRequestTypeDef](./type_defs.md#createvirtualserviceinputrequesttypedef) 

### delete\_gateway\_route

Deletes an existing gateway route.

Type annotations and code completion for `#!python session.client("appmesh").delete_gateway_route` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# delete_gateway_route method definition

await def delete_gateway_route(
    self,
    *,
    gatewayRouteName: str,
    meshName: str,
    virtualGatewayName: str,
    meshOwner: str = ...,
) -> DeleteGatewayRouteOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteGatewayRouteOutputTypeDef](./type_defs.md#deletegatewayrouteoutputtypedef) 


```python
# delete_gateway_route method usage example with argument unpacking

kwargs: DeleteGatewayRouteInputRequestTypeDef = {  # (1)
    "gatewayRouteName": ...,
    "meshName": ...,
    "virtualGatewayName": ...,
}

parent.delete_gateway_route(**kwargs)
```

1. See [:material-code-braces: DeleteGatewayRouteInputRequestTypeDef](./type_defs.md#deletegatewayrouteinputrequesttypedef) 

### delete\_mesh

Deletes an existing service mesh.

Type annotations and code completion for `#!python session.client("appmesh").delete_mesh` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# delete_mesh method definition

await def delete_mesh(
    self,
    *,
    meshName: str,
) -> DeleteMeshOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteMeshOutputTypeDef](./type_defs.md#deletemeshoutputtypedef) 


```python
# delete_mesh method usage example with argument unpacking

kwargs: DeleteMeshInputRequestTypeDef = {  # (1)
    "meshName": ...,
}

parent.delete_mesh(**kwargs)
```

1. See [:material-code-braces: DeleteMeshInputRequestTypeDef](./type_defs.md#deletemeshinputrequesttypedef) 

### delete\_route

Deletes an existing route.

Type annotations and code completion for `#!python session.client("appmesh").delete_route` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# delete_route method definition

await def delete_route(
    self,
    *,
    meshName: str,
    routeName: str,
    virtualRouterName: str,
    meshOwner: str = ...,
) -> DeleteRouteOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteRouteOutputTypeDef](./type_defs.md#deleterouteoutputtypedef) 


```python
# delete_route method usage example with argument unpacking

kwargs: DeleteRouteInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "routeName": ...,
    "virtualRouterName": ...,
}

parent.delete_route(**kwargs)
```

1. See [:material-code-braces: DeleteRouteInputRequestTypeDef](./type_defs.md#deleterouteinputrequesttypedef) 

### delete\_virtual\_gateway

Deletes an existing virtual gateway.

Type annotations and code completion for `#!python session.client("appmesh").delete_virtual_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# delete_virtual_gateway method definition

await def delete_virtual_gateway(
    self,
    *,
    meshName: str,
    virtualGatewayName: str,
    meshOwner: str = ...,
) -> DeleteVirtualGatewayOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteVirtualGatewayOutputTypeDef](./type_defs.md#deletevirtualgatewayoutputtypedef) 


```python
# delete_virtual_gateway method usage example with argument unpacking

kwargs: DeleteVirtualGatewayInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "virtualGatewayName": ...,
}

parent.delete_virtual_gateway(**kwargs)
```

1. See [:material-code-braces: DeleteVirtualGatewayInputRequestTypeDef](./type_defs.md#deletevirtualgatewayinputrequesttypedef) 

### delete\_virtual\_node

Deletes an existing virtual node.

Type annotations and code completion for `#!python session.client("appmesh").delete_virtual_node` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# delete_virtual_node method definition

await def delete_virtual_node(
    self,
    *,
    meshName: str,
    virtualNodeName: str,
    meshOwner: str = ...,
) -> DeleteVirtualNodeOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteVirtualNodeOutputTypeDef](./type_defs.md#deletevirtualnodeoutputtypedef) 


```python
# delete_virtual_node method usage example with argument unpacking

kwargs: DeleteVirtualNodeInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "virtualNodeName": ...,
}

parent.delete_virtual_node(**kwargs)
```

1. See [:material-code-braces: DeleteVirtualNodeInputRequestTypeDef](./type_defs.md#deletevirtualnodeinputrequesttypedef) 

### delete\_virtual\_router

Deletes an existing virtual router.

Type annotations and code completion for `#!python session.client("appmesh").delete_virtual_router` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# delete_virtual_router method definition

await def delete_virtual_router(
    self,
    *,
    meshName: str,
    virtualRouterName: str,
    meshOwner: str = ...,
) -> DeleteVirtualRouterOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteVirtualRouterOutputTypeDef](./type_defs.md#deletevirtualrouteroutputtypedef) 


```python
# delete_virtual_router method usage example with argument unpacking

kwargs: DeleteVirtualRouterInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "virtualRouterName": ...,
}

parent.delete_virtual_router(**kwargs)
```

1. See [:material-code-braces: DeleteVirtualRouterInputRequestTypeDef](./type_defs.md#deletevirtualrouterinputrequesttypedef) 

### delete\_virtual\_service

Deletes an existing virtual service.

Type annotations and code completion for `#!python session.client("appmesh").delete_virtual_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# delete_virtual_service method definition

await def delete_virtual_service(
    self,
    *,
    meshName: str,
    virtualServiceName: str,
    meshOwner: str = ...,
) -> DeleteVirtualServiceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteVirtualServiceOutputTypeDef](./type_defs.md#deletevirtualserviceoutputtypedef) 


```python
# delete_virtual_service method usage example with argument unpacking

kwargs: DeleteVirtualServiceInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "virtualServiceName": ...,
}

parent.delete_virtual_service(**kwargs)
```

1. See [:material-code-braces: DeleteVirtualServiceInputRequestTypeDef](./type_defs.md#deletevirtualserviceinputrequesttypedef) 

### describe\_gateway\_route

Describes an existing gateway route.

Type annotations and code completion for `#!python session.client("appmesh").describe_gateway_route` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# describe_gateway_route method definition

await def describe_gateway_route(
    self,
    *,
    gatewayRouteName: str,
    meshName: str,
    virtualGatewayName: str,
    meshOwner: str = ...,
) -> DescribeGatewayRouteOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeGatewayRouteOutputTypeDef](./type_defs.md#describegatewayrouteoutputtypedef) 


```python
# describe_gateway_route method usage example with argument unpacking

kwargs: DescribeGatewayRouteInputRequestTypeDef = {  # (1)
    "gatewayRouteName": ...,
    "meshName": ...,
    "virtualGatewayName": ...,
}

parent.describe_gateway_route(**kwargs)
```

1. See [:material-code-braces: DescribeGatewayRouteInputRequestTypeDef](./type_defs.md#describegatewayrouteinputrequesttypedef) 

### describe\_mesh

Describes an existing service mesh.

Type annotations and code completion for `#!python session.client("appmesh").describe_mesh` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# describe_mesh method definition

await def describe_mesh(
    self,
    *,
    meshName: str,
    meshOwner: str = ...,
) -> DescribeMeshOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMeshOutputTypeDef](./type_defs.md#describemeshoutputtypedef) 


```python
# describe_mesh method usage example with argument unpacking

kwargs: DescribeMeshInputRequestTypeDef = {  # (1)
    "meshName": ...,
}

parent.describe_mesh(**kwargs)
```

1. See [:material-code-braces: DescribeMeshInputRequestTypeDef](./type_defs.md#describemeshinputrequesttypedef) 

### describe\_route

Describes an existing route.

Type annotations and code completion for `#!python session.client("appmesh").describe_route` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# describe_route method definition

await def describe_route(
    self,
    *,
    meshName: str,
    routeName: str,
    virtualRouterName: str,
    meshOwner: str = ...,
) -> DescribeRouteOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRouteOutputTypeDef](./type_defs.md#describerouteoutputtypedef) 


```python
# describe_route method usage example with argument unpacking

kwargs: DescribeRouteInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "routeName": ...,
    "virtualRouterName": ...,
}

parent.describe_route(**kwargs)
```

1. See [:material-code-braces: DescribeRouteInputRequestTypeDef](./type_defs.md#describerouteinputrequesttypedef) 

### describe\_virtual\_gateway

Describes an existing virtual gateway.

Type annotations and code completion for `#!python session.client("appmesh").describe_virtual_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# describe_virtual_gateway method definition

await def describe_virtual_gateway(
    self,
    *,
    meshName: str,
    virtualGatewayName: str,
    meshOwner: str = ...,
) -> DescribeVirtualGatewayOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeVirtualGatewayOutputTypeDef](./type_defs.md#describevirtualgatewayoutputtypedef) 


```python
# describe_virtual_gateway method usage example with argument unpacking

kwargs: DescribeVirtualGatewayInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "virtualGatewayName": ...,
}

parent.describe_virtual_gateway(**kwargs)
```

1. See [:material-code-braces: DescribeVirtualGatewayInputRequestTypeDef](./type_defs.md#describevirtualgatewayinputrequesttypedef) 

### describe\_virtual\_node

Describes an existing virtual node.

Type annotations and code completion for `#!python session.client("appmesh").describe_virtual_node` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# describe_virtual_node method definition

await def describe_virtual_node(
    self,
    *,
    meshName: str,
    virtualNodeName: str,
    meshOwner: str = ...,
) -> DescribeVirtualNodeOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeVirtualNodeOutputTypeDef](./type_defs.md#describevirtualnodeoutputtypedef) 


```python
# describe_virtual_node method usage example with argument unpacking

kwargs: DescribeVirtualNodeInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "virtualNodeName": ...,
}

parent.describe_virtual_node(**kwargs)
```

1. See [:material-code-braces: DescribeVirtualNodeInputRequestTypeDef](./type_defs.md#describevirtualnodeinputrequesttypedef) 

### describe\_virtual\_router

Describes an existing virtual router.

Type annotations and code completion for `#!python session.client("appmesh").describe_virtual_router` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# describe_virtual_router method definition

await def describe_virtual_router(
    self,
    *,
    meshName: str,
    virtualRouterName: str,
    meshOwner: str = ...,
) -> DescribeVirtualRouterOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeVirtualRouterOutputTypeDef](./type_defs.md#describevirtualrouteroutputtypedef) 


```python
# describe_virtual_router method usage example with argument unpacking

kwargs: DescribeVirtualRouterInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "virtualRouterName": ...,
}

parent.describe_virtual_router(**kwargs)
```

1. See [:material-code-braces: DescribeVirtualRouterInputRequestTypeDef](./type_defs.md#describevirtualrouterinputrequesttypedef) 

### describe\_virtual\_service

Describes an existing virtual service.

Type annotations and code completion for `#!python session.client("appmesh").describe_virtual_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# describe_virtual_service method definition

await def describe_virtual_service(
    self,
    *,
    meshName: str,
    virtualServiceName: str,
    meshOwner: str = ...,
) -> DescribeVirtualServiceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeVirtualServiceOutputTypeDef](./type_defs.md#describevirtualserviceoutputtypedef) 


```python
# describe_virtual_service method usage example with argument unpacking

kwargs: DescribeVirtualServiceInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "virtualServiceName": ...,
}

parent.describe_virtual_service(**kwargs)
```

1. See [:material-code-braces: DescribeVirtualServiceInputRequestTypeDef](./type_defs.md#describevirtualserviceinputrequesttypedef) 

### list\_gateway\_routes

Returns a list of existing gateway routes that are associated to a virtual
gateway.

Type annotations and code completion for `#!python session.client("appmesh").list_gateway_routes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# list_gateway_routes method definition

await def list_gateway_routes(
    self,
    *,
    meshName: str,
    virtualGatewayName: str,
    limit: int = ...,
    meshOwner: str = ...,
    nextToken: str = ...,
) -> ListGatewayRoutesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGatewayRoutesOutputTypeDef](./type_defs.md#listgatewayroutesoutputtypedef) 


```python
# list_gateway_routes method usage example with argument unpacking

kwargs: ListGatewayRoutesInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "virtualGatewayName": ...,
}

parent.list_gateway_routes(**kwargs)
```

1. See [:material-code-braces: ListGatewayRoutesInputRequestTypeDef](./type_defs.md#listgatewayroutesinputrequesttypedef) 

### list\_meshes

Returns a list of existing service meshes.

Type annotations and code completion for `#!python session.client("appmesh").list_meshes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# list_meshes method definition

await def list_meshes(
    self,
    *,
    limit: int = ...,
    nextToken: str = ...,
) -> ListMeshesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMeshesOutputTypeDef](./type_defs.md#listmeshesoutputtypedef) 


```python
# list_meshes method usage example with argument unpacking

kwargs: ListMeshesInputRequestTypeDef = {  # (1)
    "limit": ...,
}

parent.list_meshes(**kwargs)
```

1. See [:material-code-braces: ListMeshesInputRequestTypeDef](./type_defs.md#listmeshesinputrequesttypedef) 

### list\_routes

Returns a list of existing routes in a service mesh.

Type annotations and code completion for `#!python session.client("appmesh").list_routes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# list_routes method definition

await def list_routes(
    self,
    *,
    meshName: str,
    virtualRouterName: str,
    limit: int = ...,
    meshOwner: str = ...,
    nextToken: str = ...,
) -> ListRoutesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRoutesOutputTypeDef](./type_defs.md#listroutesoutputtypedef) 


```python
# list_routes method usage example with argument unpacking

kwargs: ListRoutesInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "virtualRouterName": ...,
}

parent.list_routes(**kwargs)
```

1. See [:material-code-braces: ListRoutesInputRequestTypeDef](./type_defs.md#listroutesinputrequesttypedef) 

### list\_tags\_for\_resource

List the tags for an App Mesh resource.

Type annotations and code completion for `#!python session.client("appmesh").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
    limit: int = ...,
    nextToken: str = ...,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef) 

### list\_virtual\_gateways

Returns a list of existing virtual gateways in a service mesh.

Type annotations and code completion for `#!python session.client("appmesh").list_virtual_gateways` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# list_virtual_gateways method definition

await def list_virtual_gateways(
    self,
    *,
    meshName: str,
    limit: int = ...,
    meshOwner: str = ...,
    nextToken: str = ...,
) -> ListVirtualGatewaysOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVirtualGatewaysOutputTypeDef](./type_defs.md#listvirtualgatewaysoutputtypedef) 


```python
# list_virtual_gateways method usage example with argument unpacking

kwargs: ListVirtualGatewaysInputRequestTypeDef = {  # (1)
    "meshName": ...,
}

parent.list_virtual_gateways(**kwargs)
```

1. See [:material-code-braces: ListVirtualGatewaysInputRequestTypeDef](./type_defs.md#listvirtualgatewaysinputrequesttypedef) 

### list\_virtual\_nodes

Returns a list of existing virtual nodes.

Type annotations and code completion for `#!python session.client("appmesh").list_virtual_nodes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# list_virtual_nodes method definition

await def list_virtual_nodes(
    self,
    *,
    meshName: str,
    limit: int = ...,
    meshOwner: str = ...,
    nextToken: str = ...,
) -> ListVirtualNodesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVirtualNodesOutputTypeDef](./type_defs.md#listvirtualnodesoutputtypedef) 


```python
# list_virtual_nodes method usage example with argument unpacking

kwargs: ListVirtualNodesInputRequestTypeDef = {  # (1)
    "meshName": ...,
}

parent.list_virtual_nodes(**kwargs)
```

1. See [:material-code-braces: ListVirtualNodesInputRequestTypeDef](./type_defs.md#listvirtualnodesinputrequesttypedef) 

### list\_virtual\_routers

Returns a list of existing virtual routers in a service mesh.

Type annotations and code completion for `#!python session.client("appmesh").list_virtual_routers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# list_virtual_routers method definition

await def list_virtual_routers(
    self,
    *,
    meshName: str,
    limit: int = ...,
    meshOwner: str = ...,
    nextToken: str = ...,
) -> ListVirtualRoutersOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVirtualRoutersOutputTypeDef](./type_defs.md#listvirtualroutersoutputtypedef) 


```python
# list_virtual_routers method usage example with argument unpacking

kwargs: ListVirtualRoutersInputRequestTypeDef = {  # (1)
    "meshName": ...,
}

parent.list_virtual_routers(**kwargs)
```

1. See [:material-code-braces: ListVirtualRoutersInputRequestTypeDef](./type_defs.md#listvirtualroutersinputrequesttypedef) 

### list\_virtual\_services

Returns a list of existing virtual services in a service mesh.

Type annotations and code completion for `#!python session.client("appmesh").list_virtual_services` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# list_virtual_services method definition

await def list_virtual_services(
    self,
    *,
    meshName: str,
    limit: int = ...,
    meshOwner: str = ...,
    nextToken: str = ...,
) -> ListVirtualServicesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVirtualServicesOutputTypeDef](./type_defs.md#listvirtualservicesoutputtypedef) 


```python
# list_virtual_services method usage example with argument unpacking

kwargs: ListVirtualServicesInputRequestTypeDef = {  # (1)
    "meshName": ...,
}

parent.list_virtual_services(**kwargs)
```

1. See [:material-code-braces: ListVirtualServicesInputRequestTypeDef](./type_defs.md#listvirtualservicesinputrequesttypedef) 

### tag\_resource

Associates the specified tags to a resource with the specified
<code>resourceArn</code>.

Type annotations and code completion for `#!python session.client("appmesh").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Sequence[TagRefTypeDef],  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagRefTypeDef](./type_defs.md#tagreftypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef) 

### untag\_resource

Deletes specified tags from a resource.

Type annotations and code completion for `#!python session.client("appmesh").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

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

kwargs: UntagResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef) 

### update\_gateway\_route

Updates an existing gateway route that is associated to a specified virtual
gateway in a service mesh.

Type annotations and code completion for `#!python session.client("appmesh").update_gateway_route` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# update_gateway_route method definition

await def update_gateway_route(
    self,
    *,
    gatewayRouteName: str,
    meshName: str,
    spec: GatewayRouteSpecTypeDef,  # (1)
    virtualGatewayName: str,
    clientToken: str = ...,
    meshOwner: str = ...,
) -> UpdateGatewayRouteOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: GatewayRouteSpecTypeDef](./type_defs.md#gatewayroutespectypedef) 
2. See [:material-code-braces: UpdateGatewayRouteOutputTypeDef](./type_defs.md#updategatewayrouteoutputtypedef) 


```python
# update_gateway_route method usage example with argument unpacking

kwargs: UpdateGatewayRouteInputRequestTypeDef = {  # (1)
    "gatewayRouteName": ...,
    "meshName": ...,
    "spec": ...,
    "virtualGatewayName": ...,
}

parent.update_gateway_route(**kwargs)
```

1. See [:material-code-braces: UpdateGatewayRouteInputRequestTypeDef](./type_defs.md#updategatewayrouteinputrequesttypedef) 

### update\_mesh

Updates an existing service mesh.

Type annotations and code completion for `#!python session.client("appmesh").update_mesh` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# update_mesh method definition

await def update_mesh(
    self,
    *,
    meshName: str,
    clientToken: str = ...,
    spec: MeshSpecTypeDef = ...,  # (1)
) -> UpdateMeshOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MeshSpecTypeDef](./type_defs.md#meshspectypedef) 
2. See [:material-code-braces: UpdateMeshOutputTypeDef](./type_defs.md#updatemeshoutputtypedef) 


```python
# update_mesh method usage example with argument unpacking

kwargs: UpdateMeshInputRequestTypeDef = {  # (1)
    "meshName": ...,
}

parent.update_mesh(**kwargs)
```

1. See [:material-code-braces: UpdateMeshInputRequestTypeDef](./type_defs.md#updatemeshinputrequesttypedef) 

### update\_route

Updates an existing route for a specified service mesh and virtual router.

Type annotations and code completion for `#!python session.client("appmesh").update_route` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# update_route method definition

await def update_route(
    self,
    *,
    meshName: str,
    routeName: str,
    spec: RouteSpecTypeDef,  # (1)
    virtualRouterName: str,
    clientToken: str = ...,
    meshOwner: str = ...,
) -> UpdateRouteOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RouteSpecTypeDef](./type_defs.md#routespectypedef) 
2. See [:material-code-braces: UpdateRouteOutputTypeDef](./type_defs.md#updaterouteoutputtypedef) 


```python
# update_route method usage example with argument unpacking

kwargs: UpdateRouteInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "routeName": ...,
    "spec": ...,
    "virtualRouterName": ...,
}

parent.update_route(**kwargs)
```

1. See [:material-code-braces: UpdateRouteInputRequestTypeDef](./type_defs.md#updaterouteinputrequesttypedef) 

### update\_virtual\_gateway

Updates an existing virtual gateway in a specified service mesh.

Type annotations and code completion for `#!python session.client("appmesh").update_virtual_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# update_virtual_gateway method definition

await def update_virtual_gateway(
    self,
    *,
    meshName: str,
    spec: VirtualGatewaySpecTypeDef,  # (1)
    virtualGatewayName: str,
    clientToken: str = ...,
    meshOwner: str = ...,
) -> UpdateVirtualGatewayOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VirtualGatewaySpecTypeDef](./type_defs.md#virtualgatewayspectypedef) 
2. See [:material-code-braces: UpdateVirtualGatewayOutputTypeDef](./type_defs.md#updatevirtualgatewayoutputtypedef) 


```python
# update_virtual_gateway method usage example with argument unpacking

kwargs: UpdateVirtualGatewayInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "spec": ...,
    "virtualGatewayName": ...,
}

parent.update_virtual_gateway(**kwargs)
```

1. See [:material-code-braces: UpdateVirtualGatewayInputRequestTypeDef](./type_defs.md#updatevirtualgatewayinputrequesttypedef) 

### update\_virtual\_node

Updates an existing virtual node in a specified service mesh.

Type annotations and code completion for `#!python session.client("appmesh").update_virtual_node` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# update_virtual_node method definition

await def update_virtual_node(
    self,
    *,
    meshName: str,
    spec: VirtualNodeSpecTypeDef,  # (1)
    virtualNodeName: str,
    clientToken: str = ...,
    meshOwner: str = ...,
) -> UpdateVirtualNodeOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VirtualNodeSpecTypeDef](./type_defs.md#virtualnodespectypedef) 
2. See [:material-code-braces: UpdateVirtualNodeOutputTypeDef](./type_defs.md#updatevirtualnodeoutputtypedef) 


```python
# update_virtual_node method usage example with argument unpacking

kwargs: UpdateVirtualNodeInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "spec": ...,
    "virtualNodeName": ...,
}

parent.update_virtual_node(**kwargs)
```

1. See [:material-code-braces: UpdateVirtualNodeInputRequestTypeDef](./type_defs.md#updatevirtualnodeinputrequesttypedef) 

### update\_virtual\_router

Updates an existing virtual router in a specified service mesh.

Type annotations and code completion for `#!python session.client("appmesh").update_virtual_router` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# update_virtual_router method definition

await def update_virtual_router(
    self,
    *,
    meshName: str,
    spec: VirtualRouterSpecTypeDef,  # (1)
    virtualRouterName: str,
    clientToken: str = ...,
    meshOwner: str = ...,
) -> UpdateVirtualRouterOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VirtualRouterSpecTypeDef](./type_defs.md#virtualrouterspectypedef) 
2. See [:material-code-braces: UpdateVirtualRouterOutputTypeDef](./type_defs.md#updatevirtualrouteroutputtypedef) 


```python
# update_virtual_router method usage example with argument unpacking

kwargs: UpdateVirtualRouterInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "spec": ...,
    "virtualRouterName": ...,
}

parent.update_virtual_router(**kwargs)
```

1. See [:material-code-braces: UpdateVirtualRouterInputRequestTypeDef](./type_defs.md#updatevirtualrouterinputrequesttypedef) 

### update\_virtual\_service

Updates an existing virtual service in a specified service mesh.

Type annotations and code completion for `#!python session.client("appmesh").update_virtual_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# update_virtual_service method definition

await def update_virtual_service(
    self,
    *,
    meshName: str,
    spec: VirtualServiceSpecTypeDef,  # (1)
    virtualServiceName: str,
    clientToken: str = ...,
    meshOwner: str = ...,
) -> UpdateVirtualServiceOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VirtualServiceSpecTypeDef](./type_defs.md#virtualservicespectypedef) 
2. See [:material-code-braces: UpdateVirtualServiceOutputTypeDef](./type_defs.md#updatevirtualserviceoutputtypedef) 


```python
# update_virtual_service method usage example with argument unpacking

kwargs: UpdateVirtualServiceInputRequestTypeDef = {  # (1)
    "meshName": ...,
    "spec": ...,
    "virtualServiceName": ...,
}

parent.update_virtual_service(**kwargs)
```

1. See [:material-code-braces: UpdateVirtualServiceInputRequestTypeDef](./type_defs.md#updatevirtualserviceinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("appmesh").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("appmesh").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

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

Type annotations and code completion for `#!python session.client("appmesh").get_paginator` method with overloads.

- `client.get_paginator("list_gateway_routes")` -> [ListGatewayRoutesPaginator](./paginators.md#listgatewayroutespaginator)
- `client.get_paginator("list_meshes")` -> [ListMeshesPaginator](./paginators.md#listmeshespaginator)
- `client.get_paginator("list_routes")` -> [ListRoutesPaginator](./paginators.md#listroutespaginator)
- `client.get_paginator("list_tags_for_resource")` -> [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
- `client.get_paginator("list_virtual_gateways")` -> [ListVirtualGatewaysPaginator](./paginators.md#listvirtualgatewayspaginator)
- `client.get_paginator("list_virtual_nodes")` -> [ListVirtualNodesPaginator](./paginators.md#listvirtualnodespaginator)
- `client.get_paginator("list_virtual_routers")` -> [ListVirtualRoutersPaginator](./paginators.md#listvirtualrouterspaginator)
- `client.get_paginator("list_virtual_services")` -> [ListVirtualServicesPaginator](./paginators.md#listvirtualservicespaginator)


