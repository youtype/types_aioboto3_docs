# Examples

> [Index](../README.md) > [WAF](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WAF](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
    type annotations stubs module [types-aiobotocore-waf](https://pypi.org/project/types-aiobotocore-waf/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[waf]` package installed.

Write your `WAF` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("waf") as client:  # (1)
        result = await client.create_byte_match_set()  # (2)
    ```

    1. client: [WAFClient](./client.md)
    2. result: [:material-code-braces: CreateByteMatchSetResponseTypeDef](./type_defs.md#createbytematchsetresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("waf") as client:  # (1)
        paginator = client.get_paginator("get_rate_based_rule_managed_keys")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [WAFClient](./client.md)
    2. paginator: [GetRateBasedRuleManagedKeysPaginator](./paginators.md#getratebasedrulemanagedkeyspaginator)
    3. item: [:material-code-braces: GetRateBasedRuleManagedKeysResponseTypeDef](./type_defs.md#getratebasedrulemanagedkeysresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[waf]`
or a standalone `types_aiobotocore_waf` package, you have to explicitly specify
`client: WAFClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_waf.client import WAFClient
    from types_aiobotocore_waf.type_defs import CreateByteMatchSetResponseTypeDef
    from types_aiobotocore_waf.type_defs import CreateByteMatchSetRequestRequestTypeDef


    session = Session()

    client: WAFClient
    async with session.client("waf") as client:  # (1)
        kwargs: CreateByteMatchSetRequestRequestTypeDef = {...}  # (2)
        result: CreateByteMatchSetResponseTypeDef = await client.create_byte_match_set(**kwargs)  # (3)
    ```

    1. client: [WAFClient](./client.md)
    2. kwargs: [:material-code-braces: CreateByteMatchSetRequestRequestTypeDef](./type_defs.md#createbytematchsetrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateByteMatchSetResponseTypeDef](./type_defs.md#createbytematchsetresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_waf.client import WAFClient
    from types_aiobotocore_waf.paginator import GetRateBasedRuleManagedKeysPaginator
    from types_aiobotocore_waf.type_defs import GetRateBasedRuleManagedKeysResponseTypeDef


    session = Session()

    client: WAFClient
    async with session.client("waf") as client:  # (1)
        paginator: GetRateBasedRuleManagedKeysPaginator = client.get_paginator("get_rate_based_rule_managed_keys")  # (2)
        async for item in paginator.paginate(...):
            item: GetRateBasedRuleManagedKeysResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [WAFClient](./client.md)
    2. paginator: [GetRateBasedRuleManagedKeysPaginator](./paginators.md#getratebasedrulemanagedkeyspaginator)
    3. item: [:material-code-braces: GetRateBasedRuleManagedKeysResponseTypeDef](./type_defs.md#getratebasedrulemanagedkeysresponsetypedef) 




