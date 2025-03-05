# DynamoDBStreams module

> [Index](../README.md) > DynamoDBStreams


!!! note ""

    Auto-generated documentation for [DynamoDBStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#dynamodbstreams)
    type annotations stubs module [types-aiobotocore-dynamodbstreams](https://pypi.org/project/types-aiobotocore-dynamodbstreams/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==14.1.0' mypy-boto3-builder`
1. Select `aioboto3` AWS SDK.
1. Add `DynamoDBStreams` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `DynamoDBStreams` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[dynamodbstreams]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[dynamodbstreams]'

# standalone installation
python -m pip install types-aiobotocore-dynamodbstreams
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-dynamodbstreams
```

## Usage

Code samples can be found in [Examples](./usage.md).

## DynamoDBStreamsClient

Type annotations and code completion for  `#!python session.client("dynamodbstreams")` as [DynamoDBStreamsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client)

```python
# DynamoDBStreamsClient usage example

from aioboto3.session import Session

from types_aiobotocore_dynamodbstreams.client import DynamoDBStreamsClient


session = Session()
async with session.client("dynamodbstreams") as client:
    client: DynamoDBStreamsClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# KeyTypeType usage example

from types_aiobotocore_dynamodbstreams.literals import KeyTypeType

def get_value() -> KeyTypeType:
    return "HASH"
```

- [KeyTypeType](./literals.md#keytypetype)
- [OperationTypeType](./literals.md#operationtypetype)
- [ShardIteratorTypeType](./literals.md#sharditeratortypetype)
- [StreamStatusType](./literals.md#streamstatustype)
- [StreamViewTypeType](./literals.md#streamviewtypetype)
- [DynamoDBStreamsServiceName](./literals.md#dynamodbstreamsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AttributeValueTypeDef](./type_defs.md#attributevaluetypedef)
- [DescribeStreamInputTypeDef](./type_defs.md#describestreaminputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetRecordsInputTypeDef](./type_defs.md#getrecordsinputtypedef)
- [GetShardIteratorInputTypeDef](./type_defs.md#getsharditeratorinputtypedef)
- [IdentityTypeDef](./type_defs.md#identitytypedef)
- [KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef)
- [ListStreamsInputTypeDef](./type_defs.md#liststreamsinputtypedef)
- [StreamTypeDef](./type_defs.md#streamtypedef)
- [SequenceNumberRangeTypeDef](./type_defs.md#sequencenumberrangetypedef)
- [StreamRecordTypeDef](./type_defs.md#streamrecordtypedef)
- [GetShardIteratorOutputTypeDef](./type_defs.md#getsharditeratoroutputtypedef)
- [ListStreamsOutputTypeDef](./type_defs.md#liststreamsoutputtypedef)
- [ShardTypeDef](./type_defs.md#shardtypedef)
- [RecordTypeDef](./type_defs.md#recordtypedef)
- [StreamDescriptionTypeDef](./type_defs.md#streamdescriptiontypedef)
- [GetRecordsOutputTypeDef](./type_defs.md#getrecordsoutputtypedef)
- [DescribeStreamOutputTypeDef](./type_defs.md#describestreamoutputtypedef)

