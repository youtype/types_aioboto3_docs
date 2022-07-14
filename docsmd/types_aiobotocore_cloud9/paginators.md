# Paginators

> [Index](../README.md) > [Cloud9](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Cloud9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
    type annotations stubs module [types-aiobotocore-cloud9](https://pypi.org/project/types-aiobotocore-cloud9/).

## DescribeEnvironmentMembershipsPaginator

Type annotations and code completion for `#!python session.client("cloud9").get_paginator("describe_environment_memberships")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.DescribeEnvironmentMemberships)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_cloud9.paginator import DescribeEnvironmentMembershipsPaginator

session = Session()

session = get_session()
async with session.client("cloud9") as client:  # (1)
    paginator: DescribeEnvironmentMembershipsPaginator = client.get_paginator("describe_environment_memberships")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEnvironmentMembershipsResultTypeDef
        print(item)  # (3)
```

1. client: [Cloud9Client](./client.md)
2. paginator: [DescribeEnvironmentMembershipsPaginator](./paginators.md#describeenvironmentmembershipspaginator)
3. item: [:material-code-braces: DescribeEnvironmentMembershipsResultTypeDef](./type_defs.md#describeenvironmentmembershipsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEnvironmentMembershipsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    userArn: str = ...,
    environmentId: str = ...,
    permissions: Sequence[PermissionsType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeEnvironmentMembershipsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: PermissionsType](./literals.md#permissionstype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeEnvironmentMembershipsResultTypeDef](./type_defs.md#describeenvironmentmembershipsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef = {  # (1)
    "userArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef](./type_defs.md#describeenvironmentmembershipsrequestdescribeenvironmentmembershipspaginatetypedef) 
## ListEnvironmentsPaginator

Type annotations and code completion for `#!python session.client("cloud9").get_paginator("list_environments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.ListEnvironments)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_cloud9.paginator import ListEnvironmentsPaginator

session = Session()

session = get_session()
async with session.client("cloud9") as client:  # (1)
    paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnvironmentsResultTypeDef
        print(item)  # (3)
```

1. client: [Cloud9Client](./client.md)
2. paginator: [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
3. item: [:material-code-braces: ListEnvironmentsResultTypeDef](./type_defs.md#listenvironmentsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListEnvironmentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEnvironmentsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEnvironmentsResultTypeDef](./type_defs.md#listenvironmentsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentsRequestListEnvironmentsPaginateTypeDef](./type_defs.md#listenvironmentsrequestlistenvironmentspaginatetypedef) 
