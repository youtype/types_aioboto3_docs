# Paginators

> [Index](../README.md) > [Private5G](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Private5G](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#private5g)
    type annotations stubs module [types-aiobotocore-privatenetworks](https://pypi.org/project/types-aiobotocore-privatenetworks/).

## ListDeviceIdentifiersPaginator

Type annotations and code completion for `#!python session.client("privatenetworks").get_paginator("list_device_identifiers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks/paginator/ListDeviceIdentifiers.html#Private5G.Paginator.ListDeviceIdentifiers)

```python
# ListDeviceIdentifiersPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_privatenetworks.paginator import ListDeviceIdentifiersPaginator

session = Session()

session = get_session()
async with session.client("privatenetworks") as client:  # (1)
    paginator: ListDeviceIdentifiersPaginator = client.get_paginator("list_device_identifiers")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeviceIdentifiersResponseTypeDef
        print(item)  # (3)
```

1. client: [Private5GClient](./client.md)
2. paginator: [ListDeviceIdentifiersPaginator](./paginators.md#listdeviceidentifierspaginator)
3. item: `AioPageIterator[ListDeviceIdentifiersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDeviceIdentifiersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    networkArn: str,
    filters: Mapping[DeviceIdentifierFilterKeysType, Sequence[str]] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListDeviceIdentifiersResponseTypeDef]:  # (3)
    ...
```

1. See `Mapping[DeviceIdentifierFilterKeysType, Sequence[str]]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListDeviceIdentifiersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDeviceIdentifiersRequestPaginateTypeDef = {  # (1)
    "networkArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeviceIdentifiersRequestPaginateTypeDef](./type_defs.md#listdeviceidentifiersrequestpaginatetypedef)
## ListNetworkResourcesPaginator

Type annotations and code completion for `#!python session.client("privatenetworks").get_paginator("list_network_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks/paginator/ListNetworkResources.html#Private5G.Paginator.ListNetworkResources)

```python
# ListNetworkResourcesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_privatenetworks.paginator import ListNetworkResourcesPaginator

session = Session()

session = get_session()
async with session.client("privatenetworks") as client:  # (1)
    paginator: ListNetworkResourcesPaginator = client.get_paginator("list_network_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListNetworkResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [Private5GClient](./client.md)
2. paginator: [ListNetworkResourcesPaginator](./paginators.md#listnetworkresourcespaginator)
3. item: `AioPageIterator[ListNetworkResourcesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListNetworkResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    networkArn: str,
    filters: Mapping[NetworkResourceFilterKeysType, Sequence[str]] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListNetworkResourcesResponseTypeDef]:  # (3)
    ...
```

1. See `Mapping[NetworkResourceFilterKeysType, Sequence[str]]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListNetworkResourcesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListNetworkResourcesRequestPaginateTypeDef = {  # (1)
    "networkArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNetworkResourcesRequestPaginateTypeDef](./type_defs.md#listnetworkresourcesrequestpaginatetypedef)
## ListNetworkSitesPaginator

Type annotations and code completion for `#!python session.client("privatenetworks").get_paginator("list_network_sites")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks/paginator/ListNetworkSites.html#Private5G.Paginator.ListNetworkSites)

```python
# ListNetworkSitesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_privatenetworks.paginator import ListNetworkSitesPaginator

session = Session()

session = get_session()
async with session.client("privatenetworks") as client:  # (1)
    paginator: ListNetworkSitesPaginator = client.get_paginator("list_network_sites")  # (2)
    async for item in paginator.paginate(...):
        item: ListNetworkSitesResponseTypeDef
        print(item)  # (3)
```

1. client: [Private5GClient](./client.md)
2. paginator: [ListNetworkSitesPaginator](./paginators.md#listnetworksitespaginator)
3. item: `AioPageIterator[ListNetworkSitesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListNetworkSitesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    networkArn: str,
    filters: Mapping[NetworkSiteFilterKeysType, Sequence[str]] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListNetworkSitesResponseTypeDef]:  # (3)
    ...
```

1. See `Mapping[Literal['STATUS'], Sequence[str]]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListNetworkSitesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListNetworkSitesRequestPaginateTypeDef = {  # (1)
    "networkArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNetworkSitesRequestPaginateTypeDef](./type_defs.md#listnetworksitesrequestpaginatetypedef)
## ListNetworksPaginator

Type annotations and code completion for `#!python session.client("privatenetworks").get_paginator("list_networks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks/paginator/ListNetworks.html#Private5G.Paginator.ListNetworks)

```python
# ListNetworksPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_privatenetworks.paginator import ListNetworksPaginator

session = Session()

session = get_session()
async with session.client("privatenetworks") as client:  # (1)
    paginator: ListNetworksPaginator = client.get_paginator("list_networks")  # (2)
    async for item in paginator.paginate(...):
        item: ListNetworksResponseTypeDef
        print(item)  # (3)
```

1. client: [Private5GClient](./client.md)
2. paginator: [ListNetworksPaginator](./paginators.md#listnetworkspaginator)
3. item: `AioPageIterator[ListNetworksResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListNetworksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Mapping[NetworkFilterKeysType, Sequence[str]] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListNetworksResponseTypeDef]:  # (3)
    ...
```

1. See `Mapping[Literal['STATUS'], Sequence[str]]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListNetworksResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListNetworksRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNetworksRequestPaginateTypeDef](./type_defs.md#listnetworksrequestpaginatetypedef)
## ListOrdersPaginator

Type annotations and code completion for `#!python session.client("privatenetworks").get_paginator("list_orders")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks/paginator/ListOrders.html#Private5G.Paginator.ListOrders)

```python
# ListOrdersPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_privatenetworks.paginator import ListOrdersPaginator

session = Session()

session = get_session()
async with session.client("privatenetworks") as client:  # (1)
    paginator: ListOrdersPaginator = client.get_paginator("list_orders")  # (2)
    async for item in paginator.paginate(...):
        item: ListOrdersResponseTypeDef
        print(item)  # (3)
```

1. client: [Private5GClient](./client.md)
2. paginator: [ListOrdersPaginator](./paginators.md#listorderspaginator)
3. item: `AioPageIterator[ListOrdersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListOrdersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    networkArn: str,
    filters: Mapping[OrderFilterKeysType, Sequence[str]] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListOrdersResponseTypeDef]:  # (3)
    ...
```

1. See `Mapping[OrderFilterKeysType, Sequence[str]]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListOrdersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListOrdersRequestPaginateTypeDef = {  # (1)
    "networkArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOrdersRequestPaginateTypeDef](./type_defs.md#listordersrequestpaginatetypedef)
