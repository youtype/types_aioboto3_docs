# PinpointSMSVoiceV2 module

> [Index](../README.md) > PinpointSMSVoiceV2


!!! note ""

    Auto-generated documentation for [PinpointSMSVoiceV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
    type annotations stubs module [types-aiobotocore-pinpoint-sms-voice-v2](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice-v2/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `PinpointSMSVoiceV2` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[pinpoint-sms-voice-v2]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[pinpoint-sms-voice-v2]'


# standalone installation
python -m pip install types-aiobotocore-pinpoint-sms-voice-v2
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-pinpoint-sms-voice-v2
```

## Usage

Code samples can be found in [Examples](./usage.md).

## PinpointSMSVoiceV2Client

Type annotations and code completion for  `#!python session.client("pinpoint-sms-voice-v2")` as [PinpointSMSVoiceV2Client](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Client)

```python
# PinpointSMSVoiceV2Client usage example

from aioboto3.session import Session

from types_aiobotocore_pinpoint_sms_voice_v2.client import PinpointSMSVoiceV2Client


session = Session()
async with session.client("pinpoint-sms-voice-v2") as client:
    client: PinpointSMSVoiceV2Client
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("pinpoint-sms-voice-v2").get_paginator("...")`.

```python
# DescribeAccountAttributesPaginator usage example

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribeAccountAttributesPaginator

def get_describe_account_attributes_paginator() -> DescribeAccountAttributesPaginator:
    return client.get_paginator("describe_account_attributes"))
```

- [DescribeAccountAttributesPaginator](./paginators.md#describeaccountattributespaginator)
- [DescribeAccountLimitsPaginator](./paginators.md#describeaccountlimitspaginator)
- [DescribeConfigurationSetsPaginator](./paginators.md#describeconfigurationsetspaginator)
- [DescribeKeywordsPaginator](./paginators.md#describekeywordspaginator)
- [DescribeOptOutListsPaginator](./paginators.md#describeoptoutlistspaginator)
- [DescribeOptedOutNumbersPaginator](./paginators.md#describeoptedoutnumberspaginator)
- [DescribePhoneNumbersPaginator](./paginators.md#describephonenumberspaginator)
- [DescribePoolsPaginator](./paginators.md#describepoolspaginator)
- [DescribeRegistrationAttachmentsPaginator](./paginators.md#describeregistrationattachmentspaginator)
- [DescribeRegistrationFieldDefinitionsPaginator](./paginators.md#describeregistrationfielddefinitionspaginator)
- [DescribeRegistrationFieldValuesPaginator](./paginators.md#describeregistrationfieldvaluespaginator)
- [DescribeRegistrationSectionDefinitionsPaginator](./paginators.md#describeregistrationsectiondefinitionspaginator)
- [DescribeRegistrationTypeDefinitionsPaginator](./paginators.md#describeregistrationtypedefinitionspaginator)
- [DescribeRegistrationVersionsPaginator](./paginators.md#describeregistrationversionspaginator)
- [DescribeRegistrationsPaginator](./paginators.md#describeregistrationspaginator)
- [DescribeSenderIdsPaginator](./paginators.md#describesenderidspaginator)
- [DescribeSpendLimitsPaginator](./paginators.md#describespendlimitspaginator)
- [DescribeVerifiedDestinationNumbersPaginator](./paginators.md#describeverifieddestinationnumberspaginator)
- [ListPoolOriginationIdentitiesPaginator](./paginators.md#listpooloriginationidentitiespaginator)
- [ListRegistrationAssociationsPaginator](./paginators.md#listregistrationassociationspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccountAttributeNameType usage example

from types_aiobotocore_pinpoint_sms_voice_v2.literals import AccountAttributeNameType

def get_value() -> AccountAttributeNameType:
    return "ACCOUNT_TIER"
```

- [AccountAttributeNameType](./literals.md#accountattributenametype)
- [AccountLimitNameType](./literals.md#accountlimitnametype)
- [AttachmentStatusType](./literals.md#attachmentstatustype)
- [AttachmentUploadErrorReasonType](./literals.md#attachmentuploaderrorreasontype)
- [ConfigurationSetFilterNameType](./literals.md#configurationsetfilternametype)
- [DescribeAccountAttributesPaginatorName](./literals.md#describeaccountattributespaginatorname)
- [DescribeAccountLimitsPaginatorName](./literals.md#describeaccountlimitspaginatorname)
- [DescribeConfigurationSetsPaginatorName](./literals.md#describeconfigurationsetspaginatorname)
- [DescribeKeywordsPaginatorName](./literals.md#describekeywordspaginatorname)
- [DescribeOptOutListsPaginatorName](./literals.md#describeoptoutlistspaginatorname)
- [DescribeOptedOutNumbersPaginatorName](./literals.md#describeoptedoutnumberspaginatorname)
- [DescribePhoneNumbersPaginatorName](./literals.md#describephonenumberspaginatorname)
- [DescribePoolsPaginatorName](./literals.md#describepoolspaginatorname)
- [DescribeRegistrationAttachmentsPaginatorName](./literals.md#describeregistrationattachmentspaginatorname)
- [DescribeRegistrationFieldDefinitionsPaginatorName](./literals.md#describeregistrationfielddefinitionspaginatorname)
- [DescribeRegistrationFieldValuesPaginatorName](./literals.md#describeregistrationfieldvaluespaginatorname)
- [DescribeRegistrationSectionDefinitionsPaginatorName](./literals.md#describeregistrationsectiondefinitionspaginatorname)
- [DescribeRegistrationTypeDefinitionsPaginatorName](./literals.md#describeregistrationtypedefinitionspaginatorname)
- [DescribeRegistrationVersionsPaginatorName](./literals.md#describeregistrationversionspaginatorname)
- [DescribeRegistrationsPaginatorName](./literals.md#describeregistrationspaginatorname)
- [DescribeSenderIdsPaginatorName](./literals.md#describesenderidspaginatorname)
- [DescribeSpendLimitsPaginatorName](./literals.md#describespendlimitspaginatorname)
- [DescribeVerifiedDestinationNumbersPaginatorName](./literals.md#describeverifieddestinationnumberspaginatorname)
- [DestinationCountryParameterKeyType](./literals.md#destinationcountryparameterkeytype)
- [EventTypeType](./literals.md#eventtypetype)
- [FieldRequirementType](./literals.md#fieldrequirementtype)
- [FieldTypeType](./literals.md#fieldtypetype)
- [KeywordActionType](./literals.md#keywordactiontype)
- [KeywordFilterNameType](./literals.md#keywordfilternametype)
- [LanguageCodeType](./literals.md#languagecodetype)
- [ListPoolOriginationIdentitiesPaginatorName](./literals.md#listpooloriginationidentitiespaginatorname)
- [ListRegistrationAssociationsPaginatorName](./literals.md#listregistrationassociationspaginatorname)
- [MessageTypeType](./literals.md#messagetypetype)
- [NumberCapabilityType](./literals.md#numbercapabilitytype)
- [NumberStatusType](./literals.md#numberstatustype)
- [NumberTypeType](./literals.md#numbertypetype)
- [OptedOutFilterNameType](./literals.md#optedoutfilternametype)
- [PhoneNumberFilterNameType](./literals.md#phonenumberfilternametype)
- [PoolFilterNameType](./literals.md#poolfilternametype)
- [PoolOriginationIdentitiesFilterNameType](./literals.md#pooloriginationidentitiesfilternametype)
- [PoolStatusType](./literals.md#poolstatustype)
- [RegistrationAssociationBehaviorType](./literals.md#registrationassociationbehaviortype)
- [RegistrationAssociationFilterNameType](./literals.md#registrationassociationfilternametype)
- [RegistrationAttachmentFilterNameType](./literals.md#registrationattachmentfilternametype)
- [RegistrationDisassociationBehaviorType](./literals.md#registrationdisassociationbehaviortype)
- [RegistrationFilterNameType](./literals.md#registrationfilternametype)
- [RegistrationStatusType](./literals.md#registrationstatustype)
- [RegistrationTypeFilterNameType](./literals.md#registrationtypefilternametype)
- [RegistrationVersionFilterNameType](./literals.md#registrationversionfilternametype)
- [RegistrationVersionStatusType](./literals.md#registrationversionstatustype)
- [RequestableNumberTypeType](./literals.md#requestablenumbertypetype)
- [SenderIdFilterNameType](./literals.md#senderidfilternametype)
- [SpendLimitNameType](./literals.md#spendlimitnametype)
- [VerificationChannelType](./literals.md#verificationchanneltype)
- [VerificationStatusType](./literals.md#verificationstatustype)
- [VerifiedDestinationNumberFilterNameType](./literals.md#verifieddestinationnumberfilternametype)
- [VoiceIdType](./literals.md#voiceidtype)
- [VoiceMessageBodyTextTypeType](./literals.md#voicemessagebodytexttypetype)
- [PinpointSMSVoiceV2ServiceName](./literals.md#pinpointsmsvoicev2servicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccountAttributeTypeDef](./type_defs.md#accountattributetypedef)
- [AccountLimitTypeDef](./type_defs.md#accountlimittypedef)
- [AssociateOriginationIdentityRequestRequestTypeDef](./type_defs.md#associateoriginationidentityrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CloudWatchLogsDestinationTypeDef](./type_defs.md#cloudwatchlogsdestinationtypedef)
- [ConfigurationSetFilterTypeDef](./type_defs.md#configurationsetfiltertypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [KinesisFirehoseDestinationTypeDef](./type_defs.md#kinesisfirehosedestinationtypedef)
- [SnsDestinationTypeDef](./type_defs.md#snsdestinationtypedef)
- [CreateRegistrationAssociationRequestRequestTypeDef](./type_defs.md#createregistrationassociationrequestrequesttypedef)
- [CreateRegistrationVersionRequestRequestTypeDef](./type_defs.md#createregistrationversionrequestrequesttypedef)
- [RegistrationVersionStatusHistoryTypeDef](./type_defs.md#registrationversionstatushistorytypedef)
- [DeleteConfigurationSetRequestRequestTypeDef](./type_defs.md#deleteconfigurationsetrequestrequesttypedef)
- [DeleteDefaultMessageTypeRequestRequestTypeDef](./type_defs.md#deletedefaultmessagetyperequestrequesttypedef)
- [DeleteDefaultSenderIdRequestRequestTypeDef](./type_defs.md#deletedefaultsenderidrequestrequesttypedef)
- [DeleteEventDestinationRequestRequestTypeDef](./type_defs.md#deleteeventdestinationrequestrequesttypedef)
- [DeleteKeywordRequestRequestTypeDef](./type_defs.md#deletekeywordrequestrequesttypedef)
- [DeleteOptOutListRequestRequestTypeDef](./type_defs.md#deleteoptoutlistrequestrequesttypedef)
- [DeleteOptedOutNumberRequestRequestTypeDef](./type_defs.md#deleteoptedoutnumberrequestrequesttypedef)
- [DeletePoolRequestRequestTypeDef](./type_defs.md#deletepoolrequestrequesttypedef)
- [DeleteRegistrationAttachmentRequestRequestTypeDef](./type_defs.md#deleteregistrationattachmentrequestrequesttypedef)
- [DeleteRegistrationFieldValueRequestRequestTypeDef](./type_defs.md#deleteregistrationfieldvaluerequestrequesttypedef)
- [DeleteRegistrationRequestRequestTypeDef](./type_defs.md#deleteregistrationrequestrequesttypedef)
- [DeleteVerifiedDestinationNumberRequestRequestTypeDef](./type_defs.md#deleteverifieddestinationnumberrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeAccountAttributesRequestRequestTypeDef](./type_defs.md#describeaccountattributesrequestrequesttypedef)
- [DescribeAccountLimitsRequestRequestTypeDef](./type_defs.md#describeaccountlimitsrequestrequesttypedef)
- [KeywordFilterTypeDef](./type_defs.md#keywordfiltertypedef)
- [KeywordInformationTypeDef](./type_defs.md#keywordinformationtypedef)
- [DescribeOptOutListsRequestRequestTypeDef](./type_defs.md#describeoptoutlistsrequestrequesttypedef)
- [OptOutListInformationTypeDef](./type_defs.md#optoutlistinformationtypedef)
- [OptedOutFilterTypeDef](./type_defs.md#optedoutfiltertypedef)
- [OptedOutNumberInformationTypeDef](./type_defs.md#optedoutnumberinformationtypedef)
- [PhoneNumberFilterTypeDef](./type_defs.md#phonenumberfiltertypedef)
- [PhoneNumberInformationTypeDef](./type_defs.md#phonenumberinformationtypedef)
- [PoolFilterTypeDef](./type_defs.md#poolfiltertypedef)
- [PoolInformationTypeDef](./type_defs.md#poolinformationtypedef)
- [RegistrationAttachmentFilterTypeDef](./type_defs.md#registrationattachmentfiltertypedef)
- [RegistrationAttachmentsInformationTypeDef](./type_defs.md#registrationattachmentsinformationtypedef)
- [DescribeRegistrationFieldDefinitionsRequestRequestTypeDef](./type_defs.md#describeregistrationfielddefinitionsrequestrequesttypedef)
- [DescribeRegistrationFieldValuesRequestRequestTypeDef](./type_defs.md#describeregistrationfieldvaluesrequestrequesttypedef)
- [RegistrationFieldValueInformationTypeDef](./type_defs.md#registrationfieldvalueinformationtypedef)
- [DescribeRegistrationSectionDefinitionsRequestRequestTypeDef](./type_defs.md#describeregistrationsectiondefinitionsrequestrequesttypedef)
- [RegistrationTypeFilterTypeDef](./type_defs.md#registrationtypefiltertypedef)
- [RegistrationVersionFilterTypeDef](./type_defs.md#registrationversionfiltertypedef)
- [RegistrationFilterTypeDef](./type_defs.md#registrationfiltertypedef)
- [RegistrationInformationTypeDef](./type_defs.md#registrationinformationtypedef)
- [SenderIdAndCountryTypeDef](./type_defs.md#senderidandcountrytypedef)
- [SenderIdFilterTypeDef](./type_defs.md#senderidfiltertypedef)
- [SenderIdInformationTypeDef](./type_defs.md#senderidinformationtypedef)
- [DescribeSpendLimitsRequestRequestTypeDef](./type_defs.md#describespendlimitsrequestrequesttypedef)
- [SpendLimitTypeDef](./type_defs.md#spendlimittypedef)
- [VerifiedDestinationNumberFilterTypeDef](./type_defs.md#verifieddestinationnumberfiltertypedef)
- [VerifiedDestinationNumberInformationTypeDef](./type_defs.md#verifieddestinationnumberinformationtypedef)
- [DisassociateOriginationIdentityRequestRequestTypeDef](./type_defs.md#disassociateoriginationidentityrequestrequesttypedef)
- [DiscardRegistrationVersionRequestRequestTypeDef](./type_defs.md#discardregistrationversionrequestrequesttypedef)
- [PoolOriginationIdentitiesFilterTypeDef](./type_defs.md#pooloriginationidentitiesfiltertypedef)
- [OriginationIdentityMetadataTypeDef](./type_defs.md#originationidentitymetadatatypedef)
- [RegistrationAssociationFilterTypeDef](./type_defs.md#registrationassociationfiltertypedef)
- [RegistrationAssociationMetadataTypeDef](./type_defs.md#registrationassociationmetadatatypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [PutKeywordRequestRequestTypeDef](./type_defs.md#putkeywordrequestrequesttypedef)
- [PutOptedOutNumberRequestRequestTypeDef](./type_defs.md#putoptedoutnumberrequestrequesttypedef)
- [PutRegistrationFieldValueRequestRequestTypeDef](./type_defs.md#putregistrationfieldvaluerequestrequesttypedef)
- [RegistrationDeniedReasonInformationTypeDef](./type_defs.md#registrationdeniedreasoninformationtypedef)
- [SelectValidationTypeDef](./type_defs.md#selectvalidationtypedef)
- [TextValidationTypeDef](./type_defs.md#textvalidationtypedef)
- [SelectOptionDescriptionTypeDef](./type_defs.md#selectoptiondescriptiontypedef)
- [RegistrationSectionDisplayHintsTypeDef](./type_defs.md#registrationsectiondisplayhintstypedef)
- [RegistrationTypeDisplayHintsTypeDef](./type_defs.md#registrationtypedisplayhintstypedef)
- [SupportedAssociationTypeDef](./type_defs.md#supportedassociationtypedef)
- [ReleasePhoneNumberRequestRequestTypeDef](./type_defs.md#releasephonenumberrequestrequesttypedef)
- [ReleaseSenderIdRequestRequestTypeDef](./type_defs.md#releasesenderidrequestrequesttypedef)
- [SendDestinationNumberVerificationCodeRequestRequestTypeDef](./type_defs.md#senddestinationnumberverificationcoderequestrequesttypedef)
- [SendTextMessageRequestRequestTypeDef](./type_defs.md#sendtextmessagerequestrequesttypedef)
- [SendVoiceMessageRequestRequestTypeDef](./type_defs.md#sendvoicemessagerequestrequesttypedef)
- [SetDefaultMessageTypeRequestRequestTypeDef](./type_defs.md#setdefaultmessagetyperequestrequesttypedef)
- [SetDefaultSenderIdRequestRequestTypeDef](./type_defs.md#setdefaultsenderidrequestrequesttypedef)
- [SetTextMessageSpendLimitOverrideRequestRequestTypeDef](./type_defs.md#settextmessagespendlimitoverriderequestrequesttypedef)
- [SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef](./type_defs.md#setvoicemessagespendlimitoverriderequestrequesttypedef)
- [SubmitRegistrationVersionRequestRequestTypeDef](./type_defs.md#submitregistrationversionrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdatePhoneNumberRequestRequestTypeDef](./type_defs.md#updatephonenumberrequestrequesttypedef)
- [UpdatePoolRequestRequestTypeDef](./type_defs.md#updatepoolrequestrequesttypedef)
- [UpdateSenderIdRequestRequestTypeDef](./type_defs.md#updatesenderidrequestrequesttypedef)
- [VerifyDestinationNumberRequestRequestTypeDef](./type_defs.md#verifydestinationnumberrequestrequesttypedef)
- [AssociateOriginationIdentityResultTypeDef](./type_defs.md#associateoriginationidentityresulttypedef)
- [CreateRegistrationAssociationResultTypeDef](./type_defs.md#createregistrationassociationresulttypedef)
- [DeleteDefaultMessageTypeResultTypeDef](./type_defs.md#deletedefaultmessagetyperesulttypedef)
- [DeleteDefaultSenderIdResultTypeDef](./type_defs.md#deletedefaultsenderidresulttypedef)
- [DeleteKeywordResultTypeDef](./type_defs.md#deletekeywordresulttypedef)
- [DeleteOptOutListResultTypeDef](./type_defs.md#deleteoptoutlistresulttypedef)
- [DeleteOptedOutNumberResultTypeDef](./type_defs.md#deleteoptedoutnumberresulttypedef)
- [DeletePoolResultTypeDef](./type_defs.md#deletepoolresulttypedef)
- [DeleteRegistrationAttachmentResultTypeDef](./type_defs.md#deleteregistrationattachmentresulttypedef)
- [DeleteRegistrationFieldValueResultTypeDef](./type_defs.md#deleteregistrationfieldvalueresulttypedef)
- [DeleteRegistrationResultTypeDef](./type_defs.md#deleteregistrationresulttypedef)
- [DeleteTextMessageSpendLimitOverrideResultTypeDef](./type_defs.md#deletetextmessagespendlimitoverrideresulttypedef)
- [DeleteVerifiedDestinationNumberResultTypeDef](./type_defs.md#deleteverifieddestinationnumberresulttypedef)
- [DeleteVoiceMessageSpendLimitOverrideResultTypeDef](./type_defs.md#deletevoicemessagespendlimitoverrideresulttypedef)
- [DescribeAccountAttributesResultTypeDef](./type_defs.md#describeaccountattributesresulttypedef)
- [DescribeAccountLimitsResultTypeDef](./type_defs.md#describeaccountlimitsresulttypedef)
- [DisassociateOriginationIdentityResultTypeDef](./type_defs.md#disassociateoriginationidentityresulttypedef)
- [PutKeywordResultTypeDef](./type_defs.md#putkeywordresulttypedef)
- [PutOptedOutNumberResultTypeDef](./type_defs.md#putoptedoutnumberresulttypedef)
- [PutRegistrationFieldValueResultTypeDef](./type_defs.md#putregistrationfieldvalueresulttypedef)
- [ReleasePhoneNumberResultTypeDef](./type_defs.md#releasephonenumberresulttypedef)
- [ReleaseSenderIdResultTypeDef](./type_defs.md#releasesenderidresulttypedef)
- [SendDestinationNumberVerificationCodeResultTypeDef](./type_defs.md#senddestinationnumberverificationcoderesulttypedef)
- [SendTextMessageResultTypeDef](./type_defs.md#sendtextmessageresulttypedef)
- [SendVoiceMessageResultTypeDef](./type_defs.md#sendvoicemessageresulttypedef)
- [SetDefaultMessageTypeResultTypeDef](./type_defs.md#setdefaultmessagetyperesulttypedef)
- [SetDefaultSenderIdResultTypeDef](./type_defs.md#setdefaultsenderidresulttypedef)
- [SetTextMessageSpendLimitOverrideResultTypeDef](./type_defs.md#settextmessagespendlimitoverrideresulttypedef)
- [SetVoiceMessageSpendLimitOverrideResultTypeDef](./type_defs.md#setvoicemessagespendlimitoverrideresulttypedef)
- [UpdatePhoneNumberResultTypeDef](./type_defs.md#updatephonenumberresulttypedef)
- [UpdatePoolResultTypeDef](./type_defs.md#updatepoolresulttypedef)
- [UpdateSenderIdResultTypeDef](./type_defs.md#updatesenderidresulttypedef)
- [VerifyDestinationNumberResultTypeDef](./type_defs.md#verifydestinationnumberresulttypedef)
- [DescribeConfigurationSetsRequestRequestTypeDef](./type_defs.md#describeconfigurationsetsrequestrequesttypedef)
- [CreateConfigurationSetRequestRequestTypeDef](./type_defs.md#createconfigurationsetrequestrequesttypedef)
- [CreateConfigurationSetResultTypeDef](./type_defs.md#createconfigurationsetresulttypedef)
- [CreateOptOutListRequestRequestTypeDef](./type_defs.md#createoptoutlistrequestrequesttypedef)
- [CreateOptOutListResultTypeDef](./type_defs.md#createoptoutlistresulttypedef)
- [CreatePoolRequestRequestTypeDef](./type_defs.md#createpoolrequestrequesttypedef)
- [CreatePoolResultTypeDef](./type_defs.md#createpoolresulttypedef)
- [CreateRegistrationAttachmentRequestRequestTypeDef](./type_defs.md#createregistrationattachmentrequestrequesttypedef)
- [CreateRegistrationAttachmentResultTypeDef](./type_defs.md#createregistrationattachmentresulttypedef)
- [CreateRegistrationRequestRequestTypeDef](./type_defs.md#createregistrationrequestrequesttypedef)
- [CreateRegistrationResultTypeDef](./type_defs.md#createregistrationresulttypedef)
- [CreateVerifiedDestinationNumberRequestRequestTypeDef](./type_defs.md#createverifieddestinationnumberrequestrequesttypedef)
- [CreateVerifiedDestinationNumberResultTypeDef](./type_defs.md#createverifieddestinationnumberresulttypedef)
- [ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef)
- [RequestPhoneNumberRequestRequestTypeDef](./type_defs.md#requestphonenumberrequestrequesttypedef)
- [RequestPhoneNumberResultTypeDef](./type_defs.md#requestphonenumberresulttypedef)
- [RequestSenderIdRequestRequestTypeDef](./type_defs.md#requestsenderidrequestrequesttypedef)
- [RequestSenderIdResultTypeDef](./type_defs.md#requestsenderidresulttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateEventDestinationRequestRequestTypeDef](./type_defs.md#createeventdestinationrequestrequesttypedef)
- [EventDestinationTypeDef](./type_defs.md#eventdestinationtypedef)
- [UpdateEventDestinationRequestRequestTypeDef](./type_defs.md#updateeventdestinationrequestrequesttypedef)
- [CreateRegistrationVersionResultTypeDef](./type_defs.md#createregistrationversionresulttypedef)
- [DiscardRegistrationVersionResultTypeDef](./type_defs.md#discardregistrationversionresulttypedef)
- [SubmitRegistrationVersionResultTypeDef](./type_defs.md#submitregistrationversionresulttypedef)
- [DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef](./type_defs.md#describeaccountattributesrequestdescribeaccountattributespaginatetypedef)
- [DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef](./type_defs.md#describeaccountlimitsrequestdescribeaccountlimitspaginatetypedef)
- [DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef](./type_defs.md#describeconfigurationsetsrequestdescribeconfigurationsetspaginatetypedef)
- [DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef](./type_defs.md#describeoptoutlistsrequestdescribeoptoutlistspaginatetypedef)
- [DescribeRegistrationFieldDefinitionsRequestDescribeRegistrationFieldDefinitionsPaginateTypeDef](./type_defs.md#describeregistrationfielddefinitionsrequestdescriberegistrationfielddefinitionspaginatetypedef)
- [DescribeRegistrationFieldValuesRequestDescribeRegistrationFieldValuesPaginateTypeDef](./type_defs.md#describeregistrationfieldvaluesrequestdescriberegistrationfieldvaluespaginatetypedef)
- [DescribeRegistrationSectionDefinitionsRequestDescribeRegistrationSectionDefinitionsPaginateTypeDef](./type_defs.md#describeregistrationsectiondefinitionsrequestdescriberegistrationsectiondefinitionspaginatetypedef)
- [DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef](./type_defs.md#describespendlimitsrequestdescribespendlimitspaginatetypedef)
- [DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef](./type_defs.md#describekeywordsrequestdescribekeywordspaginatetypedef)
- [DescribeKeywordsRequestRequestTypeDef](./type_defs.md#describekeywordsrequestrequesttypedef)
- [DescribeKeywordsResultTypeDef](./type_defs.md#describekeywordsresulttypedef)
- [DescribeOptOutListsResultTypeDef](./type_defs.md#describeoptoutlistsresulttypedef)
- [DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef](./type_defs.md#describeoptedoutnumbersrequestdescribeoptedoutnumberspaginatetypedef)
- [DescribeOptedOutNumbersRequestRequestTypeDef](./type_defs.md#describeoptedoutnumbersrequestrequesttypedef)
- [DescribeOptedOutNumbersResultTypeDef](./type_defs.md#describeoptedoutnumbersresulttypedef)
- [DescribePhoneNumbersRequestDescribePhoneNumbersPaginateTypeDef](./type_defs.md#describephonenumbersrequestdescribephonenumberspaginatetypedef)
- [DescribePhoneNumbersRequestRequestTypeDef](./type_defs.md#describephonenumbersrequestrequesttypedef)
- [DescribePhoneNumbersResultTypeDef](./type_defs.md#describephonenumbersresulttypedef)
- [DescribePoolsRequestDescribePoolsPaginateTypeDef](./type_defs.md#describepoolsrequestdescribepoolspaginatetypedef)
- [DescribePoolsRequestRequestTypeDef](./type_defs.md#describepoolsrequestrequesttypedef)
- [DescribePoolsResultTypeDef](./type_defs.md#describepoolsresulttypedef)
- [DescribeRegistrationAttachmentsRequestDescribeRegistrationAttachmentsPaginateTypeDef](./type_defs.md#describeregistrationattachmentsrequestdescriberegistrationattachmentspaginatetypedef)
- [DescribeRegistrationAttachmentsRequestRequestTypeDef](./type_defs.md#describeregistrationattachmentsrequestrequesttypedef)
- [DescribeRegistrationAttachmentsResultTypeDef](./type_defs.md#describeregistrationattachmentsresulttypedef)
- [DescribeRegistrationFieldValuesResultTypeDef](./type_defs.md#describeregistrationfieldvaluesresulttypedef)
- [DescribeRegistrationTypeDefinitionsRequestDescribeRegistrationTypeDefinitionsPaginateTypeDef](./type_defs.md#describeregistrationtypedefinitionsrequestdescriberegistrationtypedefinitionspaginatetypedef)
- [DescribeRegistrationTypeDefinitionsRequestRequestTypeDef](./type_defs.md#describeregistrationtypedefinitionsrequestrequesttypedef)
- [DescribeRegistrationVersionsRequestDescribeRegistrationVersionsPaginateTypeDef](./type_defs.md#describeregistrationversionsrequestdescriberegistrationversionspaginatetypedef)
- [DescribeRegistrationVersionsRequestRequestTypeDef](./type_defs.md#describeregistrationversionsrequestrequesttypedef)
- [DescribeRegistrationsRequestDescribeRegistrationsPaginateTypeDef](./type_defs.md#describeregistrationsrequestdescriberegistrationspaginatetypedef)
- [DescribeRegistrationsRequestRequestTypeDef](./type_defs.md#describeregistrationsrequestrequesttypedef)
- [DescribeRegistrationsResultTypeDef](./type_defs.md#describeregistrationsresulttypedef)
- [DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef](./type_defs.md#describesenderidsrequestdescribesenderidspaginatetypedef)
- [DescribeSenderIdsRequestRequestTypeDef](./type_defs.md#describesenderidsrequestrequesttypedef)
- [DescribeSenderIdsResultTypeDef](./type_defs.md#describesenderidsresulttypedef)
- [DescribeSpendLimitsResultTypeDef](./type_defs.md#describespendlimitsresulttypedef)
- [DescribeVerifiedDestinationNumbersRequestDescribeVerifiedDestinationNumbersPaginateTypeDef](./type_defs.md#describeverifieddestinationnumbersrequestdescribeverifieddestinationnumberspaginatetypedef)
- [DescribeVerifiedDestinationNumbersRequestRequestTypeDef](./type_defs.md#describeverifieddestinationnumbersrequestrequesttypedef)
- [DescribeVerifiedDestinationNumbersResultTypeDef](./type_defs.md#describeverifieddestinationnumbersresulttypedef)
- [ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef](./type_defs.md#listpooloriginationidentitiesrequestlistpooloriginationidentitiespaginatetypedef)
- [ListPoolOriginationIdentitiesRequestRequestTypeDef](./type_defs.md#listpooloriginationidentitiesrequestrequesttypedef)
- [ListPoolOriginationIdentitiesResultTypeDef](./type_defs.md#listpooloriginationidentitiesresulttypedef)
- [ListRegistrationAssociationsRequestListRegistrationAssociationsPaginateTypeDef](./type_defs.md#listregistrationassociationsrequestlistregistrationassociationspaginatetypedef)
- [ListRegistrationAssociationsRequestRequestTypeDef](./type_defs.md#listregistrationassociationsrequestrequesttypedef)
- [ListRegistrationAssociationsResultTypeDef](./type_defs.md#listregistrationassociationsresulttypedef)
- [RegistrationVersionInformationTypeDef](./type_defs.md#registrationversioninformationtypedef)
- [RegistrationFieldDisplayHintsTypeDef](./type_defs.md#registrationfielddisplayhintstypedef)
- [RegistrationSectionDefinitionTypeDef](./type_defs.md#registrationsectiondefinitiontypedef)
- [RegistrationTypeDefinitionTypeDef](./type_defs.md#registrationtypedefinitiontypedef)
- [ConfigurationSetInformationTypeDef](./type_defs.md#configurationsetinformationtypedef)
- [CreateEventDestinationResultTypeDef](./type_defs.md#createeventdestinationresulttypedef)
- [DeleteConfigurationSetResultTypeDef](./type_defs.md#deleteconfigurationsetresulttypedef)
- [DeleteEventDestinationResultTypeDef](./type_defs.md#deleteeventdestinationresulttypedef)
- [UpdateEventDestinationResultTypeDef](./type_defs.md#updateeventdestinationresulttypedef)
- [DescribeRegistrationVersionsResultTypeDef](./type_defs.md#describeregistrationversionsresulttypedef)
- [RegistrationFieldDefinitionTypeDef](./type_defs.md#registrationfielddefinitiontypedef)
- [DescribeRegistrationSectionDefinitionsResultTypeDef](./type_defs.md#describeregistrationsectiondefinitionsresulttypedef)
- [DescribeRegistrationTypeDefinitionsResultTypeDef](./type_defs.md#describeregistrationtypedefinitionsresulttypedef)
- [DescribeConfigurationSetsResultTypeDef](./type_defs.md#describeconfigurationsetsresulttypedef)
- [DescribeRegistrationFieldDefinitionsResultTypeDef](./type_defs.md#describeregistrationfielddefinitionsresulttypedef)

