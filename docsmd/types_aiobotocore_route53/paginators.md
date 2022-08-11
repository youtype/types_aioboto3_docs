# Paginators

> [Index](../README.md) > [Route53](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Route53](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
    type annotations stubs module [types-aiobotocore-route53](https://pypi.org/project/types-aiobotocore-route53/).

## ListHealthChecksPaginator

Type annotations and code completion for `#!python session.client("route53").get_paginator("list_health_checks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHealthChecks)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_route53.paginator import ListHealthChecksPaginator

session = Session()

session = get_session()
async with session.client("route53") as client:  # (1)
    paginator: ListHealthChecksPaginator = client.get_paginator("list_health_checks")  # (2)
    async for item in paginator.paginate(...):
        item: ListHealthChecksResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53Client](./client.md)
2. paginator: [ListHealthChecksPaginator](./paginators.md#listhealthcheckspaginator)
3. item: [:material-code-braces: ListHealthChecksResponseTypeDef](./type_defs.md#listhealthchecksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListHealthChecksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListHealthChecksResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListHealthChecksResponseTypeDef](./type_defs.md#listhealthchecksresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListHealthChecksRequestListHealthChecksPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHealthChecksRequestListHealthChecksPaginateTypeDef](./type_defs.md#listhealthchecksrequestlisthealthcheckspaginatetypedef) 
## ListHostedZonesPaginator

Type annotations and code completion for `#!python session.client("route53").get_paginator("list_hosted_zones")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHostedZones)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_route53.paginator import ListHostedZonesPaginator

session = Session()

session = get_session()
async with session.client("route53") as client:  # (1)
    paginator: ListHostedZonesPaginator = client.get_paginator("list_hosted_zones")  # (2)
    async for item in paginator.paginate(...):
        item: ListHostedZonesResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53Client](./client.md)
2. paginator: [ListHostedZonesPaginator](./paginators.md#listhostedzonespaginator)
3. item: [:material-code-braces: ListHostedZonesResponseTypeDef](./type_defs.md#listhostedzonesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListHostedZonesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DelegationSetId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListHostedZonesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListHostedZonesResponseTypeDef](./type_defs.md#listhostedzonesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListHostedZonesRequestListHostedZonesPaginateTypeDef = {  # (1)
    "DelegationSetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHostedZonesRequestListHostedZonesPaginateTypeDef](./type_defs.md#listhostedzonesrequestlisthostedzonespaginatetypedef) 
## ListQueryLoggingConfigsPaginator

Type annotations and code completion for `#!python session.client("route53").get_paginator("list_query_logging_configs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListQueryLoggingConfigs)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_route53.paginator import ListQueryLoggingConfigsPaginator

session = Session()

session = get_session()
async with session.client("route53") as client:  # (1)
    paginator: ListQueryLoggingConfigsPaginator = client.get_paginator("list_query_logging_configs")  # (2)
    async for item in paginator.paginate(...):
        item: ListQueryLoggingConfigsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53Client](./client.md)
2. paginator: [ListQueryLoggingConfigsPaginator](./paginators.md#listqueryloggingconfigspaginator)
3. item: [:material-code-braces: ListQueryLoggingConfigsResponseTypeDef](./type_defs.md#listqueryloggingconfigsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListQueryLoggingConfigsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    HostedZoneId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListQueryLoggingConfigsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListQueryLoggingConfigsResponseTypeDef](./type_defs.md#listqueryloggingconfigsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef = {  # (1)
    "HostedZoneId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef](./type_defs.md#listqueryloggingconfigsrequestlistqueryloggingconfigspaginatetypedef) 
## ListResourceRecordSetsPaginator

Type annotations and code completion for `#!python session.client("route53").get_paginator("list_resource_record_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListResourceRecordSets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_route53.paginator import ListResourceRecordSetsPaginator

session = Session()

session = get_session()
async with session.client("route53") as client:  # (1)
    paginator: ListResourceRecordSetsPaginator = client.get_paginator("list_resource_record_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceRecordSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53Client](./client.md)
2. paginator: [ListResourceRecordSetsPaginator](./paginators.md#listresourcerecordsetspaginator)
3. item: [:material-code-braces: ListResourceRecordSetsResponseTypeDef](./type_defs.md#listresourcerecordsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResourceRecordSetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    HostedZoneId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListResourceRecordSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResourceRecordSetsResponseTypeDef](./type_defs.md#listresourcerecordsetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = {  # (1)
    "HostedZoneId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef](./type_defs.md#listresourcerecordsetsrequestlistresourcerecordsetspaginatetypedef) 
## ListVPCAssociationAuthorizationsPaginator

Type annotations and code completion for `#!python session.client("route53").get_paginator("list_vpc_association_authorizations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListVPCAssociationAuthorizations)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_route53.paginator import ListVPCAssociationAuthorizationsPaginator

session = Session()

session = get_session()
async with session.client("route53") as client:  # (1)
    paginator: ListVPCAssociationAuthorizationsPaginator = client.get_paginator("list_vpc_association_authorizations")  # (2)
    async for item in paginator.paginate(...):
        item: ListVPCAssociationAuthorizationsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53Client](./client.md)
2. paginator: [ListVPCAssociationAuthorizationsPaginator](./paginators.md#listvpcassociationauthorizationspaginator)
3. item: [:material-code-braces: ListVPCAssociationAuthorizationsResponseTypeDef](./type_defs.md#listvpcassociationauthorizationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListVPCAssociationAuthorizationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    HostedZoneId: str,
    MaxResults: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListVPCAssociationAuthorizationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListVPCAssociationAuthorizationsResponseTypeDef](./type_defs.md#listvpcassociationauthorizationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = {  # (1)
    "HostedZoneId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef](./type_defs.md#listvpcassociationauthorizationsrequestlistvpcassociationauthorizationspaginatetypedef) 
