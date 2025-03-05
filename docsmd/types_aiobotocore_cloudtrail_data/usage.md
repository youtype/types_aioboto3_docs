# Examples

> [Index](../README.md) > [CloudTrailDataService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudTrailDataService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#cloudtraildataservice)
    type annotations stubs module [types-aiobotocore-cloudtrail-data](https://pypi.org/project/types-aiobotocore-cloudtrail-data/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[cloudtrail-data]` package installed.

Write your `CloudTrailDataService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# CloudTrailDataServiceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("cloudtrail-data") as client:  # (1)
    result = await client.put_audit_events()  # (2)
```

1. client: [CloudTrailDataServiceClient](./client.md)
2. result: [:material-code-braces: PutAuditEventsResponseTypeDef](./type_defs.md#putauditeventsresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[cloudtrail-data]`
or a standalone `types_aiobotocore_cloudtrail_data` package, you have to explicitly specify
`client: CloudTrailDataServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# CloudTrailDataServiceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_cloudtrail_data.client import CloudTrailDataServiceClient
from types_aiobotocore_cloudtrail_data.type_defs import PutAuditEventsResponseTypeDef
from types_aiobotocore_cloudtrail_data.type_defs import PutAuditEventsRequestTypeDef


session = Session()

client: CloudTrailDataServiceClient
async with session.client("cloudtrail-data") as client:  # (1)
    kwargs: PutAuditEventsRequestTypeDef = {...}  # (2)
    result: PutAuditEventsResponseTypeDef = await client.put_audit_events(**kwargs)  # (3)
```

1. client: [CloudTrailDataServiceClient](./client.md)
2. kwargs: [:material-code-braces: PutAuditEventsRequestTypeDef](./type_defs.md#putauditeventsrequesttypedef)
3. result: [:material-code-braces: PutAuditEventsResponseTypeDef](./type_defs.md#putauditeventsresponsetypedef)






