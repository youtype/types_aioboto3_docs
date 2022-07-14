# Examples

> [Index](../README.md) > [CodeBuild](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodeBuild](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
    type annotations stubs module [types-aiobotocore-codebuild](https://pypi.org/project/types-aiobotocore-codebuild/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[codebuild]` package installed.

Write your `CodeBuild` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("codebuild") as client:  # (1)
        result = await client.batch_delete_builds()  # (2)
    ```

    1. client: [CodeBuildClient](./client.md)
    2. result: [:material-code-braces: BatchDeleteBuildsOutputTypeDef](./type_defs.md#batchdeletebuildsoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("codebuild") as client:  # (1)
        paginator = client.get_paginator("describe_code_coverages")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [CodeBuildClient](./client.md)
    2. paginator: [DescribeCodeCoveragesPaginator](./paginators.md#describecodecoveragespaginator)
    3. item: [:material-code-braces: DescribeCodeCoveragesOutputTypeDef](./type_defs.md#describecodecoveragesoutputtypedef) 




### Explicit type annotations

With `types-aioboto3-lite[codebuild]`
or a standalone `types_aiobotocore_codebuild` package, you have to explicitly specify
`client: CodeBuildClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_codebuild.client import CodeBuildClient
    from types_aiobotocore_codebuild.type_defs import BatchDeleteBuildsOutputTypeDef
    from types_aiobotocore_codebuild.type_defs import BatchDeleteBuildsInputRequestTypeDef


    session = Session()

    client: CodeBuildClient
    async with session.client("codebuild") as client:  # (1)
        kwargs: BatchDeleteBuildsInputRequestTypeDef = {...}  # (2)
        result: BatchDeleteBuildsOutputTypeDef = await client.batch_delete_builds(**kwargs)  # (3)
    ```

    1. client: [CodeBuildClient](./client.md)
    2. kwargs: [:material-code-braces: BatchDeleteBuildsInputRequestTypeDef](./type_defs.md#batchdeletebuildsinputrequesttypedef) 
    3. result: [:material-code-braces: BatchDeleteBuildsOutputTypeDef](./type_defs.md#batchdeletebuildsoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_codebuild.client import CodeBuildClient
    from types_aiobotocore_codebuild.paginator import DescribeCodeCoveragesPaginator
    from types_aiobotocore_codebuild.type_defs import DescribeCodeCoveragesOutputTypeDef


    session = Session()

    client: CodeBuildClient
    async with session.client("codebuild") as client:  # (1)
        paginator: DescribeCodeCoveragesPaginator = client.get_paginator("describe_code_coverages")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeCodeCoveragesOutputTypeDef
            print(item)  # (3)
    ```

    1. client: [CodeBuildClient](./client.md)
    2. paginator: [DescribeCodeCoveragesPaginator](./paginators.md#describecodecoveragespaginator)
    3. item: [:material-code-braces: DescribeCodeCoveragesOutputTypeDef](./type_defs.md#describecodecoveragesoutputtypedef) 




