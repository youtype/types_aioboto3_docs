# Examples

> [Index](../README.md) > [CloudFront](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudFront](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
    type annotations stubs module [types-aiobotocore-cloudfront](https://pypi.org/project/types-aiobotocore-cloudfront/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[cloudfront]` package installed.

Write your `CloudFront` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cloudfront") as client:  # (1)
        result = await client.associate_alias()  # (2)
    ```

    1. client: [CloudFrontClient](./client.md)
    2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cloudfront") as client:  # (1)
        paginator = client.get_paginator("list_cloud_front_origin_access_identities")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [CloudFrontClient](./client.md)
    2. paginator: [ListCloudFrontOriginAccessIdentitiesPaginator](./paginators.md#listcloudfrontoriginaccessidentitiespaginator)
    3. item: [:material-code-braces: ListCloudFrontOriginAccessIdentitiesResultTypeDef](./type_defs.md#listcloudfrontoriginaccessidentitiesresulttypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cloudfront") as client:  # (1)
        waiter = client.get_waiter("distribution_deployed")  # (2)
        await waiter.wait()
    ```

    1. client: [CloudFrontClient](./client.md)
    2. waiter: [DistributionDeployedWaiter](./waiters.md#distributiondeployedwaiter)


### Explicit type annotations

With `types-aioboto3-lite[cloudfront]`
or a standalone `types_aiobotocore_cloudfront` package, you have to explicitly specify
`client: CloudFrontClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudfront.client import CloudFrontClient
    from types_aiobotocore_cloudfront.type_defs import EmptyResponseMetadataTypeDef
    from types_aiobotocore_cloudfront.type_defs import AssociateAliasRequestRequestTypeDef


    session = Session()

    client: CloudFrontClient
    async with session.client("cloudfront") as client:  # (1)
        kwargs: AssociateAliasRequestRequestTypeDef = {...}  # (2)
        result: EmptyResponseMetadataTypeDef = await client.associate_alias(**kwargs)  # (3)
    ```

    1. client: [CloudFrontClient](./client.md)
    2. kwargs: [:material-code-braces: AssociateAliasRequestRequestTypeDef](./type_defs.md#associatealiasrequestrequesttypedef) 
    3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudfront.client import CloudFrontClient
    from types_aiobotocore_cloudfront.paginator import ListCloudFrontOriginAccessIdentitiesPaginator
    from types_aiobotocore_cloudfront.type_defs import ListCloudFrontOriginAccessIdentitiesResultTypeDef


    session = Session()

    client: CloudFrontClient
    async with session.client("cloudfront") as client:  # (1)
        paginator: ListCloudFrontOriginAccessIdentitiesPaginator = client.get_paginator("list_cloud_front_origin_access_identities")  # (2)
        async for item in paginator.paginate(...):
            item: ListCloudFrontOriginAccessIdentitiesResultTypeDef
            print(item)  # (3)
    ```

    1. client: [CloudFrontClient](./client.md)
    2. paginator: [ListCloudFrontOriginAccessIdentitiesPaginator](./paginators.md#listcloudfrontoriginaccessidentitiespaginator)
    3. item: [:material-code-braces: ListCloudFrontOriginAccessIdentitiesResultTypeDef](./type_defs.md#listcloudfrontoriginaccessidentitiesresulttypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudfront.client import CloudFrontClient
    from types_aiobotocore_cloudfront.waiter import DistributionDeployedWaiter


    session = Session()

    async with session.client("cloudfront") as client:  # (1)
        waiter = client.get_waiter("distribution_deployed")  # (2)
        await waiter.wait()
    ```

    1. client: [CloudFrontClient](./client.md)
    2. waiter: [DistributionDeployedWaiter](./waiters.md#distributiondeployedwaiter)


