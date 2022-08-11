# CostandUsageReportService module

> [Index](../README.md) > CostandUsageReportService


!!! note ""

    Auto-generated documentation for [CostandUsageReportService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
    type annotations stubs module [types-aiobotocore-cur](https://pypi.org/project/types-aiobotocore-cur/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `CostandUsageReportService` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[cur]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[cur]'


# standalone installation
python -m pip install types-aiobotocore-cur
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-cur
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CostandUsageReportServiceClient

Type annotations and code completion for  `#!python session.client("cur")` as [CostandUsageReportServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_cur.client import CostandUsageReportServiceClient


session = Session()
async with session.client("cur") as client:
    client: CostandUsageReportServiceClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("cur").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_cur.paginator import DescribeReportDefinitionsPaginator

def get_describe_report_definitions_paginator() -> DescribeReportDefinitionsPaginator:
    return client.get_paginator("describe_report_definitions"))
```

- [DescribeReportDefinitionsPaginator](./paginators.md#describereportdefinitionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_cur.literals import AWSRegionType

def get_value() -> AWSRegionType:
    return "af-south-1"
```

- [AWSRegionType](./literals.md#awsregiontype)
- [AdditionalArtifactType](./literals.md#additionalartifacttype)
- [CompressionFormatType](./literals.md#compressionformattype)
- [DescribeReportDefinitionsPaginatorName](./literals.md#describereportdefinitionspaginatorname)
- [ReportFormatType](./literals.md#reportformattype)
- [ReportVersioningType](./literals.md#reportversioningtype)
- [SchemaElementType](./literals.md#schemaelementtype)
- [TimeUnitType](./literals.md#timeunittype)
- [CostandUsageReportServiceServiceName](./literals.md#costandusagereportserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_cur.type_defs import DeleteReportDefinitionRequestRequestTypeDef

def get_value() -> DeleteReportDefinitionRequestRequestTypeDef:
    return {
        "ReportName": ...,
    }
```

- [DeleteReportDefinitionRequestRequestTypeDef](./type_defs.md#deletereportdefinitionrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeReportDefinitionsRequestRequestTypeDef](./type_defs.md#describereportdefinitionsrequestrequesttypedef)
- [ReportDefinitionTypeDef](./type_defs.md#reportdefinitiontypedef)
- [DeleteReportDefinitionResponseTypeDef](./type_defs.md#deletereportdefinitionresponsetypedef)
- [DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef](./type_defs.md#describereportdefinitionsrequestdescribereportdefinitionspaginatetypedef)
- [DescribeReportDefinitionsResponseTypeDef](./type_defs.md#describereportdefinitionsresponsetypedef)
- [ModifyReportDefinitionRequestRequestTypeDef](./type_defs.md#modifyreportdefinitionrequestrequesttypedef)
- [PutReportDefinitionRequestRequestTypeDef](./type_defs.md#putreportdefinitionrequestrequesttypedef)

