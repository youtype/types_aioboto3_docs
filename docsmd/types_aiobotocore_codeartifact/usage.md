# Examples

> [Index](../README.md) > [CodeArtifact](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodeArtifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
    type annotations stubs module [types-aiobotocore-codeartifact](https://pypi.org/project/types-aiobotocore-codeartifact/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[codeartifact]` package installed.

Write your `CodeArtifact` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("codeartifact") as client:  # (1)
        result = await client.associate_external_connection()  # (2)
    ```

    1. client: [CodeArtifactClient](./client.md)
    2. result: [:material-code-braces: AssociateExternalConnectionResultTypeDef](./type_defs.md#associateexternalconnectionresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("codeartifact") as client:  # (1)
        paginator = client.get_paginator("list_domains")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [CodeArtifactClient](./client.md)
    2. paginator: [ListDomainsPaginator](./paginators.md#listdomainspaginator)
    3. item: [:material-code-braces: ListDomainsResultTypeDef](./type_defs.md#listdomainsresulttypedef) 




### Explicit type annotations

With `types-aioboto3-lite[codeartifact]`
or a standalone `types_aiobotocore_codeartifact` package, you have to explicitly specify
`client: CodeArtifactClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_codeartifact.client import CodeArtifactClient
    from types_aiobotocore_codeartifact.type_defs import AssociateExternalConnectionResultTypeDef
    from types_aiobotocore_codeartifact.type_defs import AssociateExternalConnectionRequestRequestTypeDef


    session = Session()

    client: CodeArtifactClient
    async with session.client("codeartifact") as client:  # (1)
        kwargs: AssociateExternalConnectionRequestRequestTypeDef = {...}  # (2)
        result: AssociateExternalConnectionResultTypeDef = await client.associate_external_connection(**kwargs)  # (3)
    ```

    1. client: [CodeArtifactClient](./client.md)
    2. kwargs: [:material-code-braces: AssociateExternalConnectionRequestRequestTypeDef](./type_defs.md#associateexternalconnectionrequestrequesttypedef) 
    3. result: [:material-code-braces: AssociateExternalConnectionResultTypeDef](./type_defs.md#associateexternalconnectionresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_codeartifact.client import CodeArtifactClient
    from types_aiobotocore_codeartifact.paginator import ListDomainsPaginator
    from types_aiobotocore_codeartifact.type_defs import ListDomainsResultTypeDef


    session = Session()

    client: CodeArtifactClient
    async with session.client("codeartifact") as client:  # (1)
        paginator: ListDomainsPaginator = client.get_paginator("list_domains")  # (2)
        async for item in paginator.paginate(...):
            item: ListDomainsResultTypeDef
            print(item)  # (3)
    ```

    1. client: [CodeArtifactClient](./client.md)
    2. paginator: [ListDomainsPaginator](./paginators.md#listdomainspaginator)
    3. item: [:material-code-braces: ListDomainsResultTypeDef](./type_defs.md#listdomainsresulttypedef) 




