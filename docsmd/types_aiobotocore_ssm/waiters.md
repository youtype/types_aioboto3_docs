# Waiters

> [Index](../README.md) > [SSM](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [SSM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
    type annotations stubs module [types-aiobotocore-ssm](https://pypi.org/project/types-aiobotocore-ssm/).

## CommandExecutedWaiter

Type annotations and code completion for `#!python session.client("ssm").get_waiter("command_executed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Waiter.CommandExecuted)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_ssm.waiter import CommandExecutedWaiter

session = get_session()
async with session.client("ssm") as client:  # (1)
    waiter: CommandExecutedWaiter = client.get_waiter("command_executed")  # (2)
    await waiter.wait()
```

1. client: [SSMClient](./client.md)
2. waiter: [CommandExecutedWaiter](./waiters.md#commandexecutedwaiter)


### wait

Type annotations and code completion for `#!python CommandExecutedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    CommandId: str,
    InstanceId: str,
    PluginName: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: GetCommandInvocationRequestCommandExecutedWaitTypeDef = {  # (1)
    "CommandId": ...,
    "InstanceId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetCommandInvocationRequestCommandExecutedWaitTypeDef](./type_defs.md#getcommandinvocationrequestcommandexecutedwaittypedef) 
