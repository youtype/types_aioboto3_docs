# Type definitions

> [Index](../README.md) > [SupplyChain](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SupplyChain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain)
    type annotations stubs module [types-aiobotocore-supplychain](https://pypi.org/project/types-aiobotocore-supplychain/).



## BillOfMaterialsImportJobTypeDef

```python
# BillOfMaterialsImportJobTypeDef definition

class BillOfMaterialsImportJobTypeDef(TypedDict):
    instanceId: str,
    jobId: str,
    status: ConfigurationJobStatusType,  # (1)
    s3uri: str,
    message: NotRequired[str],
```

1. See [:material-code-brackets: ConfigurationJobStatusType](./literals.md#configurationjobstatustype) 
## CreateBillOfMaterialsImportJobRequestRequestTypeDef

```python
# CreateBillOfMaterialsImportJobRequestRequestTypeDef definition

class CreateBillOfMaterialsImportJobRequestRequestTypeDef(TypedDict):
    instanceId: str,
    s3uri: str,
    clientToken: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## GetBillOfMaterialsImportJobRequestRequestTypeDef

```python
# GetBillOfMaterialsImportJobRequestRequestTypeDef definition

class GetBillOfMaterialsImportJobRequestRequestTypeDef(TypedDict):
    instanceId: str,
    jobId: str,
```

## CreateBillOfMaterialsImportJobResponseTypeDef

```python
# CreateBillOfMaterialsImportJobResponseTypeDef definition

class CreateBillOfMaterialsImportJobResponseTypeDef(TypedDict):
    jobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBillOfMaterialsImportJobResponseTypeDef

```python
# GetBillOfMaterialsImportJobResponseTypeDef definition

class GetBillOfMaterialsImportJobResponseTypeDef(TypedDict):
    job: BillOfMaterialsImportJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BillOfMaterialsImportJobTypeDef](./type_defs.md#billofmaterialsimportjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
