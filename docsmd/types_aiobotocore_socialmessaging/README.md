# EndUserMessagingSocial module

> [Index](../README.md) > EndUserMessagingSocial


!!! note ""

    Auto-generated documentation for [EndUserMessagingSocial](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging.html#endusermessagingsocial)
    type annotations stubs module [types-aiobotocore-socialmessaging](https://pypi.org/project/types-aiobotocore-socialmessaging/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `EndUserMessagingSocial` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `EndUserMessagingSocial` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[socialmessaging]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[socialmessaging]'

# standalone installation
python -m pip install types-aiobotocore-socialmessaging
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-socialmessaging
```

## Usage

Code samples can be found in [Examples](./usage.md).

## EndUserMessagingSocialClient

Type annotations and code completion for  `#!python session.client("socialmessaging")` as [EndUserMessagingSocialClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging.html#EndUserMessagingSocial.Client)

```python
# EndUserMessagingSocialClient usage example

from aioboto3.session import Session

from types_aiobotocore_socialmessaging.client import EndUserMessagingSocialClient


session = Session()
async with session.client("socialmessaging") as client:
    client: EndUserMessagingSocialClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("socialmessaging").get_paginator("...")`.

```python
# ListLinkedWhatsAppBusinessAccountsPaginator usage example

from types_aiobotocore_socialmessaging.paginator import ListLinkedWhatsAppBusinessAccountsPaginator

def get_list_linked_whatsapp_business_accounts_paginator() -> ListLinkedWhatsAppBusinessAccountsPaginator:
    return client.get_paginator("list_linked_whatsapp_business_accounts"))
```

- [ListLinkedWhatsAppBusinessAccountsPaginator](./paginators.md#listlinkedwhatsappbusinessaccountspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ListLinkedWhatsAppBusinessAccountsPaginatorName usage example

from types_aiobotocore_socialmessaging.literals import ListLinkedWhatsAppBusinessAccountsPaginatorName

def get_value() -> ListLinkedWhatsAppBusinessAccountsPaginatorName:
    return "list_linked_whatsapp_business_accounts"
```

- [ListLinkedWhatsAppBusinessAccountsPaginatorName](./literals.md#listlinkedwhatsappbusinessaccountspaginatorname)
- [RegistrationStatusType](./literals.md#registrationstatustype)
- [EndUserMessagingSocialServiceName](./literals.md#endusermessagingsocialservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [WhatsAppSignupCallbackTypeDef](./type_defs.md#whatsappsignupcallbacktypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [DeleteWhatsAppMessageMediaInputRequestTypeDef](./type_defs.md#deletewhatsappmessagemediainputrequesttypedef)
- [DisassociateWhatsAppBusinessAccountInputRequestTypeDef](./type_defs.md#disassociatewhatsappbusinessaccountinputrequesttypedef)
- [GetLinkedWhatsAppBusinessAccountInputRequestTypeDef](./type_defs.md#getlinkedwhatsappbusinessaccountinputrequesttypedef)
- [GetLinkedWhatsAppBusinessAccountPhoneNumberInputRequestTypeDef](./type_defs.md#getlinkedwhatsappbusinessaccountphonenumberinputrequesttypedef)
- [WhatsAppPhoneNumberDetailTypeDef](./type_defs.md#whatsappphonenumberdetailtypedef)
- [S3FileTypeDef](./type_defs.md#s3filetypedef)
- [S3PresignedUrlTypeDef](./type_defs.md#s3presignedurltypedef)
- [WhatsAppBusinessAccountEventDestinationTypeDef](./type_defs.md#whatsappbusinessaccounteventdestinationtypedef)
- [WhatsAppPhoneNumberSummaryTypeDef](./type_defs.md#whatsappphonenumbersummarytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListLinkedWhatsAppBusinessAccountsInputRequestTypeDef](./type_defs.md#listlinkedwhatsappbusinessaccountsinputrequesttypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [DeleteWhatsAppMessageMediaOutputTypeDef](./type_defs.md#deletewhatsappmessagemediaoutputtypedef)
- [GetWhatsAppMessageMediaOutputTypeDef](./type_defs.md#getwhatsappmessagemediaoutputtypedef)
- [PostWhatsAppMessageMediaOutputTypeDef](./type_defs.md#postwhatsappmessagemediaoutputtypedef)
- [SendWhatsAppMessageOutputTypeDef](./type_defs.md#sendwhatsappmessageoutputtypedef)
- [TagResourceOutputTypeDef](./type_defs.md#tagresourceoutputtypedef)
- [UntagResourceOutputTypeDef](./type_defs.md#untagresourceoutputtypedef)
- [SendWhatsAppMessageInputRequestTypeDef](./type_defs.md#sendwhatsappmessageinputrequesttypedef)
- [GetLinkedWhatsAppBusinessAccountPhoneNumberOutputTypeDef](./type_defs.md#getlinkedwhatsappbusinessaccountphonenumberoutputtypedef)
- [LinkedWhatsAppBusinessAccountIdMetaDataTypeDef](./type_defs.md#linkedwhatsappbusinessaccountidmetadatatypedef)
- [GetWhatsAppMessageMediaInputRequestTypeDef](./type_defs.md#getwhatsappmessagemediainputrequesttypedef)
- [PostWhatsAppMessageMediaInputRequestTypeDef](./type_defs.md#postwhatsappmessagemediainputrequesttypedef)
- [LinkedWhatsAppBusinessAccountSummaryTypeDef](./type_defs.md#linkedwhatsappbusinessaccountsummarytypedef)
- [PutWhatsAppBusinessAccountEventDestinationsInputRequestTypeDef](./type_defs.md#putwhatsappbusinessaccounteventdestinationsinputrequesttypedef)
- [LinkedWhatsAppBusinessAccountTypeDef](./type_defs.md#linkedwhatsappbusinessaccounttypedef)
- [ListLinkedWhatsAppBusinessAccountsInputPaginateTypeDef](./type_defs.md#listlinkedwhatsappbusinessaccountsinputpaginatetypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [WabaPhoneNumberSetupFinalizationTypeDef](./type_defs.md#wabaphonenumbersetupfinalizationtypedef)
- [WabaSetupFinalizationTypeDef](./type_defs.md#wabasetupfinalizationtypedef)
- [WhatsAppSignupCallbackResultTypeDef](./type_defs.md#whatsappsignupcallbackresulttypedef)
- [ListLinkedWhatsAppBusinessAccountsOutputTypeDef](./type_defs.md#listlinkedwhatsappbusinessaccountsoutputtypedef)
- [GetLinkedWhatsAppBusinessAccountOutputTypeDef](./type_defs.md#getlinkedwhatsappbusinessaccountoutputtypedef)
- [WhatsAppSetupFinalizationTypeDef](./type_defs.md#whatsappsetupfinalizationtypedef)
- [AssociateWhatsAppBusinessAccountOutputTypeDef](./type_defs.md#associatewhatsappbusinessaccountoutputtypedef)
- [AssociateWhatsAppBusinessAccountInputRequestTypeDef](./type_defs.md#associatewhatsappbusinessaccountinputrequesttypedef)
