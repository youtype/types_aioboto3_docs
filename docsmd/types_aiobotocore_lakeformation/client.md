# LakeFormationClient

> [Index](../README.md) > [LakeFormation](./README.md) > LakeFormationClient

!!! note ""

    Auto-generated documentation for [LakeFormation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#lakeformation)
    type annotations stubs module [types-aiobotocore-lakeformation](https://pypi.org/project/types-aiobotocore-lakeformation/).

## LakeFormationClient

Type annotations and code completion for `#!python session.client("lakeformation")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# LakeFormationClient usage example

from aioboto3.session import Session
from types_aiobotocore_lakeformation.client import LakeFormationClient

session = Session()
async with session.client("lakeformation") as client:
    client: LakeFormationClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("lakeformation").exceptions` structure.

```python
# LakeFormationClient.exceptions usage example

async with session.client("lakeformation") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.AlreadyExistsException,
        client.exceptions.ClientError,
        client.exceptions.ConcurrentModificationException,
        client.exceptions.EntityNotFoundException,
        client.exceptions.ExpiredException,
        client.exceptions.GlueEncryptionException,
        client.exceptions.InternalServiceException,
        client.exceptions.InvalidInputException,
        client.exceptions.OperationTimeoutException,
        client.exceptions.PermissionTypeMismatchException,
        client.exceptions.ResourceNotReadyException,
        client.exceptions.ResourceNumberLimitExceededException,
        client.exceptions.StatisticsNotReadyYetException,
        client.exceptions.ThrottledException,
        client.exceptions.TransactionCanceledException,
        client.exceptions.TransactionCommitInProgressException,
        client.exceptions.TransactionCommittedException,
        client.exceptions.WorkUnitsNotReadyYetException,
    ) as e:
        print(e)
```

```python
# LakeFormationClient.exceptions type checking example

from types_aiobotocore_lakeformation.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("lakeformation").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("lakeformation").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

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


### add\_lf\_tags\_to\_resource

Attaches one or more LF-tags to an existing resource.

Type annotations and code completion for `#!python session.client("lakeformation").add_lf_tags_to_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# add_lf_tags_to_resource method definition

await def add_lf_tags_to_resource(
    self,
    *,
    Resource: ResourceTypeDef,  # (1)
    LFTags: Sequence[LFTagPairUnionTypeDef],  # (2)
    CatalogId: str = ...,
) -> AddLFTagsToResourceResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: LFTagPairTypeDef](./type_defs.md#lftagpairtypedef) [:material-code-braces: LFTagPairOutputTypeDef](./type_defs.md#lftagpairoutputtypedef) 
3. See [:material-code-braces: AddLFTagsToResourceResponseTypeDef](./type_defs.md#addlftagstoresourceresponsetypedef) 


```python
# add_lf_tags_to_resource method usage example with argument unpacking

kwargs: AddLFTagsToResourceRequestRequestTypeDef = {  # (1)
    "Resource": ...,
    "LFTags": ...,
}

parent.add_lf_tags_to_resource(**kwargs)
```

1. See [:material-code-braces: AddLFTagsToResourceRequestRequestTypeDef](./type_defs.md#addlftagstoresourcerequestrequesttypedef) 

### assume\_decorated\_role\_with\_saml

Allows a caller to assume an IAM role decorated as the SAML user specified in
the SAML assertion included in the request.

Type annotations and code completion for `#!python session.client("lakeformation").assume_decorated_role_with_saml` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# assume_decorated_role_with_saml method definition

await def assume_decorated_role_with_saml(
    self,
    *,
    SAMLAssertion: str,
    RoleArn: str,
    PrincipalArn: str,
    DurationSeconds: int = ...,
) -> AssumeDecoratedRoleWithSAMLResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssumeDecoratedRoleWithSAMLResponseTypeDef](./type_defs.md#assumedecoratedrolewithsamlresponsetypedef) 


```python
# assume_decorated_role_with_saml method usage example with argument unpacking

kwargs: AssumeDecoratedRoleWithSAMLRequestRequestTypeDef = {  # (1)
    "SAMLAssertion": ...,
    "RoleArn": ...,
    "PrincipalArn": ...,
}

parent.assume_decorated_role_with_saml(**kwargs)
```

1. See [:material-code-braces: AssumeDecoratedRoleWithSAMLRequestRequestTypeDef](./type_defs.md#assumedecoratedrolewithsamlrequestrequesttypedef) 

### batch\_grant\_permissions

Batch operation to grant permissions to the principal.

Type annotations and code completion for `#!python session.client("lakeformation").batch_grant_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# batch_grant_permissions method definition

await def batch_grant_permissions(
    self,
    *,
    Entries: Sequence[BatchPermissionsRequestEntryUnionTypeDef],  # (1)
    CatalogId: str = ...,
) -> BatchGrantPermissionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BatchPermissionsRequestEntryTypeDef](./type_defs.md#batchpermissionsrequestentrytypedef) [:material-code-braces: BatchPermissionsRequestEntryOutputTypeDef](./type_defs.md#batchpermissionsrequestentryoutputtypedef) 
2. See [:material-code-braces: BatchGrantPermissionsResponseTypeDef](./type_defs.md#batchgrantpermissionsresponsetypedef) 


```python
# batch_grant_permissions method usage example with argument unpacking

kwargs: BatchGrantPermissionsRequestRequestTypeDef = {  # (1)
    "Entries": ...,
}

parent.batch_grant_permissions(**kwargs)
```

1. See [:material-code-braces: BatchGrantPermissionsRequestRequestTypeDef](./type_defs.md#batchgrantpermissionsrequestrequesttypedef) 

### batch\_revoke\_permissions

Batch operation to revoke permissions from the principal.

Type annotations and code completion for `#!python session.client("lakeformation").batch_revoke_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# batch_revoke_permissions method definition

await def batch_revoke_permissions(
    self,
    *,
    Entries: Sequence[BatchPermissionsRequestEntryTypeDef],  # (1)
    CatalogId: str = ...,
) -> BatchRevokePermissionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BatchPermissionsRequestEntryTypeDef](./type_defs.md#batchpermissionsrequestentrytypedef) 
2. See [:material-code-braces: BatchRevokePermissionsResponseTypeDef](./type_defs.md#batchrevokepermissionsresponsetypedef) 


```python
# batch_revoke_permissions method usage example with argument unpacking

kwargs: BatchRevokePermissionsRequestRequestTypeDef = {  # (1)
    "Entries": ...,
}

parent.batch_revoke_permissions(**kwargs)
```

1. See [:material-code-braces: BatchRevokePermissionsRequestRequestTypeDef](./type_defs.md#batchrevokepermissionsrequestrequesttypedef) 

### cancel\_transaction

Attempts to cancel the specified transaction.

Type annotations and code completion for `#!python session.client("lakeformation").cancel_transaction` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# cancel_transaction method definition

await def cancel_transaction(
    self,
    *,
    TransactionId: str,
) -> dict[str, Any]:
    ...
```



```python
# cancel_transaction method usage example with argument unpacking

kwargs: CancelTransactionRequestRequestTypeDef = {  # (1)
    "TransactionId": ...,
}

parent.cancel_transaction(**kwargs)
```

1. See [:material-code-braces: CancelTransactionRequestRequestTypeDef](./type_defs.md#canceltransactionrequestrequesttypedef) 

### commit\_transaction

Attempts to commit the specified transaction.

Type annotations and code completion for `#!python session.client("lakeformation").commit_transaction` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# commit_transaction method definition

await def commit_transaction(
    self,
    *,
    TransactionId: str,
) -> CommitTransactionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CommitTransactionResponseTypeDef](./type_defs.md#committransactionresponsetypedef) 


```python
# commit_transaction method usage example with argument unpacking

kwargs: CommitTransactionRequestRequestTypeDef = {  # (1)
    "TransactionId": ...,
}

parent.commit_transaction(**kwargs)
```

1. See [:material-code-braces: CommitTransactionRequestRequestTypeDef](./type_defs.md#committransactionrequestrequesttypedef) 

### create\_data\_cells\_filter

Creates a data cell filter to allow one to grant access to certain columns on
certain rows.

Type annotations and code completion for `#!python session.client("lakeformation").create_data_cells_filter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# create_data_cells_filter method definition

await def create_data_cells_filter(
    self,
    *,
    TableData: DataCellsFilterTypeDef,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: DataCellsFilterTypeDef](./type_defs.md#datacellsfiltertypedef) 


```python
# create_data_cells_filter method usage example with argument unpacking

kwargs: CreateDataCellsFilterRequestRequestTypeDef = {  # (1)
    "TableData": ...,
}

parent.create_data_cells_filter(**kwargs)
```

1. See [:material-code-braces: CreateDataCellsFilterRequestRequestTypeDef](./type_defs.md#createdatacellsfilterrequestrequesttypedef) 

### create\_lf\_tag

Creates an LF-tag with the specified name and values.

Type annotations and code completion for `#!python session.client("lakeformation").create_lf_tag` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# create_lf_tag method definition

await def create_lf_tag(
    self,
    *,
    TagKey: str,
    TagValues: Sequence[str],
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# create_lf_tag method usage example with argument unpacking

kwargs: CreateLFTagRequestRequestTypeDef = {  # (1)
    "TagKey": ...,
    "TagValues": ...,
}

parent.create_lf_tag(**kwargs)
```

1. See [:material-code-braces: CreateLFTagRequestRequestTypeDef](./type_defs.md#createlftagrequestrequesttypedef) 

### create\_lf\_tag\_expression

Creates a new LF-Tag expression with the provided name, description, catalog
ID, and expression body.

Type annotations and code completion for `#!python session.client("lakeformation").create_lf_tag_expression` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# create_lf_tag_expression method definition

await def create_lf_tag_expression(
    self,
    *,
    Name: str,
    Expression: Sequence[LFTagUnionTypeDef],  # (1)
    Description: str = ...,
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: LFTagTypeDef](./type_defs.md#lftagtypedef) [:material-code-braces: LFTagOutputTypeDef](./type_defs.md#lftagoutputtypedef) 


```python
# create_lf_tag_expression method usage example with argument unpacking

kwargs: CreateLFTagExpressionRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Expression": ...,
}

parent.create_lf_tag_expression(**kwargs)
```

1. See [:material-code-braces: CreateLFTagExpressionRequestRequestTypeDef](./type_defs.md#createlftagexpressionrequestrequesttypedef) 

### create\_lake\_formation\_identity\_center\_configuration

Creates an IAM Identity Center connection with Lake Formation to allow IAM
Identity Center users and groups to access Data Catalog resources.

Type annotations and code completion for `#!python session.client("lakeformation").create_lake_formation_identity_center_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# create_lake_formation_identity_center_configuration method definition

await def create_lake_formation_identity_center_configuration(
    self,
    *,
    CatalogId: str = ...,
    InstanceArn: str = ...,
    ExternalFiltering: ExternalFilteringConfigurationTypeDef = ...,  # (1)
    ShareRecipients: Sequence[DataLakePrincipalTypeDef] = ...,  # (2)
) -> CreateLakeFormationIdentityCenterConfigurationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ExternalFilteringConfigurationTypeDef](./type_defs.md#externalfilteringconfigurationtypedef) 
2. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
3. See [:material-code-braces: CreateLakeFormationIdentityCenterConfigurationResponseTypeDef](./type_defs.md#createlakeformationidentitycenterconfigurationresponsetypedef) 


```python
# create_lake_formation_identity_center_configuration method usage example with argument unpacking

kwargs: CreateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.create_lake_formation_identity_center_configuration(**kwargs)
```

1. See [:material-code-braces: CreateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef](./type_defs.md#createlakeformationidentitycenterconfigurationrequestrequesttypedef) 

### create\_lake\_formation\_opt\_in

Enforce Lake Formation permissions for the given databases, tables, and
principals.

Type annotations and code completion for `#!python session.client("lakeformation").create_lake_formation_opt_in` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# create_lake_formation_opt_in method definition

await def create_lake_formation_opt_in(
    self,
    *,
    Principal: DataLakePrincipalTypeDef,  # (1)
    Resource: ResourceTypeDef,  # (2)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 


```python
# create_lake_formation_opt_in method usage example with argument unpacking

kwargs: CreateLakeFormationOptInRequestRequestTypeDef = {  # (1)
    "Principal": ...,
    "Resource": ...,
}

parent.create_lake_formation_opt_in(**kwargs)
```

1. See [:material-code-braces: CreateLakeFormationOptInRequestRequestTypeDef](./type_defs.md#createlakeformationoptinrequestrequesttypedef) 

### delete\_data\_cells\_filter

Deletes a data cell filter.

Type annotations and code completion for `#!python session.client("lakeformation").delete_data_cells_filter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# delete_data_cells_filter method definition

await def delete_data_cells_filter(
    self,
    *,
    TableCatalogId: str = ...,
    DatabaseName: str = ...,
    TableName: str = ...,
    Name: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_data_cells_filter method usage example with argument unpacking

kwargs: DeleteDataCellsFilterRequestRequestTypeDef = {  # (1)
    "TableCatalogId": ...,
}

parent.delete_data_cells_filter(**kwargs)
```

1. See [:material-code-braces: DeleteDataCellsFilterRequestRequestTypeDef](./type_defs.md#deletedatacellsfilterrequestrequesttypedef) 

### delete\_lf\_tag

Deletes the specified LF-tag given a key name.

Type annotations and code completion for `#!python session.client("lakeformation").delete_lf_tag` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# delete_lf_tag method definition

await def delete_lf_tag(
    self,
    *,
    TagKey: str,
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_lf_tag method usage example with argument unpacking

kwargs: DeleteLFTagRequestRequestTypeDef = {  # (1)
    "TagKey": ...,
}

parent.delete_lf_tag(**kwargs)
```

1. See [:material-code-braces: DeleteLFTagRequestRequestTypeDef](./type_defs.md#deletelftagrequestrequesttypedef) 

### delete\_lf\_tag\_expression

Deletes the LF-Tag expression.

Type annotations and code completion for `#!python session.client("lakeformation").delete_lf_tag_expression` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# delete_lf_tag_expression method definition

await def delete_lf_tag_expression(
    self,
    *,
    Name: str,
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_lf_tag_expression method usage example with argument unpacking

kwargs: DeleteLFTagExpressionRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_lf_tag_expression(**kwargs)
```

1. See [:material-code-braces: DeleteLFTagExpressionRequestRequestTypeDef](./type_defs.md#deletelftagexpressionrequestrequesttypedef) 

### delete\_lake\_formation\_identity\_center\_configuration

Deletes an IAM Identity Center connection with Lake Formation.

Type annotations and code completion for `#!python session.client("lakeformation").delete_lake_formation_identity_center_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# delete_lake_formation_identity_center_configuration method definition

await def delete_lake_formation_identity_center_configuration(
    self,
    *,
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_lake_formation_identity_center_configuration method usage example with argument unpacking

kwargs: DeleteLakeFormationIdentityCenterConfigurationRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.delete_lake_formation_identity_center_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteLakeFormationIdentityCenterConfigurationRequestRequestTypeDef](./type_defs.md#deletelakeformationidentitycenterconfigurationrequestrequesttypedef) 

### delete\_lake\_formation\_opt\_in

Remove the Lake Formation permissions enforcement of the given databases,
tables, and principals.

Type annotations and code completion for `#!python session.client("lakeformation").delete_lake_formation_opt_in` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# delete_lake_formation_opt_in method definition

await def delete_lake_formation_opt_in(
    self,
    *,
    Principal: DataLakePrincipalTypeDef,  # (1)
    Resource: ResourceTypeDef,  # (2)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 


```python
# delete_lake_formation_opt_in method usage example with argument unpacking

kwargs: DeleteLakeFormationOptInRequestRequestTypeDef = {  # (1)
    "Principal": ...,
    "Resource": ...,
}

parent.delete_lake_formation_opt_in(**kwargs)
```

1. See [:material-code-braces: DeleteLakeFormationOptInRequestRequestTypeDef](./type_defs.md#deletelakeformationoptinrequestrequesttypedef) 

### delete\_objects\_on\_cancel

For a specific governed table, provides a list of Amazon S3 objects that will
be written during the current transaction and that can be automatically deleted
if the transaction is canceled.

Type annotations and code completion for `#!python session.client("lakeformation").delete_objects_on_cancel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# delete_objects_on_cancel method definition

await def delete_objects_on_cancel(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    TransactionId: str,
    Objects: Sequence[VirtualObjectTypeDef],  # (1)
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: VirtualObjectTypeDef](./type_defs.md#virtualobjecttypedef) 


```python
# delete_objects_on_cancel method usage example with argument unpacking

kwargs: DeleteObjectsOnCancelRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "TransactionId": ...,
    "Objects": ...,
}

parent.delete_objects_on_cancel(**kwargs)
```

1. See [:material-code-braces: DeleteObjectsOnCancelRequestRequestTypeDef](./type_defs.md#deleteobjectsoncancelrequestrequesttypedef) 

### deregister\_resource

Deregisters the resource as managed by the Data Catalog.

Type annotations and code completion for `#!python session.client("lakeformation").deregister_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# deregister_resource method definition

await def deregister_resource(
    self,
    *,
    ResourceArn: str,
) -> dict[str, Any]:
    ...
```



```python
# deregister_resource method usage example with argument unpacking

kwargs: DeregisterResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.deregister_resource(**kwargs)
```

1. See [:material-code-braces: DeregisterResourceRequestRequestTypeDef](./type_defs.md#deregisterresourcerequestrequesttypedef) 

### describe\_lake\_formation\_identity\_center\_configuration

Retrieves the instance ARN and application ARN for the connection.

Type annotations and code completion for `#!python session.client("lakeformation").describe_lake_formation_identity_center_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# describe_lake_formation_identity_center_configuration method definition

await def describe_lake_formation_identity_center_configuration(
    self,
    *,
    CatalogId: str = ...,
) -> DescribeLakeFormationIdentityCenterConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLakeFormationIdentityCenterConfigurationResponseTypeDef](./type_defs.md#describelakeformationidentitycenterconfigurationresponsetypedef) 


```python
# describe_lake_formation_identity_center_configuration method usage example with argument unpacking

kwargs: DescribeLakeFormationIdentityCenterConfigurationRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.describe_lake_formation_identity_center_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeLakeFormationIdentityCenterConfigurationRequestRequestTypeDef](./type_defs.md#describelakeformationidentitycenterconfigurationrequestrequesttypedef) 

### describe\_resource

Retrieves the current data access role for the given resource registered in
Lake Formation.

Type annotations and code completion for `#!python session.client("lakeformation").describe_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# describe_resource method definition

await def describe_resource(
    self,
    *,
    ResourceArn: str,
) -> DescribeResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeResourceResponseTypeDef](./type_defs.md#describeresourceresponsetypedef) 


```python
# describe_resource method usage example with argument unpacking

kwargs: DescribeResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.describe_resource(**kwargs)
```

1. See [:material-code-braces: DescribeResourceRequestRequestTypeDef](./type_defs.md#describeresourcerequestrequesttypedef) 

### describe\_transaction

Returns the details of a single transaction.

Type annotations and code completion for `#!python session.client("lakeformation").describe_transaction` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# describe_transaction method definition

await def describe_transaction(
    self,
    *,
    TransactionId: str,
) -> DescribeTransactionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTransactionResponseTypeDef](./type_defs.md#describetransactionresponsetypedef) 


```python
# describe_transaction method usage example with argument unpacking

kwargs: DescribeTransactionRequestRequestTypeDef = {  # (1)
    "TransactionId": ...,
}

parent.describe_transaction(**kwargs)
```

1. See [:material-code-braces: DescribeTransactionRequestRequestTypeDef](./type_defs.md#describetransactionrequestrequesttypedef) 

### extend\_transaction

Indicates to the service that the specified transaction is still active and
should not be treated as idle and aborted.

Type annotations and code completion for `#!python session.client("lakeformation").extend_transaction` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# extend_transaction method definition

await def extend_transaction(
    self,
    *,
    TransactionId: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# extend_transaction method usage example with argument unpacking

kwargs: ExtendTransactionRequestRequestTypeDef = {  # (1)
    "TransactionId": ...,
}

parent.extend_transaction(**kwargs)
```

1. See [:material-code-braces: ExtendTransactionRequestRequestTypeDef](./type_defs.md#extendtransactionrequestrequesttypedef) 

### get\_data\_cells\_filter

Returns a data cells filter.

Type annotations and code completion for `#!python session.client("lakeformation").get_data_cells_filter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# get_data_cells_filter method definition

await def get_data_cells_filter(
    self,
    *,
    TableCatalogId: str,
    DatabaseName: str,
    TableName: str,
    Name: str,
) -> GetDataCellsFilterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataCellsFilterResponseTypeDef](./type_defs.md#getdatacellsfilterresponsetypedef) 


```python
# get_data_cells_filter method usage example with argument unpacking

kwargs: GetDataCellsFilterRequestRequestTypeDef = {  # (1)
    "TableCatalogId": ...,
    "DatabaseName": ...,
    "TableName": ...,
    "Name": ...,
}

parent.get_data_cells_filter(**kwargs)
```

1. See [:material-code-braces: GetDataCellsFilterRequestRequestTypeDef](./type_defs.md#getdatacellsfilterrequestrequesttypedef) 

### get\_data\_lake\_principal

Returns the identity of the invoking principal.

Type annotations and code completion for `#!python session.client("lakeformation").get_data_lake_principal` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# get_data_lake_principal method definition

await def get_data_lake_principal(
    self,
) -> GetDataLakePrincipalResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataLakePrincipalResponseTypeDef](./type_defs.md#getdatalakeprincipalresponsetypedef) 

### get\_data\_lake\_settings

Retrieves the list of the data lake administrators of a Lake Formation-managed
data lake.

Type annotations and code completion for `#!python session.client("lakeformation").get_data_lake_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# get_data_lake_settings method definition

await def get_data_lake_settings(
    self,
    *,
    CatalogId: str = ...,
) -> GetDataLakeSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataLakeSettingsResponseTypeDef](./type_defs.md#getdatalakesettingsresponsetypedef) 


```python
# get_data_lake_settings method usage example with argument unpacking

kwargs: GetDataLakeSettingsRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.get_data_lake_settings(**kwargs)
```

1. See [:material-code-braces: GetDataLakeSettingsRequestRequestTypeDef](./type_defs.md#getdatalakesettingsrequestrequesttypedef) 

### get\_effective\_permissions\_for\_path

Returns the Lake Formation permissions for a specified table or database
resource located at a path in Amazon S3.

Type annotations and code completion for `#!python session.client("lakeformation").get_effective_permissions_for_path` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# get_effective_permissions_for_path method definition

await def get_effective_permissions_for_path(
    self,
    *,
    ResourceArn: str,
    CatalogId: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetEffectivePermissionsForPathResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEffectivePermissionsForPathResponseTypeDef](./type_defs.md#geteffectivepermissionsforpathresponsetypedef) 


```python
# get_effective_permissions_for_path method usage example with argument unpacking

kwargs: GetEffectivePermissionsForPathRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_effective_permissions_for_path(**kwargs)
```

1. See [:material-code-braces: GetEffectivePermissionsForPathRequestRequestTypeDef](./type_defs.md#geteffectivepermissionsforpathrequestrequesttypedef) 

### get\_lf\_tag

Returns an LF-tag definition.

Type annotations and code completion for `#!python session.client("lakeformation").get_lf_tag` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# get_lf_tag method definition

await def get_lf_tag(
    self,
    *,
    TagKey: str,
    CatalogId: str = ...,
) -> GetLFTagResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLFTagResponseTypeDef](./type_defs.md#getlftagresponsetypedef) 


```python
# get_lf_tag method usage example with argument unpacking

kwargs: GetLFTagRequestRequestTypeDef = {  # (1)
    "TagKey": ...,
}

parent.get_lf_tag(**kwargs)
```

1. See [:material-code-braces: GetLFTagRequestRequestTypeDef](./type_defs.md#getlftagrequestrequesttypedef) 

### get\_lf\_tag\_expression

Returns the details about the LF-Tag expression.

Type annotations and code completion for `#!python session.client("lakeformation").get_lf_tag_expression` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# get_lf_tag_expression method definition

await def get_lf_tag_expression(
    self,
    *,
    Name: str,
    CatalogId: str = ...,
) -> GetLFTagExpressionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLFTagExpressionResponseTypeDef](./type_defs.md#getlftagexpressionresponsetypedef) 


```python
# get_lf_tag_expression method usage example with argument unpacking

kwargs: GetLFTagExpressionRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_lf_tag_expression(**kwargs)
```

1. See [:material-code-braces: GetLFTagExpressionRequestRequestTypeDef](./type_defs.md#getlftagexpressionrequestrequesttypedef) 

### get\_query\_state

Returns the state of a query previously submitted.

Type annotations and code completion for `#!python session.client("lakeformation").get_query_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# get_query_state method definition

await def get_query_state(
    self,
    *,
    QueryId: str,
) -> GetQueryStateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQueryStateResponseTypeDef](./type_defs.md#getquerystateresponsetypedef) 


```python
# get_query_state method usage example with argument unpacking

kwargs: GetQueryStateRequestRequestTypeDef = {  # (1)
    "QueryId": ...,
}

parent.get_query_state(**kwargs)
```

1. See [:material-code-braces: GetQueryStateRequestRequestTypeDef](./type_defs.md#getquerystaterequestrequesttypedef) 

### get\_query\_statistics

Retrieves statistics on the planning and execution of a query.

Type annotations and code completion for `#!python session.client("lakeformation").get_query_statistics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# get_query_statistics method definition

await def get_query_statistics(
    self,
    *,
    QueryId: str,
) -> GetQueryStatisticsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQueryStatisticsResponseTypeDef](./type_defs.md#getquerystatisticsresponsetypedef) 


```python
# get_query_statistics method usage example with argument unpacking

kwargs: GetQueryStatisticsRequestRequestTypeDef = {  # (1)
    "QueryId": ...,
}

parent.get_query_statistics(**kwargs)
```

1. See [:material-code-braces: GetQueryStatisticsRequestRequestTypeDef](./type_defs.md#getquerystatisticsrequestrequesttypedef) 

### get\_resource\_lf\_tags

Returns the LF-tags applied to a resource.

Type annotations and code completion for `#!python session.client("lakeformation").get_resource_lf_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# get_resource_lf_tags method definition

await def get_resource_lf_tags(
    self,
    *,
    Resource: ResourceTypeDef,  # (1)
    CatalogId: str = ...,
    ShowAssignedLFTags: bool = ...,
) -> GetResourceLFTagsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: GetResourceLFTagsResponseTypeDef](./type_defs.md#getresourcelftagsresponsetypedef) 


```python
# get_resource_lf_tags method usage example with argument unpacking

kwargs: GetResourceLFTagsRequestRequestTypeDef = {  # (1)
    "Resource": ...,
}

parent.get_resource_lf_tags(**kwargs)
```

1. See [:material-code-braces: GetResourceLFTagsRequestRequestTypeDef](./type_defs.md#getresourcelftagsrequestrequesttypedef) 

### get\_table\_objects

Returns the set of Amazon S3 objects that make up the specified governed table.

Type annotations and code completion for `#!python session.client("lakeformation").get_table_objects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# get_table_objects method definition

await def get_table_objects(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    CatalogId: str = ...,
    TransactionId: str = ...,
    QueryAsOfTime: TimestampTypeDef = ...,
    PartitionPredicate: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetTableObjectsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTableObjectsResponseTypeDef](./type_defs.md#gettableobjectsresponsetypedef) 


```python
# get_table_objects method usage example with argument unpacking

kwargs: GetTableObjectsRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
}

parent.get_table_objects(**kwargs)
```

1. See [:material-code-braces: GetTableObjectsRequestRequestTypeDef](./type_defs.md#gettableobjectsrequestrequesttypedef) 

### get\_temporary\_glue\_partition\_credentials

This API is identical to <code>GetTemporaryTableCredentials</code> except that
this is used when the target Data Catalog resource is of type Partition.

Type annotations and code completion for `#!python session.client("lakeformation").get_temporary_glue_partition_credentials` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# get_temporary_glue_partition_credentials method definition

await def get_temporary_glue_partition_credentials(
    self,
    *,
    TableArn: str,
    Partition: PartitionValueListTypeDef,  # (1)
    Permissions: Sequence[PermissionType] = ...,  # (2)
    DurationSeconds: int = ...,
    AuditContext: AuditContextTypeDef = ...,  # (3)
    SupportedPermissionTypes: Sequence[PermissionTypeType] = ...,  # (4)
) -> GetTemporaryGluePartitionCredentialsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: PartitionValueListTypeDef](./type_defs.md#partitionvaluelisttypedef) 
2. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
3. See [:material-code-braces: AuditContextTypeDef](./type_defs.md#auditcontexttypedef) 
4. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
5. See [:material-code-braces: GetTemporaryGluePartitionCredentialsResponseTypeDef](./type_defs.md#gettemporarygluepartitioncredentialsresponsetypedef) 


```python
# get_temporary_glue_partition_credentials method usage example with argument unpacking

kwargs: GetTemporaryGluePartitionCredentialsRequestRequestTypeDef = {  # (1)
    "TableArn": ...,
    "Partition": ...,
}

parent.get_temporary_glue_partition_credentials(**kwargs)
```

1. See [:material-code-braces: GetTemporaryGluePartitionCredentialsRequestRequestTypeDef](./type_defs.md#gettemporarygluepartitioncredentialsrequestrequesttypedef) 

### get\_temporary\_glue\_table\_credentials

Allows a caller in a secure environment to assume a role with permission to
access Amazon S3.

Type annotations and code completion for `#!python session.client("lakeformation").get_temporary_glue_table_credentials` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# get_temporary_glue_table_credentials method definition

await def get_temporary_glue_table_credentials(
    self,
    *,
    TableArn: str,
    Permissions: Sequence[PermissionType] = ...,  # (1)
    DurationSeconds: int = ...,
    AuditContext: AuditContextTypeDef = ...,  # (2)
    SupportedPermissionTypes: Sequence[PermissionTypeType] = ...,  # (3)
    S3Path: str = ...,
    QuerySessionContext: QuerySessionContextTypeDef = ...,  # (4)
) -> GetTemporaryGlueTableCredentialsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
2. See [:material-code-braces: AuditContextTypeDef](./type_defs.md#auditcontexttypedef) 
3. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
4. See [:material-code-braces: QuerySessionContextTypeDef](./type_defs.md#querysessioncontexttypedef) 
5. See [:material-code-braces: GetTemporaryGlueTableCredentialsResponseTypeDef](./type_defs.md#gettemporarygluetablecredentialsresponsetypedef) 


```python
# get_temporary_glue_table_credentials method usage example with argument unpacking

kwargs: GetTemporaryGlueTableCredentialsRequestRequestTypeDef = {  # (1)
    "TableArn": ...,
}

parent.get_temporary_glue_table_credentials(**kwargs)
```

1. See [:material-code-braces: GetTemporaryGlueTableCredentialsRequestRequestTypeDef](./type_defs.md#gettemporarygluetablecredentialsrequestrequesttypedef) 

### get\_work\_unit\_results

Returns the work units resulting from the query.

Type annotations and code completion for `#!python session.client("lakeformation").get_work_unit_results` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# get_work_unit_results method definition

await def get_work_unit_results(
    self,
    *,
    QueryId: str,
    WorkUnitId: int,
    WorkUnitToken: str,
) -> GetWorkUnitResultsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkUnitResultsResponseTypeDef](./type_defs.md#getworkunitresultsresponsetypedef) 


```python
# get_work_unit_results method usage example with argument unpacking

kwargs: GetWorkUnitResultsRequestRequestTypeDef = {  # (1)
    "QueryId": ...,
    "WorkUnitId": ...,
    "WorkUnitToken": ...,
}

parent.get_work_unit_results(**kwargs)
```

1. See [:material-code-braces: GetWorkUnitResultsRequestRequestTypeDef](./type_defs.md#getworkunitresultsrequestrequesttypedef) 

### get\_work\_units

Retrieves the work units generated by the <code>StartQueryPlanning</code>
operation.

Type annotations and code completion for `#!python session.client("lakeformation").get_work_units` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# get_work_units method definition

await def get_work_units(
    self,
    *,
    QueryId: str,
    NextToken: str = ...,
    PageSize: int = ...,
) -> GetWorkUnitsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkUnitsResponseTypeDef](./type_defs.md#getworkunitsresponsetypedef) 


```python
# get_work_units method usage example with argument unpacking

kwargs: GetWorkUnitsRequestRequestTypeDef = {  # (1)
    "QueryId": ...,
}

parent.get_work_units(**kwargs)
```

1. See [:material-code-braces: GetWorkUnitsRequestRequestTypeDef](./type_defs.md#getworkunitsrequestrequesttypedef) 

### grant\_permissions

Grants permissions to the principal to access metadata in the Data Catalog and
data organized in underlying data storage such as Amazon S3.

Type annotations and code completion for `#!python session.client("lakeformation").grant_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# grant_permissions method definition

await def grant_permissions(
    self,
    *,
    Principal: DataLakePrincipalTypeDef,  # (1)
    Resource: ResourceTypeDef,  # (2)
    Permissions: Sequence[PermissionType],  # (3)
    CatalogId: str = ...,
    PermissionsWithGrantOption: Sequence[PermissionType] = ...,  # (3)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
3. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
4. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 


```python
# grant_permissions method usage example with argument unpacking

kwargs: GrantPermissionsRequestRequestTypeDef = {  # (1)
    "Principal": ...,
    "Resource": ...,
    "Permissions": ...,
}

parent.grant_permissions(**kwargs)
```

1. See [:material-code-braces: GrantPermissionsRequestRequestTypeDef](./type_defs.md#grantpermissionsrequestrequesttypedef) 

### list\_data\_cells\_filter

Lists all the data cell filters on a table.

Type annotations and code completion for `#!python session.client("lakeformation").list_data_cells_filter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# list_data_cells_filter method definition

await def list_data_cells_filter(
    self,
    *,
    Table: TableResourceTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDataCellsFilterResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TableResourceTypeDef](./type_defs.md#tableresourcetypedef) 
2. See [:material-code-braces: ListDataCellsFilterResponseTypeDef](./type_defs.md#listdatacellsfilterresponsetypedef) 


```python
# list_data_cells_filter method usage example with argument unpacking

kwargs: ListDataCellsFilterRequestRequestTypeDef = {  # (1)
    "Table": ...,
}

parent.list_data_cells_filter(**kwargs)
```

1. See [:material-code-braces: ListDataCellsFilterRequestRequestTypeDef](./type_defs.md#listdatacellsfilterrequestrequesttypedef) 

### list\_lf\_tag\_expressions

Returns the LF-Tag expressions in caller's account filtered based on caller's
permissions.

Type annotations and code completion for `#!python session.client("lakeformation").list_lf_tag_expressions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# list_lf_tag_expressions method definition

await def list_lf_tag_expressions(
    self,
    *,
    CatalogId: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListLFTagExpressionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLFTagExpressionsResponseTypeDef](./type_defs.md#listlftagexpressionsresponsetypedef) 


```python
# list_lf_tag_expressions method usage example with argument unpacking

kwargs: ListLFTagExpressionsRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.list_lf_tag_expressions(**kwargs)
```

1. See [:material-code-braces: ListLFTagExpressionsRequestRequestTypeDef](./type_defs.md#listlftagexpressionsrequestrequesttypedef) 

### list\_lf\_tags

Lists LF-tags that the requester has permission to view.

Type annotations and code completion for `#!python session.client("lakeformation").list_lf_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# list_lf_tags method definition

await def list_lf_tags(
    self,
    *,
    CatalogId: str = ...,
    ResourceShareType: ResourceShareTypeType = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListLFTagsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceShareTypeType](./literals.md#resourcesharetypetype) 
2. See [:material-code-braces: ListLFTagsResponseTypeDef](./type_defs.md#listlftagsresponsetypedef) 


```python
# list_lf_tags method usage example with argument unpacking

kwargs: ListLFTagsRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.list_lf_tags(**kwargs)
```

1. See [:material-code-braces: ListLFTagsRequestRequestTypeDef](./type_defs.md#listlftagsrequestrequesttypedef) 

### list\_lake\_formation\_opt\_ins

Retrieve the current list of resources and principals that are opt in to
enforce Lake Formation permissions.

Type annotations and code completion for `#!python session.client("lakeformation").list_lake_formation_opt_ins` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# list_lake_formation_opt_ins method definition

await def list_lake_formation_opt_ins(
    self,
    *,
    Principal: DataLakePrincipalTypeDef = ...,  # (1)
    Resource: ResourceTypeDef = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListLakeFormationOptInsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
3. See [:material-code-braces: ListLakeFormationOptInsResponseTypeDef](./type_defs.md#listlakeformationoptinsresponsetypedef) 


```python
# list_lake_formation_opt_ins method usage example with argument unpacking

kwargs: ListLakeFormationOptInsRequestRequestTypeDef = {  # (1)
    "Principal": ...,
}

parent.list_lake_formation_opt_ins(**kwargs)
```

1. See [:material-code-braces: ListLakeFormationOptInsRequestRequestTypeDef](./type_defs.md#listlakeformationoptinsrequestrequesttypedef) 

### list\_permissions

Returns a list of the principal permissions on the resource, filtered by the
permissions of the caller.

Type annotations and code completion for `#!python session.client("lakeformation").list_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# list_permissions method definition

await def list_permissions(
    self,
    *,
    CatalogId: str = ...,
    Principal: DataLakePrincipalTypeDef = ...,  # (1)
    ResourceType: DataLakeResourceTypeType = ...,  # (2)
    Resource: ResourceTypeDef = ...,  # (3)
    NextToken: str = ...,
    MaxResults: int = ...,
    IncludeRelated: str = ...,
) -> ListPermissionsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-brackets: DataLakeResourceTypeType](./literals.md#datalakeresourcetypetype) 
3. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
4. See [:material-code-braces: ListPermissionsResponseTypeDef](./type_defs.md#listpermissionsresponsetypedef) 


```python
# list_permissions method usage example with argument unpacking

kwargs: ListPermissionsRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.list_permissions(**kwargs)
```

1. See [:material-code-braces: ListPermissionsRequestRequestTypeDef](./type_defs.md#listpermissionsrequestrequesttypedef) 

### list\_resources

Lists the resources registered to be managed by the Data Catalog.

Type annotations and code completion for `#!python session.client("lakeformation").list_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# list_resources method definition

await def list_resources(
    self,
    *,
    FilterConditionList: Sequence[FilterConditionTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListResourcesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterConditionTypeDef](./type_defs.md#filterconditiontypedef) 
2. See [:material-code-braces: ListResourcesResponseTypeDef](./type_defs.md#listresourcesresponsetypedef) 


```python
# list_resources method usage example with argument unpacking

kwargs: ListResourcesRequestRequestTypeDef = {  # (1)
    "FilterConditionList": ...,
}

parent.list_resources(**kwargs)
```

1. See [:material-code-braces: ListResourcesRequestRequestTypeDef](./type_defs.md#listresourcesrequestrequesttypedef) 

### list\_table\_storage\_optimizers

Returns the configuration of all storage optimizers associated with a specified
table.

Type annotations and code completion for `#!python session.client("lakeformation").list_table_storage_optimizers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# list_table_storage_optimizers method definition

await def list_table_storage_optimizers(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    CatalogId: str = ...,
    StorageOptimizerType: OptimizerTypeType = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTableStorageOptimizersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OptimizerTypeType](./literals.md#optimizertypetype) 
2. See [:material-code-braces: ListTableStorageOptimizersResponseTypeDef](./type_defs.md#listtablestorageoptimizersresponsetypedef) 


```python
# list_table_storage_optimizers method usage example with argument unpacking

kwargs: ListTableStorageOptimizersRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
}

parent.list_table_storage_optimizers(**kwargs)
```

1. See [:material-code-braces: ListTableStorageOptimizersRequestRequestTypeDef](./type_defs.md#listtablestorageoptimizersrequestrequesttypedef) 

### list\_transactions

Returns metadata about transactions and their status.

Type annotations and code completion for `#!python session.client("lakeformation").list_transactions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# list_transactions method definition

await def list_transactions(
    self,
    *,
    CatalogId: str = ...,
    StatusFilter: TransactionStatusFilterType = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTransactionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TransactionStatusFilterType](./literals.md#transactionstatusfiltertype) 
2. See [:material-code-braces: ListTransactionsResponseTypeDef](./type_defs.md#listtransactionsresponsetypedef) 


```python
# list_transactions method usage example with argument unpacking

kwargs: ListTransactionsRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.list_transactions(**kwargs)
```

1. See [:material-code-braces: ListTransactionsRequestRequestTypeDef](./type_defs.md#listtransactionsrequestrequesttypedef) 

### put\_data\_lake\_settings

Sets the list of data lake administrators who have admin privileges on all
resources managed by Lake Formation.

Type annotations and code completion for `#!python session.client("lakeformation").put_data_lake_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# put_data_lake_settings method definition

await def put_data_lake_settings(
    self,
    *,
    DataLakeSettings: DataLakeSettingsTypeDef,  # (1)
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: DataLakeSettingsTypeDef](./type_defs.md#datalakesettingstypedef) 


```python
# put_data_lake_settings method usage example with argument unpacking

kwargs: PutDataLakeSettingsRequestRequestTypeDef = {  # (1)
    "DataLakeSettings": ...,
}

parent.put_data_lake_settings(**kwargs)
```

1. See [:material-code-braces: PutDataLakeSettingsRequestRequestTypeDef](./type_defs.md#putdatalakesettingsrequestrequesttypedef) 

### register\_resource

Registers the resource as managed by the Data Catalog.

Type annotations and code completion for `#!python session.client("lakeformation").register_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# register_resource method definition

await def register_resource(
    self,
    *,
    ResourceArn: str,
    UseServiceLinkedRole: bool = ...,
    RoleArn: str = ...,
    WithFederation: bool = ...,
    HybridAccessEnabled: bool = ...,
) -> dict[str, Any]:
    ...
```



```python
# register_resource method usage example with argument unpacking

kwargs: RegisterResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.register_resource(**kwargs)
```

1. See [:material-code-braces: RegisterResourceRequestRequestTypeDef](./type_defs.md#registerresourcerequestrequesttypedef) 

### remove\_lf\_tags\_from\_resource

Removes an LF-tag from the resource.

Type annotations and code completion for `#!python session.client("lakeformation").remove_lf_tags_from_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# remove_lf_tags_from_resource method definition

await def remove_lf_tags_from_resource(
    self,
    *,
    Resource: ResourceTypeDef,  # (1)
    LFTags: Sequence[LFTagPairTypeDef],  # (2)
    CatalogId: str = ...,
) -> RemoveLFTagsFromResourceResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: LFTagPairTypeDef](./type_defs.md#lftagpairtypedef) 
3. See [:material-code-braces: RemoveLFTagsFromResourceResponseTypeDef](./type_defs.md#removelftagsfromresourceresponsetypedef) 


```python
# remove_lf_tags_from_resource method usage example with argument unpacking

kwargs: RemoveLFTagsFromResourceRequestRequestTypeDef = {  # (1)
    "Resource": ...,
    "LFTags": ...,
}

parent.remove_lf_tags_from_resource(**kwargs)
```

1. See [:material-code-braces: RemoveLFTagsFromResourceRequestRequestTypeDef](./type_defs.md#removelftagsfromresourcerequestrequesttypedef) 

### revoke\_permissions

Revokes permissions to the principal to access metadata in the Data Catalog and
data organized in underlying data storage such as Amazon S3.

Type annotations and code completion for `#!python session.client("lakeformation").revoke_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# revoke_permissions method definition

await def revoke_permissions(
    self,
    *,
    Principal: DataLakePrincipalTypeDef,  # (1)
    Resource: ResourceTypeDef,  # (2)
    Permissions: Sequence[PermissionType],  # (3)
    CatalogId: str = ...,
    PermissionsWithGrantOption: Sequence[PermissionType] = ...,  # (3)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
3. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
4. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 


```python
# revoke_permissions method usage example with argument unpacking

kwargs: RevokePermissionsRequestRequestTypeDef = {  # (1)
    "Principal": ...,
    "Resource": ...,
    "Permissions": ...,
}

parent.revoke_permissions(**kwargs)
```

1. See [:material-code-braces: RevokePermissionsRequestRequestTypeDef](./type_defs.md#revokepermissionsrequestrequesttypedef) 

### search\_databases\_by\_lf\_tags

This operation allows a search on <code>DATABASE</code> resources by
<code>TagCondition</code>.

Type annotations and code completion for `#!python session.client("lakeformation").search_databases_by_lf_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# search_databases_by_lf_tags method definition

await def search_databases_by_lf_tags(
    self,
    *,
    Expression: Sequence[LFTagTypeDef],  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
    CatalogId: str = ...,
) -> SearchDatabasesByLFTagsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LFTagTypeDef](./type_defs.md#lftagtypedef) 
2. See [:material-code-braces: SearchDatabasesByLFTagsResponseTypeDef](./type_defs.md#searchdatabasesbylftagsresponsetypedef) 


```python
# search_databases_by_lf_tags method usage example with argument unpacking

kwargs: SearchDatabasesByLFTagsRequestRequestTypeDef = {  # (1)
    "Expression": ...,
}

parent.search_databases_by_lf_tags(**kwargs)
```

1. See [:material-code-braces: SearchDatabasesByLFTagsRequestRequestTypeDef](./type_defs.md#searchdatabasesbylftagsrequestrequesttypedef) 

### search\_tables\_by\_lf\_tags

This operation allows a search on <code>TABLE</code> resources by
<code>LFTag</code>s.

Type annotations and code completion for `#!python session.client("lakeformation").search_tables_by_lf_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# search_tables_by_lf_tags method definition

await def search_tables_by_lf_tags(
    self,
    *,
    Expression: Sequence[LFTagTypeDef],  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
    CatalogId: str = ...,
) -> SearchTablesByLFTagsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LFTagTypeDef](./type_defs.md#lftagtypedef) 
2. See [:material-code-braces: SearchTablesByLFTagsResponseTypeDef](./type_defs.md#searchtablesbylftagsresponsetypedef) 


```python
# search_tables_by_lf_tags method usage example with argument unpacking

kwargs: SearchTablesByLFTagsRequestRequestTypeDef = {  # (1)
    "Expression": ...,
}

parent.search_tables_by_lf_tags(**kwargs)
```

1. See [:material-code-braces: SearchTablesByLFTagsRequestRequestTypeDef](./type_defs.md#searchtablesbylftagsrequestrequesttypedef) 

### start\_query\_planning

Submits a request to process a query statement.

Type annotations and code completion for `#!python session.client("lakeformation").start_query_planning` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# start_query_planning method definition

await def start_query_planning(
    self,
    *,
    QueryPlanningContext: QueryPlanningContextTypeDef,  # (1)
    QueryString: str,
) -> StartQueryPlanningResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: QueryPlanningContextTypeDef](./type_defs.md#queryplanningcontexttypedef) 
2. See [:material-code-braces: StartQueryPlanningResponseTypeDef](./type_defs.md#startqueryplanningresponsetypedef) 


```python
# start_query_planning method usage example with argument unpacking

kwargs: StartQueryPlanningRequestRequestTypeDef = {  # (1)
    "QueryPlanningContext": ...,
    "QueryString": ...,
}

parent.start_query_planning(**kwargs)
```

1. See [:material-code-braces: StartQueryPlanningRequestRequestTypeDef](./type_defs.md#startqueryplanningrequestrequesttypedef) 

### start\_transaction

Starts a new transaction and returns its transaction ID.

Type annotations and code completion for `#!python session.client("lakeformation").start_transaction` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# start_transaction method definition

await def start_transaction(
    self,
    *,
    TransactionType: TransactionTypeType = ...,  # (1)
) -> StartTransactionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TransactionTypeType](./literals.md#transactiontypetype) 
2. See [:material-code-braces: StartTransactionResponseTypeDef](./type_defs.md#starttransactionresponsetypedef) 


```python
# start_transaction method usage example with argument unpacking

kwargs: StartTransactionRequestRequestTypeDef = {  # (1)
    "TransactionType": ...,
}

parent.start_transaction(**kwargs)
```

1. See [:material-code-braces: StartTransactionRequestRequestTypeDef](./type_defs.md#starttransactionrequestrequesttypedef) 

### update\_data\_cells\_filter

Updates a data cell filter.

Type annotations and code completion for `#!python session.client("lakeformation").update_data_cells_filter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# update_data_cells_filter method definition

await def update_data_cells_filter(
    self,
    *,
    TableData: DataCellsFilterTypeDef,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: DataCellsFilterTypeDef](./type_defs.md#datacellsfiltertypedef) 


```python
# update_data_cells_filter method usage example with argument unpacking

kwargs: UpdateDataCellsFilterRequestRequestTypeDef = {  # (1)
    "TableData": ...,
}

parent.update_data_cells_filter(**kwargs)
```

1. See [:material-code-braces: UpdateDataCellsFilterRequestRequestTypeDef](./type_defs.md#updatedatacellsfilterrequestrequesttypedef) 

### update\_lf\_tag

Updates the list of possible values for the specified LF-tag key.

Type annotations and code completion for `#!python session.client("lakeformation").update_lf_tag` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# update_lf_tag method definition

await def update_lf_tag(
    self,
    *,
    TagKey: str,
    CatalogId: str = ...,
    TagValuesToDelete: Sequence[str] = ...,
    TagValuesToAdd: Sequence[str] = ...,
) -> dict[str, Any]:
    ...
```



```python
# update_lf_tag method usage example with argument unpacking

kwargs: UpdateLFTagRequestRequestTypeDef = {  # (1)
    "TagKey": ...,
}

parent.update_lf_tag(**kwargs)
```

1. See [:material-code-braces: UpdateLFTagRequestRequestTypeDef](./type_defs.md#updatelftagrequestrequesttypedef) 

### update\_lf\_tag\_expression

Updates the name of the LF-Tag expression to the new description and expression
body provided.

Type annotations and code completion for `#!python session.client("lakeformation").update_lf_tag_expression` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# update_lf_tag_expression method definition

await def update_lf_tag_expression(
    self,
    *,
    Name: str,
    Expression: Sequence[LFTagTypeDef],  # (1)
    Description: str = ...,
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: LFTagTypeDef](./type_defs.md#lftagtypedef) 


```python
# update_lf_tag_expression method usage example with argument unpacking

kwargs: UpdateLFTagExpressionRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Expression": ...,
}

parent.update_lf_tag_expression(**kwargs)
```

1. See [:material-code-braces: UpdateLFTagExpressionRequestRequestTypeDef](./type_defs.md#updatelftagexpressionrequestrequesttypedef) 

### update\_lake\_formation\_identity\_center\_configuration

Updates the IAM Identity Center connection parameters.

Type annotations and code completion for `#!python session.client("lakeformation").update_lake_formation_identity_center_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# update_lake_formation_identity_center_configuration method definition

await def update_lake_formation_identity_center_configuration(
    self,
    *,
    CatalogId: str = ...,
    ShareRecipients: Sequence[DataLakePrincipalTypeDef] = ...,  # (1)
    ApplicationStatus: ApplicationStatusType = ...,  # (2)
    ExternalFiltering: ExternalFilteringConfigurationTypeDef = ...,  # (3)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-brackets: ApplicationStatusType](./literals.md#applicationstatustype) 
3. See [:material-code-braces: ExternalFilteringConfigurationTypeDef](./type_defs.md#externalfilteringconfigurationtypedef) 


```python
# update_lake_formation_identity_center_configuration method usage example with argument unpacking

kwargs: UpdateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.update_lake_formation_identity_center_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef](./type_defs.md#updatelakeformationidentitycenterconfigurationrequestrequesttypedef) 

### update\_resource

Updates the data access role used for vending access to the given (registered)
resource in Lake Formation.

Type annotations and code completion for `#!python session.client("lakeformation").update_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# update_resource method definition

await def update_resource(
    self,
    *,
    RoleArn: str,
    ResourceArn: str,
    WithFederation: bool = ...,
    HybridAccessEnabled: bool = ...,
) -> dict[str, Any]:
    ...
```



```python
# update_resource method usage example with argument unpacking

kwargs: UpdateResourceRequestRequestTypeDef = {  # (1)
    "RoleArn": ...,
    "ResourceArn": ...,
}

parent.update_resource(**kwargs)
```

1. See [:material-code-braces: UpdateResourceRequestRequestTypeDef](./type_defs.md#updateresourcerequestrequesttypedef) 

### update\_table\_objects

Updates the manifest of Amazon S3 objects that make up the specified governed
table.

Type annotations and code completion for `#!python session.client("lakeformation").update_table_objects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# update_table_objects method definition

await def update_table_objects(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    WriteOperations: Sequence[WriteOperationTypeDef],  # (1)
    CatalogId: str = ...,
    TransactionId: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: WriteOperationTypeDef](./type_defs.md#writeoperationtypedef) 


```python
# update_table_objects method usage example with argument unpacking

kwargs: UpdateTableObjectsRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "WriteOperations": ...,
}

parent.update_table_objects(**kwargs)
```

1. See [:material-code-braces: UpdateTableObjectsRequestRequestTypeDef](./type_defs.md#updatetableobjectsrequestrequesttypedef) 

### update\_table\_storage\_optimizer

Updates the configuration of the storage optimizers for a table.

Type annotations and code completion for `#!python session.client("lakeformation").update_table_storage_optimizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# update_table_storage_optimizer method definition

await def update_table_storage_optimizer(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    StorageOptimizerConfig: Mapping[OptimizerTypeType, Mapping[str, str]],  # (1)
    CatalogId: str = ...,
) -> UpdateTableStorageOptimizerResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OptimizerTypeType](./literals.md#optimizertypetype) 
2. See [:material-code-braces: UpdateTableStorageOptimizerResponseTypeDef](./type_defs.md#updatetablestorageoptimizerresponsetypedef) 


```python
# update_table_storage_optimizer method usage example with argument unpacking

kwargs: UpdateTableStorageOptimizerRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "StorageOptimizerConfig": ...,
}

parent.update_table_storage_optimizer(**kwargs)
```

1. See [:material-code-braces: UpdateTableStorageOptimizerRequestRequestTypeDef](./type_defs.md#updatetablestorageoptimizerrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("lakeformation").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("lakeformation").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client)

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

Type annotations and code completion for `#!python session.client("lakeformation").get_paginator` method with overloads.

- `client.get_paginator("get_work_units")` -> [GetWorkUnitsPaginator](./paginators.md#getworkunitspaginator)
- `client.get_paginator("list_data_cells_filter")` -> [ListDataCellsFilterPaginator](./paginators.md#listdatacellsfilterpaginator)
- `client.get_paginator("list_lf_tag_expressions")` -> [ListLFTagExpressionsPaginator](./paginators.md#listlftagexpressionspaginator)
- `client.get_paginator("list_lf_tags")` -> [ListLFTagsPaginator](./paginators.md#listlftagspaginator)
- `client.get_paginator("search_databases_by_lf_tags")` -> [SearchDatabasesByLFTagsPaginator](./paginators.md#searchdatabasesbylftagspaginator)
- `client.get_paginator("search_tables_by_lf_tags")` -> [SearchTablesByLFTagsPaginator](./paginators.md#searchtablesbylftagspaginator)


