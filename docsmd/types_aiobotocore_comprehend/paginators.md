# Paginators

> [Index](../README.md) > [Comprehend](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Comprehend](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
    type annotations stubs module [types-aiobotocore-comprehend](https://pypi.org/project/types-aiobotocore-comprehend/).

## ListDocumentClassificationJobsPaginator

Type annotations and code completion for `#!python session.client("comprehend").get_paginator("list_document_classification_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassificationJobs)

```python
# ListDocumentClassificationJobsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_comprehend.paginator import ListDocumentClassificationJobsPaginator

session = Session()

session = get_session()
async with session.client("comprehend") as client:  # (1)
    paginator: ListDocumentClassificationJobsPaginator = client.get_paginator("list_document_classification_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListDocumentClassificationJobsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListDocumentClassificationJobsPaginator](./paginators.md#listdocumentclassificationjobspaginator)
3. item: [:material-code-braces: ListDocumentClassificationJobsResponsePaginatorTypeDef](./type_defs.md#listdocumentclassificationjobsresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListDocumentClassificationJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: DocumentClassificationJobFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDocumentClassificationJobsResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DocumentClassificationJobFilterTypeDef](./type_defs.md#documentclassificationjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDocumentClassificationJobsResponsePaginatorTypeDef](./type_defs.md#listdocumentclassificationjobsresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef](./type_defs.md#listdocumentclassificationjobsrequestlistdocumentclassificationjobspaginatetypedef) 
## ListDocumentClassifiersPaginator

Type annotations and code completion for `#!python session.client("comprehend").get_paginator("list_document_classifiers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassifiers)

```python
# ListDocumentClassifiersPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_comprehend.paginator import ListDocumentClassifiersPaginator

session = Session()

session = get_session()
async with session.client("comprehend") as client:  # (1)
    paginator: ListDocumentClassifiersPaginator = client.get_paginator("list_document_classifiers")  # (2)
    async for item in paginator.paginate(...):
        item: ListDocumentClassifiersResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListDocumentClassifiersPaginator](./paginators.md#listdocumentclassifierspaginator)
3. item: [:material-code-braces: ListDocumentClassifiersResponsePaginatorTypeDef](./type_defs.md#listdocumentclassifiersresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListDocumentClassifiersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: DocumentClassifierFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDocumentClassifiersResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DocumentClassifierFilterTypeDef](./type_defs.md#documentclassifierfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDocumentClassifiersResponsePaginatorTypeDef](./type_defs.md#listdocumentclassifiersresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef](./type_defs.md#listdocumentclassifiersrequestlistdocumentclassifierspaginatetypedef) 
## ListDominantLanguageDetectionJobsPaginator

Type annotations and code completion for `#!python session.client("comprehend").get_paginator("list_dominant_language_detection_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDominantLanguageDetectionJobs)

```python
# ListDominantLanguageDetectionJobsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_comprehend.paginator import ListDominantLanguageDetectionJobsPaginator

session = Session()

session = get_session()
async with session.client("comprehend") as client:  # (1)
    paginator: ListDominantLanguageDetectionJobsPaginator = client.get_paginator("list_dominant_language_detection_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListDominantLanguageDetectionJobsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListDominantLanguageDetectionJobsPaginator](./paginators.md#listdominantlanguagedetectionjobspaginator)
3. item: [:material-code-braces: ListDominantLanguageDetectionJobsResponsePaginatorTypeDef](./type_defs.md#listdominantlanguagedetectionjobsresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListDominantLanguageDetectionJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: DominantLanguageDetectionJobFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDominantLanguageDetectionJobsResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DominantLanguageDetectionJobFilterTypeDef](./type_defs.md#dominantlanguagedetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDominantLanguageDetectionJobsResponsePaginatorTypeDef](./type_defs.md#listdominantlanguagedetectionjobsresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef](./type_defs.md#listdominantlanguagedetectionjobsrequestlistdominantlanguagedetectionjobspaginatetypedef) 
## ListEndpointsPaginator

Type annotations and code completion for `#!python session.client("comprehend").get_paginator("list_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEndpoints)

```python
# ListEndpointsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_comprehend.paginator import ListEndpointsPaginator

session = Session()

session = get_session()
async with session.client("comprehend") as client:  # (1)
    paginator: ListEndpointsPaginator = client.get_paginator("list_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: ListEndpointsResponseTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListEndpointsPaginator](./paginators.md#listendpointspaginator)
3. item: [:material-code-braces: ListEndpointsResponseTypeDef](./type_defs.md#listendpointsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEndpointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: EndpointFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListEndpointsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: EndpointFilterTypeDef](./type_defs.md#endpointfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListEndpointsResponseTypeDef](./type_defs.md#listendpointsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEndpointsRequestListEndpointsPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEndpointsRequestListEndpointsPaginateTypeDef](./type_defs.md#listendpointsrequestlistendpointspaginatetypedef) 
## ListEntitiesDetectionJobsPaginator

Type annotations and code completion for `#!python session.client("comprehend").get_paginator("list_entities_detection_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntitiesDetectionJobs)

```python
# ListEntitiesDetectionJobsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_comprehend.paginator import ListEntitiesDetectionJobsPaginator

session = Session()

session = get_session()
async with session.client("comprehend") as client:  # (1)
    paginator: ListEntitiesDetectionJobsPaginator = client.get_paginator("list_entities_detection_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListEntitiesDetectionJobsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListEntitiesDetectionJobsPaginator](./paginators.md#listentitiesdetectionjobspaginator)
3. item: [:material-code-braces: ListEntitiesDetectionJobsResponsePaginatorTypeDef](./type_defs.md#listentitiesdetectionjobsresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListEntitiesDetectionJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: EntitiesDetectionJobFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListEntitiesDetectionJobsResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: EntitiesDetectionJobFilterTypeDef](./type_defs.md#entitiesdetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListEntitiesDetectionJobsResponsePaginatorTypeDef](./type_defs.md#listentitiesdetectionjobsresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef](./type_defs.md#listentitiesdetectionjobsrequestlistentitiesdetectionjobspaginatetypedef) 
## ListEntityRecognizersPaginator

Type annotations and code completion for `#!python session.client("comprehend").get_paginator("list_entity_recognizers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntityRecognizers)

```python
# ListEntityRecognizersPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_comprehend.paginator import ListEntityRecognizersPaginator

session = Session()

session = get_session()
async with session.client("comprehend") as client:  # (1)
    paginator: ListEntityRecognizersPaginator = client.get_paginator("list_entity_recognizers")  # (2)
    async for item in paginator.paginate(...):
        item: ListEntityRecognizersResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListEntityRecognizersPaginator](./paginators.md#listentityrecognizerspaginator)
3. item: [:material-code-braces: ListEntityRecognizersResponsePaginatorTypeDef](./type_defs.md#listentityrecognizersresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListEntityRecognizersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: EntityRecognizerFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListEntityRecognizersResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: EntityRecognizerFilterTypeDef](./type_defs.md#entityrecognizerfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListEntityRecognizersResponsePaginatorTypeDef](./type_defs.md#listentityrecognizersresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef](./type_defs.md#listentityrecognizersrequestlistentityrecognizerspaginatetypedef) 
## ListKeyPhrasesDetectionJobsPaginator

Type annotations and code completion for `#!python session.client("comprehend").get_paginator("list_key_phrases_detection_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListKeyPhrasesDetectionJobs)

```python
# ListKeyPhrasesDetectionJobsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_comprehend.paginator import ListKeyPhrasesDetectionJobsPaginator

session = Session()

session = get_session()
async with session.client("comprehend") as client:  # (1)
    paginator: ListKeyPhrasesDetectionJobsPaginator = client.get_paginator("list_key_phrases_detection_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListKeyPhrasesDetectionJobsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListKeyPhrasesDetectionJobsPaginator](./paginators.md#listkeyphrasesdetectionjobspaginator)
3. item: [:material-code-braces: ListKeyPhrasesDetectionJobsResponsePaginatorTypeDef](./type_defs.md#listkeyphrasesdetectionjobsresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListKeyPhrasesDetectionJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: KeyPhrasesDetectionJobFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListKeyPhrasesDetectionJobsResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: KeyPhrasesDetectionJobFilterTypeDef](./type_defs.md#keyphrasesdetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListKeyPhrasesDetectionJobsResponsePaginatorTypeDef](./type_defs.md#listkeyphrasesdetectionjobsresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef](./type_defs.md#listkeyphrasesdetectionjobsrequestlistkeyphrasesdetectionjobspaginatetypedef) 
## ListPiiEntitiesDetectionJobsPaginator

Type annotations and code completion for `#!python session.client("comprehend").get_paginator("list_pii_entities_detection_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListPiiEntitiesDetectionJobs)

```python
# ListPiiEntitiesDetectionJobsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_comprehend.paginator import ListPiiEntitiesDetectionJobsPaginator

session = Session()

session = get_session()
async with session.client("comprehend") as client:  # (1)
    paginator: ListPiiEntitiesDetectionJobsPaginator = client.get_paginator("list_pii_entities_detection_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListPiiEntitiesDetectionJobsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListPiiEntitiesDetectionJobsPaginator](./paginators.md#listpiientitiesdetectionjobspaginator)
3. item: [:material-code-braces: ListPiiEntitiesDetectionJobsResponsePaginatorTypeDef](./type_defs.md#listpiientitiesdetectionjobsresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListPiiEntitiesDetectionJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: PiiEntitiesDetectionJobFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListPiiEntitiesDetectionJobsResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: PiiEntitiesDetectionJobFilterTypeDef](./type_defs.md#piientitiesdetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPiiEntitiesDetectionJobsResponsePaginatorTypeDef](./type_defs.md#listpiientitiesdetectionjobsresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPiiEntitiesDetectionJobsRequestListPiiEntitiesDetectionJobsPaginateTypeDef](./type_defs.md#listpiientitiesdetectionjobsrequestlistpiientitiesdetectionjobspaginatetypedef) 
## ListSentimentDetectionJobsPaginator

Type annotations and code completion for `#!python session.client("comprehend").get_paginator("list_sentiment_detection_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListSentimentDetectionJobs)

```python
# ListSentimentDetectionJobsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_comprehend.paginator import ListSentimentDetectionJobsPaginator

session = Session()

session = get_session()
async with session.client("comprehend") as client:  # (1)
    paginator: ListSentimentDetectionJobsPaginator = client.get_paginator("list_sentiment_detection_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListSentimentDetectionJobsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListSentimentDetectionJobsPaginator](./paginators.md#listsentimentdetectionjobspaginator)
3. item: [:material-code-braces: ListSentimentDetectionJobsResponsePaginatorTypeDef](./type_defs.md#listsentimentdetectionjobsresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListSentimentDetectionJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: SentimentDetectionJobFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListSentimentDetectionJobsResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SentimentDetectionJobFilterTypeDef](./type_defs.md#sentimentdetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSentimentDetectionJobsResponsePaginatorTypeDef](./type_defs.md#listsentimentdetectionjobsresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef](./type_defs.md#listsentimentdetectionjobsrequestlistsentimentdetectionjobspaginatetypedef) 
## ListTopicsDetectionJobsPaginator

Type annotations and code completion for `#!python session.client("comprehend").get_paginator("list_topics_detection_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListTopicsDetectionJobs)

```python
# ListTopicsDetectionJobsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_comprehend.paginator import ListTopicsDetectionJobsPaginator

session = Session()

session = get_session()
async with session.client("comprehend") as client:  # (1)
    paginator: ListTopicsDetectionJobsPaginator = client.get_paginator("list_topics_detection_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListTopicsDetectionJobsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListTopicsDetectionJobsPaginator](./paginators.md#listtopicsdetectionjobspaginator)
3. item: [:material-code-braces: ListTopicsDetectionJobsResponsePaginatorTypeDef](./type_defs.md#listtopicsdetectionjobsresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListTopicsDetectionJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: TopicsDetectionJobFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListTopicsDetectionJobsResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: TopicsDetectionJobFilterTypeDef](./type_defs.md#topicsdetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListTopicsDetectionJobsResponsePaginatorTypeDef](./type_defs.md#listtopicsdetectionjobsresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef](./type_defs.md#listtopicsdetectionjobsrequestlisttopicsdetectionjobspaginatetypedef) 
