# Examples

> [Index](../README.md) > [Route53Domains](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Route53Domains](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#route53domains)
    type annotations stubs module [types-aiobotocore-route53domains](https://pypi.org/project/types-aiobotocore-route53domains/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[route53domains]` package installed.

Write your `Route53Domains` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# Route53DomainsClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("route53domains") as client:  # (1)
    result = await client.accept_domain_transfer_from_another_aws_account()  # (2)
```

1. client: [Route53DomainsClient](./client.md)
2. result: [:material-code-braces: AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef](./type_defs.md#acceptdomaintransferfromanotherawsaccountresponsetypedef)



#### Paginator usage example

```python
# ListDomainsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("route53domains") as client:  # (1)
    paginator = client.get_paginator("list_domains")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [Route53DomainsClient](./client.md)
2. paginator: [ListDomainsPaginator](./paginators.md#listdomainspaginator)
3. item: [:material-code-braces: ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[route53domains]`
or a standalone `types_aiobotocore_route53domains` package, you have to explicitly specify
`client: Route53DomainsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# Route53DomainsClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_route53domains.client import Route53DomainsClient
from types_aiobotocore_route53domains.type_defs import AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef
from types_aiobotocore_route53domains.type_defs import AcceptDomainTransferFromAnotherAwsAccountRequestTypeDef


session = Session()

client: Route53DomainsClient
async with session.client("route53domains") as client:  # (1)
    kwargs: AcceptDomainTransferFromAnotherAwsAccountRequestTypeDef = {...}  # (2)
    result: AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef = await client.accept_domain_transfer_from_another_aws_account(**kwargs)  # (3)
```

1. client: [Route53DomainsClient](./client.md)
2. kwargs: [:material-code-braces: AcceptDomainTransferFromAnotherAwsAccountRequestTypeDef](./type_defs.md#acceptdomaintransferfromanotherawsaccountrequesttypedef)
3. result: [:material-code-braces: AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef](./type_defs.md#acceptdomaintransferfromanotherawsaccountresponsetypedef)



#### Paginator usage example

```python
# ListDomainsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_route53domains.client import Route53DomainsClient
from types_aiobotocore_route53domains.paginator import ListDomainsPaginator
from types_aiobotocore_route53domains.type_defs import ListDomainsResponseTypeDef


session = Session()

client: Route53DomainsClient
async with session.client("route53domains") as client:  # (1)
    paginator: ListDomainsPaginator = client.get_paginator("list_domains")  # (2)
    async for item in paginator.paginate(...):
        item: ListDomainsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53DomainsClient](./client.md)
2. paginator: [ListDomainsPaginator](./paginators.md#listdomainspaginator)
3. item: [:material-code-braces: ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef)




