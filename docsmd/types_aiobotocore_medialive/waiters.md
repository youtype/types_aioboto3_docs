# Waiters

> [Index](../README.md) > [MediaLive](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [MediaLive](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#medialive)
    type annotations stubs module [types-aiobotocore-medialive](https://pypi.org/project/types-aiobotocore-medialive/).

## ChannelCreatedWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("channel_created")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/ChannelCreated.html#MediaLive.Waiter.ChannelCreated)

```python
# ChannelCreatedWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import ChannelCreatedWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: ChannelCreatedWaiter = client.get_waiter("channel_created")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [ChannelCreatedWaiter](./waiters.md#channelcreatedwaiter)


### wait

Type annotations and code completion for `#!python ChannelCreatedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    ChannelId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeChannelRequestWaitTypeDef = {  # (1)
    "ChannelId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeChannelRequestWaitTypeDef](./type_defs.md#describechannelrequestwaittypedef) 
## ChannelDeletedWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("channel_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/ChannelDeleted.html#MediaLive.Waiter.ChannelDeleted)

```python
# ChannelDeletedWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import ChannelDeletedWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: ChannelDeletedWaiter = client.get_waiter("channel_deleted")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [ChannelDeletedWaiter](./waiters.md#channeldeletedwaiter)


### wait

Type annotations and code completion for `#!python ChannelDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    ChannelId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeChannelRequestWaitTypeDef = {  # (1)
    "ChannelId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeChannelRequestWaitTypeDef](./type_defs.md#describechannelrequestwaittypedef) 
## ChannelPlacementGroupAssignedWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("channel_placement_group_assigned")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/ChannelPlacementGroupAssigned.html#MediaLive.Waiter.ChannelPlacementGroupAssigned)

```python
# ChannelPlacementGroupAssignedWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import ChannelPlacementGroupAssignedWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: ChannelPlacementGroupAssignedWaiter = client.get_waiter("channel_placement_group_assigned")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [ChannelPlacementGroupAssignedWaiter](./waiters.md#channelplacementgroupassignedwaiter)


### wait

Type annotations and code completion for `#!python ChannelPlacementGroupAssignedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    ChannelPlacementGroupId: str,
    ClusterId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeChannelPlacementGroupRequestWaitTypeDef = {  # (1)
    "ChannelPlacementGroupId": ...,
    "ClusterId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeChannelPlacementGroupRequestWaitTypeDef](./type_defs.md#describechannelplacementgrouprequestwaittypedef) 
## ChannelPlacementGroupDeletedWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("channel_placement_group_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/ChannelPlacementGroupDeleted.html#MediaLive.Waiter.ChannelPlacementGroupDeleted)

```python
# ChannelPlacementGroupDeletedWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import ChannelPlacementGroupDeletedWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: ChannelPlacementGroupDeletedWaiter = client.get_waiter("channel_placement_group_deleted")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [ChannelPlacementGroupDeletedWaiter](./waiters.md#channelplacementgroupdeletedwaiter)


### wait

Type annotations and code completion for `#!python ChannelPlacementGroupDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    ChannelPlacementGroupId: str,
    ClusterId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeChannelPlacementGroupRequestWaitTypeDef = {  # (1)
    "ChannelPlacementGroupId": ...,
    "ClusterId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeChannelPlacementGroupRequestWaitTypeDef](./type_defs.md#describechannelplacementgrouprequestwaittypedef) 
## ChannelPlacementGroupUnassignedWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("channel_placement_group_unassigned")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/ChannelPlacementGroupUnassigned.html#MediaLive.Waiter.ChannelPlacementGroupUnassigned)

```python
# ChannelPlacementGroupUnassignedWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import ChannelPlacementGroupUnassignedWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: ChannelPlacementGroupUnassignedWaiter = client.get_waiter("channel_placement_group_unassigned")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [ChannelPlacementGroupUnassignedWaiter](./waiters.md#channelplacementgroupunassignedwaiter)


### wait

Type annotations and code completion for `#!python ChannelPlacementGroupUnassignedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    ChannelPlacementGroupId: str,
    ClusterId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeChannelPlacementGroupRequestWaitTypeDef = {  # (1)
    "ChannelPlacementGroupId": ...,
    "ClusterId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeChannelPlacementGroupRequestWaitTypeDef](./type_defs.md#describechannelplacementgrouprequestwaittypedef) 
## ChannelRunningWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("channel_running")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/ChannelRunning.html#MediaLive.Waiter.ChannelRunning)

```python
# ChannelRunningWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import ChannelRunningWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: ChannelRunningWaiter = client.get_waiter("channel_running")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [ChannelRunningWaiter](./waiters.md#channelrunningwaiter)


### wait

Type annotations and code completion for `#!python ChannelRunningWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    ChannelId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeChannelRequestWaitTypeDef = {  # (1)
    "ChannelId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeChannelRequestWaitTypeDef](./type_defs.md#describechannelrequestwaittypedef) 
## ChannelStoppedWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("channel_stopped")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/ChannelStopped.html#MediaLive.Waiter.ChannelStopped)

```python
# ChannelStoppedWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import ChannelStoppedWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: ChannelStoppedWaiter = client.get_waiter("channel_stopped")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [ChannelStoppedWaiter](./waiters.md#channelstoppedwaiter)


### wait

Type annotations and code completion for `#!python ChannelStoppedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    ChannelId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeChannelRequestWaitTypeDef = {  # (1)
    "ChannelId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeChannelRequestWaitTypeDef](./type_defs.md#describechannelrequestwaittypedef) 
## ClusterCreatedWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("cluster_created")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/ClusterCreated.html#MediaLive.Waiter.ClusterCreated)

```python
# ClusterCreatedWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import ClusterCreatedWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: ClusterCreatedWaiter = client.get_waiter("cluster_created")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [ClusterCreatedWaiter](./waiters.md#clustercreatedwaiter)


### wait

Type annotations and code completion for `#!python ClusterCreatedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    ClusterId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeClusterRequestWaitTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeClusterRequestWaitTypeDef](./type_defs.md#describeclusterrequestwaittypedef) 
## ClusterDeletedWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("cluster_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/ClusterDeleted.html#MediaLive.Waiter.ClusterDeleted)

```python
# ClusterDeletedWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import ClusterDeletedWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: ClusterDeletedWaiter = client.get_waiter("cluster_deleted")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [ClusterDeletedWaiter](./waiters.md#clusterdeletedwaiter)


### wait

Type annotations and code completion for `#!python ClusterDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    ClusterId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeClusterRequestWaitTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeClusterRequestWaitTypeDef](./type_defs.md#describeclusterrequestwaittypedef) 
## InputAttachedWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("input_attached")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/InputAttached.html#MediaLive.Waiter.InputAttached)

```python
# InputAttachedWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import InputAttachedWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: InputAttachedWaiter = client.get_waiter("input_attached")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [InputAttachedWaiter](./waiters.md#inputattachedwaiter)


### wait

Type annotations and code completion for `#!python InputAttachedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    InputId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeInputRequestWaitTypeDef = {  # (1)
    "InputId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeInputRequestWaitTypeDef](./type_defs.md#describeinputrequestwaittypedef) 
## InputDeletedWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("input_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/InputDeleted.html#MediaLive.Waiter.InputDeleted)

```python
# InputDeletedWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import InputDeletedWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: InputDeletedWaiter = client.get_waiter("input_deleted")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [InputDeletedWaiter](./waiters.md#inputdeletedwaiter)


### wait

Type annotations and code completion for `#!python InputDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    InputId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeInputRequestWaitTypeDef = {  # (1)
    "InputId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeInputRequestWaitTypeDef](./type_defs.md#describeinputrequestwaittypedef) 
## InputDetachedWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("input_detached")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/InputDetached.html#MediaLive.Waiter.InputDetached)

```python
# InputDetachedWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import InputDetachedWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: InputDetachedWaiter = client.get_waiter("input_detached")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [InputDetachedWaiter](./waiters.md#inputdetachedwaiter)


### wait

Type annotations and code completion for `#!python InputDetachedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    InputId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeInputRequestWaitTypeDef = {  # (1)
    "InputId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeInputRequestWaitTypeDef](./type_defs.md#describeinputrequestwaittypedef) 
## MultiplexCreatedWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("multiplex_created")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/MultiplexCreated.html#MediaLive.Waiter.MultiplexCreated)

```python
# MultiplexCreatedWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import MultiplexCreatedWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: MultiplexCreatedWaiter = client.get_waiter("multiplex_created")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [MultiplexCreatedWaiter](./waiters.md#multiplexcreatedwaiter)


### wait

Type annotations and code completion for `#!python MultiplexCreatedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    MultiplexId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeMultiplexRequestWaitTypeDef = {  # (1)
    "MultiplexId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeMultiplexRequestWaitTypeDef](./type_defs.md#describemultiplexrequestwaittypedef) 
## MultiplexDeletedWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("multiplex_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/MultiplexDeleted.html#MediaLive.Waiter.MultiplexDeleted)

```python
# MultiplexDeletedWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import MultiplexDeletedWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: MultiplexDeletedWaiter = client.get_waiter("multiplex_deleted")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [MultiplexDeletedWaiter](./waiters.md#multiplexdeletedwaiter)


### wait

Type annotations and code completion for `#!python MultiplexDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    MultiplexId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeMultiplexRequestWaitTypeDef = {  # (1)
    "MultiplexId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeMultiplexRequestWaitTypeDef](./type_defs.md#describemultiplexrequestwaittypedef) 
## MultiplexRunningWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("multiplex_running")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/MultiplexRunning.html#MediaLive.Waiter.MultiplexRunning)

```python
# MultiplexRunningWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import MultiplexRunningWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: MultiplexRunningWaiter = client.get_waiter("multiplex_running")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [MultiplexRunningWaiter](./waiters.md#multiplexrunningwaiter)


### wait

Type annotations and code completion for `#!python MultiplexRunningWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    MultiplexId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeMultiplexRequestWaitTypeDef = {  # (1)
    "MultiplexId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeMultiplexRequestWaitTypeDef](./type_defs.md#describemultiplexrequestwaittypedef) 
## MultiplexStoppedWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("multiplex_stopped")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/MultiplexStopped.html#MediaLive.Waiter.MultiplexStopped)

```python
# MultiplexStoppedWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import MultiplexStoppedWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: MultiplexStoppedWaiter = client.get_waiter("multiplex_stopped")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [MultiplexStoppedWaiter](./waiters.md#multiplexstoppedwaiter)


### wait

Type annotations and code completion for `#!python MultiplexStoppedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    MultiplexId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeMultiplexRequestWaitTypeDef = {  # (1)
    "MultiplexId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeMultiplexRequestWaitTypeDef](./type_defs.md#describemultiplexrequestwaittypedef) 
## NodeDeregisteredWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("node_deregistered")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/NodeDeregistered.html#MediaLive.Waiter.NodeDeregistered)

```python
# NodeDeregisteredWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import NodeDeregisteredWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: NodeDeregisteredWaiter = client.get_waiter("node_deregistered")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [NodeDeregisteredWaiter](./waiters.md#nodederegisteredwaiter)


### wait

Type annotations and code completion for `#!python NodeDeregisteredWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    ClusterId: str,
    NodeId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeNodeRequestWaitTypeDef = {  # (1)
    "ClusterId": ...,
    "NodeId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeNodeRequestWaitTypeDef](./type_defs.md#describenoderequestwaittypedef) 
## NodeRegisteredWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("node_registered")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/NodeRegistered.html#MediaLive.Waiter.NodeRegistered)

```python
# NodeRegisteredWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import NodeRegisteredWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: NodeRegisteredWaiter = client.get_waiter("node_registered")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [NodeRegisteredWaiter](./waiters.md#noderegisteredwaiter)


### wait

Type annotations and code completion for `#!python NodeRegisteredWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    ClusterId: str,
    NodeId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeNodeRequestWaitTypeDef = {  # (1)
    "ClusterId": ...,
    "NodeId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeNodeRequestWaitTypeDef](./type_defs.md#describenoderequestwaittypedef) 
## SignalMapCreatedWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("signal_map_created")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/SignalMapCreated.html#MediaLive.Waiter.SignalMapCreated)

```python
# SignalMapCreatedWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import SignalMapCreatedWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: SignalMapCreatedWaiter = client.get_waiter("signal_map_created")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [SignalMapCreatedWaiter](./waiters.md#signalmapcreatedwaiter)


### wait

Type annotations and code completion for `#!python SignalMapCreatedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Identifier: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetSignalMapRequestWaitTypeDef = {  # (1)
    "Identifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetSignalMapRequestWaitTypeDef](./type_defs.md#getsignalmaprequestwaittypedef) 
## SignalMapMonitorDeletedWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("signal_map_monitor_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/SignalMapMonitorDeleted.html#MediaLive.Waiter.SignalMapMonitorDeleted)

```python
# SignalMapMonitorDeletedWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import SignalMapMonitorDeletedWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: SignalMapMonitorDeletedWaiter = client.get_waiter("signal_map_monitor_deleted")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [SignalMapMonitorDeletedWaiter](./waiters.md#signalmapmonitordeletedwaiter)


### wait

Type annotations and code completion for `#!python SignalMapMonitorDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Identifier: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetSignalMapRequestWaitTypeDef = {  # (1)
    "Identifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetSignalMapRequestWaitTypeDef](./type_defs.md#getsignalmaprequestwaittypedef) 
## SignalMapMonitorDeployedWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("signal_map_monitor_deployed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/SignalMapMonitorDeployed.html#MediaLive.Waiter.SignalMapMonitorDeployed)

```python
# SignalMapMonitorDeployedWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import SignalMapMonitorDeployedWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: SignalMapMonitorDeployedWaiter = client.get_waiter("signal_map_monitor_deployed")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [SignalMapMonitorDeployedWaiter](./waiters.md#signalmapmonitordeployedwaiter)


### wait

Type annotations and code completion for `#!python SignalMapMonitorDeployedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Identifier: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetSignalMapRequestWaitTypeDef = {  # (1)
    "Identifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetSignalMapRequestWaitTypeDef](./type_defs.md#getsignalmaprequestwaittypedef) 
## SignalMapUpdatedWaiter

Type annotations and code completion for `#!python session.client("medialive").get_waiter("signal_map_updated")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/waiter/SignalMapUpdated.html#MediaLive.Waiter.SignalMapUpdated)

```python
# SignalMapUpdatedWaiter usage example

from aioboto3.session import Session

from types_aiobotocore_medialive.waiter import SignalMapUpdatedWaiter

session = get_session()
async with session.client("medialive") as client:  # (1)
    waiter: SignalMapUpdatedWaiter = client.get_waiter("signal_map_updated")  # (2)
    await waiter.wait()
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [SignalMapUpdatedWaiter](./waiters.md#signalmapupdatedwaiter)


### wait

Type annotations and code completion for `#!python SignalMapUpdatedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    Identifier: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetSignalMapRequestWaitTypeDef = {  # (1)
    "Identifier": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetSignalMapRequestWaitTypeDef](./type_defs.md#getsignalmaprequestwaittypedef) 