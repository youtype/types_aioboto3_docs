# Examples

> [Index](../README.md) > [ServiceQuotas](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ServiceQuotas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#servicequotas)
    type annotations stubs module [types-aiobotocore-service-quotas](https://pypi.org/project/types-aiobotocore-service-quotas/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[service-quotas]` package installed.

Write your `ServiceQuotas` code as usual,
type checking and code completion should work out of the box.



```python
# ServiceQuotasClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("service-quotas") as client:  # (1)
    result = await client.get_aws_default_service_quota()  # (2)
```

1. client: [ServiceQuotasClient](./client.md)
2. result: [:material-code-braces: GetAWSDefaultServiceQuotaResponseTypeDef](./type_defs.md#getawsdefaultservicequotaresponsetypedef) 



```python
# ListAWSDefaultServiceQuotasPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("service-quotas") as client:  # (1)
    paginator = client.get_paginator("list_aws_default_service_quotas")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ServiceQuotasClient](./client.md)
2. paginator: [ListAWSDefaultServiceQuotasPaginator](./paginators.md#listawsdefaultservicequotaspaginator)
3. item: [:material-code-braces: ListAWSDefaultServiceQuotasResponseTypeDef](./type_defs.md#listawsdefaultservicequotasresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[service-quotas]`
or a standalone `types_aiobotocore_service_quotas` package, you have to explicitly specify
`client: ServiceQuotasClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ServiceQuotasClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_service_quotas.client import ServiceQuotasClient
from types_aiobotocore_service_quotas.type_defs import GetAWSDefaultServiceQuotaResponseTypeDef
from types_aiobotocore_service_quotas.type_defs import GetAWSDefaultServiceQuotaRequestRequestTypeDef


session = Session()

client: ServiceQuotasClient
async with session.client("service-quotas") as client:  # (1)
    kwargs: GetAWSDefaultServiceQuotaRequestRequestTypeDef = {...}  # (2)
    result: GetAWSDefaultServiceQuotaResponseTypeDef = await client.get_aws_default_service_quota(**kwargs)  # (3)
```

1. client: [ServiceQuotasClient](./client.md)
2. kwargs: [:material-code-braces: GetAWSDefaultServiceQuotaRequestRequestTypeDef](./type_defs.md#getawsdefaultservicequotarequestrequesttypedef) 
3. result: [:material-code-braces: GetAWSDefaultServiceQuotaResponseTypeDef](./type_defs.md#getawsdefaultservicequotaresponsetypedef) 



```python
# ListAWSDefaultServiceQuotasPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_service_quotas.client import ServiceQuotasClient
from types_aiobotocore_service_quotas.paginator import ListAWSDefaultServiceQuotasPaginator
from types_aiobotocore_service_quotas.type_defs import ListAWSDefaultServiceQuotasResponseTypeDef


session = Session()

client: ServiceQuotasClient
async with session.client("service-quotas") as client:  # (1)
    paginator: ListAWSDefaultServiceQuotasPaginator = client.get_paginator("list_aws_default_service_quotas")  # (2)
    async for item in paginator.paginate(...):
        item: ListAWSDefaultServiceQuotasResponseTypeDef
        print(item)  # (3)
```

1. client: [ServiceQuotasClient](./client.md)
2. paginator: [ListAWSDefaultServiceQuotasPaginator](./paginators.md#listawsdefaultservicequotaspaginator)
3. item: [:material-code-braces: ListAWSDefaultServiceQuotasResponseTypeDef](./type_defs.md#listawsdefaultservicequotasresponsetypedef) 



