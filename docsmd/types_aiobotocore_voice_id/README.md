# VoiceID module

> [Index](../README.md) > VoiceID


!!! note ""

    Auto-generated documentation for [VoiceID](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
    type annotations stubs module [types-aiobotocore-voice-id](https://pypi.org/project/types-aiobotocore-voice-id/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `VoiceID`.

### From PyPI with pip

Install `types-aioboto3` for `VoiceID` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[voice-id]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[voice-id]'


# standalone installation
python -m pip install types-aiobotocore-voice-id
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-voice-id
```

## Usage

Code samples can be found in [Examples](./usage.md).

## VoiceIDClient

Type annotations and code completion for  `#!python session.client("voice-id")` as [VoiceIDClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_voice_id.client import VoiceIDClient


session = Session()
async with session.client("voice-id") as client:
    client: VoiceIDClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("voice-id").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_voice_id.paginator import ListDomainsPaginator

def get_list_domains_paginator() -> ListDomainsPaginator:
    return client.get_paginator("list_domains"))
```

- [ListDomainsPaginator](./paginators.md#listdomainspaginator)
- [ListFraudsterRegistrationJobsPaginator](./paginators.md#listfraudsterregistrationjobspaginator)
- [ListSpeakerEnrollmentJobsPaginator](./paginators.md#listspeakerenrollmentjobspaginator)
- [ListSpeakersPaginator](./paginators.md#listspeakerspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_voice_id.literals import AuthenticationDecisionType

def get_value() -> AuthenticationDecisionType:
    return "ACCEPT"
```

- [AuthenticationDecisionType](./literals.md#authenticationdecisiontype)
- [DomainStatusType](./literals.md#domainstatustype)
- [DuplicateRegistrationActionType](./literals.md#duplicateregistrationactiontype)
- [ExistingEnrollmentActionType](./literals.md#existingenrollmentactiontype)
- [FraudDetectionActionType](./literals.md#frauddetectionactiontype)
- [FraudDetectionDecisionType](./literals.md#frauddetectiondecisiontype)
- [FraudDetectionReasonType](./literals.md#frauddetectionreasontype)
- [FraudsterRegistrationJobStatusType](./literals.md#fraudsterregistrationjobstatustype)
- [ListDomainsPaginatorName](./literals.md#listdomainspaginatorname)
- [ListFraudsterRegistrationJobsPaginatorName](./literals.md#listfraudsterregistrationjobspaginatorname)
- [ListSpeakerEnrollmentJobsPaginatorName](./literals.md#listspeakerenrollmentjobspaginatorname)
- [ListSpeakersPaginatorName](./literals.md#listspeakerspaginatorname)
- [ServerSideEncryptionUpdateStatusType](./literals.md#serversideencryptionupdatestatustype)
- [SpeakerEnrollmentJobStatusType](./literals.md#speakerenrollmentjobstatustype)
- [SpeakerStatusType](./literals.md#speakerstatustype)
- [StreamingStatusType](./literals.md#streamingstatustype)
- [VoiceIDServiceName](./literals.md#voiceidservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_voice_id.type_defs import AuthenticationConfigurationTypeDef

def get_value() -> AuthenticationConfigurationTypeDef:
    return {
        "AcceptanceThreshold": ...,
    }
```

- [AuthenticationConfigurationTypeDef](./type_defs.md#authenticationconfigurationtypedef)
- [ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteDomainRequestRequestTypeDef](./type_defs.md#deletedomainrequestrequesttypedef)
- [DeleteFraudsterRequestRequestTypeDef](./type_defs.md#deletefraudsterrequestrequesttypedef)
- [DeleteSpeakerRequestRequestTypeDef](./type_defs.md#deletespeakerrequestrequesttypedef)
- [DescribeDomainRequestRequestTypeDef](./type_defs.md#describedomainrequestrequesttypedef)
- [DescribeFraudsterRegistrationJobRequestRequestTypeDef](./type_defs.md#describefraudsterregistrationjobrequestrequesttypedef)
- [DescribeFraudsterRequestRequestTypeDef](./type_defs.md#describefraudsterrequestrequesttypedef)
- [FraudsterTypeDef](./type_defs.md#fraudstertypedef)
- [DescribeSpeakerEnrollmentJobRequestRequestTypeDef](./type_defs.md#describespeakerenrollmentjobrequestrequesttypedef)
- [DescribeSpeakerRequestRequestTypeDef](./type_defs.md#describespeakerrequestrequesttypedef)
- [SpeakerTypeDef](./type_defs.md#speakertypedef)
- [ServerSideEncryptionUpdateDetailsTypeDef](./type_defs.md#serversideencryptionupdatedetailstypedef)
- [EnrollmentJobFraudDetectionConfigTypeDef](./type_defs.md#enrollmentjobfrauddetectionconfigtypedef)
- [EvaluateSessionRequestRequestTypeDef](./type_defs.md#evaluatesessionrequestrequesttypedef)
- [FailureDetailsTypeDef](./type_defs.md#failuredetailstypedef)
- [FraudDetectionConfigurationTypeDef](./type_defs.md#frauddetectionconfigurationtypedef)
- [KnownFraudsterRiskTypeDef](./type_defs.md#knownfraudsterrisktypedef)
- [JobProgressTypeDef](./type_defs.md#jobprogresstypedef)
- [InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef)
- [OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef)
- [RegistrationConfigTypeDef](./type_defs.md#registrationconfigtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListDomainsRequestRequestTypeDef](./type_defs.md#listdomainsrequestrequesttypedef)
- [ListFraudsterRegistrationJobsRequestRequestTypeDef](./type_defs.md#listfraudsterregistrationjobsrequestrequesttypedef)
- [ListSpeakerEnrollmentJobsRequestRequestTypeDef](./type_defs.md#listspeakerenrollmentjobsrequestrequesttypedef)
- [ListSpeakersRequestRequestTypeDef](./type_defs.md#listspeakersrequestrequesttypedef)
- [SpeakerSummaryTypeDef](./type_defs.md#speakersummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [OptOutSpeakerRequestRequestTypeDef](./type_defs.md#optoutspeakerrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [AuthenticationResultTypeDef](./type_defs.md#authenticationresulttypedef)
- [UpdateDomainRequestRequestTypeDef](./type_defs.md#updatedomainrequestrequesttypedef)
- [CreateDomainRequestRequestTypeDef](./type_defs.md#createdomainrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [DescribeFraudsterResponseTypeDef](./type_defs.md#describefraudsterresponsetypedef)
- [DescribeSpeakerResponseTypeDef](./type_defs.md#describespeakerresponsetypedef)
- [OptOutSpeakerResponseTypeDef](./type_defs.md#optoutspeakerresponsetypedef)
- [DomainSummaryTypeDef](./type_defs.md#domainsummarytypedef)
- [DomainTypeDef](./type_defs.md#domaintypedef)
- [EnrollmentConfigTypeDef](./type_defs.md#enrollmentconfigtypedef)
- [FraudRiskDetailsTypeDef](./type_defs.md#fraudriskdetailstypedef)
- [FraudsterRegistrationJobSummaryTypeDef](./type_defs.md#fraudsterregistrationjobsummarytypedef)
- [SpeakerEnrollmentJobSummaryTypeDef](./type_defs.md#speakerenrollmentjobsummarytypedef)
- [FraudsterRegistrationJobTypeDef](./type_defs.md#fraudsterregistrationjobtypedef)
- [StartFraudsterRegistrationJobRequestRequestTypeDef](./type_defs.md#startfraudsterregistrationjobrequestrequesttypedef)
- [ListDomainsRequestListDomainsPaginateTypeDef](./type_defs.md#listdomainsrequestlistdomainspaginatetypedef)
- [ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef](./type_defs.md#listfraudsterregistrationjobsrequestlistfraudsterregistrationjobspaginatetypedef)
- [ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef](./type_defs.md#listspeakerenrollmentjobsrequestlistspeakerenrollmentjobspaginatetypedef)
- [ListSpeakersRequestListSpeakersPaginateTypeDef](./type_defs.md#listspeakersrequestlistspeakerspaginatetypedef)
- [ListSpeakersResponseTypeDef](./type_defs.md#listspeakersresponsetypedef)
- [ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef)
- [CreateDomainResponseTypeDef](./type_defs.md#createdomainresponsetypedef)
- [DescribeDomainResponseTypeDef](./type_defs.md#describedomainresponsetypedef)
- [UpdateDomainResponseTypeDef](./type_defs.md#updatedomainresponsetypedef)
- [SpeakerEnrollmentJobTypeDef](./type_defs.md#speakerenrollmentjobtypedef)
- [StartSpeakerEnrollmentJobRequestRequestTypeDef](./type_defs.md#startspeakerenrollmentjobrequestrequesttypedef)
- [FraudDetectionResultTypeDef](./type_defs.md#frauddetectionresulttypedef)
- [ListFraudsterRegistrationJobsResponseTypeDef](./type_defs.md#listfraudsterregistrationjobsresponsetypedef)
- [ListSpeakerEnrollmentJobsResponseTypeDef](./type_defs.md#listspeakerenrollmentjobsresponsetypedef)
- [DescribeFraudsterRegistrationJobResponseTypeDef](./type_defs.md#describefraudsterregistrationjobresponsetypedef)
- [StartFraudsterRegistrationJobResponseTypeDef](./type_defs.md#startfraudsterregistrationjobresponsetypedef)
- [DescribeSpeakerEnrollmentJobResponseTypeDef](./type_defs.md#describespeakerenrollmentjobresponsetypedef)
- [StartSpeakerEnrollmentJobResponseTypeDef](./type_defs.md#startspeakerenrollmentjobresponsetypedef)
- [EvaluateSessionResponseTypeDef](./type_defs.md#evaluatesessionresponsetypedef)

