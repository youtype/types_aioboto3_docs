# Examples

> [Index](../README.md) > [SSMContacts](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SSMContacts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
    type annotations stubs module [types-aiobotocore-ssm-contacts](https://pypi.org/project/types-aiobotocore-ssm-contacts/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[ssm-contacts]` package installed.

Write your `SSMContacts` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("ssm-contacts") as client:  # (1)
        result = await client.create_contact()  # (2)
    ```

    1. client: [SSMContactsClient](./client.md)
    2. result: [:material-code-braces: CreateContactResultTypeDef](./type_defs.md#createcontactresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("ssm-contacts") as client:  # (1)
        paginator = client.get_paginator("list_contact_channels")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [SSMContactsClient](./client.md)
    2. paginator: [ListContactChannelsPaginator](./paginators.md#listcontactchannelspaginator)
    3. item: [:material-code-braces: ListContactChannelsResultTypeDef](./type_defs.md#listcontactchannelsresulttypedef) 




### Explicit type annotations

With `types-aioboto3-lite[ssm-contacts]`
or a standalone `types_aiobotocore_ssm_contacts` package, you have to explicitly specify
`client: SSMContactsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_ssm_contacts.client import SSMContactsClient
    from types_aiobotocore_ssm_contacts.type_defs import CreateContactResultTypeDef
    from types_aiobotocore_ssm_contacts.type_defs import CreateContactRequestRequestTypeDef


    session = Session()

    client: SSMContactsClient
    async with session.client("ssm-contacts") as client:  # (1)
        kwargs: CreateContactRequestRequestTypeDef = {...}  # (2)
        result: CreateContactResultTypeDef = await client.create_contact(**kwargs)  # (3)
    ```

    1. client: [SSMContactsClient](./client.md)
    2. kwargs: [:material-code-braces: CreateContactRequestRequestTypeDef](./type_defs.md#createcontactrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateContactResultTypeDef](./type_defs.md#createcontactresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_ssm_contacts.client import SSMContactsClient
    from types_aiobotocore_ssm_contacts.paginator import ListContactChannelsPaginator
    from types_aiobotocore_ssm_contacts.type_defs import ListContactChannelsResultTypeDef


    session = Session()

    client: SSMContactsClient
    async with session.client("ssm-contacts") as client:  # (1)
        paginator: ListContactChannelsPaginator = client.get_paginator("list_contact_channels")  # (2)
        async for item in paginator.paginate(...):
            item: ListContactChannelsResultTypeDef
            print(item)  # (3)
    ```

    1. client: [SSMContactsClient](./client.md)
    2. paginator: [ListContactChannelsPaginator](./paginators.md#listcontactchannelspaginator)
    3. item: [:material-code-braces: ListContactChannelsResultTypeDef](./type_defs.md#listcontactchannelsresulttypedef) 



