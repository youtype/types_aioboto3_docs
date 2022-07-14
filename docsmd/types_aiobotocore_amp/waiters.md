# Waiters

> [Index](../README.md) > [PrometheusService](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [PrometheusService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
    type annotations stubs module [types-aiobotocore-amp](https://pypi.org/project/types-aiobotocore-amp/).

## WorkspaceActiveWaiter

Type annotations and code completion for `#!python session.client("amp").get_waiter("workspace_active")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Waiter.WorkspaceActive)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_amp.waiter import WorkspaceActiveWaiter

session = get_session()
async with session.client("amp") as client:  # (1)
    waiter: WorkspaceActiveWaiter = client.get_waiter("workspace_active")  # (2)
    await waiter.wait()
```

1. client: [PrometheusServiceClient](./client.md)
2. waiter: [WorkspaceActiveWaiter](./waiters.md#workspaceactivewaiter)


### wait

Type annotations and code completion for `#!python WorkspaceActiveWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    workspaceId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeWorkspaceRequestWorkspaceActiveWaitTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceRequestWorkspaceActiveWaitTypeDef](./type_defs.md#describeworkspacerequestworkspaceactivewaittypedef) 
## WorkspaceDeletedWaiter

Type annotations and code completion for `#!python session.client("amp").get_waiter("workspace_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Waiter.WorkspaceDeleted)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_amp.waiter import WorkspaceDeletedWaiter

session = get_session()
async with session.client("amp") as client:  # (1)
    waiter: WorkspaceDeletedWaiter = client.get_waiter("workspace_deleted")  # (2)
    await waiter.wait()
```

1. client: [PrometheusServiceClient](./client.md)
2. waiter: [WorkspaceDeletedWaiter](./waiters.md#workspacedeletedwaiter)


### wait

Type annotations and code completion for `#!python WorkspaceDeletedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    workspaceId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeWorkspaceRequestWorkspaceDeletedWaitTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceRequestWorkspaceDeletedWaitTypeDef](./type_defs.md#describeworkspacerequestworkspacedeletedwaittypedef) 
