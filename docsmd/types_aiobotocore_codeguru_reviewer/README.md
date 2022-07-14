# CodeGuruReviewer module

> [Index](../README.md) > CodeGuruReviewer


!!! note ""

    Auto-generated documentation for [CodeGuruReviewer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
    type annotations stubs module [types-aiobotocore-codeguru-reviewer](https://pypi.org/project/types-aiobotocore-codeguru-reviewer/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `CodeGuruReviewer`.

### From PyPI with pip

Install `types-aioboto3` for `CodeGuruReviewer` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[codeguru-reviewer]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[codeguru-reviewer]'


# standalone installation
python -m pip install types-aiobotocore-codeguru-reviewer
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-codeguru-reviewer
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CodeGuruReviewerClient

Type annotations and code completion for  `#!python session.client("codeguru-reviewer")` as [CodeGuruReviewerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_codeguru_reviewer.client import CodeGuruReviewerClient


session = Session()
async with session.client("codeguru-reviewer") as client:
    client: CodeGuruReviewerClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("codeguru-reviewer").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_codeguru_reviewer.paginator import ListRepositoryAssociationsPaginator

def get_list_repository_associations_paginator() -> ListRepositoryAssociationsPaginator:
    return client.get_paginator("list_repository_associations"))
```

- [ListRepositoryAssociationsPaginator](./paginators.md#listrepositoryassociationspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.client("codeguru-reviewer").get_waiter("...")`.

```python title="Usage example"
from types_aiobotocore_codeguru_reviewer.waiter import CodeReviewCompletedWaiter

def get_code_review_completed_waiter() -> CodeReviewCompletedWaiter:
    return Session().client("codeguru-reviewer").get_waiter("code_review_completed")
```

- [CodeReviewCompletedWaiter](./waiters.md#codereviewcompletedwaiter)
- [RepositoryAssociationSucceededWaiter](./waiters.md#repositoryassociationsucceededwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_codeguru_reviewer.literals import AnalysisTypeType

def get_value() -> AnalysisTypeType:
    return "CodeQuality"
```

- [AnalysisTypeType](./literals.md#analysistypetype)
- [CodeReviewCompletedWaiterName](./literals.md#codereviewcompletedwaitername)
- [ConfigFileStateType](./literals.md#configfilestatetype)
- [EncryptionOptionType](./literals.md#encryptionoptiontype)
- [JobStateType](./literals.md#jobstatetype)
- [ListRepositoryAssociationsPaginatorName](./literals.md#listrepositoryassociationspaginatorname)
- [ProviderTypeType](./literals.md#providertypetype)
- [ReactionType](./literals.md#reactiontype)
- [RecommendationCategoryType](./literals.md#recommendationcategorytype)
- [RepositoryAssociationStateType](./literals.md#repositoryassociationstatetype)
- [RepositoryAssociationSucceededWaiterName](./literals.md#repositoryassociationsucceededwaitername)
- [SeverityType](./literals.md#severitytype)
- [TypeType](./literals.md#typetype)
- [VendorNameType](./literals.md#vendornametype)
- [CodeGuruReviewerServiceName](./literals.md#codegurureviewerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_codeguru_reviewer.type_defs import KMSKeyDetailsTypeDef

def get_value() -> KMSKeyDetailsTypeDef:
    return {
        "KMSKeyId": ...,
    }
```

- [KMSKeyDetailsTypeDef](./type_defs.md#kmskeydetailstypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BranchDiffSourceCodeTypeTypeDef](./type_defs.md#branchdiffsourcecodetypetypedef)
- [CodeArtifactsTypeDef](./type_defs.md#codeartifactstypedef)
- [CodeCommitRepositoryTypeDef](./type_defs.md#codecommitrepositorytypedef)
- [MetricsSummaryTypeDef](./type_defs.md#metricssummarytypedef)
- [MetricsTypeDef](./type_defs.md#metricstypedef)
- [CommitDiffSourceCodeTypeTypeDef](./type_defs.md#commitdiffsourcecodetypetypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [DescribeCodeReviewRequestRequestTypeDef](./type_defs.md#describecodereviewrequestrequesttypedef)
- [DescribeRecommendationFeedbackRequestRequestTypeDef](./type_defs.md#describerecommendationfeedbackrequestrequesttypedef)
- [RecommendationFeedbackTypeDef](./type_defs.md#recommendationfeedbacktypedef)
- [DescribeRepositoryAssociationRequestRequestTypeDef](./type_defs.md#describerepositoryassociationrequestrequesttypedef)
- [DisassociateRepositoryRequestRequestTypeDef](./type_defs.md#disassociaterepositoryrequestrequesttypedef)
- [EventInfoTypeDef](./type_defs.md#eventinfotypedef)
- [ListCodeReviewsRequestRequestTypeDef](./type_defs.md#listcodereviewsrequestrequesttypedef)
- [ListRecommendationFeedbackRequestRequestTypeDef](./type_defs.md#listrecommendationfeedbackrequestrequesttypedef)
- [RecommendationFeedbackSummaryTypeDef](./type_defs.md#recommendationfeedbacksummarytypedef)
- [ListRecommendationsRequestRequestTypeDef](./type_defs.md#listrecommendationsrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListRepositoryAssociationsRequestRequestTypeDef](./type_defs.md#listrepositoryassociationsrequestrequesttypedef)
- [RepositoryAssociationSummaryTypeDef](./type_defs.md#repositoryassociationsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [PutRecommendationFeedbackRequestRequestTypeDef](./type_defs.md#putrecommendationfeedbackrequestrequesttypedef)
- [RuleMetadataTypeDef](./type_defs.md#rulemetadatatypedef)
- [RepositoryHeadSourceCodeTypeTypeDef](./type_defs.md#repositoryheadsourcecodetypetypedef)
- [S3RepositoryTypeDef](./type_defs.md#s3repositorytypedef)
- [ThirdPartySourceRepositoryTypeDef](./type_defs.md#thirdpartysourcerepositorytypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [S3RepositoryDetailsTypeDef](./type_defs.md#s3repositorydetailstypedef)
- [DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef](./type_defs.md#describecodereviewrequestcodereviewcompletedwaittypedef)
- [DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef](./type_defs.md#describerepositoryassociationrequestrepositoryassociationsucceededwaittypedef)
- [DescribeRecommendationFeedbackResponseTypeDef](./type_defs.md#describerecommendationfeedbackresponsetypedef)
- [RequestMetadataTypeDef](./type_defs.md#requestmetadatatypedef)
- [ListRecommendationFeedbackResponseTypeDef](./type_defs.md#listrecommendationfeedbackresponsetypedef)
- [ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef](./type_defs.md#listrepositoryassociationsrequestlistrepositoryassociationspaginatetypedef)
- [ListRepositoryAssociationsResponseTypeDef](./type_defs.md#listrepositoryassociationsresponsetypedef)
- [RecommendationSummaryTypeDef](./type_defs.md#recommendationsummarytypedef)
- [RepositoryTypeDef](./type_defs.md#repositorytypedef)
- [RepositoryAssociationTypeDef](./type_defs.md#repositoryassociationtypedef)
- [S3BucketRepositoryTypeDef](./type_defs.md#s3bucketrepositorytypedef)
- [ListRecommendationsResponseTypeDef](./type_defs.md#listrecommendationsresponsetypedef)
- [AssociateRepositoryRequestRequestTypeDef](./type_defs.md#associaterepositoryrequestrequesttypedef)
- [AssociateRepositoryResponseTypeDef](./type_defs.md#associaterepositoryresponsetypedef)
- [DescribeRepositoryAssociationResponseTypeDef](./type_defs.md#describerepositoryassociationresponsetypedef)
- [DisassociateRepositoryResponseTypeDef](./type_defs.md#disassociaterepositoryresponsetypedef)
- [SourceCodeTypeTypeDef](./type_defs.md#sourcecodetypetypedef)
- [CodeReviewSummaryTypeDef](./type_defs.md#codereviewsummarytypedef)
- [CodeReviewTypeDef](./type_defs.md#codereviewtypedef)
- [RepositoryAnalysisTypeDef](./type_defs.md#repositoryanalysistypedef)
- [ListCodeReviewsResponseTypeDef](./type_defs.md#listcodereviewsresponsetypedef)
- [CreateCodeReviewResponseTypeDef](./type_defs.md#createcodereviewresponsetypedef)
- [DescribeCodeReviewResponseTypeDef](./type_defs.md#describecodereviewresponsetypedef)
- [CodeReviewTypeTypeDef](./type_defs.md#codereviewtypetypedef)
- [CreateCodeReviewRequestRequestTypeDef](./type_defs.md#createcodereviewrequestrequesttypedef)

