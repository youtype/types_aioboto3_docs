# Type definitions

> [Index](../README.md) > [B2BI](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [B2BI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI)
    type annotations stubs module [types-aiobotocore-b2bi](https://pypi.org/project/types-aiobotocore-b2bi/).



## CapabilitySummaryTypeDef

```python
# CapabilitySummaryTypeDef definition

class CapabilitySummaryTypeDef(TypedDict):
    capabilityId: str,
    name: str,
    type: CapabilityTypeType,  # (1)
    createdAt: datetime,
    modifiedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: CapabilityTypeType](./literals.md#capabilitytypetype) 
## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    bucketName: NotRequired[str],
    key: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
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

## DeleteCapabilityRequestRequestTypeDef

```python
# DeleteCapabilityRequestRequestTypeDef definition

class DeleteCapabilityRequestRequestTypeDef(TypedDict):
    capabilityId: str,
```

## DeletePartnershipRequestRequestTypeDef

```python
# DeletePartnershipRequestRequestTypeDef definition

class DeletePartnershipRequestRequestTypeDef(TypedDict):
    partnershipId: str,
```

## DeleteProfileRequestRequestTypeDef

```python
# DeleteProfileRequestRequestTypeDef definition

class DeleteProfileRequestRequestTypeDef(TypedDict):
    profileId: str,
```

## DeleteTransformerRequestRequestTypeDef

```python
# DeleteTransformerRequestRequestTypeDef definition

class DeleteTransformerRequestRequestTypeDef(TypedDict):
    transformerId: str,
```

## X12DetailsTypeDef

```python
# X12DetailsTypeDef definition

class X12DetailsTypeDef(TypedDict):
    transactionSet: NotRequired[X12TransactionSetType],  # (1)
    version: NotRequired[X12VersionType],  # (2)
```

1. See [:material-code-brackets: X12TransactionSetType](./literals.md#x12transactionsettype) 
2. See [:material-code-brackets: X12VersionType](./literals.md#x12versiontype) 
## GetCapabilityRequestRequestTypeDef

```python
# GetCapabilityRequestRequestTypeDef definition

class GetCapabilityRequestRequestTypeDef(TypedDict):
    capabilityId: str,
```

## GetPartnershipRequestRequestTypeDef

```python
# GetPartnershipRequestRequestTypeDef definition

class GetPartnershipRequestRequestTypeDef(TypedDict):
    partnershipId: str,
```

## GetProfileRequestRequestTypeDef

```python
# GetProfileRequestRequestTypeDef definition

class GetProfileRequestRequestTypeDef(TypedDict):
    profileId: str,
```

## GetTransformerJobRequestRequestTypeDef

```python
# GetTransformerJobRequestRequestTypeDef definition

class GetTransformerJobRequestRequestTypeDef(TypedDict):
    transformerJobId: str,
    transformerId: str,
```

## GetTransformerRequestRequestTypeDef

```python
# GetTransformerRequestRequestTypeDef definition

class GetTransformerRequestRequestTypeDef(TypedDict):
    transformerId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListCapabilitiesRequestRequestTypeDef

```python
# ListCapabilitiesRequestRequestTypeDef definition

class ListCapabilitiesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListPartnershipsRequestRequestTypeDef

```python
# ListPartnershipsRequestRequestTypeDef definition

class ListPartnershipsRequestRequestTypeDef(TypedDict):
    profileId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## PartnershipSummaryTypeDef

```python
# PartnershipSummaryTypeDef definition

class PartnershipSummaryTypeDef(TypedDict):
    profileId: str,
    partnershipId: str,
    createdAt: datetime,
    name: NotRequired[str],
    capabilities: NotRequired[List[str]],
    tradingPartnerId: NotRequired[str],
    modifiedAt: NotRequired[datetime],
```

## ListProfilesRequestRequestTypeDef

```python
# ListProfilesRequestRequestTypeDef definition

class ListProfilesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ProfileSummaryTypeDef

```python
# ProfileSummaryTypeDef definition

class ProfileSummaryTypeDef(TypedDict):
    profileId: str,
    name: str,
    businessName: str,
    createdAt: datetime,
    logging: NotRequired[LoggingType],  # (1)
    logGroupName: NotRequired[str],
    modifiedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: LoggingType](./literals.md#loggingtype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## ListTransformersRequestRequestTypeDef

```python
# ListTransformersRequestRequestTypeDef definition

class ListTransformersRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## TestMappingRequestRequestTypeDef

```python
# TestMappingRequestRequestTypeDef definition

class TestMappingRequestRequestTypeDef(TypedDict):
    inputFileContent: str,
    mappingTemplate: str,
    fileFormat: FileFormatType,  # (1)
```

1. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdatePartnershipRequestRequestTypeDef

```python
# UpdatePartnershipRequestRequestTypeDef definition

class UpdatePartnershipRequestRequestTypeDef(TypedDict):
    partnershipId: str,
    name: NotRequired[str],
    capabilities: NotRequired[Sequence[str]],
```

## UpdateProfileRequestRequestTypeDef

```python
# UpdateProfileRequestRequestTypeDef definition

class UpdateProfileRequestRequestTypeDef(TypedDict):
    profileId: str,
    name: NotRequired[str],
    email: NotRequired[str],
    phone: NotRequired[str],
    businessName: NotRequired[str],
```

## StartTransformerJobRequestRequestTypeDef

```python
# StartTransformerJobRequestRequestTypeDef definition

class StartTransformerJobRequestRequestTypeDef(TypedDict):
    inputFile: S3LocationTypeDef,  # (1)
    outputLocation: S3LocationTypeDef,  # (1)
    transformerId: str,
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## CreatePartnershipRequestRequestTypeDef

```python
# CreatePartnershipRequestRequestTypeDef definition

class CreatePartnershipRequestRequestTypeDef(TypedDict):
    profileId: str,
    name: str,
    email: str,
    phone: NotRequired[str],
    capabilities: NotRequired[Sequence[str]],
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateProfileRequestRequestTypeDef

```python
# CreateProfileRequestRequestTypeDef definition

class CreateProfileRequestRequestTypeDef(TypedDict):
    name: str,
    phone: str,
    businessName: str,
    logging: LoggingType,  # (1)
    email: NotRequired[str],
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: LoggingType](./literals.md#loggingtype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePartnershipResponseTypeDef

```python
# CreatePartnershipResponseTypeDef definition

class CreatePartnershipResponseTypeDef(TypedDict):
    profileId: str,
    partnershipId: str,
    partnershipArn: str,
    name: str,
    email: str,
    phone: str,
    capabilities: List[str],
    tradingPartnerId: str,
    createdAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProfileResponseTypeDef

```python
# CreateProfileResponseTypeDef definition

class CreateProfileResponseTypeDef(TypedDict):
    profileId: str,
    profileArn: str,
    name: str,
    businessName: str,
    phone: str,
    email: str,
    logging: LoggingType,  # (1)
    logGroupName: str,
    createdAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LoggingType](./literals.md#loggingtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPartnershipResponseTypeDef

```python
# GetPartnershipResponseTypeDef definition

class GetPartnershipResponseTypeDef(TypedDict):
    profileId: str,
    partnershipId: str,
    partnershipArn: str,
    name: str,
    email: str,
    phone: str,
    capabilities: List[str],
    tradingPartnerId: str,
    createdAt: datetime,
    modifiedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProfileResponseTypeDef

```python
# GetProfileResponseTypeDef definition

class GetProfileResponseTypeDef(TypedDict):
    profileId: str,
    profileArn: str,
    name: str,
    email: str,
    phone: str,
    businessName: str,
    logging: LoggingType,  # (1)
    logGroupName: str,
    createdAt: datetime,
    modifiedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LoggingType](./literals.md#loggingtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTransformerJobResponseTypeDef

```python
# GetTransformerJobResponseTypeDef definition

class GetTransformerJobResponseTypeDef(TypedDict):
    status: TransformerJobStatusType,  # (1)
    outputFiles: List[S3LocationTypeDef],  # (2)
    message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: TransformerJobStatusType](./literals.md#transformerjobstatustype) 
2. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCapabilitiesResponseTypeDef

```python
# ListCapabilitiesResponseTypeDef definition

class ListCapabilitiesResponseTypeDef(TypedDict):
    capabilities: List[CapabilitySummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CapabilitySummaryTypeDef](./type_defs.md#capabilitysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTransformerJobResponseTypeDef

```python
# StartTransformerJobResponseTypeDef definition

class StartTransformerJobResponseTypeDef(TypedDict):
    transformerJobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestMappingResponseTypeDef

```python
# TestMappingResponseTypeDef definition

class TestMappingResponseTypeDef(TypedDict):
    mappedFileContent: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestParsingResponseTypeDef

```python
# TestParsingResponseTypeDef definition

class TestParsingResponseTypeDef(TypedDict):
    parsedFileContent: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePartnershipResponseTypeDef

```python
# UpdatePartnershipResponseTypeDef definition

class UpdatePartnershipResponseTypeDef(TypedDict):
    profileId: str,
    partnershipId: str,
    partnershipArn: str,
    name: str,
    email: str,
    phone: str,
    capabilities: List[str],
    tradingPartnerId: str,
    createdAt: datetime,
    modifiedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProfileResponseTypeDef

```python
# UpdateProfileResponseTypeDef definition

class UpdateProfileResponseTypeDef(TypedDict):
    profileId: str,
    profileArn: str,
    name: str,
    email: str,
    phone: str,
    businessName: str,
    logging: LoggingType,  # (1)
    logGroupName: str,
    createdAt: datetime,
    modifiedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LoggingType](./literals.md#loggingtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EdiTypeTypeDef

```python
# EdiTypeTypeDef definition

class EdiTypeTypeDef(TypedDict):
    x12Details: NotRequired[X12DetailsTypeDef],  # (1)
```

1. See [:material-code-braces: X12DetailsTypeDef](./type_defs.md#x12detailstypedef) 
## ListCapabilitiesRequestListCapabilitiesPaginateTypeDef

```python
# ListCapabilitiesRequestListCapabilitiesPaginateTypeDef definition

class ListCapabilitiesRequestListCapabilitiesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPartnershipsRequestListPartnershipsPaginateTypeDef

```python
# ListPartnershipsRequestListPartnershipsPaginateTypeDef definition

class ListPartnershipsRequestListPartnershipsPaginateTypeDef(TypedDict):
    profileId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProfilesRequestListProfilesPaginateTypeDef

```python
# ListProfilesRequestListProfilesPaginateTypeDef definition

class ListProfilesRequestListProfilesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTransformersRequestListTransformersPaginateTypeDef

```python
# ListTransformersRequestListTransformersPaginateTypeDef definition

class ListTransformersRequestListTransformersPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPartnershipsResponseTypeDef

```python
# ListPartnershipsResponseTypeDef definition

class ListPartnershipsResponseTypeDef(TypedDict):
    partnerships: List[PartnershipSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PartnershipSummaryTypeDef](./type_defs.md#partnershipsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProfilesResponseTypeDef

```python
# ListProfilesResponseTypeDef definition

class ListProfilesResponseTypeDef(TypedDict):
    profiles: List[ProfileSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfileSummaryTypeDef](./type_defs.md#profilesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTransformerRequestRequestTypeDef

```python
# CreateTransformerRequestRequestTypeDef definition

class CreateTransformerRequestRequestTypeDef(TypedDict):
    name: str,
    fileFormat: FileFormatType,  # (1)
    mappingTemplate: str,
    ediType: EdiTypeTypeDef,  # (2)
    sampleDocument: NotRequired[str],
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
2. See [:material-code-braces: EdiTypeTypeDef](./type_defs.md#editypetypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateTransformerResponseTypeDef

```python
# CreateTransformerResponseTypeDef definition

class CreateTransformerResponseTypeDef(TypedDict):
    transformerId: str,
    transformerArn: str,
    name: str,
    fileFormat: FileFormatType,  # (1)
    mappingTemplate: str,
    status: TransformerStatusType,  # (2)
    ediType: EdiTypeTypeDef,  # (3)
    sampleDocument: str,
    createdAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
2. See [:material-code-brackets: TransformerStatusType](./literals.md#transformerstatustype) 
3. See [:material-code-braces: EdiTypeTypeDef](./type_defs.md#editypetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EdiConfigurationTypeDef

```python
# EdiConfigurationTypeDef definition

class EdiConfigurationTypeDef(TypedDict):
    type: EdiTypeTypeDef,  # (1)
    inputLocation: S3LocationTypeDef,  # (2)
    outputLocation: S3LocationTypeDef,  # (2)
    transformerId: str,
```

1. See [:material-code-braces: EdiTypeTypeDef](./type_defs.md#editypetypedef) 
2. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## GetTransformerResponseTypeDef

```python
# GetTransformerResponseTypeDef definition

class GetTransformerResponseTypeDef(TypedDict):
    transformerId: str,
    transformerArn: str,
    name: str,
    fileFormat: FileFormatType,  # (1)
    mappingTemplate: str,
    status: TransformerStatusType,  # (2)
    ediType: EdiTypeTypeDef,  # (3)
    sampleDocument: str,
    createdAt: datetime,
    modifiedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
2. See [:material-code-brackets: TransformerStatusType](./literals.md#transformerstatustype) 
3. See [:material-code-braces: EdiTypeTypeDef](./type_defs.md#editypetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestParsingRequestRequestTypeDef

```python
# TestParsingRequestRequestTypeDef definition

class TestParsingRequestRequestTypeDef(TypedDict):
    inputFile: S3LocationTypeDef,  # (1)
    fileFormat: FileFormatType,  # (2)
    ediType: EdiTypeTypeDef,  # (3)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
3. See [:material-code-braces: EdiTypeTypeDef](./type_defs.md#editypetypedef) 
## TransformerSummaryTypeDef

```python
# TransformerSummaryTypeDef definition

class TransformerSummaryTypeDef(TypedDict):
    transformerId: str,
    name: str,
    fileFormat: FileFormatType,  # (1)
    mappingTemplate: str,
    status: TransformerStatusType,  # (2)
    ediType: EdiTypeTypeDef,  # (3)
    createdAt: datetime,
    sampleDocument: NotRequired[str],
    modifiedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
2. See [:material-code-brackets: TransformerStatusType](./literals.md#transformerstatustype) 
3. See [:material-code-braces: EdiTypeTypeDef](./type_defs.md#editypetypedef) 
## UpdateTransformerRequestRequestTypeDef

```python
# UpdateTransformerRequestRequestTypeDef definition

class UpdateTransformerRequestRequestTypeDef(TypedDict):
    transformerId: str,
    name: NotRequired[str],
    fileFormat: NotRequired[FileFormatType],  # (1)
    mappingTemplate: NotRequired[str],
    status: NotRequired[TransformerStatusType],  # (2)
    ediType: NotRequired[EdiTypeTypeDef],  # (3)
    sampleDocument: NotRequired[str],
```

1. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
2. See [:material-code-brackets: TransformerStatusType](./literals.md#transformerstatustype) 
3. See [:material-code-braces: EdiTypeTypeDef](./type_defs.md#editypetypedef) 
## UpdateTransformerResponseTypeDef

```python
# UpdateTransformerResponseTypeDef definition

class UpdateTransformerResponseTypeDef(TypedDict):
    transformerId: str,
    transformerArn: str,
    name: str,
    fileFormat: FileFormatType,  # (1)
    mappingTemplate: str,
    status: TransformerStatusType,  # (2)
    ediType: EdiTypeTypeDef,  # (3)
    sampleDocument: str,
    createdAt: datetime,
    modifiedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: FileFormatType](./literals.md#fileformattype) 
2. See [:material-code-brackets: TransformerStatusType](./literals.md#transformerstatustype) 
3. See [:material-code-braces: EdiTypeTypeDef](./type_defs.md#editypetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CapabilityConfigurationTypeDef

```python
# CapabilityConfigurationTypeDef definition

class CapabilityConfigurationTypeDef(TypedDict):
    edi: NotRequired[EdiConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: EdiConfigurationTypeDef](./type_defs.md#ediconfigurationtypedef) 
## ListTransformersResponseTypeDef

```python
# ListTransformersResponseTypeDef definition

class ListTransformersResponseTypeDef(TypedDict):
    transformers: List[TransformerSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TransformerSummaryTypeDef](./type_defs.md#transformersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCapabilityRequestRequestTypeDef

```python
# CreateCapabilityRequestRequestTypeDef definition

class CreateCapabilityRequestRequestTypeDef(TypedDict):
    name: str,
    type: CapabilityTypeType,  # (1)
    configuration: CapabilityConfigurationTypeDef,  # (2)
    instructionsDocuments: NotRequired[Sequence[S3LocationTypeDef]],  # (3)
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-brackets: CapabilityTypeType](./literals.md#capabilitytypetype) 
2. See [:material-code-braces: CapabilityConfigurationTypeDef](./type_defs.md#capabilityconfigurationtypedef) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateCapabilityResponseTypeDef

```python
# CreateCapabilityResponseTypeDef definition

class CreateCapabilityResponseTypeDef(TypedDict):
    capabilityId: str,
    capabilityArn: str,
    name: str,
    type: CapabilityTypeType,  # (1)
    configuration: CapabilityConfigurationTypeDef,  # (2)
    instructionsDocuments: List[S3LocationTypeDef],  # (3)
    createdAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: CapabilityTypeType](./literals.md#capabilitytypetype) 
2. See [:material-code-braces: CapabilityConfigurationTypeDef](./type_defs.md#capabilityconfigurationtypedef) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCapabilityResponseTypeDef

```python
# GetCapabilityResponseTypeDef definition

class GetCapabilityResponseTypeDef(TypedDict):
    capabilityId: str,
    capabilityArn: str,
    name: str,
    type: CapabilityTypeType,  # (1)
    configuration: CapabilityConfigurationTypeDef,  # (2)
    instructionsDocuments: List[S3LocationTypeDef],  # (3)
    createdAt: datetime,
    modifiedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: CapabilityTypeType](./literals.md#capabilitytypetype) 
2. See [:material-code-braces: CapabilityConfigurationTypeDef](./type_defs.md#capabilityconfigurationtypedef) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCapabilityRequestRequestTypeDef

```python
# UpdateCapabilityRequestRequestTypeDef definition

class UpdateCapabilityRequestRequestTypeDef(TypedDict):
    capabilityId: str,
    name: NotRequired[str],
    configuration: NotRequired[CapabilityConfigurationTypeDef],  # (1)
    instructionsDocuments: NotRequired[Sequence[S3LocationTypeDef]],  # (2)
```

1. See [:material-code-braces: CapabilityConfigurationTypeDef](./type_defs.md#capabilityconfigurationtypedef) 
2. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## UpdateCapabilityResponseTypeDef

```python
# UpdateCapabilityResponseTypeDef definition

class UpdateCapabilityResponseTypeDef(TypedDict):
    capabilityId: str,
    capabilityArn: str,
    name: str,
    type: CapabilityTypeType,  # (1)
    configuration: CapabilityConfigurationTypeDef,  # (2)
    instructionsDocuments: List[S3LocationTypeDef],  # (3)
    createdAt: datetime,
    modifiedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: CapabilityTypeType](./literals.md#capabilitytypetype) 
2. See [:material-code-braces: CapabilityConfigurationTypeDef](./type_defs.md#capabilityconfigurationtypedef) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
