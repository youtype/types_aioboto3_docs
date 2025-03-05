# Examples

> [Index](../README.md) > [PI](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#pi)
    type annotations stubs module [types-aiobotocore-pi](https://pypi.org/project/types-aiobotocore-pi/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[pi]` package installed.

Write your `PI` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# PIClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("pi") as client:  # (1)
    result = await client.create_performance_analysis_report()  # (2)
```

1. client: [PIClient](./client.md)
2. result: [:material-code-braces: CreatePerformanceAnalysisReportResponseTypeDef](./type_defs.md#createperformanceanalysisreportresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[pi]`
or a standalone `types_aiobotocore_pi` package, you have to explicitly specify
`client: PIClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# PIClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_pi.client import PIClient
from types_aiobotocore_pi.type_defs import CreatePerformanceAnalysisReportResponseTypeDef
from types_aiobotocore_pi.type_defs import CreatePerformanceAnalysisReportRequestTypeDef


session = Session()

client: PIClient
async with session.client("pi") as client:  # (1)
    kwargs: CreatePerformanceAnalysisReportRequestTypeDef = {...}  # (2)
    result: CreatePerformanceAnalysisReportResponseTypeDef = await client.create_performance_analysis_report(**kwargs)  # (3)
```

1. client: [PIClient](./client.md)
2. kwargs: [:material-code-braces: CreatePerformanceAnalysisReportRequestTypeDef](./type_defs.md#createperformanceanalysisreportrequesttypedef)
3. result: [:material-code-braces: CreatePerformanceAnalysisReportResponseTypeDef](./type_defs.md#createperformanceanalysisreportresponsetypedef)






