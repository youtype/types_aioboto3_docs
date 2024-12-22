# CostandUsageReportService module

> [Index](../README.md) > CostandUsageReportService


!!! note ""

    Auto-generated documentation for [CostandUsageReportService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#costandusagereportservice)
    type annotations stubs module [types-aiobotocore-cur](https://pypi.org/project/types-aiobotocore-cur/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `CostandUsageReportService` service.
1. Use provided commands to install generated packages.



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

```python
# CostandUsageReportServiceClient usage example

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

```python
# DescribeReportDefinitionsPaginator usage example

from types_aiobotocore_cur.paginator import DescribeReportDefinitionsPaginator

def get_describe_report_definitions_paginator() -> DescribeReportDefinitionsPaginator:
    return client.get_paginator("describe_report_definitions"))
```

- [DescribeReportDefinitionsPaginator](./paginators.md#describereportdefinitionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AWSRegionType usage example

from types_aiobotocore_cur.literals import AWSRegionType

def get_value() -> AWSRegionType:
    return "af-south-1"
```

- [AWSRegionType](./literals.md#awsregiontype)
- [AdditionalArtifactType](./literals.md#additionalartifacttype)
- [CompressionFormatType](./literals.md#compressionformattype)
- [DescribeReportDefinitionsPaginatorName](./literals.md#describereportdefinitionspaginatorname)
- [LastStatusType](./literals.md#laststatustype)
- [ReportFormatType](./literals.md#reportformattype)
- [ReportVersioningType](./literals.md#reportversioningtype)
- [SchemaElementType](./literals.md#schemaelementtype)
- [TimeUnitType](./literals.md#timeunittype)
- [CostandUsageReportServiceServiceName](./literals.md#costandusagereportserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [DeleteReportDefinitionRequestRequestTypeDef](./type_defs.md#deletereportdefinitionrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeReportDefinitionsRequestRequestTypeDef](./type_defs.md#describereportdefinitionsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ReportStatusTypeDef](./type_defs.md#reportstatustypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [DeleteReportDefinitionResponseTypeDef](./type_defs.md#deletereportdefinitionresponsetypedef)
- [DescribeReportDefinitionsRequestPaginateTypeDef](./type_defs.md#describereportdefinitionsrequestpaginatetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [ReportDefinitionOutputTypeDef](./type_defs.md#reportdefinitionoutputtypedef)
- [ReportDefinitionTypeDef](./type_defs.md#reportdefinitiontypedef)
- [DescribeReportDefinitionsResponseTypeDef](./type_defs.md#describereportdefinitionsresponsetypedef)
- [ModifyReportDefinitionRequestRequestTypeDef](./type_defs.md#modifyreportdefinitionrequestrequesttypedef)
- [PutReportDefinitionRequestRequestTypeDef](./type_defs.md#putreportdefinitionrequestrequesttypedef)

