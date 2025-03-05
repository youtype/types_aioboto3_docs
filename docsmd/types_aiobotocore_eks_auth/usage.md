# Examples

> [Index](../README.md) > [EKSAuth](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EKSAuth](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks-auth.html#eksauth)
    type annotations stubs module [types-aiobotocore-eks-auth](https://pypi.org/project/types-aiobotocore-eks-auth/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[eks-auth]` package installed.

Write your `EKSAuth` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# EKSAuthClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("eks-auth") as client:  # (1)
    result = await client.assume_role_for_pod_identity()  # (2)
```

1. client: [EKSAuthClient](./client.md)
2. result: [:material-code-braces: AssumeRoleForPodIdentityResponseTypeDef](./type_defs.md#assumeroleforpodidentityresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[eks-auth]`
or a standalone `types_aiobotocore_eks_auth` package, you have to explicitly specify
`client: EKSAuthClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# EKSAuthClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_eks_auth.client import EKSAuthClient
from types_aiobotocore_eks_auth.type_defs import AssumeRoleForPodIdentityResponseTypeDef
from types_aiobotocore_eks_auth.type_defs import AssumeRoleForPodIdentityRequestTypeDef


session = Session()

client: EKSAuthClient
async with session.client("eks-auth") as client:  # (1)
    kwargs: AssumeRoleForPodIdentityRequestTypeDef = {...}  # (2)
    result: AssumeRoleForPodIdentityResponseTypeDef = await client.assume_role_for_pod_identity(**kwargs)  # (3)
```

1. client: [EKSAuthClient](./client.md)
2. kwargs: [:material-code-braces: AssumeRoleForPodIdentityRequestTypeDef](./type_defs.md#assumeroleforpodidentityrequesttypedef)
3. result: [:material-code-braces: AssumeRoleForPodIdentityResponseTypeDef](./type_defs.md#assumeroleforpodidentityresponsetypedef)






