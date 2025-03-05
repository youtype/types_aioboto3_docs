# Examples

> [Index](../README.md) > [OpenSearchIngestion](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [OpenSearchIngestion](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#opensearchingestion)
    type annotations stubs module [types-aiobotocore-osis](https://pypi.org/project/types-aiobotocore-osis/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[osis]` package installed.

Write your `OpenSearchIngestion` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# OpenSearchIngestionClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("osis") as client:  # (1)
    result = await client.create_pipeline()  # (2)
```

1. client: [OpenSearchIngestionClient](./client.md)
2. result: [:material-code-braces: CreatePipelineResponseTypeDef](./type_defs.md#createpipelineresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[osis]`
or a standalone `types_aiobotocore_osis` package, you have to explicitly specify
`client: OpenSearchIngestionClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# OpenSearchIngestionClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_osis.client import OpenSearchIngestionClient
from types_aiobotocore_osis.type_defs import CreatePipelineResponseTypeDef
from types_aiobotocore_osis.type_defs import CreatePipelineRequestTypeDef


session = Session()

client: OpenSearchIngestionClient
async with session.client("osis") as client:  # (1)
    kwargs: CreatePipelineRequestTypeDef = {...}  # (2)
    result: CreatePipelineResponseTypeDef = await client.create_pipeline(**kwargs)  # (3)
```

1. client: [OpenSearchIngestionClient](./client.md)
2. kwargs: [:material-code-braces: CreatePipelineRequestTypeDef](./type_defs.md#createpipelinerequesttypedef)
3. result: [:material-code-braces: CreatePipelineResponseTypeDef](./type_defs.md#createpipelineresponsetypedef)






