# Examples

> [Index](../README.md) > [Kafka](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Kafka](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
    type annotations stubs module [types-aiobotocore-kafka](https://pypi.org/project/types-aiobotocore-kafka/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[kafka]` package installed.

Write your `Kafka` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("kafka") as client:  # (1)
        result = await client.batch_associate_scram_secret()  # (2)
    ```

    1. client: [KafkaClient](./client.md)
    2. result: [:material-code-braces: BatchAssociateScramSecretResponseTypeDef](./type_defs.md#batchassociatescramsecretresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("kafka") as client:  # (1)
        paginator = client.get_paginator("list_cluster_operations")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [KafkaClient](./client.md)
    2. paginator: [ListClusterOperationsPaginator](./paginators.md#listclusteroperationspaginator)
    3. item: [:material-code-braces: ListClusterOperationsResponseTypeDef](./type_defs.md#listclusteroperationsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[kafka]`
or a standalone `types_aiobotocore_kafka` package, you have to explicitly specify
`client: KafkaClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_kafka.client import KafkaClient
    from types_aiobotocore_kafka.type_defs import BatchAssociateScramSecretResponseTypeDef
    from types_aiobotocore_kafka.type_defs import BatchAssociateScramSecretRequestRequestTypeDef


    session = Session()

    client: KafkaClient
    async with session.client("kafka") as client:  # (1)
        kwargs: BatchAssociateScramSecretRequestRequestTypeDef = {...}  # (2)
        result: BatchAssociateScramSecretResponseTypeDef = await client.batch_associate_scram_secret(**kwargs)  # (3)
    ```

    1. client: [KafkaClient](./client.md)
    2. kwargs: [:material-code-braces: BatchAssociateScramSecretRequestRequestTypeDef](./type_defs.md#batchassociatescramsecretrequestrequesttypedef) 
    3. result: [:material-code-braces: BatchAssociateScramSecretResponseTypeDef](./type_defs.md#batchassociatescramsecretresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_kafka.client import KafkaClient
    from types_aiobotocore_kafka.paginator import ListClusterOperationsPaginator
    from types_aiobotocore_kafka.type_defs import ListClusterOperationsResponseTypeDef


    session = Session()

    client: KafkaClient
    async with session.client("kafka") as client:  # (1)
        paginator: ListClusterOperationsPaginator = client.get_paginator("list_cluster_operations")  # (2)
        async for item in paginator.paginate(...):
            item: ListClusterOperationsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [KafkaClient](./client.md)
    2. paginator: [ListClusterOperationsPaginator](./paginators.md#listclusteroperationspaginator)
    3. item: [:material-code-braces: ListClusterOperationsResponseTypeDef](./type_defs.md#listclusteroperationsresponsetypedef) 




