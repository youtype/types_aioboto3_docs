# Paginators

> [Index](../README.md) > [CloudDirectory](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudDirectory](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#clouddirectory)
    type annotations stubs module [types-aiobotocore-clouddirectory](https://pypi.org/project/types-aiobotocore-clouddirectory/).

## ListAppliedSchemaArnsPaginator

Type annotations and code completion for `#!python session.client("clouddirectory").get_paginator("list_applied_schema_arns")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory/paginator/ListAppliedSchemaArns.html#CloudDirectory.Paginator.ListAppliedSchemaArns)

```python
# ListAppliedSchemaArnsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.paginator import ListAppliedSchemaArnsPaginator

session = Session()

session = get_session()
async with session.client("clouddirectory") as client:  # (1)
    paginator: ListAppliedSchemaArnsPaginator = client.get_paginator("list_applied_schema_arns")  # (2)
    async for item in paginator.paginate(...):
        item: ListAppliedSchemaArnsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListAppliedSchemaArnsPaginator](./paginators.md#listappliedschemaarnspaginator)
3. item: [:material-code-braces: ListAppliedSchemaArnsResponseTypeDef](./type_defs.md#listappliedschemaarnsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAppliedSchemaArnsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryArn: str,
    SchemaArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAppliedSchemaArnsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAppliedSchemaArnsResponseTypeDef](./type_defs.md#listappliedschemaarnsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAppliedSchemaArnsRequestPaginateTypeDef = {  # (1)
    "DirectoryArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAppliedSchemaArnsRequestPaginateTypeDef](./type_defs.md#listappliedschemaarnsrequestpaginatetypedef) 
## ListAttachedIndicesPaginator

Type annotations and code completion for `#!python session.client("clouddirectory").get_paginator("list_attached_indices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory/paginator/ListAttachedIndices.html#CloudDirectory.Paginator.ListAttachedIndices)

```python
# ListAttachedIndicesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.paginator import ListAttachedIndicesPaginator

session = Session()

session = get_session()
async with session.client("clouddirectory") as client:  # (1)
    paginator: ListAttachedIndicesPaginator = client.get_paginator("list_attached_indices")  # (2)
    async for item in paginator.paginate(...):
        item: ListAttachedIndicesResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListAttachedIndicesPaginator](./paginators.md#listattachedindicespaginator)
3. item: [:material-code-braces: ListAttachedIndicesResponseTypeDef](./type_defs.md#listattachedindicesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAttachedIndicesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryArn: str,
    TargetReference: ObjectReferenceTypeDef,  # (1)
    ConsistencyLevel: ConsistencyLevelType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListAttachedIndicesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListAttachedIndicesResponseTypeDef](./type_defs.md#listattachedindicesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAttachedIndicesRequestPaginateTypeDef = {  # (1)
    "DirectoryArn": ...,
    "TargetReference": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAttachedIndicesRequestPaginateTypeDef](./type_defs.md#listattachedindicesrequestpaginatetypedef) 
## ListDevelopmentSchemaArnsPaginator

Type annotations and code completion for `#!python session.client("clouddirectory").get_paginator("list_development_schema_arns")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory/paginator/ListDevelopmentSchemaArns.html#CloudDirectory.Paginator.ListDevelopmentSchemaArns)

```python
# ListDevelopmentSchemaArnsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.paginator import ListDevelopmentSchemaArnsPaginator

session = Session()

session = get_session()
async with session.client("clouddirectory") as client:  # (1)
    paginator: ListDevelopmentSchemaArnsPaginator = client.get_paginator("list_development_schema_arns")  # (2)
    async for item in paginator.paginate(...):
        item: ListDevelopmentSchemaArnsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListDevelopmentSchemaArnsPaginator](./paginators.md#listdevelopmentschemaarnspaginator)
3. item: [:material-code-braces: ListDevelopmentSchemaArnsResponseTypeDef](./type_defs.md#listdevelopmentschemaarnsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDevelopmentSchemaArnsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDevelopmentSchemaArnsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDevelopmentSchemaArnsResponseTypeDef](./type_defs.md#listdevelopmentschemaarnsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDevelopmentSchemaArnsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDevelopmentSchemaArnsRequestPaginateTypeDef](./type_defs.md#listdevelopmentschemaarnsrequestpaginatetypedef) 
## ListDirectoriesPaginator

Type annotations and code completion for `#!python session.client("clouddirectory").get_paginator("list_directories")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory/paginator/ListDirectories.html#CloudDirectory.Paginator.ListDirectories)

```python
# ListDirectoriesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.paginator import ListDirectoriesPaginator

session = Session()

session = get_session()
async with session.client("clouddirectory") as client:  # (1)
    paginator: ListDirectoriesPaginator = client.get_paginator("list_directories")  # (2)
    async for item in paginator.paginate(...):
        item: ListDirectoriesResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListDirectoriesPaginator](./paginators.md#listdirectoriespaginator)
3. item: [:material-code-braces: ListDirectoriesResponseTypeDef](./type_defs.md#listdirectoriesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDirectoriesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    state: DirectoryStateType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListDirectoriesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DirectoryStateType](./literals.md#directorystatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDirectoriesResponseTypeDef](./type_defs.md#listdirectoriesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDirectoriesRequestPaginateTypeDef = {  # (1)
    "state": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDirectoriesRequestPaginateTypeDef](./type_defs.md#listdirectoriesrequestpaginatetypedef) 
## ListFacetAttributesPaginator

Type annotations and code completion for `#!python session.client("clouddirectory").get_paginator("list_facet_attributes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory/paginator/ListFacetAttributes.html#CloudDirectory.Paginator.ListFacetAttributes)

```python
# ListFacetAttributesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.paginator import ListFacetAttributesPaginator

session = Session()

session = get_session()
async with session.client("clouddirectory") as client:  # (1)
    paginator: ListFacetAttributesPaginator = client.get_paginator("list_facet_attributes")  # (2)
    async for item in paginator.paginate(...):
        item: ListFacetAttributesResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListFacetAttributesPaginator](./paginators.md#listfacetattributespaginator)
3. item: [:material-code-braces: ListFacetAttributesResponseTypeDef](./type_defs.md#listfacetattributesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFacetAttributesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SchemaArn: str,
    Name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFacetAttributesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFacetAttributesResponseTypeDef](./type_defs.md#listfacetattributesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFacetAttributesRequestPaginateTypeDef = {  # (1)
    "SchemaArn": ...,
    "Name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFacetAttributesRequestPaginateTypeDef](./type_defs.md#listfacetattributesrequestpaginatetypedef) 
## ListFacetNamesPaginator

Type annotations and code completion for `#!python session.client("clouddirectory").get_paginator("list_facet_names")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory/paginator/ListFacetNames.html#CloudDirectory.Paginator.ListFacetNames)

```python
# ListFacetNamesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.paginator import ListFacetNamesPaginator

session = Session()

session = get_session()
async with session.client("clouddirectory") as client:  # (1)
    paginator: ListFacetNamesPaginator = client.get_paginator("list_facet_names")  # (2)
    async for item in paginator.paginate(...):
        item: ListFacetNamesResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListFacetNamesPaginator](./paginators.md#listfacetnamespaginator)
3. item: [:material-code-braces: ListFacetNamesResponseTypeDef](./type_defs.md#listfacetnamesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFacetNamesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SchemaArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFacetNamesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFacetNamesResponseTypeDef](./type_defs.md#listfacetnamesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFacetNamesRequestPaginateTypeDef = {  # (1)
    "SchemaArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFacetNamesRequestPaginateTypeDef](./type_defs.md#listfacetnamesrequestpaginatetypedef) 
## ListIncomingTypedLinksPaginator

Type annotations and code completion for `#!python session.client("clouddirectory").get_paginator("list_incoming_typed_links")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory/paginator/ListIncomingTypedLinks.html#CloudDirectory.Paginator.ListIncomingTypedLinks)

```python
# ListIncomingTypedLinksPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.paginator import ListIncomingTypedLinksPaginator

session = Session()

session = get_session()
async with session.client("clouddirectory") as client:  # (1)
    paginator: ListIncomingTypedLinksPaginator = client.get_paginator("list_incoming_typed_links")  # (2)
    async for item in paginator.paginate(...):
        item: ListIncomingTypedLinksResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListIncomingTypedLinksPaginator](./paginators.md#listincomingtypedlinkspaginator)
3. item: [:material-code-braces: ListIncomingTypedLinksResponseTypeDef](./type_defs.md#listincomingtypedlinksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListIncomingTypedLinksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    FilterAttributeRanges: Sequence[TypedLinkAttributeRangeTypeDef] = ...,  # (2)
    FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,  # (3)
    ConsistencyLevel: ConsistencyLevelType = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> AioPageIterator[ListIncomingTypedLinksResponseTypeDef]:  # (6)
    ...
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: TypedLinkAttributeRangeTypeDef](./type_defs.md#typedlinkattributerangetypedef) 
3. See [:material-code-braces: TypedLinkSchemaAndFacetNameTypeDef](./type_defs.md#typedlinkschemaandfacetnametypedef) 
4. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
6. See [:material-code-braces: ListIncomingTypedLinksResponseTypeDef](./type_defs.md#listincomingtypedlinksresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIncomingTypedLinksRequestPaginateTypeDef = {  # (1)
    "DirectoryArn": ...,
    "ObjectReference": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIncomingTypedLinksRequestPaginateTypeDef](./type_defs.md#listincomingtypedlinksrequestpaginatetypedef) 
## ListIndexPaginator

Type annotations and code completion for `#!python session.client("clouddirectory").get_paginator("list_index")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory/paginator/ListIndex.html#CloudDirectory.Paginator.ListIndex)

```python
# ListIndexPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.paginator import ListIndexPaginator

session = Session()

session = get_session()
async with session.client("clouddirectory") as client:  # (1)
    paginator: ListIndexPaginator = client.get_paginator("list_index")  # (2)
    async for item in paginator.paginate(...):
        item: ListIndexResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListIndexPaginator](./paginators.md#listindexpaginator)
3. item: [:material-code-braces: ListIndexResponseTypeDef](./type_defs.md#listindexresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListIndexPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryArn: str,
    IndexReference: ObjectReferenceTypeDef,  # (1)
    RangesOnIndexedValues: Sequence[ObjectAttributeRangeTypeDef] = ...,  # (2)
    ConsistencyLevel: ConsistencyLevelType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[ListIndexResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: ObjectAttributeRangeTypeDef](./type_defs.md#objectattributerangetypedef) 
3. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListIndexResponseTypeDef](./type_defs.md#listindexresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIndexRequestPaginateTypeDef = {  # (1)
    "DirectoryArn": ...,
    "IndexReference": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIndexRequestPaginateTypeDef](./type_defs.md#listindexrequestpaginatetypedef) 
## ListManagedSchemaArnsPaginator

Type annotations and code completion for `#!python session.client("clouddirectory").get_paginator("list_managed_schema_arns")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory/paginator/ListManagedSchemaArns.html#CloudDirectory.Paginator.ListManagedSchemaArns)

```python
# ListManagedSchemaArnsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.paginator import ListManagedSchemaArnsPaginator

session = Session()

session = get_session()
async with session.client("clouddirectory") as client:  # (1)
    paginator: ListManagedSchemaArnsPaginator = client.get_paginator("list_managed_schema_arns")  # (2)
    async for item in paginator.paginate(...):
        item: ListManagedSchemaArnsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListManagedSchemaArnsPaginator](./paginators.md#listmanagedschemaarnspaginator)
3. item: [:material-code-braces: ListManagedSchemaArnsResponseTypeDef](./type_defs.md#listmanagedschemaarnsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListManagedSchemaArnsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SchemaArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListManagedSchemaArnsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListManagedSchemaArnsResponseTypeDef](./type_defs.md#listmanagedschemaarnsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListManagedSchemaArnsRequestPaginateTypeDef = {  # (1)
    "SchemaArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListManagedSchemaArnsRequestPaginateTypeDef](./type_defs.md#listmanagedschemaarnsrequestpaginatetypedef) 
## ListObjectAttributesPaginator

Type annotations and code completion for `#!python session.client("clouddirectory").get_paginator("list_object_attributes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory/paginator/ListObjectAttributes.html#CloudDirectory.Paginator.ListObjectAttributes)

```python
# ListObjectAttributesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.paginator import ListObjectAttributesPaginator

session = Session()

session = get_session()
async with session.client("clouddirectory") as client:  # (1)
    paginator: ListObjectAttributesPaginator = client.get_paginator("list_object_attributes")  # (2)
    async for item in paginator.paginate(...):
        item: ListObjectAttributesResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListObjectAttributesPaginator](./paginators.md#listobjectattributespaginator)
3. item: [:material-code-braces: ListObjectAttributesResponseTypeDef](./type_defs.md#listobjectattributesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListObjectAttributesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    ConsistencyLevel: ConsistencyLevelType = ...,  # (2)
    FacetFilter: SchemaFacetTypeDef = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[ListObjectAttributesResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
3. See [:material-code-braces: SchemaFacetTypeDef](./type_defs.md#schemafacettypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListObjectAttributesResponseTypeDef](./type_defs.md#listobjectattributesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListObjectAttributesRequestPaginateTypeDef = {  # (1)
    "DirectoryArn": ...,
    "ObjectReference": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListObjectAttributesRequestPaginateTypeDef](./type_defs.md#listobjectattributesrequestpaginatetypedef) 
## ListObjectParentPathsPaginator

Type annotations and code completion for `#!python session.client("clouddirectory").get_paginator("list_object_parent_paths")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory/paginator/ListObjectParentPaths.html#CloudDirectory.Paginator.ListObjectParentPaths)

```python
# ListObjectParentPathsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.paginator import ListObjectParentPathsPaginator

session = Session()

session = get_session()
async with session.client("clouddirectory") as client:  # (1)
    paginator: ListObjectParentPathsPaginator = client.get_paginator("list_object_parent_paths")  # (2)
    async for item in paginator.paginate(...):
        item: ListObjectParentPathsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListObjectParentPathsPaginator](./paginators.md#listobjectparentpathspaginator)
3. item: [:material-code-braces: ListObjectParentPathsResponseTypeDef](./type_defs.md#listobjectparentpathsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListObjectParentPathsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListObjectParentPathsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListObjectParentPathsResponseTypeDef](./type_defs.md#listobjectparentpathsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListObjectParentPathsRequestPaginateTypeDef = {  # (1)
    "DirectoryArn": ...,
    "ObjectReference": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListObjectParentPathsRequestPaginateTypeDef](./type_defs.md#listobjectparentpathsrequestpaginatetypedef) 
## ListObjectPoliciesPaginator

Type annotations and code completion for `#!python session.client("clouddirectory").get_paginator("list_object_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory/paginator/ListObjectPolicies.html#CloudDirectory.Paginator.ListObjectPolicies)

```python
# ListObjectPoliciesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.paginator import ListObjectPoliciesPaginator

session = Session()

session = get_session()
async with session.client("clouddirectory") as client:  # (1)
    paginator: ListObjectPoliciesPaginator = client.get_paginator("list_object_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListObjectPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListObjectPoliciesPaginator](./paginators.md#listobjectpoliciespaginator)
3. item: [:material-code-braces: ListObjectPoliciesResponseTypeDef](./type_defs.md#listobjectpoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListObjectPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    ConsistencyLevel: ConsistencyLevelType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListObjectPoliciesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListObjectPoliciesResponseTypeDef](./type_defs.md#listobjectpoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListObjectPoliciesRequestPaginateTypeDef = {  # (1)
    "DirectoryArn": ...,
    "ObjectReference": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListObjectPoliciesRequestPaginateTypeDef](./type_defs.md#listobjectpoliciesrequestpaginatetypedef) 
## ListOutgoingTypedLinksPaginator

Type annotations and code completion for `#!python session.client("clouddirectory").get_paginator("list_outgoing_typed_links")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory/paginator/ListOutgoingTypedLinks.html#CloudDirectory.Paginator.ListOutgoingTypedLinks)

```python
# ListOutgoingTypedLinksPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.paginator import ListOutgoingTypedLinksPaginator

session = Session()

session = get_session()
async with session.client("clouddirectory") as client:  # (1)
    paginator: ListOutgoingTypedLinksPaginator = client.get_paginator("list_outgoing_typed_links")  # (2)
    async for item in paginator.paginate(...):
        item: ListOutgoingTypedLinksResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListOutgoingTypedLinksPaginator](./paginators.md#listoutgoingtypedlinkspaginator)
3. item: [:material-code-braces: ListOutgoingTypedLinksResponseTypeDef](./type_defs.md#listoutgoingtypedlinksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListOutgoingTypedLinksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    FilterAttributeRanges: Sequence[TypedLinkAttributeRangeTypeDef] = ...,  # (2)
    FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,  # (3)
    ConsistencyLevel: ConsistencyLevelType = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> AioPageIterator[ListOutgoingTypedLinksResponseTypeDef]:  # (6)
    ...
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: TypedLinkAttributeRangeTypeDef](./type_defs.md#typedlinkattributerangetypedef) 
3. See [:material-code-braces: TypedLinkSchemaAndFacetNameTypeDef](./type_defs.md#typedlinkschemaandfacetnametypedef) 
4. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
6. See [:material-code-braces: ListOutgoingTypedLinksResponseTypeDef](./type_defs.md#listoutgoingtypedlinksresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOutgoingTypedLinksRequestPaginateTypeDef = {  # (1)
    "DirectoryArn": ...,
    "ObjectReference": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOutgoingTypedLinksRequestPaginateTypeDef](./type_defs.md#listoutgoingtypedlinksrequestpaginatetypedef) 
## ListPolicyAttachmentsPaginator

Type annotations and code completion for `#!python session.client("clouddirectory").get_paginator("list_policy_attachments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory/paginator/ListPolicyAttachments.html#CloudDirectory.Paginator.ListPolicyAttachments)

```python
# ListPolicyAttachmentsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.paginator import ListPolicyAttachmentsPaginator

session = Session()

session = get_session()
async with session.client("clouddirectory") as client:  # (1)
    paginator: ListPolicyAttachmentsPaginator = client.get_paginator("list_policy_attachments")  # (2)
    async for item in paginator.paginate(...):
        item: ListPolicyAttachmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListPolicyAttachmentsPaginator](./paginators.md#listpolicyattachmentspaginator)
3. item: [:material-code-braces: ListPolicyAttachmentsResponseTypeDef](./type_defs.md#listpolicyattachmentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPolicyAttachmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryArn: str,
    PolicyReference: ObjectReferenceTypeDef,  # (1)
    ConsistencyLevel: ConsistencyLevelType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListPolicyAttachmentsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-brackets: ConsistencyLevelType](./literals.md#consistencyleveltype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListPolicyAttachmentsResponseTypeDef](./type_defs.md#listpolicyattachmentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPolicyAttachmentsRequestPaginateTypeDef = {  # (1)
    "DirectoryArn": ...,
    "PolicyReference": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPolicyAttachmentsRequestPaginateTypeDef](./type_defs.md#listpolicyattachmentsrequestpaginatetypedef) 
## ListPublishedSchemaArnsPaginator

Type annotations and code completion for `#!python session.client("clouddirectory").get_paginator("list_published_schema_arns")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory/paginator/ListPublishedSchemaArns.html#CloudDirectory.Paginator.ListPublishedSchemaArns)

```python
# ListPublishedSchemaArnsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.paginator import ListPublishedSchemaArnsPaginator

session = Session()

session = get_session()
async with session.client("clouddirectory") as client:  # (1)
    paginator: ListPublishedSchemaArnsPaginator = client.get_paginator("list_published_schema_arns")  # (2)
    async for item in paginator.paginate(...):
        item: ListPublishedSchemaArnsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListPublishedSchemaArnsPaginator](./paginators.md#listpublishedschemaarnspaginator)
3. item: [:material-code-braces: ListPublishedSchemaArnsResponseTypeDef](./type_defs.md#listpublishedschemaarnsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPublishedSchemaArnsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SchemaArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPublishedSchemaArnsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPublishedSchemaArnsResponseTypeDef](./type_defs.md#listpublishedschemaarnsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPublishedSchemaArnsRequestPaginateTypeDef = {  # (1)
    "SchemaArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPublishedSchemaArnsRequestPaginateTypeDef](./type_defs.md#listpublishedschemaarnsrequestpaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.client("clouddirectory").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory/paginator/ListTagsForResource.html#CloudDirectory.Paginator.ListTagsForResource)

```python
# ListTagsForResourcePaginator usage example

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.paginator import ListTagsForResourcePaginator

session = Session()

session = get_session()
async with session.client("clouddirectory") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTagsForResourceRequestPaginateTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestPaginateTypeDef](./type_defs.md#listtagsforresourcerequestpaginatetypedef) 
## ListTypedLinkFacetAttributesPaginator

Type annotations and code completion for `#!python session.client("clouddirectory").get_paginator("list_typed_link_facet_attributes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory/paginator/ListTypedLinkFacetAttributes.html#CloudDirectory.Paginator.ListTypedLinkFacetAttributes)

```python
# ListTypedLinkFacetAttributesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.paginator import ListTypedLinkFacetAttributesPaginator

session = Session()

session = get_session()
async with session.client("clouddirectory") as client:  # (1)
    paginator: ListTypedLinkFacetAttributesPaginator = client.get_paginator("list_typed_link_facet_attributes")  # (2)
    async for item in paginator.paginate(...):
        item: ListTypedLinkFacetAttributesResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListTypedLinkFacetAttributesPaginator](./paginators.md#listtypedlinkfacetattributespaginator)
3. item: [:material-code-braces: ListTypedLinkFacetAttributesResponseTypeDef](./type_defs.md#listtypedlinkfacetattributesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTypedLinkFacetAttributesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SchemaArn: str,
    Name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTypedLinkFacetAttributesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTypedLinkFacetAttributesResponseTypeDef](./type_defs.md#listtypedlinkfacetattributesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTypedLinkFacetAttributesRequestPaginateTypeDef = {  # (1)
    "SchemaArn": ...,
    "Name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTypedLinkFacetAttributesRequestPaginateTypeDef](./type_defs.md#listtypedlinkfacetattributesrequestpaginatetypedef) 
## ListTypedLinkFacetNamesPaginator

Type annotations and code completion for `#!python session.client("clouddirectory").get_paginator("list_typed_link_facet_names")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory/paginator/ListTypedLinkFacetNames.html#CloudDirectory.Paginator.ListTypedLinkFacetNames)

```python
# ListTypedLinkFacetNamesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.paginator import ListTypedLinkFacetNamesPaginator

session = Session()

session = get_session()
async with session.client("clouddirectory") as client:  # (1)
    paginator: ListTypedLinkFacetNamesPaginator = client.get_paginator("list_typed_link_facet_names")  # (2)
    async for item in paginator.paginate(...):
        item: ListTypedLinkFacetNamesResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListTypedLinkFacetNamesPaginator](./paginators.md#listtypedlinkfacetnamespaginator)
3. item: [:material-code-braces: ListTypedLinkFacetNamesResponseTypeDef](./type_defs.md#listtypedlinkfacetnamesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTypedLinkFacetNamesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SchemaArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTypedLinkFacetNamesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTypedLinkFacetNamesResponseTypeDef](./type_defs.md#listtypedlinkfacetnamesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTypedLinkFacetNamesRequestPaginateTypeDef = {  # (1)
    "SchemaArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTypedLinkFacetNamesRequestPaginateTypeDef](./type_defs.md#listtypedlinkfacetnamesrequestpaginatetypedef) 
## LookupPolicyPaginator

Type annotations and code completion for `#!python session.client("clouddirectory").get_paginator("lookup_policy")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory/paginator/LookupPolicy.html#CloudDirectory.Paginator.LookupPolicy)

```python
# LookupPolicyPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_clouddirectory.paginator import LookupPolicyPaginator

session = Session()

session = get_session()
async with session.client("clouddirectory") as client:  # (1)
    paginator: LookupPolicyPaginator = client.get_paginator("lookup_policy")  # (2)
    async for item in paginator.paginate(...):
        item: LookupPolicyResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [LookupPolicyPaginator](./paginators.md#lookuppolicypaginator)
3. item: [:material-code-braces: LookupPolicyResponseTypeDef](./type_defs.md#lookuppolicyresponsetypedef) 


### paginate

Type annotations and code completion for `#!python LookupPolicyPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryArn: str,
    ObjectReference: ObjectReferenceTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[LookupPolicyResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ObjectReferenceTypeDef](./type_defs.md#objectreferencetypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: LookupPolicyResponseTypeDef](./type_defs.md#lookuppolicyresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: LookupPolicyRequestPaginateTypeDef = {  # (1)
    "DirectoryArn": ...,
    "ObjectReference": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: LookupPolicyRequestPaginateTypeDef](./type_defs.md#lookuppolicyrequestpaginatetypedef) 