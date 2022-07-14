# Examples

> [Index](../README.md) > [CloudSearchDomain](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudSearchDomain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
    type annotations stubs module [types-aiobotocore-cloudsearchdomain](https://pypi.org/project/types-aiobotocore-cloudsearchdomain/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[cloudsearchdomain]` package installed.

Write your `CloudSearchDomain` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cloudsearchdomain") as client:  # (1)
        result = await client.search()  # (2)
    ```

    1. client: [CloudSearchDomainClient](./client.md)
    2. result: [:material-code-braces: SearchResponseTypeDef](./type_defs.md#searchresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[cloudsearchdomain]`
or a standalone `types_aiobotocore_cloudsearchdomain` package, you have to explicitly specify
`client: CloudSearchDomainClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudsearchdomain.client import CloudSearchDomainClient
    from types_aiobotocore_cloudsearchdomain.type_defs import SearchResponseTypeDef
    from types_aiobotocore_cloudsearchdomain.type_defs import SearchRequestRequestTypeDef


    session = Session()

    client: CloudSearchDomainClient
    async with session.client("cloudsearchdomain") as client:  # (1)
        kwargs: SearchRequestRequestTypeDef = {...}  # (2)
        result: SearchResponseTypeDef = await client.search(**kwargs)  # (3)
    ```

    1. client: [CloudSearchDomainClient](./client.md)
    2. kwargs: [:material-code-braces: SearchRequestRequestTypeDef](./type_defs.md#searchrequestrequesttypedef) 
    3. result: [:material-code-braces: SearchResponseTypeDef](./type_defs.md#searchresponsetypedef) 






