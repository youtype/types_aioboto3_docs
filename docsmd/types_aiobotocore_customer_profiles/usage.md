# Examples

> [Index](../README.md) > [CustomerProfiles](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CustomerProfiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
    type annotations stubs module [types-aiobotocore-customer-profiles](https://pypi.org/project/types-aiobotocore-customer-profiles/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[customer-profiles]` package installed.

Write your `CustomerProfiles` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("customer-profiles") as client:  # (1)
        result = await client.add_profile_key()  # (2)
    ```

    1. client: [CustomerProfilesClient](./client.md)
    2. result: [:material-code-braces: AddProfileKeyResponseTypeDef](./type_defs.md#addprofilekeyresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[customer-profiles]`
or a standalone `types_aiobotocore_customer_profiles` package, you have to explicitly specify
`client: CustomerProfilesClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_customer_profiles.client import CustomerProfilesClient
    from types_aiobotocore_customer_profiles.type_defs import AddProfileKeyResponseTypeDef
    from types_aiobotocore_customer_profiles.type_defs import AddProfileKeyRequestRequestTypeDef


    session = Session()

    client: CustomerProfilesClient
    async with session.client("customer-profiles") as client:  # (1)
        kwargs: AddProfileKeyRequestRequestTypeDef = {...}  # (2)
        result: AddProfileKeyResponseTypeDef = await client.add_profile_key(**kwargs)  # (3)
    ```

    1. client: [CustomerProfilesClient](./client.md)
    2. kwargs: [:material-code-braces: AddProfileKeyRequestRequestTypeDef](./type_defs.md#addprofilekeyrequestrequesttypedef) 
    3. result: [:material-code-braces: AddProfileKeyResponseTypeDef](./type_defs.md#addprofilekeyresponsetypedef) 






