# TextractClient

> [Index](../README.md) > [Textract](./README.md) > TextractClient

!!! note ""

    Auto-generated documentation for [Textract](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#textract)
    type annotations stubs module [types-aiobotocore-textract](https://pypi.org/project/types-aiobotocore-textract/).

## TextractClient

Type annotations and code completion for `#!python session.client("textract")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# TextractClient usage example

from aioboto3.session import Session
from types_aiobotocore_textract.client import TextractClient

session = Session()
async with session.client("textract") as client:
    client: TextractClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("textract").exceptions` structure.

```python
# TextractClient.exceptions usage example

async with session.client("textract") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.BadDocumentException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.DocumentTooLargeException,
        client.exceptions.HumanLoopQuotaExceededException,
        client.exceptions.IdempotentParameterMismatchException,
        client.exceptions.InternalServerError,
        client.exceptions.InvalidJobIdException,
        client.exceptions.InvalidKMSKeyException,
        client.exceptions.InvalidParameterException,
        client.exceptions.InvalidS3ObjectException,
        client.exceptions.LimitExceededException,
        client.exceptions.ProvisionedThroughputExceededException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.UnsupportedDocumentException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# TextractClient.exceptions type checking example

from types_aiobotocore_textract.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("textract").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("textract").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

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


### analyze\_document

Analyzes an input document for relationships between detected items.

Type annotations and code completion for `#!python session.client("textract").analyze_document` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# analyze_document method definition

await def analyze_document(
    self,
    *,
    Document: DocumentTypeDef,  # (1)
    FeatureTypes: Sequence[FeatureTypeType],  # (2)
    HumanLoopConfig: HumanLoopConfigTypeDef = ...,  # (3)
    QueriesConfig: QueriesConfigTypeDef = ...,  # (4)
    AdaptersConfig: AdaptersConfigTypeDef = ...,  # (5)
) -> AnalyzeDocumentResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
2. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
3. See [:material-code-braces: HumanLoopConfigTypeDef](./type_defs.md#humanloopconfigtypedef) 
4. See [:material-code-braces: QueriesConfigTypeDef](./type_defs.md#queriesconfigtypedef) 
5. See [:material-code-braces: AdaptersConfigTypeDef](./type_defs.md#adaptersconfigtypedef) 
6. See [:material-code-braces: AnalyzeDocumentResponseTypeDef](./type_defs.md#analyzedocumentresponsetypedef) 


```python
# analyze_document method usage example with argument unpacking

kwargs: AnalyzeDocumentRequestRequestTypeDef = {  # (1)
    "Document": ...,
    "FeatureTypes": ...,
}

parent.analyze_document(**kwargs)
```

1. See [:material-code-braces: AnalyzeDocumentRequestRequestTypeDef](./type_defs.md#analyzedocumentrequestrequesttypedef) 

### analyze\_expense

<code>AnalyzeExpense</code> synchronously analyzes an input document for
financially related relationships between text.

Type annotations and code completion for `#!python session.client("textract").analyze_expense` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# analyze_expense method definition

await def analyze_expense(
    self,
    *,
    Document: DocumentTypeDef,  # (1)
) -> AnalyzeExpenseResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
2. See [:material-code-braces: AnalyzeExpenseResponseTypeDef](./type_defs.md#analyzeexpenseresponsetypedef) 


```python
# analyze_expense method usage example with argument unpacking

kwargs: AnalyzeExpenseRequestRequestTypeDef = {  # (1)
    "Document": ...,
}

parent.analyze_expense(**kwargs)
```

1. See [:material-code-braces: AnalyzeExpenseRequestRequestTypeDef](./type_defs.md#analyzeexpenserequestrequesttypedef) 

### analyze\_id

Analyzes identity documents for relevant information.

Type annotations and code completion for `#!python session.client("textract").analyze_id` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# analyze_id method definition

await def analyze_id(
    self,
    *,
    DocumentPages: Sequence[DocumentTypeDef],  # (1)
) -> AnalyzeIDResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
2. See [:material-code-braces: AnalyzeIDResponseTypeDef](./type_defs.md#analyzeidresponsetypedef) 


```python
# analyze_id method usage example with argument unpacking

kwargs: AnalyzeIDRequestRequestTypeDef = {  # (1)
    "DocumentPages": ...,
}

parent.analyze_id(**kwargs)
```

1. See [:material-code-braces: AnalyzeIDRequestRequestTypeDef](./type_defs.md#analyzeidrequestrequesttypedef) 

### create\_adapter

Creates an adapter, which can be fine-tuned for enhanced performance on user
provided documents.

Type annotations and code completion for `#!python session.client("textract").create_adapter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# create_adapter method definition

await def create_adapter(
    self,
    *,
    AdapterName: str,
    FeatureTypes: Sequence[FeatureTypeType],  # (1)
    ClientRequestToken: str = ...,
    Description: str = ...,
    AutoUpdate: AutoUpdateType = ...,  # (2)
    Tags: Mapping[str, str] = ...,
) -> CreateAdapterResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
2. See [:material-code-brackets: AutoUpdateType](./literals.md#autoupdatetype) 
3. See [:material-code-braces: CreateAdapterResponseTypeDef](./type_defs.md#createadapterresponsetypedef) 


```python
# create_adapter method usage example with argument unpacking

kwargs: CreateAdapterRequestRequestTypeDef = {  # (1)
    "AdapterName": ...,
    "FeatureTypes": ...,
}

parent.create_adapter(**kwargs)
```

1. See [:material-code-braces: CreateAdapterRequestRequestTypeDef](./type_defs.md#createadapterrequestrequesttypedef) 

### create\_adapter\_version

Creates a new version of an adapter.

Type annotations and code completion for `#!python session.client("textract").create_adapter_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# create_adapter_version method definition

await def create_adapter_version(
    self,
    *,
    AdapterId: str,
    DatasetConfig: AdapterVersionDatasetConfigTypeDef,  # (1)
    OutputConfig: OutputConfigTypeDef,  # (2)
    ClientRequestToken: str = ...,
    KMSKeyId: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateAdapterVersionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AdapterVersionDatasetConfigTypeDef](./type_defs.md#adapterversiondatasetconfigtypedef) 
2. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
3. See [:material-code-braces: CreateAdapterVersionResponseTypeDef](./type_defs.md#createadapterversionresponsetypedef) 


```python
# create_adapter_version method usage example with argument unpacking

kwargs: CreateAdapterVersionRequestRequestTypeDef = {  # (1)
    "AdapterId": ...,
    "DatasetConfig": ...,
    "OutputConfig": ...,
}

parent.create_adapter_version(**kwargs)
```

1. See [:material-code-braces: CreateAdapterVersionRequestRequestTypeDef](./type_defs.md#createadapterversionrequestrequesttypedef) 

### delete\_adapter

Deletes an Amazon Textract adapter.

Type annotations and code completion for `#!python session.client("textract").delete_adapter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# delete_adapter method definition

await def delete_adapter(
    self,
    *,
    AdapterId: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_adapter method usage example with argument unpacking

kwargs: DeleteAdapterRequestRequestTypeDef = {  # (1)
    "AdapterId": ...,
}

parent.delete_adapter(**kwargs)
```

1. See [:material-code-braces: DeleteAdapterRequestRequestTypeDef](./type_defs.md#deleteadapterrequestrequesttypedef) 

### delete\_adapter\_version

Deletes an Amazon Textract adapter version.

Type annotations and code completion for `#!python session.client("textract").delete_adapter_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# delete_adapter_version method definition

await def delete_adapter_version(
    self,
    *,
    AdapterId: str,
    AdapterVersion: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_adapter_version method usage example with argument unpacking

kwargs: DeleteAdapterVersionRequestRequestTypeDef = {  # (1)
    "AdapterId": ...,
    "AdapterVersion": ...,
}

parent.delete_adapter_version(**kwargs)
```

1. See [:material-code-braces: DeleteAdapterVersionRequestRequestTypeDef](./type_defs.md#deleteadapterversionrequestrequesttypedef) 

### detect\_document\_text

Detects text in the input document.

Type annotations and code completion for `#!python session.client("textract").detect_document_text` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# detect_document_text method definition

await def detect_document_text(
    self,
    *,
    Document: DocumentTypeDef,  # (1)
) -> DetectDocumentTextResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
2. See [:material-code-braces: DetectDocumentTextResponseTypeDef](./type_defs.md#detectdocumenttextresponsetypedef) 


```python
# detect_document_text method usage example with argument unpacking

kwargs: DetectDocumentTextRequestRequestTypeDef = {  # (1)
    "Document": ...,
}

parent.detect_document_text(**kwargs)
```

1. See [:material-code-braces: DetectDocumentTextRequestRequestTypeDef](./type_defs.md#detectdocumenttextrequestrequesttypedef) 

### get\_adapter

Gets configuration information for an adapter specified by an AdapterId,
returning information on AdapterName, Description, CreationTime, AutoUpdate
status, and FeatureTypes.

Type annotations and code completion for `#!python session.client("textract").get_adapter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# get_adapter method definition

await def get_adapter(
    self,
    *,
    AdapterId: str,
) -> GetAdapterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAdapterResponseTypeDef](./type_defs.md#getadapterresponsetypedef) 


```python
# get_adapter method usage example with argument unpacking

kwargs: GetAdapterRequestRequestTypeDef = {  # (1)
    "AdapterId": ...,
}

parent.get_adapter(**kwargs)
```

1. See [:material-code-braces: GetAdapterRequestRequestTypeDef](./type_defs.md#getadapterrequestrequesttypedef) 

### get\_adapter\_version

Gets configuration information for the specified adapter version, including:
AdapterId, AdapterVersion, FeatureTypes, Status, StatusMessage, DatasetConfig,
KMSKeyId, OutputConfig, Tags and EvaluationMetrics.

Type annotations and code completion for `#!python session.client("textract").get_adapter_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# get_adapter_version method definition

await def get_adapter_version(
    self,
    *,
    AdapterId: str,
    AdapterVersion: str,
) -> GetAdapterVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAdapterVersionResponseTypeDef](./type_defs.md#getadapterversionresponsetypedef) 


```python
# get_adapter_version method usage example with argument unpacking

kwargs: GetAdapterVersionRequestRequestTypeDef = {  # (1)
    "AdapterId": ...,
    "AdapterVersion": ...,
}

parent.get_adapter_version(**kwargs)
```

1. See [:material-code-braces: GetAdapterVersionRequestRequestTypeDef](./type_defs.md#getadapterversionrequestrequesttypedef) 

### get\_document\_analysis

Gets the results for an Amazon Textract asynchronous operation that analyzes
text in a document.

Type annotations and code completion for `#!python session.client("textract").get_document_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# get_document_analysis method definition

await def get_document_analysis(
    self,
    *,
    JobId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetDocumentAnalysisResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDocumentAnalysisResponseTypeDef](./type_defs.md#getdocumentanalysisresponsetypedef) 


```python
# get_document_analysis method usage example with argument unpacking

kwargs: GetDocumentAnalysisRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.get_document_analysis(**kwargs)
```

1. See [:material-code-braces: GetDocumentAnalysisRequestRequestTypeDef](./type_defs.md#getdocumentanalysisrequestrequesttypedef) 

### get\_document\_text\_detection

Gets the results for an Amazon Textract asynchronous operation that detects
text in a document.

Type annotations and code completion for `#!python session.client("textract").get_document_text_detection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# get_document_text_detection method definition

await def get_document_text_detection(
    self,
    *,
    JobId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetDocumentTextDetectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDocumentTextDetectionResponseTypeDef](./type_defs.md#getdocumenttextdetectionresponsetypedef) 


```python
# get_document_text_detection method usage example with argument unpacking

kwargs: GetDocumentTextDetectionRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.get_document_text_detection(**kwargs)
```

1. See [:material-code-braces: GetDocumentTextDetectionRequestRequestTypeDef](./type_defs.md#getdocumenttextdetectionrequestrequesttypedef) 

### get\_expense\_analysis

Gets the results for an Amazon Textract asynchronous operation that analyzes
invoices and receipts.

Type annotations and code completion for `#!python session.client("textract").get_expense_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# get_expense_analysis method definition

await def get_expense_analysis(
    self,
    *,
    JobId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetExpenseAnalysisResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetExpenseAnalysisResponseTypeDef](./type_defs.md#getexpenseanalysisresponsetypedef) 


```python
# get_expense_analysis method usage example with argument unpacking

kwargs: GetExpenseAnalysisRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.get_expense_analysis(**kwargs)
```

1. See [:material-code-braces: GetExpenseAnalysisRequestRequestTypeDef](./type_defs.md#getexpenseanalysisrequestrequesttypedef) 

### get\_lending\_analysis

Gets the results for an Amazon Textract asynchronous operation that analyzes
text in a lending document.

Type annotations and code completion for `#!python session.client("textract").get_lending_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# get_lending_analysis method definition

await def get_lending_analysis(
    self,
    *,
    JobId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetLendingAnalysisResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLendingAnalysisResponseTypeDef](./type_defs.md#getlendinganalysisresponsetypedef) 


```python
# get_lending_analysis method usage example with argument unpacking

kwargs: GetLendingAnalysisRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.get_lending_analysis(**kwargs)
```

1. See [:material-code-braces: GetLendingAnalysisRequestRequestTypeDef](./type_defs.md#getlendinganalysisrequestrequesttypedef) 

### get\_lending\_analysis\_summary

Gets summarized results for the <code>StartLendingAnalysis</code> operation,
which analyzes text in a lending document.

Type annotations and code completion for `#!python session.client("textract").get_lending_analysis_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# get_lending_analysis_summary method definition

await def get_lending_analysis_summary(
    self,
    *,
    JobId: str,
) -> GetLendingAnalysisSummaryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLendingAnalysisSummaryResponseTypeDef](./type_defs.md#getlendinganalysissummaryresponsetypedef) 


```python
# get_lending_analysis_summary method usage example with argument unpacking

kwargs: GetLendingAnalysisSummaryRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.get_lending_analysis_summary(**kwargs)
```

1. See [:material-code-braces: GetLendingAnalysisSummaryRequestRequestTypeDef](./type_defs.md#getlendinganalysissummaryrequestrequesttypedef) 

### list\_adapter\_versions

List all version of an adapter that meet the specified filtration criteria.

Type annotations and code completion for `#!python session.client("textract").list_adapter_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# list_adapter_versions method definition

await def list_adapter_versions(
    self,
    *,
    AdapterId: str = ...,
    AfterCreationTime: TimestampTypeDef = ...,
    BeforeCreationTime: TimestampTypeDef = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAdapterVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAdapterVersionsResponseTypeDef](./type_defs.md#listadapterversionsresponsetypedef) 


```python
# list_adapter_versions method usage example with argument unpacking

kwargs: ListAdapterVersionsRequestRequestTypeDef = {  # (1)
    "AdapterId": ...,
}

parent.list_adapter_versions(**kwargs)
```

1. See [:material-code-braces: ListAdapterVersionsRequestRequestTypeDef](./type_defs.md#listadapterversionsrequestrequesttypedef) 

### list\_adapters

Lists all adapters that match the specified filtration criteria.

Type annotations and code completion for `#!python session.client("textract").list_adapters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# list_adapters method definition

await def list_adapters(
    self,
    *,
    AfterCreationTime: TimestampTypeDef = ...,
    BeforeCreationTime: TimestampTypeDef = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAdaptersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAdaptersResponseTypeDef](./type_defs.md#listadaptersresponsetypedef) 


```python
# list_adapters method usage example with argument unpacking

kwargs: ListAdaptersRequestRequestTypeDef = {  # (1)
    "AfterCreationTime": ...,
}

parent.list_adapters(**kwargs)
```

1. See [:material-code-braces: ListAdaptersRequestRequestTypeDef](./type_defs.md#listadaptersrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists all tags for an Amazon Textract resource.

Type annotations and code completion for `#!python session.client("textract").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### start\_document\_analysis

Starts the asynchronous analysis of an input document for relationships between
detected items such as key-value pairs, tables, and selection elements.

Type annotations and code completion for `#!python session.client("textract").start_document_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# start_document_analysis method definition

await def start_document_analysis(
    self,
    *,
    DocumentLocation: DocumentLocationTypeDef,  # (1)
    FeatureTypes: Sequence[FeatureTypeType],  # (2)
    ClientRequestToken: str = ...,
    JobTag: str = ...,
    NotificationChannel: NotificationChannelTypeDef = ...,  # (3)
    OutputConfig: OutputConfigTypeDef = ...,  # (4)
    KMSKeyId: str = ...,
    QueriesConfig: QueriesConfigTypeDef = ...,  # (5)
    AdaptersConfig: AdaptersConfigTypeDef = ...,  # (6)
) -> StartDocumentAnalysisResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: DocumentLocationTypeDef](./type_defs.md#documentlocationtypedef) 
2. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
3. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
4. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
5. See [:material-code-braces: QueriesConfigTypeDef](./type_defs.md#queriesconfigtypedef) 
6. See [:material-code-braces: AdaptersConfigTypeDef](./type_defs.md#adaptersconfigtypedef) 
7. See [:material-code-braces: StartDocumentAnalysisResponseTypeDef](./type_defs.md#startdocumentanalysisresponsetypedef) 


```python
# start_document_analysis method usage example with argument unpacking

kwargs: StartDocumentAnalysisRequestRequestTypeDef = {  # (1)
    "DocumentLocation": ...,
    "FeatureTypes": ...,
}

parent.start_document_analysis(**kwargs)
```

1. See [:material-code-braces: StartDocumentAnalysisRequestRequestTypeDef](./type_defs.md#startdocumentanalysisrequestrequesttypedef) 

### start\_document\_text\_detection

Starts the asynchronous detection of text in a document.

Type annotations and code completion for `#!python session.client("textract").start_document_text_detection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# start_document_text_detection method definition

await def start_document_text_detection(
    self,
    *,
    DocumentLocation: DocumentLocationTypeDef,  # (1)
    ClientRequestToken: str = ...,
    JobTag: str = ...,
    NotificationChannel: NotificationChannelTypeDef = ...,  # (2)
    OutputConfig: OutputConfigTypeDef = ...,  # (3)
    KMSKeyId: str = ...,
) -> StartDocumentTextDetectionResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DocumentLocationTypeDef](./type_defs.md#documentlocationtypedef) 
2. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
3. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
4. See [:material-code-braces: StartDocumentTextDetectionResponseTypeDef](./type_defs.md#startdocumenttextdetectionresponsetypedef) 


```python
# start_document_text_detection method usage example with argument unpacking

kwargs: StartDocumentTextDetectionRequestRequestTypeDef = {  # (1)
    "DocumentLocation": ...,
}

parent.start_document_text_detection(**kwargs)
```

1. See [:material-code-braces: StartDocumentTextDetectionRequestRequestTypeDef](./type_defs.md#startdocumenttextdetectionrequestrequesttypedef) 

### start\_expense\_analysis

Starts the asynchronous analysis of invoices or receipts for data like contact
information, items purchased, and vendor names.

Type annotations and code completion for `#!python session.client("textract").start_expense_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# start_expense_analysis method definition

await def start_expense_analysis(
    self,
    *,
    DocumentLocation: DocumentLocationTypeDef,  # (1)
    ClientRequestToken: str = ...,
    JobTag: str = ...,
    NotificationChannel: NotificationChannelTypeDef = ...,  # (2)
    OutputConfig: OutputConfigTypeDef = ...,  # (3)
    KMSKeyId: str = ...,
) -> StartExpenseAnalysisResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DocumentLocationTypeDef](./type_defs.md#documentlocationtypedef) 
2. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
3. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
4. See [:material-code-braces: StartExpenseAnalysisResponseTypeDef](./type_defs.md#startexpenseanalysisresponsetypedef) 


```python
# start_expense_analysis method usage example with argument unpacking

kwargs: StartExpenseAnalysisRequestRequestTypeDef = {  # (1)
    "DocumentLocation": ...,
}

parent.start_expense_analysis(**kwargs)
```

1. See [:material-code-braces: StartExpenseAnalysisRequestRequestTypeDef](./type_defs.md#startexpenseanalysisrequestrequesttypedef) 

### start\_lending\_analysis

Starts the classification and analysis of an input document.

Type annotations and code completion for `#!python session.client("textract").start_lending_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# start_lending_analysis method definition

await def start_lending_analysis(
    self,
    *,
    DocumentLocation: DocumentLocationTypeDef,  # (1)
    ClientRequestToken: str = ...,
    JobTag: str = ...,
    NotificationChannel: NotificationChannelTypeDef = ...,  # (2)
    OutputConfig: OutputConfigTypeDef = ...,  # (3)
    KMSKeyId: str = ...,
) -> StartLendingAnalysisResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DocumentLocationTypeDef](./type_defs.md#documentlocationtypedef) 
2. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
3. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
4. See [:material-code-braces: StartLendingAnalysisResponseTypeDef](./type_defs.md#startlendinganalysisresponsetypedef) 


```python
# start_lending_analysis method usage example with argument unpacking

kwargs: StartLendingAnalysisRequestRequestTypeDef = {  # (1)
    "DocumentLocation": ...,
}

parent.start_lending_analysis(**kwargs)
```

1. See [:material-code-braces: StartLendingAnalysisRequestRequestTypeDef](./type_defs.md#startlendinganalysisrequestrequesttypedef) 

### tag\_resource

Adds one or more tags to the specified resource.

Type annotations and code completion for `#!python session.client("textract").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Mapping[str, str],
) -> dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes any tags with the specified keys from the specified resource.

Type annotations and code completion for `#!python session.client("textract").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_adapter

Update the configuration for an adapter.

Type annotations and code completion for `#!python session.client("textract").update_adapter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# update_adapter method definition

await def update_adapter(
    self,
    *,
    AdapterId: str,
    Description: str = ...,
    AdapterName: str = ...,
    AutoUpdate: AutoUpdateType = ...,  # (1)
) -> UpdateAdapterResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AutoUpdateType](./literals.md#autoupdatetype) 
2. See [:material-code-braces: UpdateAdapterResponseTypeDef](./type_defs.md#updateadapterresponsetypedef) 


```python
# update_adapter method usage example with argument unpacking

kwargs: UpdateAdapterRequestRequestTypeDef = {  # (1)
    "AdapterId": ...,
}

parent.update_adapter(**kwargs)
```

1. See [:material-code-braces: UpdateAdapterRequestRequestTypeDef](./type_defs.md#updateadapterrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("textract").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("textract").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

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




### get_paginator

Type annotations and code completion for `#!python session.client("textract").get_paginator` method with overloads.

- `client.get_paginator("list_adapter_versions")` -> [ListAdapterVersionsPaginator](./paginators.md#listadapterversionspaginator)
- `client.get_paginator("list_adapters")` -> [ListAdaptersPaginator](./paginators.md#listadapterspaginator)


