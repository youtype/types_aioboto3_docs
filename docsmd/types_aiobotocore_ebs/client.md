# EBSClient

> [Index](../README.md) > [EBS](./README.md) > EBSClient

!!! note ""

    Auto-generated documentation for [EBS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#ebs)
    type annotations stubs module [types-aiobotocore-ebs](https://pypi.org/project/types-aiobotocore-ebs/).

## EBSClient

Type annotations and code completion for `#!python session.client("ebs")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client)

```python
# EBSClient usage example

from aioboto3.session import Session
from types_aiobotocore_ebs.client import EBSClient

session = Session()
async with session.client("ebs") as client:
    client: EBSClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("ebs").exceptions` structure.

```python
# EBSClient.exceptions usage example

async with session.client("ebs") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConcurrentLimitExceededException,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.RequestThrottledException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# EBSClient.exceptions type checking example

from types_aiobotocore_ebs.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("ebs").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("ebs").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### complete\_snapshot

Seals and completes the snapshot after all of the required blocks of data have
been written to it.

Type annotations and code completion for `#!python session.client("ebs").complete_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client)

```python
# complete_snapshot method definition

await def complete_snapshot(
    self,
    *,
    SnapshotId: str,
    ChangedBlocksCount: int,
    Checksum: str = ...,
    ChecksumAlgorithm: ChecksumAlgorithmType = ...,  # (1)
    ChecksumAggregationMethod: ChecksumAggregationMethodType = ...,  # (2)
) -> CompleteSnapshotResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
2. See [:material-code-brackets: ChecksumAggregationMethodType](./literals.md#checksumaggregationmethodtype) 
3. See [:material-code-braces: CompleteSnapshotResponseTypeDef](./type_defs.md#completesnapshotresponsetypedef) 


```python
# complete_snapshot method usage example with argument unpacking

kwargs: CompleteSnapshotRequestRequestTypeDef = {  # (1)
    "SnapshotId": ...,
    "ChangedBlocksCount": ...,
}

parent.complete_snapshot(**kwargs)
```

1. See [:material-code-braces: CompleteSnapshotRequestRequestTypeDef](./type_defs.md#completesnapshotrequestrequesttypedef) 

### get\_snapshot\_block

Returns the data in a block in an Amazon Elastic Block Store snapshot.

Type annotations and code completion for `#!python session.client("ebs").get_snapshot_block` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client)

```python
# get_snapshot_block method definition

await def get_snapshot_block(
    self,
    *,
    SnapshotId: str,
    BlockIndex: int,
    BlockToken: str,
) -> GetSnapshotBlockResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSnapshotBlockResponseTypeDef](./type_defs.md#getsnapshotblockresponsetypedef) 


```python
# get_snapshot_block method usage example with argument unpacking

kwargs: GetSnapshotBlockRequestRequestTypeDef = {  # (1)
    "SnapshotId": ...,
    "BlockIndex": ...,
    "BlockToken": ...,
}

parent.get_snapshot_block(**kwargs)
```

1. See [:material-code-braces: GetSnapshotBlockRequestRequestTypeDef](./type_defs.md#getsnapshotblockrequestrequesttypedef) 

### list\_changed\_blocks

Returns information about the blocks that are different between two Amazon
Elastic Block Store snapshots of the same volume/snapshot lineage.

Type annotations and code completion for `#!python session.client("ebs").list_changed_blocks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client)

```python
# list_changed_blocks method definition

await def list_changed_blocks(
    self,
    *,
    SecondSnapshotId: str,
    FirstSnapshotId: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    StartingBlockIndex: int = ...,
) -> ListChangedBlocksResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListChangedBlocksResponseTypeDef](./type_defs.md#listchangedblocksresponsetypedef) 


```python
# list_changed_blocks method usage example with argument unpacking

kwargs: ListChangedBlocksRequestRequestTypeDef = {  # (1)
    "SecondSnapshotId": ...,
}

parent.list_changed_blocks(**kwargs)
```

1. See [:material-code-braces: ListChangedBlocksRequestRequestTypeDef](./type_defs.md#listchangedblocksrequestrequesttypedef) 

### list\_snapshot\_blocks

Returns information about the blocks in an Amazon Elastic Block Store snapshot.

Type annotations and code completion for `#!python session.client("ebs").list_snapshot_blocks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client)

```python
# list_snapshot_blocks method definition

await def list_snapshot_blocks(
    self,
    *,
    SnapshotId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    StartingBlockIndex: int = ...,
) -> ListSnapshotBlocksResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSnapshotBlocksResponseTypeDef](./type_defs.md#listsnapshotblocksresponsetypedef) 


```python
# list_snapshot_blocks method usage example with argument unpacking

kwargs: ListSnapshotBlocksRequestRequestTypeDef = {  # (1)
    "SnapshotId": ...,
}

parent.list_snapshot_blocks(**kwargs)
```

1. See [:material-code-braces: ListSnapshotBlocksRequestRequestTypeDef](./type_defs.md#listsnapshotblocksrequestrequesttypedef) 

### put\_snapshot\_block

Writes a block of data to a snapshot.

Type annotations and code completion for `#!python session.client("ebs").put_snapshot_block` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client)

```python
# put_snapshot_block method definition

await def put_snapshot_block(
    self,
    *,
    SnapshotId: str,
    BlockIndex: int,
    BlockData: BlobTypeDef,
    DataLength: int,
    Checksum: str,
    ChecksumAlgorithm: ChecksumAlgorithmType,  # (1)
    Progress: int = ...,
) -> PutSnapshotBlockResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
2. See [:material-code-braces: PutSnapshotBlockResponseTypeDef](./type_defs.md#putsnapshotblockresponsetypedef) 


```python
# put_snapshot_block method usage example with argument unpacking

kwargs: PutSnapshotBlockRequestRequestTypeDef = {  # (1)
    "SnapshotId": ...,
    "BlockIndex": ...,
    "BlockData": ...,
    "DataLength": ...,
    "Checksum": ...,
    "ChecksumAlgorithm": ...,
}

parent.put_snapshot_block(**kwargs)
```

1. See [:material-code-braces: PutSnapshotBlockRequestRequestTypeDef](./type_defs.md#putsnapshotblockrequestrequesttypedef) 

### start\_snapshot

Creates a new Amazon EBS snapshot.

Type annotations and code completion for `#!python session.client("ebs").start_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client)

```python
# start_snapshot method definition

await def start_snapshot(
    self,
    *,
    VolumeSize: int,
    ParentSnapshotId: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    Description: str = ...,
    ClientToken: str = ...,
    Encrypted: bool = ...,
    KmsKeyArn: str = ...,
    Timeout: int = ...,
) -> StartSnapshotResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: StartSnapshotResponseTypeDef](./type_defs.md#startsnapshotresponsetypedef) 


```python
# start_snapshot method usage example with argument unpacking

kwargs: StartSnapshotRequestRequestTypeDef = {  # (1)
    "VolumeSize": ...,
}

parent.start_snapshot(**kwargs)
```

1. See [:material-code-braces: StartSnapshotRequestRequestTypeDef](./type_defs.md#startsnapshotrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("ebs").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("ebs").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




