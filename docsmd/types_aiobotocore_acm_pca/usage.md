# Examples

> [Index](../README.md) > [ACMPCA](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ACMPCA](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
    type annotations stubs module [types-aiobotocore-acm-pca](https://pypi.org/project/types-aiobotocore-acm-pca/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[acm-pca]` package installed.

Write your `ACMPCA` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("acm-pca") as client:  # (1)
        result = await client.create_certificate_authority()  # (2)
    ```

    1. client: [ACMPCAClient](./client.md)
    2. result: [:material-code-braces: CreateCertificateAuthorityResponseTypeDef](./type_defs.md#createcertificateauthorityresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("acm-pca") as client:  # (1)
        paginator = client.get_paginator("list_certificate_authorities")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [ACMPCAClient](./client.md)
    2. paginator: [ListCertificateAuthoritiesPaginator](./paginators.md#listcertificateauthoritiespaginator)
    3. item: [:material-code-braces: ListCertificateAuthoritiesResponseTypeDef](./type_defs.md#listcertificateauthoritiesresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("acm-pca") as client:  # (1)
        waiter = client.get_waiter("audit_report_created")  # (2)
        await waiter.wait()
    ```

    1. client: [ACMPCAClient](./client.md)
    2. waiter: [AuditReportCreatedWaiter](./waiters.md#auditreportcreatedwaiter)


### Explicit type annotations

With `types-aioboto3-lite[acm-pca]`
or a standalone `types_aiobotocore_acm_pca` package, you have to explicitly specify
`client: ACMPCAClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_acm_pca.client import ACMPCAClient
    from types_aiobotocore_acm_pca.type_defs import CreateCertificateAuthorityResponseTypeDef
    from types_aiobotocore_acm_pca.type_defs import CreateCertificateAuthorityRequestRequestTypeDef


    session = Session()

    client: ACMPCAClient
    async with session.client("acm-pca") as client:  # (1)
        kwargs: CreateCertificateAuthorityRequestRequestTypeDef = {...}  # (2)
        result: CreateCertificateAuthorityResponseTypeDef = await client.create_certificate_authority(**kwargs)  # (3)
    ```

    1. client: [ACMPCAClient](./client.md)
    2. kwargs: [:material-code-braces: CreateCertificateAuthorityRequestRequestTypeDef](./type_defs.md#createcertificateauthorityrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateCertificateAuthorityResponseTypeDef](./type_defs.md#createcertificateauthorityresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_acm_pca.client import ACMPCAClient
    from types_aiobotocore_acm_pca.paginator import ListCertificateAuthoritiesPaginator
    from types_aiobotocore_acm_pca.type_defs import ListCertificateAuthoritiesResponseTypeDef


    session = Session()

    client: ACMPCAClient
    async with session.client("acm-pca") as client:  # (1)
        paginator: ListCertificateAuthoritiesPaginator = client.get_paginator("list_certificate_authorities")  # (2)
        async for item in paginator.paginate(...):
            item: ListCertificateAuthoritiesResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [ACMPCAClient](./client.md)
    2. paginator: [ListCertificateAuthoritiesPaginator](./paginators.md#listcertificateauthoritiespaginator)
    3. item: [:material-code-braces: ListCertificateAuthoritiesResponseTypeDef](./type_defs.md#listcertificateauthoritiesresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_acm_pca.client import ACMPCAClient
    from types_aiobotocore_acm_pca.waiter import AuditReportCreatedWaiter


    session = Session()

    async with session.client("acm-pca") as client:  # (1)
        waiter = client.get_waiter("audit_report_created")  # (2)
        await waiter.wait()
    ```

    1. client: [ACMPCAClient](./client.md)
    2. waiter: [AuditReportCreatedWaiter](./waiters.md#auditreportcreatedwaiter)


