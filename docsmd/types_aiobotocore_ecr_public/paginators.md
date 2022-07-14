# Paginators

> [Index](../README.md) > [ECRPublic](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ECRPublic](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
    type annotations stubs module [types-aiobotocore-ecr-public](https://pypi.org/project/types-aiobotocore-ecr-public/).

## DescribeImageTagsPaginator

Type annotations and code completion for `#!python session.client("ecr-public").get_paginator("describe_image_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImageTags)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_ecr_public.paginator import DescribeImageTagsPaginator

session = Session()

session = get_session()
async with session.client("ecr-public") as client:  # (1)
    paginator: DescribeImageTagsPaginator = client.get_paginator("describe_image_tags")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeImageTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [ECRPublicClient](./client.md)
2. paginator: [DescribeImageTagsPaginator](./paginators.md#describeimagetagspaginator)
3. item: [:material-code-braces: DescribeImageTagsResponseTypeDef](./type_defs.md#describeimagetagsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeImageTagsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    repositoryName: str,
    registryId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeImageTagsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeImageTagsResponseTypeDef](./type_defs.md#describeimagetagsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef = {  # (1)
    "repositoryName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef](./type_defs.md#describeimagetagsrequestdescribeimagetagspaginatetypedef) 
## DescribeImagesPaginator

Type annotations and code completion for `#!python session.client("ecr-public").get_paginator("describe_images")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeImages)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_ecr_public.paginator import DescribeImagesPaginator

session = Session()

session = get_session()
async with session.client("ecr-public") as client:  # (1)
    paginator: DescribeImagesPaginator = client.get_paginator("describe_images")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeImagesResponseTypeDef
        print(item)  # (3)
```

1. client: [ECRPublicClient](./client.md)
2. paginator: [DescribeImagesPaginator](./paginators.md#describeimagespaginator)
3. item: [:material-code-braces: DescribeImagesResponseTypeDef](./type_defs.md#describeimagesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeImagesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    repositoryName: str,
    registryId: str = ...,
    imageIds: Sequence[ImageIdentifierTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeImagesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeImagesResponseTypeDef](./type_defs.md#describeimagesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeImagesRequestDescribeImagesPaginateTypeDef = {  # (1)
    "repositoryName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImagesRequestDescribeImagesPaginateTypeDef](./type_defs.md#describeimagesrequestdescribeimagespaginatetypedef) 
## DescribeRegistriesPaginator

Type annotations and code completion for `#!python session.client("ecr-public").get_paginator("describe_registries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRegistries)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_ecr_public.paginator import DescribeRegistriesPaginator

session = Session()

session = get_session()
async with session.client("ecr-public") as client:  # (1)
    paginator: DescribeRegistriesPaginator = client.get_paginator("describe_registries")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRegistriesResponseTypeDef
        print(item)  # (3)
```

1. client: [ECRPublicClient](./client.md)
2. paginator: [DescribeRegistriesPaginator](./paginators.md#describeregistriespaginator)
3. item: [:material-code-braces: DescribeRegistriesResponseTypeDef](./type_defs.md#describeregistriesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeRegistriesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeRegistriesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeRegistriesResponseTypeDef](./type_defs.md#describeregistriesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef](./type_defs.md#describeregistriesrequestdescriberegistriespaginatetypedef) 
## DescribeRepositoriesPaginator

Type annotations and code completion for `#!python session.client("ecr-public").get_paginator("describe_repositories")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic.Paginator.DescribeRepositories)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_ecr_public.paginator import DescribeRepositoriesPaginator

session = Session()

session = get_session()
async with session.client("ecr-public") as client:  # (1)
    paginator: DescribeRepositoriesPaginator = client.get_paginator("describe_repositories")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRepositoriesResponseTypeDef
        print(item)  # (3)
```

1. client: [ECRPublicClient](./client.md)
2. paginator: [DescribeRepositoriesPaginator](./paginators.md#describerepositoriespaginator)
3. item: [:material-code-braces: DescribeRepositoriesResponseTypeDef](./type_defs.md#describerepositoriesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeRepositoriesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    registryId: str = ...,
    repositoryNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeRepositoriesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeRepositoriesResponseTypeDef](./type_defs.md#describerepositoriesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = {  # (1)
    "registryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef](./type_defs.md#describerepositoriesrequestdescriberepositoriespaginatetypedef) 
