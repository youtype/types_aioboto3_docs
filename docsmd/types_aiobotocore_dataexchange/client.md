# DataExchangeClient

> [Index](../README.md) > [DataExchange](./README.md) > DataExchangeClient

!!! note ""

    Auto-generated documentation for [DataExchange](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#dataexchange)
    type annotations stubs module [types-aiobotocore-dataexchange](https://pypi.org/project/types-aiobotocore-dataexchange/).

## DataExchangeClient

Type annotations and code completion for `#!python session.client("dataexchange")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# DataExchangeClient usage example

from aioboto3.session import Session
from types_aiobotocore_dataexchange.client import DataExchangeClient

session = Session()
async with session.client("dataexchange") as client:
    client: DataExchangeClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("dataexchange").exceptions` structure.

```python
# DataExchangeClient.exceptions usage example

async with session.client("dataexchange") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceLimitExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# DataExchangeClient.exceptions type checking example

from types_aiobotocore_dataexchange.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("dataexchange").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("dataexchange").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

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


### accept\_data\_grant

This operation accepts a data grant.

Type annotations and code completion for `#!python session.client("dataexchange").accept_data_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# accept_data_grant method definition

await def accept_data_grant(
    self,
    *,
    DataGrantArn: str,
) -> AcceptDataGrantResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AcceptDataGrantResponseTypeDef](./type_defs.md#acceptdatagrantresponsetypedef) 


```python
# accept_data_grant method usage example with argument unpacking

kwargs: AcceptDataGrantRequestRequestTypeDef = {  # (1)
    "DataGrantArn": ...,
}

parent.accept_data_grant(**kwargs)
```

1. See [:material-code-braces: AcceptDataGrantRequestRequestTypeDef](./type_defs.md#acceptdatagrantrequestrequesttypedef) 

### cancel\_job

This operation cancels a job.

Type annotations and code completion for `#!python session.client("dataexchange").cancel_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# cancel_job method definition

await def cancel_job(
    self,
    *,
    JobId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# cancel_job method usage example with argument unpacking

kwargs: CancelJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.cancel_job(**kwargs)
```

1. See [:material-code-braces: CancelJobRequestRequestTypeDef](./type_defs.md#canceljobrequestrequesttypedef) 

### create\_data\_grant

This operation creates a data grant.

Type annotations and code completion for `#!python session.client("dataexchange").create_data_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# create_data_grant method definition

await def create_data_grant(
    self,
    *,
    Name: str,
    GrantDistributionScope: GrantDistributionScopeType,  # (1)
    ReceiverPrincipal: str,
    SourceDataSetId: str,
    EndsAt: TimestampTypeDef = ...,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateDataGrantResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: GrantDistributionScopeType](./literals.md#grantdistributionscopetype) 
2. See [:material-code-braces: CreateDataGrantResponseTypeDef](./type_defs.md#createdatagrantresponsetypedef) 


```python
# create_data_grant method usage example with argument unpacking

kwargs: CreateDataGrantRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "GrantDistributionScope": ...,
    "ReceiverPrincipal": ...,
    "SourceDataSetId": ...,
}

parent.create_data_grant(**kwargs)
```

1. See [:material-code-braces: CreateDataGrantRequestRequestTypeDef](./type_defs.md#createdatagrantrequestrequesttypedef) 

### create\_data\_set

This operation creates a data set.

Type annotations and code completion for `#!python session.client("dataexchange").create_data_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# create_data_set method definition

await def create_data_set(
    self,
    *,
    AssetType: AssetTypeType,  # (1)
    Description: str,
    Name: str,
    Tags: Mapping[str, str] = ...,
) -> CreateDataSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AssetTypeType](./literals.md#assettypetype) 
2. See [:material-code-braces: CreateDataSetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef) 


```python
# create_data_set method usage example with argument unpacking

kwargs: CreateDataSetRequestRequestTypeDef = {  # (1)
    "AssetType": ...,
    "Description": ...,
    "Name": ...,
}

parent.create_data_set(**kwargs)
```

1. See [:material-code-braces: CreateDataSetRequestRequestTypeDef](./type_defs.md#createdatasetrequestrequesttypedef) 

### create\_event\_action

This operation creates an event action.

Type annotations and code completion for `#!python session.client("dataexchange").create_event_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# create_event_action method definition

await def create_event_action(
    self,
    *,
    Action: ActionTypeDef,  # (1)
    Event: EventTypeDef,  # (2)
) -> CreateEventActionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
3. See [:material-code-braces: CreateEventActionResponseTypeDef](./type_defs.md#createeventactionresponsetypedef) 


```python
# create_event_action method usage example with argument unpacking

kwargs: CreateEventActionRequestRequestTypeDef = {  # (1)
    "Action": ...,
    "Event": ...,
}

parent.create_event_action(**kwargs)
```

1. See [:material-code-braces: CreateEventActionRequestRequestTypeDef](./type_defs.md#createeventactionrequestrequesttypedef) 

### create\_job

This operation creates a job.

Type annotations and code completion for `#!python session.client("dataexchange").create_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# create_job method definition

await def create_job(
    self,
    *,
    Details: RequestDetailsTypeDef,  # (1)
    Type: TypeType,  # (2)
) -> CreateJobResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RequestDetailsTypeDef](./type_defs.md#requestdetailstypedef) 
2. See [:material-code-brackets: TypeType](./literals.md#typetype) 
3. See [:material-code-braces: CreateJobResponseTypeDef](./type_defs.md#createjobresponsetypedef) 


```python
# create_job method usage example with argument unpacking

kwargs: CreateJobRequestRequestTypeDef = {  # (1)
    "Details": ...,
    "Type": ...,
}

parent.create_job(**kwargs)
```

1. See [:material-code-braces: CreateJobRequestRequestTypeDef](./type_defs.md#createjobrequestrequesttypedef) 

### create\_revision

This operation creates a revision for a data set.

Type annotations and code completion for `#!python session.client("dataexchange").create_revision` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# create_revision method definition

await def create_revision(
    self,
    *,
    DataSetId: str,
    Comment: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateRevisionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateRevisionResponseTypeDef](./type_defs.md#createrevisionresponsetypedef) 


```python
# create_revision method usage example with argument unpacking

kwargs: CreateRevisionRequestRequestTypeDef = {  # (1)
    "DataSetId": ...,
}

parent.create_revision(**kwargs)
```

1. See [:material-code-braces: CreateRevisionRequestRequestTypeDef](./type_defs.md#createrevisionrequestrequesttypedef) 

### delete\_asset

This operation deletes an asset.

Type annotations and code completion for `#!python session.client("dataexchange").delete_asset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# delete_asset method definition

await def delete_asset(
    self,
    *,
    AssetId: str,
    DataSetId: str,
    RevisionId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_asset method usage example with argument unpacking

kwargs: DeleteAssetRequestRequestTypeDef = {  # (1)
    "AssetId": ...,
    "DataSetId": ...,
    "RevisionId": ...,
}

parent.delete_asset(**kwargs)
```

1. See [:material-code-braces: DeleteAssetRequestRequestTypeDef](./type_defs.md#deleteassetrequestrequesttypedef) 

### delete\_data\_grant

This operation deletes a data grant.

Type annotations and code completion for `#!python session.client("dataexchange").delete_data_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# delete_data_grant method definition

await def delete_data_grant(
    self,
    *,
    DataGrantId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_data_grant method usage example with argument unpacking

kwargs: DeleteDataGrantRequestRequestTypeDef = {  # (1)
    "DataGrantId": ...,
}

parent.delete_data_grant(**kwargs)
```

1. See [:material-code-braces: DeleteDataGrantRequestRequestTypeDef](./type_defs.md#deletedatagrantrequestrequesttypedef) 

### delete\_data\_set

This operation deletes a data set.

Type annotations and code completion for `#!python session.client("dataexchange").delete_data_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# delete_data_set method definition

await def delete_data_set(
    self,
    *,
    DataSetId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_data_set method usage example with argument unpacking

kwargs: DeleteDataSetRequestRequestTypeDef = {  # (1)
    "DataSetId": ...,
}

parent.delete_data_set(**kwargs)
```

1. See [:material-code-braces: DeleteDataSetRequestRequestTypeDef](./type_defs.md#deletedatasetrequestrequesttypedef) 

### delete\_event\_action

This operation deletes the event action.

Type annotations and code completion for `#!python session.client("dataexchange").delete_event_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# delete_event_action method definition

await def delete_event_action(
    self,
    *,
    EventActionId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_event_action method usage example with argument unpacking

kwargs: DeleteEventActionRequestRequestTypeDef = {  # (1)
    "EventActionId": ...,
}

parent.delete_event_action(**kwargs)
```

1. See [:material-code-braces: DeleteEventActionRequestRequestTypeDef](./type_defs.md#deleteeventactionrequestrequesttypedef) 

### delete\_revision

This operation deletes a revision.

Type annotations and code completion for `#!python session.client("dataexchange").delete_revision` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# delete_revision method definition

await def delete_revision(
    self,
    *,
    DataSetId: str,
    RevisionId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_revision method usage example with argument unpacking

kwargs: DeleteRevisionRequestRequestTypeDef = {  # (1)
    "DataSetId": ...,
    "RevisionId": ...,
}

parent.delete_revision(**kwargs)
```

1. See [:material-code-braces: DeleteRevisionRequestRequestTypeDef](./type_defs.md#deleterevisionrequestrequesttypedef) 

### get\_asset

This operation returns information about an asset.

Type annotations and code completion for `#!python session.client("dataexchange").get_asset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# get_asset method definition

await def get_asset(
    self,
    *,
    AssetId: str,
    DataSetId: str,
    RevisionId: str,
) -> GetAssetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAssetResponseTypeDef](./type_defs.md#getassetresponsetypedef) 


```python
# get_asset method usage example with argument unpacking

kwargs: GetAssetRequestRequestTypeDef = {  # (1)
    "AssetId": ...,
    "DataSetId": ...,
    "RevisionId": ...,
}

parent.get_asset(**kwargs)
```

1. See [:material-code-braces: GetAssetRequestRequestTypeDef](./type_defs.md#getassetrequestrequesttypedef) 

### get\_data\_grant

This operation returns information about a data grant.

Type annotations and code completion for `#!python session.client("dataexchange").get_data_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# get_data_grant method definition

await def get_data_grant(
    self,
    *,
    DataGrantId: str,
) -> GetDataGrantResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataGrantResponseTypeDef](./type_defs.md#getdatagrantresponsetypedef) 


```python
# get_data_grant method usage example with argument unpacking

kwargs: GetDataGrantRequestRequestTypeDef = {  # (1)
    "DataGrantId": ...,
}

parent.get_data_grant(**kwargs)
```

1. See [:material-code-braces: GetDataGrantRequestRequestTypeDef](./type_defs.md#getdatagrantrequestrequesttypedef) 

### get\_data\_set

This operation returns information about a data set.

Type annotations and code completion for `#!python session.client("dataexchange").get_data_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# get_data_set method definition

await def get_data_set(
    self,
    *,
    DataSetId: str,
) -> GetDataSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataSetResponseTypeDef](./type_defs.md#getdatasetresponsetypedef) 


```python
# get_data_set method usage example with argument unpacking

kwargs: GetDataSetRequestRequestTypeDef = {  # (1)
    "DataSetId": ...,
}

parent.get_data_set(**kwargs)
```

1. See [:material-code-braces: GetDataSetRequestRequestTypeDef](./type_defs.md#getdatasetrequestrequesttypedef) 

### get\_event\_action

This operation retrieves information about an event action.

Type annotations and code completion for `#!python session.client("dataexchange").get_event_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# get_event_action method definition

await def get_event_action(
    self,
    *,
    EventActionId: str,
) -> GetEventActionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEventActionResponseTypeDef](./type_defs.md#geteventactionresponsetypedef) 


```python
# get_event_action method usage example with argument unpacking

kwargs: GetEventActionRequestRequestTypeDef = {  # (1)
    "EventActionId": ...,
}

parent.get_event_action(**kwargs)
```

1. See [:material-code-braces: GetEventActionRequestRequestTypeDef](./type_defs.md#geteventactionrequestrequesttypedef) 

### get\_job

This operation returns information about a job.

Type annotations and code completion for `#!python session.client("dataexchange").get_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# get_job method definition

await def get_job(
    self,
    *,
    JobId: str,
) -> GetJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetJobResponseTypeDef](./type_defs.md#getjobresponsetypedef) 


```python
# get_job method usage example with argument unpacking

kwargs: GetJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.get_job(**kwargs)
```

1. See [:material-code-braces: GetJobRequestRequestTypeDef](./type_defs.md#getjobrequestrequesttypedef) 

### get\_received\_data\_grant

This operation returns information about a received data grant.

Type annotations and code completion for `#!python session.client("dataexchange").get_received_data_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# get_received_data_grant method definition

await def get_received_data_grant(
    self,
    *,
    DataGrantArn: str,
) -> GetReceivedDataGrantResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetReceivedDataGrantResponseTypeDef](./type_defs.md#getreceiveddatagrantresponsetypedef) 


```python
# get_received_data_grant method usage example with argument unpacking

kwargs: GetReceivedDataGrantRequestRequestTypeDef = {  # (1)
    "DataGrantArn": ...,
}

parent.get_received_data_grant(**kwargs)
```

1. See [:material-code-braces: GetReceivedDataGrantRequestRequestTypeDef](./type_defs.md#getreceiveddatagrantrequestrequesttypedef) 

### get\_revision

This operation returns information about a revision.

Type annotations and code completion for `#!python session.client("dataexchange").get_revision` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# get_revision method definition

await def get_revision(
    self,
    *,
    DataSetId: str,
    RevisionId: str,
) -> GetRevisionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRevisionResponseTypeDef](./type_defs.md#getrevisionresponsetypedef) 


```python
# get_revision method usage example with argument unpacking

kwargs: GetRevisionRequestRequestTypeDef = {  # (1)
    "DataSetId": ...,
    "RevisionId": ...,
}

parent.get_revision(**kwargs)
```

1. See [:material-code-braces: GetRevisionRequestRequestTypeDef](./type_defs.md#getrevisionrequestrequesttypedef) 

### list\_data\_grants

This operation returns information about all data grants.

Type annotations and code completion for `#!python session.client("dataexchange").list_data_grants` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# list_data_grants method definition

await def list_data_grants(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListDataGrantsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataGrantsResponseTypeDef](./type_defs.md#listdatagrantsresponsetypedef) 


```python
# list_data_grants method usage example with argument unpacking

kwargs: ListDataGrantsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_data_grants(**kwargs)
```

1. See [:material-code-braces: ListDataGrantsRequestRequestTypeDef](./type_defs.md#listdatagrantsrequestrequesttypedef) 

### list\_data\_set\_revisions

This operation lists a data set's revisions sorted by CreatedAt in descending
order.

Type annotations and code completion for `#!python session.client("dataexchange").list_data_set_revisions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# list_data_set_revisions method definition

await def list_data_set_revisions(
    self,
    *,
    DataSetId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListDataSetRevisionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataSetRevisionsResponseTypeDef](./type_defs.md#listdatasetrevisionsresponsetypedef) 


```python
# list_data_set_revisions method usage example with argument unpacking

kwargs: ListDataSetRevisionsRequestRequestTypeDef = {  # (1)
    "DataSetId": ...,
}

parent.list_data_set_revisions(**kwargs)
```

1. See [:material-code-braces: ListDataSetRevisionsRequestRequestTypeDef](./type_defs.md#listdatasetrevisionsrequestrequesttypedef) 

### list\_data\_sets

This operation lists your data sets.

Type annotations and code completion for `#!python session.client("dataexchange").list_data_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# list_data_sets method definition

await def list_data_sets(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    Origin: str = ...,
) -> ListDataSetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataSetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python
# list_data_sets method usage example with argument unpacking

kwargs: ListDataSetsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_data_sets(**kwargs)
```

1. See [:material-code-braces: ListDataSetsRequestRequestTypeDef](./type_defs.md#listdatasetsrequestrequesttypedef) 

### list\_event\_actions

This operation lists your event actions.

Type annotations and code completion for `#!python session.client("dataexchange").list_event_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# list_event_actions method definition

await def list_event_actions(
    self,
    *,
    EventSourceId: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListEventActionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEventActionsResponseTypeDef](./type_defs.md#listeventactionsresponsetypedef) 


```python
# list_event_actions method usage example with argument unpacking

kwargs: ListEventActionsRequestRequestTypeDef = {  # (1)
    "EventSourceId": ...,
}

parent.list_event_actions(**kwargs)
```

1. See [:material-code-braces: ListEventActionsRequestRequestTypeDef](./type_defs.md#listeventactionsrequestrequesttypedef) 

### list\_jobs

This operation lists your jobs sorted by CreatedAt in descending order.

Type annotations and code completion for `#!python session.client("dataexchange").list_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# list_jobs method definition

await def list_jobs(
    self,
    *,
    DataSetId: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    RevisionId: str = ...,
) -> ListJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef) 


```python
# list_jobs method usage example with argument unpacking

kwargs: ListJobsRequestRequestTypeDef = {  # (1)
    "DataSetId": ...,
}

parent.list_jobs(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestRequestTypeDef](./type_defs.md#listjobsrequestrequesttypedef) 

### list\_received\_data\_grants

This operation returns information about all received data grants.

Type annotations and code completion for `#!python session.client("dataexchange").list_received_data_grants` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# list_received_data_grants method definition

await def list_received_data_grants(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    AcceptanceState: Sequence[AcceptanceStateFilterValueType] = ...,  # (1)
) -> ListReceivedDataGrantsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AcceptanceStateFilterValueType](./literals.md#acceptancestatefiltervaluetype) 
2. See [:material-code-braces: ListReceivedDataGrantsResponseTypeDef](./type_defs.md#listreceiveddatagrantsresponsetypedef) 


```python
# list_received_data_grants method usage example with argument unpacking

kwargs: ListReceivedDataGrantsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_received_data_grants(**kwargs)
```

1. See [:material-code-braces: ListReceivedDataGrantsRequestRequestTypeDef](./type_defs.md#listreceiveddatagrantsrequestrequesttypedef) 

### list\_revision\_assets

This operation lists a revision's assets sorted alphabetically in descending
order.

Type annotations and code completion for `#!python session.client("dataexchange").list_revision_assets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# list_revision_assets method definition

await def list_revision_assets(
    self,
    *,
    DataSetId: str,
    RevisionId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListRevisionAssetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRevisionAssetsResponseTypeDef](./type_defs.md#listrevisionassetsresponsetypedef) 


```python
# list_revision_assets method usage example with argument unpacking

kwargs: ListRevisionAssetsRequestRequestTypeDef = {  # (1)
    "DataSetId": ...,
    "RevisionId": ...,
}

parent.list_revision_assets(**kwargs)
```

1. See [:material-code-braces: ListRevisionAssetsRequestRequestTypeDef](./type_defs.md#listrevisionassetsrequestrequesttypedef) 

### list\_tags\_for\_resource

This operation lists the tags on the resource.

Type annotations and code completion for `#!python session.client("dataexchange").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### revoke\_revision

This operation revokes subscribers' access to a revision.

Type annotations and code completion for `#!python session.client("dataexchange").revoke_revision` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# revoke_revision method definition

await def revoke_revision(
    self,
    *,
    DataSetId: str,
    RevisionId: str,
    RevocationComment: str,
) -> RevokeRevisionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RevokeRevisionResponseTypeDef](./type_defs.md#revokerevisionresponsetypedef) 


```python
# revoke_revision method usage example with argument unpacking

kwargs: RevokeRevisionRequestRequestTypeDef = {  # (1)
    "DataSetId": ...,
    "RevisionId": ...,
    "RevocationComment": ...,
}

parent.revoke_revision(**kwargs)
```

1. See [:material-code-braces: RevokeRevisionRequestRequestTypeDef](./type_defs.md#revokerevisionrequestrequesttypedef) 

### send\_api\_asset

This operation invokes an API Gateway API asset.

Type annotations and code completion for `#!python session.client("dataexchange").send_api_asset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# send_api_asset method definition

await def send_api_asset(
    self,
    *,
    AssetId: str,
    DataSetId: str,
    RevisionId: str,
    Body: str = ...,
    QueryStringParameters: Mapping[str, str] = ...,
    RequestHeaders: Mapping[str, str] = ...,
    Method: str = ...,
    Path: str = ...,
) -> SendApiAssetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SendApiAssetResponseTypeDef](./type_defs.md#sendapiassetresponsetypedef) 


```python
# send_api_asset method usage example with argument unpacking

kwargs: SendApiAssetRequestRequestTypeDef = {  # (1)
    "AssetId": ...,
    "DataSetId": ...,
    "RevisionId": ...,
}

parent.send_api_asset(**kwargs)
```

1. See [:material-code-braces: SendApiAssetRequestRequestTypeDef](./type_defs.md#sendapiassetrequestrequesttypedef) 

### send\_data\_set\_notification

The type of event associated with the data set.

Type annotations and code completion for `#!python session.client("dataexchange").send_data_set_notification` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# send_data_set_notification method definition

await def send_data_set_notification(
    self,
    *,
    DataSetId: str,
    Type: NotificationTypeType,  # (1)
    Scope: ScopeDetailsTypeDef = ...,  # (2)
    ClientToken: str = ...,
    Comment: str = ...,
    Details: NotificationDetailsTypeDef = ...,  # (3)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
2. See [:material-code-braces: ScopeDetailsTypeDef](./type_defs.md#scopedetailstypedef) 
3. See [:material-code-braces: NotificationDetailsTypeDef](./type_defs.md#notificationdetailstypedef) 


```python
# send_data_set_notification method usage example with argument unpacking

kwargs: SendDataSetNotificationRequestRequestTypeDef = {  # (1)
    "DataSetId": ...,
    "Type": ...,
}

parent.send_data_set_notification(**kwargs)
```

1. See [:material-code-braces: SendDataSetNotificationRequestRequestTypeDef](./type_defs.md#senddatasetnotificationrequestrequesttypedef) 

### start\_job

This operation starts a job.

Type annotations and code completion for `#!python session.client("dataexchange").start_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# start_job method definition

await def start_job(
    self,
    *,
    JobId: str,
) -> dict[str, Any]:
    ...
```



```python
# start_job method usage example with argument unpacking

kwargs: StartJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.start_job(**kwargs)
```

1. See [:material-code-braces: StartJobRequestRequestTypeDef](./type_defs.md#startjobrequestrequesttypedef) 

### tag\_resource

This operation tags a resource.

Type annotations and code completion for `#!python session.client("dataexchange").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

This operation removes one or more tags from a resource.

Type annotations and code completion for `#!python session.client("dataexchange").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_asset

This operation updates an asset.

Type annotations and code completion for `#!python session.client("dataexchange").update_asset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# update_asset method definition

await def update_asset(
    self,
    *,
    AssetId: str,
    DataSetId: str,
    Name: str,
    RevisionId: str,
) -> UpdateAssetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateAssetResponseTypeDef](./type_defs.md#updateassetresponsetypedef) 


```python
# update_asset method usage example with argument unpacking

kwargs: UpdateAssetRequestRequestTypeDef = {  # (1)
    "AssetId": ...,
    "DataSetId": ...,
    "Name": ...,
    "RevisionId": ...,
}

parent.update_asset(**kwargs)
```

1. See [:material-code-braces: UpdateAssetRequestRequestTypeDef](./type_defs.md#updateassetrequestrequesttypedef) 

### update\_data\_set

This operation updates a data set.

Type annotations and code completion for `#!python session.client("dataexchange").update_data_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# update_data_set method definition

await def update_data_set(
    self,
    *,
    DataSetId: str,
    Description: str = ...,
    Name: str = ...,
) -> UpdateDataSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateDataSetResponseTypeDef](./type_defs.md#updatedatasetresponsetypedef) 


```python
# update_data_set method usage example with argument unpacking

kwargs: UpdateDataSetRequestRequestTypeDef = {  # (1)
    "DataSetId": ...,
}

parent.update_data_set(**kwargs)
```

1. See [:material-code-braces: UpdateDataSetRequestRequestTypeDef](./type_defs.md#updatedatasetrequestrequesttypedef) 

### update\_event\_action

This operation updates the event action.

Type annotations and code completion for `#!python session.client("dataexchange").update_event_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# update_event_action method definition

await def update_event_action(
    self,
    *,
    EventActionId: str,
    Action: ActionTypeDef = ...,  # (1)
) -> UpdateEventActionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: UpdateEventActionResponseTypeDef](./type_defs.md#updateeventactionresponsetypedef) 


```python
# update_event_action method usage example with argument unpacking

kwargs: UpdateEventActionRequestRequestTypeDef = {  # (1)
    "EventActionId": ...,
}

parent.update_event_action(**kwargs)
```

1. See [:material-code-braces: UpdateEventActionRequestRequestTypeDef](./type_defs.md#updateeventactionrequestrequesttypedef) 

### update\_revision

This operation updates a revision.

Type annotations and code completion for `#!python session.client("dataexchange").update_revision` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# update_revision method definition

await def update_revision(
    self,
    *,
    DataSetId: str,
    RevisionId: str,
    Comment: str = ...,
    Finalized: bool = ...,
) -> UpdateRevisionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateRevisionResponseTypeDef](./type_defs.md#updaterevisionresponsetypedef) 


```python
# update_revision method usage example with argument unpacking

kwargs: UpdateRevisionRequestRequestTypeDef = {  # (1)
    "DataSetId": ...,
    "RevisionId": ...,
}

parent.update_revision(**kwargs)
```

1. See [:material-code-braces: UpdateRevisionRequestRequestTypeDef](./type_defs.md#updaterevisionrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("dataexchange").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("dataexchange").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Client)

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




### get_paginator

Type annotations and code completion for `#!python session.client("dataexchange").get_paginator` method with overloads.

- `client.get_paginator("list_data_grants")` -> [ListDataGrantsPaginator](./paginators.md#listdatagrantspaginator)
- `client.get_paginator("list_data_set_revisions")` -> [ListDataSetRevisionsPaginator](./paginators.md#listdatasetrevisionspaginator)
- `client.get_paginator("list_data_sets")` -> [ListDataSetsPaginator](./paginators.md#listdatasetspaginator)
- `client.get_paginator("list_event_actions")` -> [ListEventActionsPaginator](./paginators.md#listeventactionspaginator)
- `client.get_paginator("list_jobs")` -> [ListJobsPaginator](./paginators.md#listjobspaginator)
- `client.get_paginator("list_received_data_grants")` -> [ListReceivedDataGrantsPaginator](./paginators.md#listreceiveddatagrantspaginator)
- `client.get_paginator("list_revision_assets")` -> [ListRevisionAssetsPaginator](./paginators.md#listrevisionassetspaginator)


