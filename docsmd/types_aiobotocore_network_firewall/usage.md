# Examples

> [Index](../README.md) > [NetworkFirewall](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [NetworkFirewall](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
    type annotations stubs module [types-aiobotocore-network-firewall](https://pypi.org/project/types-aiobotocore-network-firewall/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[network-firewall]` package installed.

Write your `NetworkFirewall` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("network-firewall") as client:  # (1)
        result = await client.associate_firewall_policy()  # (2)
    ```

    1. client: [NetworkFirewallClient](./client.md)
    2. result: [:material-code-braces: AssociateFirewallPolicyResponseTypeDef](./type_defs.md#associatefirewallpolicyresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("network-firewall") as client:  # (1)
        paginator = client.get_paginator("list_firewall_policies")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [NetworkFirewallClient](./client.md)
    2. paginator: [ListFirewallPoliciesPaginator](./paginators.md#listfirewallpoliciespaginator)
    3. item: [:material-code-braces: ListFirewallPoliciesResponseTypeDef](./type_defs.md#listfirewallpoliciesresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[network-firewall]`
or a standalone `types_aiobotocore_network_firewall` package, you have to explicitly specify
`client: NetworkFirewallClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_network_firewall.client import NetworkFirewallClient
    from types_aiobotocore_network_firewall.type_defs import AssociateFirewallPolicyResponseTypeDef
    from types_aiobotocore_network_firewall.type_defs import AssociateFirewallPolicyRequestRequestTypeDef


    session = Session()

    client: NetworkFirewallClient
    async with session.client("network-firewall") as client:  # (1)
        kwargs: AssociateFirewallPolicyRequestRequestTypeDef = {...}  # (2)
        result: AssociateFirewallPolicyResponseTypeDef = await client.associate_firewall_policy(**kwargs)  # (3)
    ```

    1. client: [NetworkFirewallClient](./client.md)
    2. kwargs: [:material-code-braces: AssociateFirewallPolicyRequestRequestTypeDef](./type_defs.md#associatefirewallpolicyrequestrequesttypedef) 
    3. result: [:material-code-braces: AssociateFirewallPolicyResponseTypeDef](./type_defs.md#associatefirewallpolicyresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_network_firewall.client import NetworkFirewallClient
    from types_aiobotocore_network_firewall.paginator import ListFirewallPoliciesPaginator
    from types_aiobotocore_network_firewall.type_defs import ListFirewallPoliciesResponseTypeDef


    session = Session()

    client: NetworkFirewallClient
    async with session.client("network-firewall") as client:  # (1)
        paginator: ListFirewallPoliciesPaginator = client.get_paginator("list_firewall_policies")  # (2)
        async for item in paginator.paginate(...):
            item: ListFirewallPoliciesResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [NetworkFirewallClient](./client.md)
    2. paginator: [ListFirewallPoliciesPaginator](./paginators.md#listfirewallpoliciespaginator)
    3. item: [:material-code-braces: ListFirewallPoliciesResponseTypeDef](./type_defs.md#listfirewallpoliciesresponsetypedef) 




