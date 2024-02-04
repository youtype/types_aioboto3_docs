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

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("supplychain").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> SupplyChainClient:
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





