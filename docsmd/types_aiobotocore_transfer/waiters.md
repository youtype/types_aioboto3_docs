# Waiters

> [Index](../README.md) > [Transfer](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [Transfer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
    type annotations stubs module [types-aiobotocore-transfer](https://pypi.org/project/types-aiobotocore-transfer/).

## ServerOfflineWaiter

Type annotations and code completion for `#!python session.client("transfer").get_waiter("server_offline")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Waiter.ServerOffline)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_transfer.waiter import ServerOfflineWaiter

session = get_session()
async with session.client("transfer") as client:  # (1)
    waiter: ServerOfflineWaiter = client.get_waiter("server_offline")  # (2)
    await waiter.wait()
```

1. client: [TransferClient](./client.md)
2. waiter: [ServerOfflineWaiter](./waiters.md#serverofflinewaiter)


### wait

Type annotations and code completion for `#!python ServerOfflineWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    ServerId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeServerRequestServerOfflineWaitTypeDef = {  # (1)
    "ServerId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeServerRequestServerOfflineWaitTypeDef](./type_defs.md#describeserverrequestserverofflinewaittypedef) 
## ServerOnlineWaiter

Type annotations and code completion for `#!python session.client("transfer").get_waiter("server_online")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Waiter.ServerOnline)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_transfer.waiter import ServerOnlineWaiter

session = get_session()
async with session.client("transfer") as client:  # (1)
    waiter: ServerOnlineWaiter = client.get_waiter("server_online")  # (2)
    await waiter.wait()
```

1. client: [TransferClient](./client.md)
2. waiter: [ServerOnlineWaiter](./waiters.md#serveronlinewaiter)


### wait

Type annotations and code completion for `#!python ServerOnlineWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    ServerId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeServerRequestServerOnlineWaitTypeDef = {  # (1)
    "ServerId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeServerRequestServerOnlineWaitTypeDef](./type_defs.md#describeserverrequestserveronlinewaittypedef) 
