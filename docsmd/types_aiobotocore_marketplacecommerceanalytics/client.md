# MarketplaceCommerceAnalyticsClient

> [Index](../README.md) > [MarketplaceCommerceAnalytics](./README.md) > MarketplaceCommerceAnalyticsClient

!!! note ""

    Auto-generated documentation for [MarketplaceCommerceAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#marketplacecommerceanalytics)
    type annotations stubs module [types-aiobotocore-marketplacecommerceanalytics](https://pypi.org/project/types-aiobotocore-marketplacecommerceanalytics/).

## MarketplaceCommerceAnalyticsClient

Type annotations and code completion for `#!python session.client("marketplacecommerceanalytics")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics.Client)

```python
# MarketplaceCommerceAnalyticsClient usage example

from aioboto3.session import Session
from types_aiobotocore_marketplacecommerceanalytics.client import MarketplaceCommerceAnalyticsClient

session = Session()
async with session.client("marketplacecommerceanalytics") as client:
    client: MarketplaceCommerceAnalyticsClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("marketplacecommerceanalytics").exceptions` structure.

```python
# MarketplaceCommerceAnalyticsClient.exceptions usage example

async with session.client("marketplacecommerceanalytics") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.MarketplaceCommerceAnalyticsException,
    ) as e:
        print(e)
```

```python
# MarketplaceCommerceAnalyticsClient.exceptions type checking example

from types_aiobotocore_marketplacecommerceanalytics.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("marketplacecommerceanalytics").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("marketplacecommerceanalytics").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics.Client)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### generate\_data\_set

Given a data set type and data set publication date, asynchronously publishes
the requested data set to the specified S3 bucket and notifies the specified
SNS topic once the data is available.

Type annotations and code completion for `#!python session.client("marketplacecommerceanalytics").generate_data_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics.Client)

```python
# generate_data_set method definition

await def generate_data_set(
    self,
    *,
    dataSetType: DataSetTypeType,  # (1)
    dataSetPublicationDate: TimestampTypeDef,
    roleNameArn: str,
    destinationS3BucketName: str,
    snsTopicArn: str,
    destinationS3Prefix: str = ...,
    customerDefinedValues: Mapping[str, str] = ...,
) -> GenerateDataSetResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DataSetTypeType](./literals.md#datasettypetype) 
2. See [:material-code-braces: GenerateDataSetResultTypeDef](./type_defs.md#generatedatasetresulttypedef) 


```python
# generate_data_set method usage example with argument unpacking

kwargs: GenerateDataSetRequestRequestTypeDef = {  # (1)
    "dataSetType": ...,
    "dataSetPublicationDate": ...,
    "roleNameArn": ...,
    "destinationS3BucketName": ...,
    "snsTopicArn": ...,
}

parent.generate_data_set(**kwargs)
```

1. See [:material-code-braces: GenerateDataSetRequestRequestTypeDef](./type_defs.md#generatedatasetrequestrequesttypedef) 

### start\_support\_data\_export

<i>This target has been deprecated.</i> Given a data set type and a from date,
asynchronously publishes the requested customer support data to the specified
S3 bucket and notifies the specified SNS topic once the data is available.

Type annotations and code completion for `#!python session.client("marketplacecommerceanalytics").start_support_data_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics.Client)

```python
# start_support_data_export method definition

await def start_support_data_export(
    self,
    *,
    dataSetType: SupportDataSetTypeType,  # (1)
    fromDate: TimestampTypeDef,
    roleNameArn: str,
    destinationS3BucketName: str,
    snsTopicArn: str,
    destinationS3Prefix: str = ...,
    customerDefinedValues: Mapping[str, str] = ...,
) -> StartSupportDataExportResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SupportDataSetTypeType](./literals.md#supportdatasettypetype) 
2. See [:material-code-braces: StartSupportDataExportResultTypeDef](./type_defs.md#startsupportdataexportresulttypedef) 


```python
# start_support_data_export method usage example with argument unpacking

kwargs: StartSupportDataExportRequestRequestTypeDef = {  # (1)
    "dataSetType": ...,
    "fromDate": ...,
    "roleNameArn": ...,
    "destinationS3BucketName": ...,
    "snsTopicArn": ...,
}

parent.start_support_data_export(**kwargs)
```

1. See [:material-code-braces: StartSupportDataExportRequestRequestTypeDef](./type_defs.md#startsupportdataexportrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("marketplacecommerceanalytics").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("marketplacecommerceanalytics").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#MarketplaceCommerceAnalytics.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




