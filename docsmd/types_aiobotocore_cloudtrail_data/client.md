# CloudTrailDataServiceClient

> [Index](../README.md) > [CloudTrailDataService](./README.md) > CloudTrailDataServiceClient

!!! note ""

    Auto-generated documentation for [CloudTrailDataService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#cloudtraildataservice)
    type annotations stubs module [types-aiobotocore-cloudtrail-data](https://pypi.org/project/types-aiobotocore-cloudtrail-data/).

## CloudTrailDataServiceClient

Type annotations and code completion for `#!python session.client("cloudtrail-data")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#CloudTrailDataService.Client)

```python
# CloudTrailDataServiceClient usage example

from aioboto3.session import Session
from types_aiobotocore_cloudtrail_data.client import CloudTrailDataServiceClient

session = Session()
async with session.client("cloudtrail-data") as client:
    client: CloudTrailDataServiceClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("cloudtrail-data").exceptions` structure.

```python
# CloudTrailDataServiceClient.exceptions usage example

async with session.client("cloudtrail-data") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ChannelInsufficientPermission,
        client.exceptions.ChannelNotFound,
        client.exceptions.ChannelUnsupportedSchema,
        client.exceptions.ClientError,
        client.exceptions.DuplicatedAuditEventId,
        client.exceptions.InvalidChannelARN,
        client.exceptions.UnsupportedOperationException,
    ) as e:
        print(e)
```

```python
# CloudTrailDataServiceClient.exceptions type checking example

from types_aiobotocore_cloudtrail_data.client import Exceptions

def handle_error(exc: Exceptions.ChannelInsufficientPermission) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("cloudtrail-data").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#CloudTrailDataService.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("cloudtrail-data").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#CloudTrailDataService.Client)

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


### put\_audit\_events

Ingests your application events into CloudTrail Lake.

Type annotations and code completion for `#!python session.client("cloudtrail-data").put_audit_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#CloudTrailDataService.Client)

```python
# put_audit_events method definition

await def put_audit_events(
    self,
    *,
    auditEvents: Sequence[AuditEventTypeDef],  # (1)
    channelArn: str,
    externalId: str = ...,
) -> PutAuditEventsResponseTypeDef:  # (2)
    ...
```

1. See `Sequence[AuditEventTypeDef]`
2. See [:material-code-braces: PutAuditEventsResponseTypeDef](./type_defs.md#putauditeventsresponsetypedef)


```python
# put_audit_events method usage example with argument unpacking

kwargs: PutAuditEventsRequestTypeDef = {  # (1)
    "auditEvents": ...,
    "channelArn": ...,
}

parent.put_audit_events(**kwargs)
```

1. See [:material-code-braces: PutAuditEventsRequestTypeDef](./type_defs.md#putauditeventsrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("cloudtrail-data").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#CloudTrailDataService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("cloudtrail-data").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#CloudTrailDataService.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```





