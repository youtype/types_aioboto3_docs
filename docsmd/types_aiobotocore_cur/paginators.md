# Paginators

> [Index](../README.md) > [CostandUsageReportService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CostandUsageReportService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
    type annotations stubs module [types-aiobotocore-cur](https://pypi.org/project/types-aiobotocore-cur/).

## DescribeReportDefinitionsPaginator

Type annotations and code completion for `#!python session.client("cur").get_paginator("describe_report_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Paginator.DescribeReportDefinitions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_cur.paginator import DescribeReportDefinitionsPaginator

session = Session()

session = get_session()
async with session.client("cur") as client:  # (1)
    paginator: DescribeReportDefinitionsPaginator = client.get_paginator("describe_report_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeReportDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [CostandUsageReportServiceClient](./client.md)
2. paginator: [DescribeReportDefinitionsPaginator](./paginators.md#describereportdefinitionspaginator)
3. item: [:material-code-braces: DescribeReportDefinitionsResponseTypeDef](./type_defs.md#describereportdefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReportDefinitionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeReportDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeReportDefinitionsResponseTypeDef](./type_defs.md#describereportdefinitionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef](./type_defs.md#describereportdefinitionsrequestdescribereportdefinitionspaginatetypedef) 
