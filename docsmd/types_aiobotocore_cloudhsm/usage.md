# Examples

> [Index](../README.md) > [CloudHSM](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudHSM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
    type annotations stubs module [types-aiobotocore-cloudhsm](https://pypi.org/project/types-aiobotocore-cloudhsm/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[cloudhsm]` package installed.

Write your `CloudHSM` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cloudhsm") as client:  # (1)
        result = await client.add_tags_to_resource()  # (2)
    ```

    1. client: [CloudHSMClient](./client.md)
    2. result: [:material-code-braces: AddTagsToResourceResponseTypeDef](./type_defs.md#addtagstoresourceresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cloudhsm") as client:  # (1)
        paginator = client.get_paginator("list_hapgs")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [CloudHSMClient](./client.md)
    2. paginator: [ListHapgsPaginator](./paginators.md#listhapgspaginator)
    3. item: [:material-code-braces: ListHapgsResponseTypeDef](./type_defs.md#listhapgsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[cloudhsm]`
or a standalone `types_aiobotocore_cloudhsm` package, you have to explicitly specify
`client: CloudHSMClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudhsm.client import CloudHSMClient
    from types_aiobotocore_cloudhsm.type_defs import AddTagsToResourceResponseTypeDef
    from types_aiobotocore_cloudhsm.type_defs import AddTagsToResourceRequestRequestTypeDef


    session = Session()

    client: CloudHSMClient
    async with session.client("cloudhsm") as client:  # (1)
        kwargs: AddTagsToResourceRequestRequestTypeDef = {...}  # (2)
        result: AddTagsToResourceResponseTypeDef = await client.add_tags_to_resource(**kwargs)  # (3)
    ```

    1. client: [CloudHSMClient](./client.md)
    2. kwargs: [:material-code-braces: AddTagsToResourceRequestRequestTypeDef](./type_defs.md#addtagstoresourcerequestrequesttypedef) 
    3. result: [:material-code-braces: AddTagsToResourceResponseTypeDef](./type_defs.md#addtagstoresourceresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudhsm.client import CloudHSMClient
    from types_aiobotocore_cloudhsm.paginator import ListHapgsPaginator
    from types_aiobotocore_cloudhsm.type_defs import ListHapgsResponseTypeDef


    session = Session()

    client: CloudHSMClient
    async with session.client("cloudhsm") as client:  # (1)
        paginator: ListHapgsPaginator = client.get_paginator("list_hapgs")  # (2)
        async for item in paginator.paginate(...):
            item: ListHapgsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [CloudHSMClient](./client.md)
    2. paginator: [ListHapgsPaginator](./paginators.md#listhapgspaginator)
    3. item: [:material-code-braces: ListHapgsResponseTypeDef](./type_defs.md#listhapgsresponsetypedef) 




