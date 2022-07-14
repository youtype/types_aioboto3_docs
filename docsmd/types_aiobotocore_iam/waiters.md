# Waiters

> [Index](../README.md) > [IAM](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [IAM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
    type annotations stubs module [types-aiobotocore-iam](https://pypi.org/project/types-aiobotocore-iam/).

## InstanceProfileExistsWaiter

Type annotations and code completion for `#!python session.client("iam").get_waiter("instance_profile_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Waiter.InstanceProfileExists)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.waiter import InstanceProfileExistsWaiter

session = get_session()
async with session.client("iam") as client:  # (1)
    waiter: InstanceProfileExistsWaiter = client.get_waiter("instance_profile_exists")  # (2)
    await waiter.wait()
```

1. client: [IAMClient](./client.md)
2. waiter: [InstanceProfileExistsWaiter](./waiters.md#instanceprofileexistswaiter)


### wait

Type annotations and code completion for `#!python InstanceProfileExistsWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    InstanceProfileName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef = {  # (1)
    "InstanceProfileName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef](./type_defs.md#getinstanceprofilerequestinstanceprofileexistswaittypedef) 
## PolicyExistsWaiter

Type annotations and code completion for `#!python session.client("iam").get_waiter("policy_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Waiter.PolicyExists)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.waiter import PolicyExistsWaiter

session = get_session()
async with session.client("iam") as client:  # (1)
    waiter: PolicyExistsWaiter = client.get_waiter("policy_exists")  # (2)
    await waiter.wait()
```

1. client: [IAMClient](./client.md)
2. waiter: [PolicyExistsWaiter](./waiters.md#policyexistswaiter)


### wait

Type annotations and code completion for `#!python PolicyExistsWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    PolicyArn: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: GetPolicyRequestPolicyExistsWaitTypeDef = {  # (1)
    "PolicyArn": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetPolicyRequestPolicyExistsWaitTypeDef](./type_defs.md#getpolicyrequestpolicyexistswaittypedef) 
## RoleExistsWaiter

Type annotations and code completion for `#!python session.client("iam").get_waiter("role_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Waiter.RoleExists)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.waiter import RoleExistsWaiter

session = get_session()
async with session.client("iam") as client:  # (1)
    waiter: RoleExistsWaiter = client.get_waiter("role_exists")  # (2)
    await waiter.wait()
```

1. client: [IAMClient](./client.md)
2. waiter: [RoleExistsWaiter](./waiters.md#roleexistswaiter)


### wait

Type annotations and code completion for `#!python RoleExistsWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    RoleName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: GetRoleRequestRoleExistsWaitTypeDef = {  # (1)
    "RoleName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetRoleRequestRoleExistsWaitTypeDef](./type_defs.md#getrolerequestroleexistswaittypedef) 
## UserExistsWaiter

Type annotations and code completion for `#!python session.client("iam").get_waiter("user_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Waiter.UserExists)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iam.waiter import UserExistsWaiter

session = get_session()
async with session.client("iam") as client:  # (1)
    waiter: UserExistsWaiter = client.get_waiter("user_exists")  # (2)
    await waiter.wait()
```

1. client: [IAMClient](./client.md)
2. waiter: [UserExistsWaiter](./waiters.md#userexistswaiter)


### wait

Type annotations and code completion for `#!python UserExistsWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    UserName: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: GetUserRequestUserExistsWaitTypeDef = {  # (1)
    "UserName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetUserRequestUserExistsWaitTypeDef](./type_defs.md#getuserrequestuserexistswaittypedef) 
