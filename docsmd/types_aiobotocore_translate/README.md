# Translate module

> [Index](../README.md) > Translate


!!! note ""

    Auto-generated documentation for [Translate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#translate)
    type annotations stubs module [types-aiobotocore-translate](https://pypi.org/project/types-aiobotocore-translate/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `Translate` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `Translate` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[translate]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[translate]'

# standalone installation
python -m pip install types-aiobotocore-translate
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-translate
```

## Usage

Code samples can be found in [Examples](./usage.md).

## TranslateClient

Type annotations and code completion for  `#!python session.client("translate")` as [TranslateClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client)

```python
# TranslateClient usage example

from aioboto3.session import Session

from types_aiobotocore_translate.client import TranslateClient


session = Session()
async with session.client("translate") as client:
    client: TranslateClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("translate").get_paginator("...")`.

```python
# ListTerminologiesPaginator usage example

from types_aiobotocore_translate.paginator import ListTerminologiesPaginator

def get_list_terminologies_paginator() -> ListTerminologiesPaginator:
    return client.get_paginator("list_terminologies"))
```

- [ListTerminologiesPaginator](./paginators.md#listterminologiespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BrevityType usage example

from types_aiobotocore_translate.literals import BrevityType

def get_value() -> BrevityType:
    return "ON"
```

- [BrevityType](./literals.md#brevitytype)
- [DirectionalityType](./literals.md#directionalitytype)
- [DisplayLanguageCodeType](./literals.md#displaylanguagecodetype)
- [EncryptionKeyTypeType](./literals.md#encryptionkeytypetype)
- [FormalityType](./literals.md#formalitytype)
- [JobStatusType](./literals.md#jobstatustype)
- [ListTerminologiesPaginatorName](./literals.md#listterminologiespaginatorname)
- [MergeStrategyType](./literals.md#mergestrategytype)
- [ParallelDataFormatType](./literals.md#paralleldataformattype)
- [ParallelDataStatusType](./literals.md#paralleldatastatustype)
- [ProfanityType](./literals.md#profanitytype)
- [TerminologyDataFormatType](./literals.md#terminologydataformattype)
- [TranslateServiceName](./literals.md#translateservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [TermTypeDef](./type_defs.md#termtypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [EncryptionKeyTypeDef](./type_defs.md#encryptionkeytypedef)
- [ParallelDataConfigTypeDef](./type_defs.md#paralleldataconfigtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteParallelDataRequestRequestTypeDef](./type_defs.md#deleteparalleldatarequestrequesttypedef)
- [DeleteTerminologyRequestRequestTypeDef](./type_defs.md#deleteterminologyrequestrequesttypedef)
- [DescribeTextTranslationJobRequestRequestTypeDef](./type_defs.md#describetexttranslationjobrequestrequesttypedef)
- [GetParallelDataRequestRequestTypeDef](./type_defs.md#getparalleldatarequestrequesttypedef)
- [ParallelDataDataLocationTypeDef](./type_defs.md#paralleldatadatalocationtypedef)
- [GetTerminologyRequestRequestTypeDef](./type_defs.md#getterminologyrequestrequesttypedef)
- [TerminologyDataLocationTypeDef](./type_defs.md#terminologydatalocationtypedef)
- [InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef)
- [JobDetailsTypeDef](./type_defs.md#jobdetailstypedef)
- [LanguageTypeDef](./type_defs.md#languagetypedef)
- [ListLanguagesRequestRequestTypeDef](./type_defs.md#listlanguagesrequestrequesttypedef)
- [ListParallelDataRequestRequestTypeDef](./type_defs.md#listparalleldatarequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListTerminologiesRequestRequestTypeDef](./type_defs.md#listterminologiesrequestrequesttypedef)
- [TranslationSettingsTypeDef](./type_defs.md#translationsettingstypedef)
- [StopTextTranslationJobRequestRequestTypeDef](./type_defs.md#stoptexttranslationjobrequestrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [TranslatedDocumentTypeDef](./type_defs.md#translateddocumenttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [AppliedTerminologyTypeDef](./type_defs.md#appliedterminologytypedef)
- [DocumentTypeDef](./type_defs.md#documenttypedef)
- [TerminologyDataTypeDef](./type_defs.md#terminologydatatypedef)
- [OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef)
- [TerminologyPropertiesTypeDef](./type_defs.md#terminologypropertiestypedef)
- [ParallelDataPropertiesTypeDef](./type_defs.md#paralleldatapropertiestypedef)
- [UpdateParallelDataRequestRequestTypeDef](./type_defs.md#updateparalleldatarequestrequesttypedef)
- [CreateParallelDataRequestRequestTypeDef](./type_defs.md#createparalleldatarequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateParallelDataResponseTypeDef](./type_defs.md#createparalleldataresponsetypedef)
- [DeleteParallelDataResponseTypeDef](./type_defs.md#deleteparalleldataresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartTextTranslationJobResponseTypeDef](./type_defs.md#starttexttranslationjobresponsetypedef)
- [StopTextTranslationJobResponseTypeDef](./type_defs.md#stoptexttranslationjobresponsetypedef)
- [UpdateParallelDataResponseTypeDef](./type_defs.md#updateparalleldataresponsetypedef)
- [ListLanguagesResponseTypeDef](./type_defs.md#listlanguagesresponsetypedef)
- [ListTerminologiesRequestPaginateTypeDef](./type_defs.md#listterminologiesrequestpaginatetypedef)
- [TranslateTextRequestRequestTypeDef](./type_defs.md#translatetextrequestrequesttypedef)
- [TextTranslationJobFilterTypeDef](./type_defs.md#texttranslationjobfiltertypedef)
- [TranslateDocumentResponseTypeDef](./type_defs.md#translatedocumentresponsetypedef)
- [TranslateTextResponseTypeDef](./type_defs.md#translatetextresponsetypedef)
- [TranslateDocumentRequestRequestTypeDef](./type_defs.md#translatedocumentrequestrequesttypedef)
- [ImportTerminologyRequestRequestTypeDef](./type_defs.md#importterminologyrequestrequesttypedef)
- [StartTextTranslationJobRequestRequestTypeDef](./type_defs.md#starttexttranslationjobrequestrequesttypedef)
- [TextTranslationJobPropertiesTypeDef](./type_defs.md#texttranslationjobpropertiestypedef)
- [GetTerminologyResponseTypeDef](./type_defs.md#getterminologyresponsetypedef)
- [ImportTerminologyResponseTypeDef](./type_defs.md#importterminologyresponsetypedef)
- [ListTerminologiesResponseTypeDef](./type_defs.md#listterminologiesresponsetypedef)
- [GetParallelDataResponseTypeDef](./type_defs.md#getparalleldataresponsetypedef)
- [ListParallelDataResponseTypeDef](./type_defs.md#listparalleldataresponsetypedef)
- [ListTextTranslationJobsRequestRequestTypeDef](./type_defs.md#listtexttranslationjobsrequestrequesttypedef)
- [DescribeTextTranslationJobResponseTypeDef](./type_defs.md#describetexttranslationjobresponsetypedef)
- [ListTextTranslationJobsResponseTypeDef](./type_defs.md#listtexttranslationjobsresponsetypedef)
