# Examples

> [Index](../README.md) > [Firehose](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Firehose](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
    type annotations stubs module [types-aiobotocore-firehose](https://pypi.org/project/types-aiobotocore-firehose/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[firehose]` package installed.

Write your `Firehose` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("firehose") as client:  # (1)
        result = await client.create_delivery_stream()  # (2)
    ```

    1. client: [FirehoseClient](./client.md)
    2. result: [:material-code-braces: CreateDeliveryStreamOutputTypeDef](./type_defs.md#createdeliverystreamoutputtypedef) 






### Explicit type annotations

With `types-aioboto3-lite[firehose]`
or a standalone `types_aiobotocore_firehose` package, you have to explicitly specify
`client: FirehoseClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_firehose.client import FirehoseClient
    from types_aiobotocore_firehose.type_defs import CreateDeliveryStreamOutputTypeDef
    from types_aiobotocore_firehose.type_defs import CreateDeliveryStreamInputRequestTypeDef


    session = Session()

    client: FirehoseClient
    async with session.client("firehose") as client:  # (1)
        kwargs: CreateDeliveryStreamInputRequestTypeDef = {...}  # (2)
        result: CreateDeliveryStreamOutputTypeDef = await client.create_delivery_stream(**kwargs)  # (3)
    ```

    1. client: [FirehoseClient](./client.md)
    2. kwargs: [:material-code-braces: CreateDeliveryStreamInputRequestTypeDef](./type_defs.md#createdeliverystreaminputrequesttypedef) 
    3. result: [:material-code-braces: CreateDeliveryStreamOutputTypeDef](./type_defs.md#createdeliverystreamoutputtypedef) 






