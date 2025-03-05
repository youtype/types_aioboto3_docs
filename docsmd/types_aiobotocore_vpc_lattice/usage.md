# Examples

> [Index](../README.md) > [VPCLattice](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [VPCLattice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#vpclattice)
    type annotations stubs module [types-aiobotocore-vpc-lattice](https://pypi.org/project/types-aiobotocore-vpc-lattice/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[vpc-lattice]` package installed.

Write your `VPCLattice` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# VPCLatticeClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("vpc-lattice") as client:  # (1)
    result = await client.batch_update_rule()  # (2)
```

1. client: [VPCLatticeClient](./client.md)
2. result: [:material-code-braces: BatchUpdateRuleResponseTypeDef](./type_defs.md#batchupdateruleresponsetypedef)



#### Paginator usage example

```python
# ListAccessLogSubscriptionsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("vpc-lattice") as client:  # (1)
    paginator = client.get_paginator("list_access_log_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [VPCLatticeClient](./client.md)
2. paginator: [ListAccessLogSubscriptionsPaginator](./paginators.md#listaccesslogsubscriptionspaginator)
3. item: [:material-code-braces: ListAccessLogSubscriptionsResponseTypeDef](./type_defs.md#listaccesslogsubscriptionsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[vpc-lattice]`
or a standalone `types_aiobotocore_vpc_lattice` package, you have to explicitly specify
`client: VPCLatticeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# VPCLatticeClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_vpc_lattice.client import VPCLatticeClient
from types_aiobotocore_vpc_lattice.type_defs import BatchUpdateRuleResponseTypeDef
from types_aiobotocore_vpc_lattice.type_defs import BatchUpdateRuleRequestTypeDef


session = Session()

client: VPCLatticeClient
async with session.client("vpc-lattice") as client:  # (1)
    kwargs: BatchUpdateRuleRequestTypeDef = {...}  # (2)
    result: BatchUpdateRuleResponseTypeDef = await client.batch_update_rule(**kwargs)  # (3)
```

1. client: [VPCLatticeClient](./client.md)
2. kwargs: [:material-code-braces: BatchUpdateRuleRequestTypeDef](./type_defs.md#batchupdaterulerequesttypedef)
3. result: [:material-code-braces: BatchUpdateRuleResponseTypeDef](./type_defs.md#batchupdateruleresponsetypedef)



#### Paginator usage example

```python
# ListAccessLogSubscriptionsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_vpc_lattice.client import VPCLatticeClient
from types_aiobotocore_vpc_lattice.paginator import ListAccessLogSubscriptionsPaginator
from types_aiobotocore_vpc_lattice.type_defs import ListAccessLogSubscriptionsResponseTypeDef


session = Session()

client: VPCLatticeClient
async with session.client("vpc-lattice") as client:  # (1)
    paginator: ListAccessLogSubscriptionsPaginator = client.get_paginator("list_access_log_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccessLogSubscriptionsResponseTypeDef
        print(item)  # (3)
```

1. client: [VPCLatticeClient](./client.md)
2. paginator: [ListAccessLogSubscriptionsPaginator](./paginators.md#listaccesslogsubscriptionspaginator)
3. item: [:material-code-braces: ListAccessLogSubscriptionsResponseTypeDef](./type_defs.md#listaccesslogsubscriptionsresponsetypedef)




