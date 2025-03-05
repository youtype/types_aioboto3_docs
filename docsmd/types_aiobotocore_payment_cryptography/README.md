# PaymentCryptographyControlPlane module

> [Index](../README.md) > PaymentCryptographyControlPlane


!!! note ""

    Auto-generated documentation for [PaymentCryptographyControlPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#paymentcryptographycontrolplane)
    type annotations stubs module [types-aiobotocore-payment-cryptography](https://pypi.org/project/types-aiobotocore-payment-cryptography/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==14.1.0' mypy-boto3-builder`
1. Select `aioboto3` AWS SDK.
1. Add `PaymentCryptographyControlPlane` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `PaymentCryptographyControlPlane` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[payment-cryptography]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[payment-cryptography]'

# standalone installation
python -m pip install types-aiobotocore-payment-cryptography
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-payment-cryptography
```

## Usage

Code samples can be found in [Examples](./usage.md).

## PaymentCryptographyControlPlaneClient

Type annotations and code completion for  `#!python session.client("payment-cryptography")` as [PaymentCryptographyControlPlaneClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Client)

```python
# PaymentCryptographyControlPlaneClient usage example

from aioboto3.session import Session

from types_aiobotocore_payment_cryptography.client import PaymentCryptographyControlPlaneClient


session = Session()
async with session.client("payment-cryptography") as client:
    client: PaymentCryptographyControlPlaneClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("payment-cryptography").get_paginator("...")`.

```python
# ListAliasesPaginator usage example

from types_aiobotocore_payment_cryptography.paginator import ListAliasesPaginator

def get_list_aliases_paginator() -> ListAliasesPaginator:
    return client.get_paginator("list_aliases"))
```

- [ListAliasesPaginator](./paginators.md#listaliasespaginator)
- [ListKeysPaginator](./paginators.md#listkeyspaginator)
- [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# KeyAlgorithmType usage example

from types_aiobotocore_payment_cryptography.literals import KeyAlgorithmType

def get_value() -> KeyAlgorithmType:
    return "AES_128"
```

- [KeyAlgorithmType](./literals.md#keyalgorithmtype)
- [KeyCheckValueAlgorithmType](./literals.md#keycheckvaluealgorithmtype)
- [KeyClassType](./literals.md#keyclasstype)
- [KeyExportabilityType](./literals.md#keyexportabilitytype)
- [KeyMaterialTypeType](./literals.md#keymaterialtypetype)
- [KeyOriginType](./literals.md#keyorigintype)
- [KeyStateType](./literals.md#keystatetype)
- [KeyUsageType](./literals.md#keyusagetype)
- [ListAliasesPaginatorName](./literals.md#listaliasespaginatorname)
- [ListKeysPaginatorName](./literals.md#listkeyspaginatorname)
- [ListTagsForResourcePaginatorName](./literals.md#listtagsforresourcepaginatorname)
- [Tr34KeyBlockFormatType](./literals.md#tr34keyblockformattype)
- [WrappedKeyMaterialFormatType](./literals.md#wrappedkeymaterialformattype)
- [WrappingKeySpecType](./literals.md#wrappingkeyspectype)
- [PaymentCryptographyControlPlaneServiceName](./literals.md#paymentcryptographycontrolplaneservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AliasTypeDef](./type_defs.md#aliastypedef)
- [CreateAliasInputTypeDef](./type_defs.md#createaliasinputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [DeleteAliasInputTypeDef](./type_defs.md#deletealiasinputtypedef)
- [DeleteKeyInputTypeDef](./type_defs.md#deletekeyinputtypedef)
- [ExportDukptInitialKeyTypeDef](./type_defs.md#exportdukptinitialkeytypedef)
- [ExportKeyCryptogramTypeDef](./type_defs.md#exportkeycryptogramtypedef)
- [WrappedKeyTypeDef](./type_defs.md#wrappedkeytypedef)
- [GetAliasInputTypeDef](./type_defs.md#getaliasinputtypedef)
- [GetKeyInputTypeDef](./type_defs.md#getkeyinputtypedef)
- [GetParametersForExportInputTypeDef](./type_defs.md#getparametersforexportinputtypedef)
- [GetParametersForImportInputTypeDef](./type_defs.md#getparametersforimportinputtypedef)
- [GetPublicKeyCertificateInputTypeDef](./type_defs.md#getpublickeycertificateinputtypedef)
- [ImportTr31KeyBlockTypeDef](./type_defs.md#importtr31keyblocktypedef)
- [ImportTr34KeyBlockTypeDef](./type_defs.md#importtr34keyblocktypedef)
- [KeyModesOfUseTypeDef](./type_defs.md#keymodesofusetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAliasesInputTypeDef](./type_defs.md#listaliasesinputtypedef)
- [ListKeysInputTypeDef](./type_defs.md#listkeysinputtypedef)
- [ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef)
- [RestoreKeyInputTypeDef](./type_defs.md#restorekeyinputtypedef)
- [StartKeyUsageInputTypeDef](./type_defs.md#startkeyusageinputtypedef)
- [StopKeyUsageInputTypeDef](./type_defs.md#stopkeyusageinputtypedef)
- [UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef)
- [UpdateAliasInputTypeDef](./type_defs.md#updatealiasinputtypedef)
- [CreateAliasOutputTypeDef](./type_defs.md#createaliasoutputtypedef)
- [GetAliasOutputTypeDef](./type_defs.md#getaliasoutputtypedef)
- [GetParametersForExportOutputTypeDef](./type_defs.md#getparametersforexportoutputtypedef)
- [GetParametersForImportOutputTypeDef](./type_defs.md#getparametersforimportoutputtypedef)
- [GetPublicKeyCertificateOutputTypeDef](./type_defs.md#getpublickeycertificateoutputtypedef)
- [ListAliasesOutputTypeDef](./type_defs.md#listaliasesoutputtypedef)
- [UpdateAliasOutputTypeDef](./type_defs.md#updatealiasoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef)
- [ExportAttributesTypeDef](./type_defs.md#exportattributestypedef)
- [ExportKeyOutputTypeDef](./type_defs.md#exportkeyoutputtypedef)
- [KeyAttributesTypeDef](./type_defs.md#keyattributestypedef)
- [KeyBlockHeadersTypeDef](./type_defs.md#keyblockheaderstypedef)
- [ListAliasesInputPaginateTypeDef](./type_defs.md#listaliasesinputpaginatetypedef)
- [ListKeysInputPaginateTypeDef](./type_defs.md#listkeysinputpaginatetypedef)
- [ListTagsForResourceInputPaginateTypeDef](./type_defs.md#listtagsforresourceinputpaginatetypedef)
- [CreateKeyInputTypeDef](./type_defs.md#createkeyinputtypedef)
- [ImportKeyCryptogramTypeDef](./type_defs.md#importkeycryptogramtypedef)
- [KeySummaryTypeDef](./type_defs.md#keysummarytypedef)
- [KeyTypeDef](./type_defs.md#keytypedef)
- [RootCertificatePublicKeyTypeDef](./type_defs.md#rootcertificatepublickeytypedef)
- [TrustedCertificatePublicKeyTypeDef](./type_defs.md#trustedcertificatepublickeytypedef)
- [ExportTr31KeyBlockTypeDef](./type_defs.md#exporttr31keyblocktypedef)
- [ExportTr34KeyBlockTypeDef](./type_defs.md#exporttr34keyblocktypedef)
- [ListKeysOutputTypeDef](./type_defs.md#listkeysoutputtypedef)
- [CreateKeyOutputTypeDef](./type_defs.md#createkeyoutputtypedef)
- [DeleteKeyOutputTypeDef](./type_defs.md#deletekeyoutputtypedef)
- [GetKeyOutputTypeDef](./type_defs.md#getkeyoutputtypedef)
- [ImportKeyOutputTypeDef](./type_defs.md#importkeyoutputtypedef)
- [RestoreKeyOutputTypeDef](./type_defs.md#restorekeyoutputtypedef)
- [StartKeyUsageOutputTypeDef](./type_defs.md#startkeyusageoutputtypedef)
- [StopKeyUsageOutputTypeDef](./type_defs.md#stopkeyusageoutputtypedef)
- [ImportKeyMaterialTypeDef](./type_defs.md#importkeymaterialtypedef)
- [ExportKeyMaterialTypeDef](./type_defs.md#exportkeymaterialtypedef)
- [ImportKeyInputTypeDef](./type_defs.md#importkeyinputtypedef)
- [ExportKeyInputTypeDef](./type_defs.md#exportkeyinputtypedef)

