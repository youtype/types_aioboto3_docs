# DynamoDBServiceResource

> [Index](../README.md) > [DynamoDB](./README.md) > DynamoDBServiceResource

!!! note ""

    Auto-generated documentation for [DynamoDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
    type annotations stubs module [types-aiobotocore-dynamodb](https://pypi.org/project/types-aiobotocore-dynamodb/).

## DynamoDBServiceResource

Type annotations and code completion for `#!python session.resource("dynamodb")`, included resources and collections.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource)

```python title="Usage example"
from aioboto3.session import Session
from types_aiobotocore_dynamodb.service_resource import DynamoDBServiceResource

session = Session()
async with session.resource("dynamodb") as resource:
    resource: DynamoDBServiceResource
```


## Attributes


- `meta`: [DynamoDBResourceMeta](#dynamodbresourcemeta)

- `tables`: [ServiceResourceTablesCollection](#serviceresourcetablescollection)




## Collections

### ServiceResourceTablesCollection

Provides access to [Table](#table) resource.

Type annotations and code completion for `#!python session.resource("dynamodb").tables` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.tables)

```python title="Usage example"
from types_aiobotocore_dynamodb.service_resource import ServiceResourceTablesCollection,

def get_collection() -> ServiceResourceTablesCollection:
    return session.resource("dynamodb").tables
```



## Methods

### DynamoDBServiceResource.Table method

Creates a Table resource.

Type annotations and code completion for `#!python session.resource("dynamodb").Table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)

```python title="Method definition"
await def Table(
    self,
    name: str,
) -> Table:
    ...
```



```python title="Usage example with kwargs"
kwargs: ServiceResourceTableRequestTypeDef = {  # (1)
    "name": ...,
}

parent.Table(**kwargs)
```

1. See [:material-code-braces: ServiceResourceTableRequestTypeDef](./type_defs.md#serviceresourcetablerequesttypedef) 

### DynamoDBServiceResource.batch\_get\_item method

The `BatchGetItem` operation returns the attributes of one or more items from
one or more tables.

Type annotations and code completion for `#!python session.resource("dynamodb").batch_get_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.batch_get_item)

```python title="Method definition"
await def batch_get_item(
    self,
    *,
    RequestItems: Mapping[str, KeysAndAttributesServiceResourceTypeDef],  # (1)
    ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,  # (2)
) -> BatchGetItemOutputServiceResourceTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: KeysAndAttributesServiceResourceTypeDef](./type_defs.md#keysandattributesserviceresourcetypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
3. See [:material-code-braces: BatchGetItemOutputServiceResourceTypeDef](./type_defs.md#batchgetitemoutputserviceresourcetypedef) 


```python title="Usage example with kwargs"
kwargs: BatchGetItemInputServiceResourceBatchGetItemTypeDef = {  # (1)
    "RequestItems": ...,
}

parent.batch_get_item(**kwargs)
```

1. See [:material-code-braces: BatchGetItemInputServiceResourceBatchGetItemTypeDef](./type_defs.md#batchgetiteminputserviceresourcebatchgetitemtypedef) 

### DynamoDBServiceResource.batch\_write\_item method

The `BatchWriteItem` operation puts or deletes multiple items in one or more
tables.

Type annotations and code completion for `#!python session.resource("dynamodb").batch_write_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.batch_write_item)

```python title="Method definition"
await def batch_write_item(
    self,
    *,
    RequestItems: Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],  # (1)
    ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,  # (2)
    ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,  # (3)
) -> BatchWriteItemOutputServiceResourceTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: WriteRequestServiceResourceTypeDef](./type_defs.md#writerequestserviceresourcetypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
3. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
4. See [:material-code-braces: BatchWriteItemOutputServiceResourceTypeDef](./type_defs.md#batchwriteitemoutputserviceresourcetypedef) 


```python title="Usage example with kwargs"
kwargs: BatchWriteItemInputServiceResourceBatchWriteItemTypeDef = {  # (1)
    "RequestItems": ...,
}

parent.batch_write_item(**kwargs)
```

1. See [:material-code-braces: BatchWriteItemInputServiceResourceBatchWriteItemTypeDef](./type_defs.md#batchwriteiteminputserviceresourcebatchwriteitemtypedef) 

### DynamoDBServiceResource.create\_table method

The `CreateTable` operation adds a new table to your account.

Type annotations and code completion for `#!python session.resource("dynamodb").create_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.create_table)

```python title="Method definition"
await def create_table(
    self,
    *,
    AttributeDefinitions: Sequence[AttributeDefinitionServiceResourceTypeDef],  # (1)
    TableName: str,
    KeySchema: Sequence[KeySchemaElementServiceResourceTypeDef],  # (2)
    LocalSecondaryIndexes: Sequence[LocalSecondaryIndexServiceResourceTypeDef] = ...,  # (3)
    GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexServiceResourceTypeDef] = ...,  # (4)
    BillingMode: BillingModeType = ...,  # (5)
    ProvisionedThroughput: ProvisionedThroughputServiceResourceTypeDef = ...,  # (6)
    StreamSpecification: StreamSpecificationServiceResourceTypeDef = ...,  # (7)
    SSESpecification: SSESpecificationServiceResourceTypeDef = ...,  # (8)
    Tags: Sequence[TagServiceResourceTypeDef] = ...,  # (9)
    TableClass: TableClassType = ...,  # (10)
) -> Table:
    ...
```

1. See [:material-code-braces: AttributeDefinitionServiceResourceTypeDef](./type_defs.md#attributedefinitionserviceresourcetypedef) 
2. See [:material-code-braces: KeySchemaElementServiceResourceTypeDef](./type_defs.md#keyschemaelementserviceresourcetypedef) 
3. See [:material-code-braces: LocalSecondaryIndexServiceResourceTypeDef](./type_defs.md#localsecondaryindexserviceresourcetypedef) 
4. See [:material-code-braces: GlobalSecondaryIndexServiceResourceTypeDef](./type_defs.md#globalsecondaryindexserviceresourcetypedef) 
5. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
6. See [:material-code-braces: ProvisionedThroughputServiceResourceTypeDef](./type_defs.md#provisionedthroughputserviceresourcetypedef) 
7. See [:material-code-braces: StreamSpecificationServiceResourceTypeDef](./type_defs.md#streamspecificationserviceresourcetypedef) 
8. See [:material-code-braces: SSESpecificationServiceResourceTypeDef](./type_defs.md#ssespecificationserviceresourcetypedef) 
9. See [:material-code-braces: TagServiceResourceTypeDef](./type_defs.md#tagserviceresourcetypedef) 
10. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 


```python title="Usage example with kwargs"
kwargs: CreateTableInputServiceResourceCreateTableTypeDef = {  # (1)
    "AttributeDefinitions": ...,
    "TableName": ...,
    "KeySchema": ...,
}

parent.create_table(**kwargs)
```

1. See [:material-code-braces: CreateTableInputServiceResourceCreateTableTypeDef](./type_defs.md#createtableinputserviceresourcecreatetabletypedef) 

### DynamoDBServiceResource.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python session.resource("dynamodb").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.get_available_subresources)

```python title="Method definition"
await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```




## Table

Type annotations and code completion for `#!python session.resource("dynamodb").Table` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)

```python title="Usage example"
from types_aiobotocore_dynamodb.service_resource import Table


async def get_resource() -> Table:
    async with session.resource("dynamodb") as resource:
        return await resource.Table(...)
```


### Table attributes


- `attribute_definitions`: `List`[[AttributeDefinitionTableTypeDef](./type_defs.md#attributedefinitiontabletypedef)]
- `table_name`: `str`
- `key_schema`: `List`[[KeySchemaElementTableTypeDef](./type_defs.md#keyschemaelementtabletypedef)]
- `table_status`: [TableStatusType](./literals.md#tablestatustype)
- `creation_date_time`: `datetime`
- `provisioned_throughput`: [ProvisionedThroughputDescriptionResponseMetadataTypeDef](./type_defs.md#provisionedthroughputdescriptionresponsemetadatatypedef)
- `table_size_bytes`: `int`
- `item_count`: `int`
- `table_arn`: `str`
- `table_id`: `str`
- `billing_mode_summary`: [BillingModeSummaryResponseMetadataTypeDef](./type_defs.md#billingmodesummaryresponsemetadatatypedef)
- `local_secondary_indexes`: `List`[[LocalSecondaryIndexDescriptionTableTypeDef](./type_defs.md#localsecondaryindexdescriptiontabletypedef)]
- `global_secondary_indexes`: `List`[[GlobalSecondaryIndexDescriptionTableTypeDef](./type_defs.md#globalsecondaryindexdescriptiontabletypedef)]
- `stream_specification`: [StreamSpecificationResponseMetadataTypeDef](./type_defs.md#streamspecificationresponsemetadatatypedef)
- `latest_stream_label`: `str`
- `latest_stream_arn`: `str`
- `global_table_version`: `str`
- `replicas`: `List`[[ReplicaDescriptionTableTypeDef](./type_defs.md#replicadescriptiontabletypedef)]
- `restore_summary`: [RestoreSummaryResponseMetadataTypeDef](./type_defs.md#restoresummaryresponsemetadatatypedef)
- `sse_description`: [SSEDescriptionResponseMetadataTypeDef](./type_defs.md#ssedescriptionresponsemetadatatypedef)
- `archival_summary`: [ArchivalSummaryResponseMetadataTypeDef](./type_defs.md#archivalsummaryresponsemetadatatypedef)
- `table_class_summary`: [TableClassSummaryResponseMetadataTypeDef](./type_defs.md#tableclasssummaryresponsemetadatatypedef)
- `name`: `str`





### Table methods


#### Table.batch\_writer method

Create a batch writer object.

Type annotations and code completion for `#!python aioboto3.resource("dynamodb").batch_writer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.batch_writer)

```python title="Method definition"
await def batch_writer(
    self,
    overwrite_by_pkeys: List[str] = ...,
) -> BatchWriter:
    ...
```



```python title="Usage example with kwargs"
kwargs: TableBatchWriterRequestTypeDef = {  # (1)
    "overwrite_by_pkeys": ...,
}

parent.batch_writer(**kwargs)
```

1. See [:material-code-braces: TableBatchWriterRequestTypeDef](./type_defs.md#tablebatchwriterrequesttypedef) 

#### Table.delete method

The `DeleteTable` operation deletes a table and all of its items.

Type annotations and code completion for `#!python aioboto3.resource("dynamodb").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete)

```python title="Method definition"
await def delete(
    self,
) -> DeleteTableOutputTableTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteTableOutputTableTypeDef](./type_defs.md#deletetableoutputtabletypedef) 

#### Table.delete\_item method

Deletes a single item in a table by primary key.

Type annotations and code completion for `#!python aioboto3.resource("dynamodb").delete_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete_item)

```python title="Method definition"
await def delete_item(
    self,
    *,
    Key: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,  # (1)
    ConditionalOperator: ConditionalOperatorType = ...,  # (2)
    ReturnValues: ReturnValueType = ...,  # (3)
    ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,  # (4)
    ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,  # (5)
    ConditionExpression: Union[str, ConditionBase] = ...,
    ExpressionAttributeNames: Mapping[str, str] = ...,
    ExpressionAttributeValues: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]] = ...,
) -> DeleteItemOutputTableTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: ExpectedAttributeValueTableTypeDef](./type_defs.md#expectedattributevaluetabletypedef) 
2. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
3. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
4. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
5. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
6. See [:material-code-braces: DeleteItemOutputTableTypeDef](./type_defs.md#deleteitemoutputtabletypedef) 


```python title="Usage example with kwargs"
kwargs: DeleteItemInputTableDeleteItemTypeDef = {  # (1)
    "Key": ...,
}

parent.delete_item(**kwargs)
```

1. See [:material-code-braces: DeleteItemInputTableDeleteItemTypeDef](./type_defs.md#deleteiteminputtabledeleteitemtypedef) 

#### Table.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aioboto3.resource("dynamodb").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.get_available_subresources)

```python title="Method definition"
await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Table.get\_item method

The `GetItem` operation returns a set of attributes for the item with the given
primary key.

Type annotations and code completion for `#!python aioboto3.resource("dynamodb").get_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.get_item)

```python title="Method definition"
await def get_item(
    self,
    *,
    Key: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    AttributesToGet: Sequence[str] = ...,
    ConsistentRead: bool = ...,
    ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,  # (1)
    ProjectionExpression: str = ...,
    ExpressionAttributeNames: Mapping[str, str] = ...,
) -> GetItemOutputTableTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
2. See [:material-code-braces: GetItemOutputTableTypeDef](./type_defs.md#getitemoutputtabletypedef) 


```python title="Usage example with kwargs"
kwargs: GetItemInputTableGetItemTypeDef = {  # (1)
    "Key": ...,
}

parent.get_item(**kwargs)
```

1. See [:material-code-braces: GetItemInputTableGetItemTypeDef](./type_defs.md#getiteminputtablegetitemtypedef) 

#### Table.load method

Calls :py:meth:`DynamoDB.Client.describe_table` to update the attributes of the
Table resource.

Type annotations and code completion for `#!python aioboto3.resource("dynamodb").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.load)

```python title="Method definition"
await def load(
    self,
) -> None:
    ...
```


#### Table.put\_item method

Creates a new item, or replaces an old item with a new item.

Type annotations and code completion for `#!python aioboto3.resource("dynamodb").put_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.put_item)

```python title="Method definition"
await def put_item(
    self,
    *,
    Item: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,  # (1)
    ReturnValues: ReturnValueType = ...,  # (2)
    ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,  # (3)
    ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,  # (4)
    ConditionalOperator: ConditionalOperatorType = ...,  # (5)
    ConditionExpression: Union[str, ConditionBase] = ...,
    ExpressionAttributeNames: Mapping[str, str] = ...,
    ExpressionAttributeValues: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]] = ...,
) -> PutItemOutputTableTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: ExpectedAttributeValueTableTypeDef](./type_defs.md#expectedattributevaluetabletypedef) 
2. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
3. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
4. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
5. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
6. See [:material-code-braces: PutItemOutputTableTypeDef](./type_defs.md#putitemoutputtabletypedef) 


```python title="Usage example with kwargs"
kwargs: PutItemInputTablePutItemTypeDef = {  # (1)
    "Item": ...,
}

parent.put_item(**kwargs)
```

1. See [:material-code-braces: PutItemInputTablePutItemTypeDef](./type_defs.md#putiteminputtableputitemtypedef) 

#### Table.query method

You must provide the name of the partition key attribute and a single value for
that attribute.

Type annotations and code completion for `#!python aioboto3.resource("dynamodb").query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.query)

```python title="Method definition"
await def query(
    self,
    *,
    IndexName: str = ...,
    Select: SelectType = ...,  # (1)
    AttributesToGet: Sequence[str] = ...,
    Limit: int = ...,
    ConsistentRead: bool = ...,
    KeyConditions: Mapping[str, ConditionTableTypeDef] = ...,  # (2)
    QueryFilter: Mapping[str, ConditionTableTypeDef] = ...,  # (2)
    ConditionalOperator: ConditionalOperatorType = ...,  # (4)
    ScanIndexForward: bool = ...,
    ExclusiveStartKey: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]] = ...,
    ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,  # (5)
    ProjectionExpression: str = ...,
    FilterExpression: Union[str, ConditionBase] = ...,
    KeyConditionExpression: Union[str, ConditionBase] = ...,
    ExpressionAttributeNames: Mapping[str, str] = ...,
    ExpressionAttributeValues: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]] = ...,
) -> QueryOutputTableTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTableTypeDef](./type_defs.md#conditiontabletypedef) 
3. See [:material-code-braces: ConditionTableTypeDef](./type_defs.md#conditiontabletypedef) 
4. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
6. See [:material-code-braces: QueryOutputTableTypeDef](./type_defs.md#queryoutputtabletypedef) 


```python title="Usage example with kwargs"
kwargs: QueryInputTableQueryTypeDef = {  # (1)
    "IndexName": ...,
}

parent.query(**kwargs)
```

1. See [:material-code-braces: QueryInputTableQueryTypeDef](./type_defs.md#queryinputtablequerytypedef) 

#### Table.reload method

Calls :py:meth:`DynamoDB.Client.describe_table` to update the attributes of the
Table resource.

Type annotations and code completion for `#!python aioboto3.resource("dynamodb").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.reload)

```python title="Method definition"
await def reload(
    self,
) -> None:
    ...
```


#### Table.scan method

The `Scan` operation returns one or more items and item attributes by accessing
every item in a table or a secondary index.

Type annotations and code completion for `#!python aioboto3.resource("dynamodb").scan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.scan)

```python title="Method definition"
await def scan(
    self,
    *,
    IndexName: str = ...,
    AttributesToGet: Sequence[str] = ...,
    Limit: int = ...,
    Select: SelectType = ...,  # (1)
    ScanFilter: Mapping[str, ConditionTableTypeDef] = ...,  # (2)
    ConditionalOperator: ConditionalOperatorType = ...,  # (3)
    ExclusiveStartKey: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]] = ...,
    ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,  # (4)
    TotalSegments: int = ...,
    Segment: int = ...,
    ProjectionExpression: str = ...,
    FilterExpression: Union[str, ConditionBase] = ...,
    ExpressionAttributeNames: Mapping[str, str] = ...,
    ExpressionAttributeValues: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]] = ...,
    ConsistentRead: bool = ...,
) -> ScanOutputTableTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTableTypeDef](./type_defs.md#conditiontabletypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
5. See [:material-code-braces: ScanOutputTableTypeDef](./type_defs.md#scanoutputtabletypedef) 


```python title="Usage example with kwargs"
kwargs: ScanInputTableScanTypeDef = {  # (1)
    "IndexName": ...,
}

parent.scan(**kwargs)
```

1. See [:material-code-braces: ScanInputTableScanTypeDef](./type_defs.md#scaninputtablescantypedef) 

#### Table.update method

Modifies the provisioned throughput settings, global secondary indexes, or
DynamoDB Streams settings for a given table.

Type annotations and code completion for `#!python aioboto3.resource("dynamodb").update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update)

```python title="Method definition"
await def update(
    self,
    *,
    AttributeDefinitions: Sequence[AttributeDefinitionTableTypeDef] = ...,  # (1)
    BillingMode: BillingModeType = ...,  # (2)
    ProvisionedThroughput: ProvisionedThroughputTableTypeDef = ...,  # (3)
    GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTableTypeDef] = ...,  # (4)
    StreamSpecification: StreamSpecificationTableTypeDef = ...,  # (5)
    SSESpecification: SSESpecificationTableTypeDef = ...,  # (6)
    ReplicaUpdates: Sequence[ReplicationGroupUpdateTableTypeDef] = ...,  # (7)
    TableClass: TableClassType = ...,  # (8)
) -> Table:
    ...
```

1. See [:material-code-braces: AttributeDefinitionTableTypeDef](./type_defs.md#attributedefinitiontabletypedef) 
2. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
3. See [:material-code-braces: ProvisionedThroughputTableTypeDef](./type_defs.md#provisionedthroughputtabletypedef) 
4. See [:material-code-braces: GlobalSecondaryIndexUpdateTableTypeDef](./type_defs.md#globalsecondaryindexupdatetabletypedef) 
5. See [:material-code-braces: StreamSpecificationTableTypeDef](./type_defs.md#streamspecificationtabletypedef) 
6. See [:material-code-braces: SSESpecificationTableTypeDef](./type_defs.md#ssespecificationtabletypedef) 
7. See [:material-code-braces: ReplicationGroupUpdateTableTypeDef](./type_defs.md#replicationgroupupdatetabletypedef) 
8. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 


```python title="Usage example with kwargs"
kwargs: UpdateTableInputTableUpdateTypeDef = {  # (1)
    "AttributeDefinitions": ...,
}

parent.update(**kwargs)
```

1. See [:material-code-braces: UpdateTableInputTableUpdateTypeDef](./type_defs.md#updatetableinputtableupdatetypedef) 

#### Table.update\_item method

Edits an existing item's attributes, or adds a new item to the table if it does
not already exist.

Type annotations and code completion for `#!python aioboto3.resource("dynamodb").update_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update_item)

```python title="Method definition"
await def update_item(
    self,
    *,
    Key: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    AttributeUpdates: Mapping[str, AttributeValueUpdateTableTypeDef] = ...,  # (1)
    Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,  # (2)
    ConditionalOperator: ConditionalOperatorType = ...,  # (3)
    ReturnValues: ReturnValueType = ...,  # (4)
    ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,  # (5)
    ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,  # (6)
    UpdateExpression: str = ...,
    ConditionExpression: Union[str, ConditionBase] = ...,
    ExpressionAttributeNames: Mapping[str, str] = ...,
    ExpressionAttributeValues: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]] = ...,
) -> UpdateItemOutputTableTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: AttributeValueUpdateTableTypeDef](./type_defs.md#attributevalueupdatetabletypedef) 
2. See [:material-code-braces: ExpectedAttributeValueTableTypeDef](./type_defs.md#expectedattributevaluetabletypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
6. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
7. See [:material-code-braces: UpdateItemOutputTableTypeDef](./type_defs.md#updateitemoutputtabletypedef) 


```python title="Usage example with kwargs"
kwargs: UpdateItemInputTableUpdateItemTypeDef = {  # (1)
    "Key": ...,
}

parent.update_item(**kwargs)
```

1. See [:material-code-braces: UpdateItemInputTableUpdateItemTypeDef](./type_defs.md#updateiteminputtableupdateitemtypedef) 

#### Table.wait\_until\_exists method

Waits until this Table is exists.

Type annotations and code completion for `#!python aioboto3.resource("dynamodb").wait_until_exists` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.wait_until_exists)

```python title="Method definition"
await def wait_until_exists(
    self,
) -> None:
    ...
```


#### Table.wait\_until\_not\_exists method

Waits until this Table is not exists.

Type annotations and code completion for `#!python aioboto3.resource("dynamodb").wait_until_not_exists` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.wait_until_not_exists)

```python title="Method definition"
await def wait_until_not_exists(
    self,
) -> None:
    ...
```




