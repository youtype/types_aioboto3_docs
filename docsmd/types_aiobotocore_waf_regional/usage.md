# Examples

> [Index](../README.md) > [WAFRegional](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WAFRegional](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#wafregional)
    type annotations stubs module [types-aiobotocore-waf-regional](https://pypi.org/project/types-aiobotocore-waf-regional/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[waf-regional]` package installed.

Write your `WAFRegional` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# WAFRegionalClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("waf-regional") as client:  # (1)
    result = await client.create_byte_match_set()  # (2)
```

1. client: [WAFRegionalClient](./client.md)
2. result: [:material-code-braces: CreateByteMatchSetResponseTypeDef](./type_defs.md#createbytematchsetresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[waf-regional]`
or a standalone `types_aiobotocore_waf_regional` package, you have to explicitly specify
`client: WAFRegionalClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# WAFRegionalClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_waf_regional.client import WAFRegionalClient
from types_aiobotocore_waf_regional.type_defs import CreateByteMatchSetResponseTypeDef
from types_aiobotocore_waf_regional.type_defs import CreateByteMatchSetRequestTypeDef


session = Session()

client: WAFRegionalClient
async with session.client("waf-regional") as client:  # (1)
    kwargs: CreateByteMatchSetRequestTypeDef = {...}  # (2)
    result: CreateByteMatchSetResponseTypeDef = await client.create_byte_match_set(**kwargs)  # (3)
```

1. client: [WAFRegionalClient](./client.md)
2. kwargs: [:material-code-braces: CreateByteMatchSetRequestTypeDef](./type_defs.md#createbytematchsetrequesttypedef)
3. result: [:material-code-braces: CreateByteMatchSetResponseTypeDef](./type_defs.md#createbytematchsetresponsetypedef)






