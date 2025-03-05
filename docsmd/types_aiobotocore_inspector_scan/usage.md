# Examples

> [Index](../README.md) > [Inspectorscan](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Inspectorscan](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan.html#inspectorscan)
    type annotations stubs module [types-aiobotocore-inspector-scan](https://pypi.org/project/types-aiobotocore-inspector-scan/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[inspector-scan]` package installed.

Write your `Inspectorscan` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# InspectorscanClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("inspector-scan") as client:  # (1)
    result = await client.scan_sbom()  # (2)
```

1. client: [InspectorscanClient](./client.md)
2. result: [:material-code-braces: ScanSbomResponseTypeDef](./type_defs.md#scansbomresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[inspector-scan]`
or a standalone `types_aiobotocore_inspector_scan` package, you have to explicitly specify
`client: InspectorscanClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# InspectorscanClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_inspector_scan.client import InspectorscanClient
from types_aiobotocore_inspector_scan.type_defs import ScanSbomResponseTypeDef
from types_aiobotocore_inspector_scan.type_defs import ScanSbomRequestTypeDef


session = Session()

client: InspectorscanClient
async with session.client("inspector-scan") as client:  # (1)
    kwargs: ScanSbomRequestTypeDef = {...}  # (2)
    result: ScanSbomResponseTypeDef = await client.scan_sbom(**kwargs)  # (3)
```

1. client: [InspectorscanClient](./client.md)
2. kwargs: [:material-code-braces: ScanSbomRequestTypeDef](./type_defs.md#scansbomrequesttypedef)
3. result: [:material-code-braces: ScanSbomResponseTypeDef](./type_defs.md#scansbomresponsetypedef)






