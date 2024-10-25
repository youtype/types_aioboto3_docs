# SupplyChainClient

> [Index](../README.md) > [SupplyChain](./README.md) > SupplyChainClient

!!! note ""

    Auto-generated documentation for [SupplyChain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain)
    type annotations stubs module [types-aiobotocore-supplychain](https://pypi.org/project/types-aiobotocore-supplychain/).

## SupplyChainClient

Type annotations and code completion for `#!python session.client("supplychain")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client)

```python
# SupplyChainClient usage example

from aioboto3.session import Session
from types_aiobotocore_supplychain.client import SupplyChainClient

session = Session()
async with session.client("supplychain") as client:
    client: SupplyChainClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("supplychain").exceptions` structure.

```python
# SupplyChainClient.exceptions usage example

async with session.client("supplychain") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# SupplyChainClient.exceptions type checking example

from types_aiobotocore_supplychain.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.client("supplychain").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.client("supplychain").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_bill\_of\_materials\_import\_job

CreateBillOfMaterialsImportJob creates an import job for the Product Bill Of
Materials (BOM)
entity.

Type annotations and code completion for `#!python session.client("supplychain").create_bill_of_materials_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.create_bill_of_materials_import_job)

```python
# create_bill_of_materials_import_job method definition

await def create_bill_of_materials_import_job(
    self,
    *,
    instanceId: str,
    s3uri: str,
    clientToken: str = ...,
) -> CreateBillOfMaterialsImportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateBillOfMaterialsImportJobResponseTypeDef](./type_defs.md#createbillofmaterialsimportjobresponsetypedef) 


```python
# create_bill_of_materials_import_job method usage example with argument unpacking

kwargs: CreateBillOfMaterialsImportJobRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "s3uri": ...,
}

parent.create_bill_of_materials_import_job(**kwargs)
```

1. See [:material-code-braces: CreateBillOfMaterialsImportJobRequestRequestTypeDef](./type_defs.md#createbillofmaterialsimportjobrequestrequesttypedef) 

### create\_data\_integration\_flow

Create DataIntegrationFlow to map one or more different sources to one target
using the SQL transformation
query.

Type annotations and code completion for `#!python session.client("supplychain").create_data_integration_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.create_data_integration_flow)

```python
# create_data_integration_flow method definition

await def create_data_integration_flow(
    self,
    *,
    instanceId: str,
    name: str,
    sources: Sequence[DataIntegrationFlowSourceTypeDef],  # (1)
    transformation: DataIntegrationFlowTransformationTypeDef,  # (2)
    target: DataIntegrationFlowTargetTypeDef,  # (3)
    tags: Mapping[str, str] = ...,
) -> CreateDataIntegrationFlowResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DataIntegrationFlowSourceTypeDef](./type_defs.md#dataintegrationflowsourcetypedef) 
2. See [:material-code-braces: DataIntegrationFlowTransformationTypeDef](./type_defs.md#dataintegrationflowtransformationtypedef) 
3. See [:material-code-braces: DataIntegrationFlowTargetTypeDef](./type_defs.md#dataintegrationflowtargettypedef) 
4. See [:material-code-braces: CreateDataIntegrationFlowResponseTypeDef](./type_defs.md#createdataintegrationflowresponsetypedef) 


```python
# create_data_integration_flow method usage example with argument unpacking

kwargs: CreateDataIntegrationFlowRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "name": ...,
    "sources": ...,
    "transformation": ...,
    "target": ...,
}

parent.create_data_integration_flow(**kwargs)
```

1. See [:material-code-braces: CreateDataIntegrationFlowRequestRequestTypeDef](./type_defs.md#createdataintegrationflowrequestrequesttypedef) 

### create\_data\_lake\_dataset

Create a data lake dataset.

Type annotations and code completion for `#!python session.client("supplychain").create_data_lake_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.create_data_lake_dataset)

```python
# create_data_lake_dataset method definition

await def create_data_lake_dataset(
    self,
    *,
    instanceId: str,
    namespace: str,
    name: str,
    schema: DataLakeDatasetSchemaTypeDef = ...,  # (1)
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateDataLakeDatasetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DataLakeDatasetSchemaTypeDef](./type_defs.md#datalakedatasetschematypedef) 
2. See [:material-code-braces: CreateDataLakeDatasetResponseTypeDef](./type_defs.md#createdatalakedatasetresponsetypedef) 


```python
# create_data_lake_dataset method usage example with argument unpacking

kwargs: CreateDataLakeDatasetRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "namespace": ...,
    "name": ...,
}

parent.create_data_lake_dataset(**kwargs)
```

1. See [:material-code-braces: CreateDataLakeDatasetRequestRequestTypeDef](./type_defs.md#createdatalakedatasetrequestrequesttypedef) 

### delete\_data\_integration\_flow

Delete the DataIntegrationFlow.

Type annotations and code completion for `#!python session.client("supplychain").delete_data_integration_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.delete_data_integration_flow)

```python
# delete_data_integration_flow method definition

await def delete_data_integration_flow(
    self,
    *,
    instanceId: str,
    name: str,
) -> DeleteDataIntegrationFlowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDataIntegrationFlowResponseTypeDef](./type_defs.md#deletedataintegrationflowresponsetypedef) 


```python
# delete_data_integration_flow method usage example with argument unpacking

kwargs: DeleteDataIntegrationFlowRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "name": ...,
}

parent.delete_data_integration_flow(**kwargs)
```

1. See [:material-code-braces: DeleteDataIntegrationFlowRequestRequestTypeDef](./type_defs.md#deletedataintegrationflowrequestrequesttypedef) 

### delete\_data\_lake\_dataset

Delete a data lake dataset.

Type annotations and code completion for `#!python session.client("supplychain").delete_data_lake_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.delete_data_lake_dataset)

```python
# delete_data_lake_dataset method definition

await def delete_data_lake_dataset(
    self,
    *,
    instanceId: str,
    namespace: str,
    name: str,
) -> DeleteDataLakeDatasetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDataLakeDatasetResponseTypeDef](./type_defs.md#deletedatalakedatasetresponsetypedef) 


```python
# delete_data_lake_dataset method usage example with argument unpacking

kwargs: DeleteDataLakeDatasetRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "namespace": ...,
    "name": ...,
}

parent.delete_data_lake_dataset(**kwargs)
```

1. See [:material-code-braces: DeleteDataLakeDatasetRequestRequestTypeDef](./type_defs.md#deletedatalakedatasetrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.client("supplychain").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.generate_presigned_url)

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


### get\_bill\_of\_materials\_import\_job

Get status and details of a BillOfMaterialsImportJob.

Type annotations and code completion for `#!python session.client("supplychain").get_bill_of_materials_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.get_bill_of_materials_import_job)

```python
# get_bill_of_materials_import_job method definition

await def get_bill_of_materials_import_job(
    self,
    *,
    instanceId: str,
    jobId: str,
) -> GetBillOfMaterialsImportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBillOfMaterialsImportJobResponseTypeDef](./type_defs.md#getbillofmaterialsimportjobresponsetypedef) 


```python
# get_bill_of_materials_import_job method usage example with argument unpacking

kwargs: GetBillOfMaterialsImportJobRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "jobId": ...,
}

parent.get_bill_of_materials_import_job(**kwargs)
```

1. See [:material-code-braces: GetBillOfMaterialsImportJobRequestRequestTypeDef](./type_defs.md#getbillofmaterialsimportjobrequestrequesttypedef) 

### get\_data\_integration\_flow

View the DataIntegrationFlow details.

Type annotations and code completion for `#!python session.client("supplychain").get_data_integration_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.get_data_integration_flow)

```python
# get_data_integration_flow method definition

await def get_data_integration_flow(
    self,
    *,
    instanceId: str,
    name: str,
) -> GetDataIntegrationFlowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataIntegrationFlowResponseTypeDef](./type_defs.md#getdataintegrationflowresponsetypedef) 


```python
# get_data_integration_flow method usage example with argument unpacking

kwargs: GetDataIntegrationFlowRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "name": ...,
}

parent.get_data_integration_flow(**kwargs)
```

1. See [:material-code-braces: GetDataIntegrationFlowRequestRequestTypeDef](./type_defs.md#getdataintegrationflowrequestrequesttypedef) 

### get\_data\_lake\_dataset

Get a data lake dataset.

Type annotations and code completion for `#!python session.client("supplychain").get_data_lake_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.get_data_lake_dataset)

```python
# get_data_lake_dataset method definition

await def get_data_lake_dataset(
    self,
    *,
    instanceId: str,
    namespace: str,
    name: str,
) -> GetDataLakeDatasetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataLakeDatasetResponseTypeDef](./type_defs.md#getdatalakedatasetresponsetypedef) 


```python
# get_data_lake_dataset method usage example with argument unpacking

kwargs: GetDataLakeDatasetRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "namespace": ...,
    "name": ...,
}

parent.get_data_lake_dataset(**kwargs)
```

1. See [:material-code-braces: GetDataLakeDatasetRequestRequestTypeDef](./type_defs.md#getdatalakedatasetrequestrequesttypedef) 

### list\_data\_integration\_flows

Lists all the DataIntegrationFlows in a paginated way.

Type annotations and code completion for `#!python session.client("supplychain").list_data_integration_flows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.list_data_integration_flows)

```python
# list_data_integration_flows method definition

await def list_data_integration_flows(
    self,
    *,
    instanceId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDataIntegrationFlowsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataIntegrationFlowsResponseTypeDef](./type_defs.md#listdataintegrationflowsresponsetypedef) 


```python
# list_data_integration_flows method usage example with argument unpacking

kwargs: ListDataIntegrationFlowsRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
}

parent.list_data_integration_flows(**kwargs)
```

1. See [:material-code-braces: ListDataIntegrationFlowsRequestRequestTypeDef](./type_defs.md#listdataintegrationflowsrequestrequesttypedef) 

### list\_data\_lake\_datasets

List the data lake datasets for a specific instance and name space.

Type annotations and code completion for `#!python session.client("supplychain").list_data_lake_datasets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.list_data_lake_datasets)

```python
# list_data_lake_datasets method definition

await def list_data_lake_datasets(
    self,
    *,
    instanceId: str,
    namespace: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDataLakeDatasetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataLakeDatasetsResponseTypeDef](./type_defs.md#listdatalakedatasetsresponsetypedef) 


```python
# list_data_lake_datasets method usage example with argument unpacking

kwargs: ListDataLakeDatasetsRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "namespace": ...,
}

parent.list_data_lake_datasets(**kwargs)
```

1. See [:material-code-braces: ListDataLakeDatasetsRequestRequestTypeDef](./type_defs.md#listdatalakedatasetsrequestrequesttypedef) 

### list\_tags\_for\_resource

List all the tags for an Amazon Web ServicesSupply Chain resource.

Type annotations and code completion for `#!python session.client("supplychain").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### send\_data\_integration\_event

Send the transactional data payload for the event with real-time data for
analysis or
monitoring.

Type annotations and code completion for `#!python session.client("supplychain").send_data_integration_event` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.send_data_integration_event)

```python
# send_data_integration_event method definition

await def send_data_integration_event(
    self,
    *,
    instanceId: str,
    eventType: DataIntegrationEventTypeType,  # (1)
    data: str,
    eventGroupId: str,
    eventTimestamp: TimestampTypeDef = ...,
    clientToken: str = ...,
) -> SendDataIntegrationEventResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DataIntegrationEventTypeType](./literals.md#dataintegrationeventtypetype) 
2. See [:material-code-braces: SendDataIntegrationEventResponseTypeDef](./type_defs.md#senddataintegrationeventresponsetypedef) 


```python
# send_data_integration_event method usage example with argument unpacking

kwargs: SendDataIntegrationEventRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "eventType": ...,
    "data": ...,
    "eventGroupId": ...,
}

parent.send_data_integration_event(**kwargs)
```

1. See [:material-code-braces: SendDataIntegrationEventRequestRequestTypeDef](./type_defs.md#senddataintegrationeventrequestrequesttypedef) 

### tag\_resource

Create tags for an Amazon Web Services Supply chain resource.

Type annotations and code completion for `#!python session.client("supplychain").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Delete tags for an Amazon Web Services Supply chain resource.

Type annotations and code completion for `#!python session.client("supplychain").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_data\_integration\_flow

Update the DataIntegrationFlow.

Type annotations and code completion for `#!python session.client("supplychain").update_data_integration_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.update_data_integration_flow)

```python
# update_data_integration_flow method definition

await def update_data_integration_flow(
    self,
    *,
    instanceId: str,
    name: str,
    sources: Sequence[DataIntegrationFlowSourceTypeDef] = ...,  # (1)
    transformation: DataIntegrationFlowTransformationTypeDef = ...,  # (2)
    target: DataIntegrationFlowTargetTypeDef = ...,  # (3)
) -> UpdateDataIntegrationFlowResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DataIntegrationFlowSourceTypeDef](./type_defs.md#dataintegrationflowsourcetypedef) 
2. See [:material-code-braces: DataIntegrationFlowTransformationTypeDef](./type_defs.md#dataintegrationflowtransformationtypedef) 
3. See [:material-code-braces: DataIntegrationFlowTargetTypeDef](./type_defs.md#dataintegrationflowtargettypedef) 
4. See [:material-code-braces: UpdateDataIntegrationFlowResponseTypeDef](./type_defs.md#updatedataintegrationflowresponsetypedef) 


```python
# update_data_integration_flow method usage example with argument unpacking

kwargs: UpdateDataIntegrationFlowRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "name": ...,
}

parent.update_data_integration_flow(**kwargs)
```

1. See [:material-code-braces: UpdateDataIntegrationFlowRequestRequestTypeDef](./type_defs.md#updatedataintegrationflowrequestrequesttypedef) 

### update\_data\_lake\_dataset

Update a data lake dataset.

Type annotations and code completion for `#!python session.client("supplychain").update_data_lake_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.update_data_lake_dataset)

```python
# update_data_lake_dataset method definition

await def update_data_lake_dataset(
    self,
    *,
    instanceId: str,
    namespace: str,
    name: str,
    description: str = ...,
) -> UpdateDataLakeDatasetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateDataLakeDatasetResponseTypeDef](./type_defs.md#updatedatalakedatasetresponsetypedef) 


```python
# update_data_lake_dataset method usage example with argument unpacking

kwargs: UpdateDataLakeDatasetRequestRequestTypeDef = {  # (1)
    "instanceId": ...,
    "namespace": ...,
    "name": ...,
}

parent.update_data_lake_dataset(**kwargs)
```

1. See [:material-code-braces: UpdateDataLakeDatasetRequestRequestTypeDef](./type_defs.md#updatedatalakedatasetrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("supplychain").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "SupplyChainClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("supplychain").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("supplychain").get_paginator` method with overloads.

- `client.get_paginator("list_data_integration_flows")` -> [ListDataIntegrationFlowsPaginator](./paginators.md#listdataintegrationflowspaginator)
- `client.get_paginator("list_data_lake_datasets")` -> [ListDataLakeDatasetsPaginator](./paginators.md#listdatalakedatasetspaginator)



