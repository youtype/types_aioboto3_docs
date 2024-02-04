# Paginators

> [Index](../README.md) > [ControlTower](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ControlTower](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
    type annotations stubs module [types-aiobotocore-controltower](https://pypi.org/project/types-aiobotocore-controltower/).

## ListEnabledControlsPaginator

Type annotations and code completion for `#!python session.client("controltower").get_paginator("list_enabled_controls")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListEnabledControls)

```python
# ListEnabledControlsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_controltower.paginator import ListEnabledControlsPaginator

session = Session()

session = get_session()
async with session.client("controltower") as client:  # (1)
    paginator: ListEnabledControlsPaginator = client.get_paginator("list_enabled_controls")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnabledControlsOutputTypeDef
        print(item)  # (3)
```

1. client: [ControlTowerClient](./client.md)
2. paginator: [ListEnabledControlsPaginator](./paginators.md#listenabledcontrolspaginator)
3. item: [:material-code-braces: ListEnabledControlsOutputTypeDef](./type_defs.md#listenabledcontrolsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListEnabledControlsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    targetIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEnabledControlsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEnabledControlsOutputTypeDef](./type_defs.md#listenabledcontrolsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEnabledControlsInputListEnabledControlsPaginateTypeDef = {  # (1)
    "targetIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnabledControlsInputListEnabledControlsPaginateTypeDef](./type_defs.md#listenabledcontrolsinputlistenabledcontrolspaginatetypedef) 
## ListLandingZonesPaginator

Type annotations and code completion for `#!python session.client("controltower").get_paginator("list_landing_zones")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListLandingZones)

```python
# ListLandingZonesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_controltower.paginator import ListLandingZonesPaginator

session = Session()

session = get_session()
async with session.client("controltower") as client:  # (1)
    paginator: ListLandingZonesPaginator = client.get_paginator("list_landing_zones")  # (2)
    async for item in paginator.paginate(...):
        item: ListLandingZonesOutputTypeDef
        print(item)  # (3)
```

1. client: [ControlTowerClient](./client.md)
2. paginator: [ListLandingZonesPaginator](./paginators.md#listlandingzonespaginator)
3. item: [:material-code-braces: ListLandingZonesOutputTypeDef](./type_defs.md#listlandingzonesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListLandingZonesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListLandingZonesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLandingZonesOutputTypeDef](./type_defs.md#listlandingzonesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLandingZonesInputListLandingZonesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLandingZonesInputListLandingZonesPaginateTypeDef](./type_defs.md#listlandingzonesinputlistlandingzonespaginatetypedef) 
