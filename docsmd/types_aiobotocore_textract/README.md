# Textract module

> [Index](../README.md) > Textract


!!! note ""

    Auto-generated documentation for [Textract](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
    type annotations stubs module [types-aiobotocore-textract](https://pypi.org/project/types-aiobotocore-textract/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `Textract` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[textract]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[textract]'


# standalone installation
python -m pip install types-aiobotocore-textract
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-textract
```

## Usage

Code samples can be found in [Examples](./usage.md).

## TextractClient

Type annotations and code completion for  `#!python session.client("textract")` as [TextractClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_textract.client import TextractClient


session = Session()
async with session.client("textract") as client:
    client: TextractClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_textract.literals import BlockTypeType

def get_value() -> BlockTypeType:
    return "CELL"
```

- [BlockTypeType](./literals.md#blocktypetype)
- [ContentClassifierType](./literals.md#contentclassifiertype)
- [EntityTypeType](./literals.md#entitytypetype)
- [FeatureTypeType](./literals.md#featuretypetype)
- [JobStatusType](./literals.md#jobstatustype)
- [RelationshipTypeType](./literals.md#relationshiptypetype)
- [SelectionStatusType](./literals.md#selectionstatustype)
- [TextTypeType](./literals.md#texttypetype)
- [ValueTypeType](./literals.md#valuetypetype)
- [TextractServiceName](./literals.md#textractservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_textract.type_defs import DocumentMetadataTypeDef

def get_value() -> DocumentMetadataTypeDef:
    return {
        "Pages": ...,
    }
```

- [DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef)
- [HumanLoopActivationOutputTypeDef](./type_defs.md#humanloopactivationoutputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [NormalizedValueTypeDef](./type_defs.md#normalizedvaluetypedef)
- [QueryTypeDef](./type_defs.md#querytypedef)
- [RelationshipTypeDef](./type_defs.md#relationshiptypedef)
- [BoundingBoxTypeDef](./type_defs.md#boundingboxtypedef)
- [S3ObjectTypeDef](./type_defs.md#s3objecttypedef)
- [ExpenseTypeTypeDef](./type_defs.md#expensetypetypedef)
- [PointTypeDef](./type_defs.md#pointtypedef)
- [GetDocumentAnalysisRequestRequestTypeDef](./type_defs.md#getdocumentanalysisrequestrequesttypedef)
- [WarningTypeDef](./type_defs.md#warningtypedef)
- [GetDocumentTextDetectionRequestRequestTypeDef](./type_defs.md#getdocumenttextdetectionrequestrequesttypedef)
- [GetExpenseAnalysisRequestRequestTypeDef](./type_defs.md#getexpenseanalysisrequestrequesttypedef)
- [HumanLoopDataAttributesTypeDef](./type_defs.md#humanloopdataattributestypedef)
- [NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef)
- [OutputConfigTypeDef](./type_defs.md#outputconfigtypedef)
- [StartDocumentAnalysisResponseTypeDef](./type_defs.md#startdocumentanalysisresponsetypedef)
- [StartDocumentTextDetectionResponseTypeDef](./type_defs.md#startdocumenttextdetectionresponsetypedef)
- [StartExpenseAnalysisResponseTypeDef](./type_defs.md#startexpenseanalysisresponsetypedef)
- [AnalyzeIDDetectionsTypeDef](./type_defs.md#analyzeiddetectionstypedef)
- [QueriesConfigTypeDef](./type_defs.md#queriesconfigtypedef)
- [DocumentLocationTypeDef](./type_defs.md#documentlocationtypedef)
- [DocumentTypeDef](./type_defs.md#documenttypedef)
- [GeometryTypeDef](./type_defs.md#geometrytypedef)
- [HumanLoopConfigTypeDef](./type_defs.md#humanloopconfigtypedef)
- [IdentityDocumentFieldTypeDef](./type_defs.md#identitydocumentfieldtypedef)
- [StartDocumentAnalysisRequestRequestTypeDef](./type_defs.md#startdocumentanalysisrequestrequesttypedef)
- [StartDocumentTextDetectionRequestRequestTypeDef](./type_defs.md#startdocumenttextdetectionrequestrequesttypedef)
- [StartExpenseAnalysisRequestRequestTypeDef](./type_defs.md#startexpenseanalysisrequestrequesttypedef)
- [AnalyzeExpenseRequestRequestTypeDef](./type_defs.md#analyzeexpenserequestrequesttypedef)
- [AnalyzeIDRequestRequestTypeDef](./type_defs.md#analyzeidrequestrequesttypedef)
- [DetectDocumentTextRequestRequestTypeDef](./type_defs.md#detectdocumenttextrequestrequesttypedef)
- [BlockTypeDef](./type_defs.md#blocktypedef)
- [ExpenseDetectionTypeDef](./type_defs.md#expensedetectiontypedef)
- [AnalyzeDocumentRequestRequestTypeDef](./type_defs.md#analyzedocumentrequestrequesttypedef)
- [IdentityDocumentTypeDef](./type_defs.md#identitydocumenttypedef)
- [AnalyzeDocumentResponseTypeDef](./type_defs.md#analyzedocumentresponsetypedef)
- [DetectDocumentTextResponseTypeDef](./type_defs.md#detectdocumenttextresponsetypedef)
- [GetDocumentAnalysisResponseTypeDef](./type_defs.md#getdocumentanalysisresponsetypedef)
- [GetDocumentTextDetectionResponseTypeDef](./type_defs.md#getdocumenttextdetectionresponsetypedef)
- [ExpenseFieldTypeDef](./type_defs.md#expensefieldtypedef)
- [AnalyzeIDResponseTypeDef](./type_defs.md#analyzeidresponsetypedef)
- [LineItemFieldsTypeDef](./type_defs.md#lineitemfieldstypedef)
- [LineItemGroupTypeDef](./type_defs.md#lineitemgrouptypedef)
- [ExpenseDocumentTypeDef](./type_defs.md#expensedocumenttypedef)
- [AnalyzeExpenseResponseTypeDef](./type_defs.md#analyzeexpenseresponsetypedef)
- [GetExpenseAnalysisResponseTypeDef](./type_defs.md#getexpenseanalysisresponsetypedef)

