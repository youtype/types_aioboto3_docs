# Examples

> [Index](../README.md) > [SageMakergeospatialcapabilities](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SageMakergeospatialcapabilities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#sagemakergeospatialcapabilities)
    type annotations stubs module [types-aiobotocore-sagemaker-geospatial](https://pypi.org/project/types-aiobotocore-sagemaker-geospatial/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[sagemaker-geospatial]` package installed.

Write your `SageMakergeospatialcapabilities` code as usual,
type checking and code completion should work out of the box.



```python
# SageMakergeospatialcapabilitiesClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("sagemaker-geospatial") as client:  # (1)
    result = await client.export_earth_observation_job()  # (2)
```

1. client: [SageMakergeospatialcapabilitiesClient](./client.md)
2. result: [:material-code-braces: ExportEarthObservationJobOutputTypeDef](./type_defs.md#exportearthobservationjoboutputtypedef) 



```python
# ListEarthObservationJobsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("sagemaker-geospatial") as client:  # (1)
    paginator = client.get_paginator("list_earth_observation_jobs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SageMakergeospatialcapabilitiesClient](./client.md)
2. paginator: [ListEarthObservationJobsPaginator](./paginators.md#listearthobservationjobspaginator)
3. item: [:material-code-braces: ListEarthObservationJobOutputTypeDef](./type_defs.md#listearthobservationjoboutputtypedef) 




### Explicit type annotations

With `types-aioboto3-lite[sagemaker-geospatial]`
or a standalone `types_aiobotocore_sagemaker_geospatial` package, you have to explicitly specify
`client: SageMakergeospatialcapabilitiesClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SageMakergeospatialcapabilitiesClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_sagemaker_geospatial.client import SageMakergeospatialcapabilitiesClient
from types_aiobotocore_sagemaker_geospatial.type_defs import ExportEarthObservationJobOutputTypeDef
from types_aiobotocore_sagemaker_geospatial.type_defs import ExportEarthObservationJobInputRequestTypeDef


session = Session()

client: SageMakergeospatialcapabilitiesClient
async with session.client("sagemaker-geospatial") as client:  # (1)
    kwargs: ExportEarthObservationJobInputRequestTypeDef = {...}  # (2)
    result: ExportEarthObservationJobOutputTypeDef = await client.export_earth_observation_job(**kwargs)  # (3)
```

1. client: [SageMakergeospatialcapabilitiesClient](./client.md)
2. kwargs: [:material-code-braces: ExportEarthObservationJobInputRequestTypeDef](./type_defs.md#exportearthobservationjobinputrequesttypedef) 
3. result: [:material-code-braces: ExportEarthObservationJobOutputTypeDef](./type_defs.md#exportearthobservationjoboutputtypedef) 



```python
# ListEarthObservationJobsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_sagemaker_geospatial.client import SageMakergeospatialcapabilitiesClient
from types_aiobotocore_sagemaker_geospatial.paginator import ListEarthObservationJobsPaginator
from types_aiobotocore_sagemaker_geospatial.type_defs import ListEarthObservationJobOutputTypeDef


session = Session()

client: SageMakergeospatialcapabilitiesClient
async with session.client("sagemaker-geospatial") as client:  # (1)
    paginator: ListEarthObservationJobsPaginator = client.get_paginator("list_earth_observation_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListEarthObservationJobOutputTypeDef
        print(item)  # (3)
```

1. client: [SageMakergeospatialcapabilitiesClient](./client.md)
2. paginator: [ListEarthObservationJobsPaginator](./paginators.md#listearthobservationjobspaginator)
3. item: [:material-code-braces: ListEarthObservationJobOutputTypeDef](./type_defs.md#listearthobservationjoboutputtypedef) 



