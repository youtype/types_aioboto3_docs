# Examples

> [Index](../README.md) > [HealthImaging](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [HealthImaging](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#healthimaging)
    type annotations stubs module [types-aiobotocore-medical-imaging](https://pypi.org/project/types-aiobotocore-medical-imaging/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[medical-imaging]` package installed.

Write your `HealthImaging` code as usual,
type checking and code completion should work out of the box.



```python
# HealthImagingClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("medical-imaging") as client:  # (1)
    result = await client.copy_image_set()  # (2)
```

1. client: [HealthImagingClient](./client.md)
2. result: [:material-code-braces: CopyImageSetResponseTypeDef](./type_defs.md#copyimagesetresponsetypedef) 



```python
# ListDICOMImportJobsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("medical-imaging") as client:  # (1)
    paginator = client.get_paginator("list_dicom_import_jobs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [HealthImagingClient](./client.md)
2. paginator: [ListDICOMImportJobsPaginator](./paginators.md#listdicomimportjobspaginator)
3. item: [:material-code-braces: ListDICOMImportJobsResponseTypeDef](./type_defs.md#listdicomimportjobsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[medical-imaging]`
or a standalone `types_aiobotocore_medical_imaging` package, you have to explicitly specify
`client: HealthImagingClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# HealthImagingClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_medical_imaging.client import HealthImagingClient
from types_aiobotocore_medical_imaging.type_defs import CopyImageSetResponseTypeDef
from types_aiobotocore_medical_imaging.type_defs import CopyImageSetRequestRequestTypeDef


session = Session()

client: HealthImagingClient
async with session.client("medical-imaging") as client:  # (1)
    kwargs: CopyImageSetRequestRequestTypeDef = {...}  # (2)
    result: CopyImageSetResponseTypeDef = await client.copy_image_set(**kwargs)  # (3)
```

1. client: [HealthImagingClient](./client.md)
2. kwargs: [:material-code-braces: CopyImageSetRequestRequestTypeDef](./type_defs.md#copyimagesetrequestrequesttypedef) 
3. result: [:material-code-braces: CopyImageSetResponseTypeDef](./type_defs.md#copyimagesetresponsetypedef) 



```python
# ListDICOMImportJobsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_medical_imaging.client import HealthImagingClient
from types_aiobotocore_medical_imaging.paginator import ListDICOMImportJobsPaginator
from types_aiobotocore_medical_imaging.type_defs import ListDICOMImportJobsResponseTypeDef


session = Session()

client: HealthImagingClient
async with session.client("medical-imaging") as client:  # (1)
    paginator: ListDICOMImportJobsPaginator = client.get_paginator("list_dicom_import_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListDICOMImportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [HealthImagingClient](./client.md)
2. paginator: [ListDICOMImportJobsPaginator](./paginators.md#listdicomimportjobspaginator)
3. item: [:material-code-braces: ListDICOMImportJobsResponseTypeDef](./type_defs.md#listdicomimportjobsresponsetypedef) 



