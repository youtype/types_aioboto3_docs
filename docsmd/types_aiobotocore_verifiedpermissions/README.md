# VerifiedPermissions module

> [Index](../README.md) > VerifiedPermissions


!!! note ""

    Auto-generated documentation for [VerifiedPermissions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#verifiedpermissions)
    type annotations stubs module [types-aiobotocore-verifiedpermissions](https://pypi.org/project/types-aiobotocore-verifiedpermissions/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `VerifiedPermissions` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `VerifiedPermissions` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[verifiedpermissions]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[verifiedpermissions]'

# standalone installation
python -m pip install types-aiobotocore-verifiedpermissions
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-verifiedpermissions
```

## Usage

Code samples can be found in [Examples](./usage.md).

## VerifiedPermissionsClient

Type annotations and code completion for  `#!python session.client("verifiedpermissions")` as [VerifiedPermissionsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Client)

```python
# VerifiedPermissionsClient usage example

from aioboto3.session import Session

from types_aiobotocore_verifiedpermissions.client import VerifiedPermissionsClient


session = Session()
async with session.client("verifiedpermissions") as client:
    client: VerifiedPermissionsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("verifiedpermissions").get_paginator("...")`.

```python
# ListIdentitySourcesPaginator usage example

from types_aiobotocore_verifiedpermissions.paginator import ListIdentitySourcesPaginator

def get_list_identity_sources_paginator() -> ListIdentitySourcesPaginator:
    return client.get_paginator("list_identity_sources"))
```

- [ListIdentitySourcesPaginator](./paginators.md#listidentitysourcespaginator)
- [ListPoliciesPaginator](./paginators.md#listpoliciespaginator)
- [ListPolicyStoresPaginator](./paginators.md#listpolicystorespaginator)
- [ListPolicyTemplatesPaginator](./paginators.md#listpolicytemplatespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BatchGetPolicyErrorCodeType usage example

from types_aiobotocore_verifiedpermissions.literals import BatchGetPolicyErrorCodeType

def get_value() -> BatchGetPolicyErrorCodeType:
    return "POLICY_NOT_FOUND"
```

- [BatchGetPolicyErrorCodeType](./literals.md#batchgetpolicyerrorcodetype)
- [DecisionType](./literals.md#decisiontype)
- [ListIdentitySourcesPaginatorName](./literals.md#listidentitysourcespaginatorname)
- [ListPoliciesPaginatorName](./literals.md#listpoliciespaginatorname)
- [ListPolicyStoresPaginatorName](./literals.md#listpolicystorespaginatorname)
- [ListPolicyTemplatesPaginatorName](./literals.md#listpolicytemplatespaginatorname)
- [OpenIdIssuerType](./literals.md#openidissuertype)
- [PolicyEffectType](./literals.md#policyeffecttype)
- [PolicyTypeType](./literals.md#policytypetype)
- [ValidationModeType](./literals.md#validationmodetype)
- [VerifiedPermissionsServiceName](./literals.md#verifiedpermissionsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ActionIdentifierTypeDef](./type_defs.md#actionidentifiertypedef)
- [EntityIdentifierTypeDef](./type_defs.md#entityidentifiertypedef)
- [BatchGetPolicyErrorItemTypeDef](./type_defs.md#batchgetpolicyerroritemtypedef)
- [BatchGetPolicyInputItemTypeDef](./type_defs.md#batchgetpolicyinputitemtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeterminingPolicyItemTypeDef](./type_defs.md#determiningpolicyitemtypedef)
- [EvaluationErrorItemTypeDef](./type_defs.md#evaluationerroritemtypedef)
- [CognitoGroupConfigurationDetailTypeDef](./type_defs.md#cognitogroupconfigurationdetailtypedef)
- [CognitoGroupConfigurationItemTypeDef](./type_defs.md#cognitogroupconfigurationitemtypedef)
- [CognitoGroupConfigurationTypeDef](./type_defs.md#cognitogroupconfigurationtypedef)
- [ValidationSettingsTypeDef](./type_defs.md#validationsettingstypedef)
- [CreatePolicyTemplateInputRequestTypeDef](./type_defs.md#createpolicytemplateinputrequesttypedef)
- [DeleteIdentitySourceInputRequestTypeDef](./type_defs.md#deleteidentitysourceinputrequesttypedef)
- [DeletePolicyInputRequestTypeDef](./type_defs.md#deletepolicyinputrequesttypedef)
- [DeletePolicyStoreInputRequestTypeDef](./type_defs.md#deletepolicystoreinputrequesttypedef)
- [DeletePolicyTemplateInputRequestTypeDef](./type_defs.md#deletepolicytemplateinputrequesttypedef)
- [GetIdentitySourceInputRequestTypeDef](./type_defs.md#getidentitysourceinputrequesttypedef)
- [IdentitySourceDetailsTypeDef](./type_defs.md#identitysourcedetailstypedef)
- [GetPolicyInputRequestTypeDef](./type_defs.md#getpolicyinputrequesttypedef)
- [GetPolicyStoreInputRequestTypeDef](./type_defs.md#getpolicystoreinputrequesttypedef)
- [GetPolicyTemplateInputRequestTypeDef](./type_defs.md#getpolicytemplateinputrequesttypedef)
- [GetSchemaInputRequestTypeDef](./type_defs.md#getschemainputrequesttypedef)
- [IdentitySourceFilterTypeDef](./type_defs.md#identitysourcefiltertypedef)
- [IdentitySourceItemDetailsTypeDef](./type_defs.md#identitysourceitemdetailstypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListPolicyStoresInputRequestTypeDef](./type_defs.md#listpolicystoresinputrequesttypedef)
- [PolicyStoreItemTypeDef](./type_defs.md#policystoreitemtypedef)
- [ListPolicyTemplatesInputRequestTypeDef](./type_defs.md#listpolicytemplatesinputrequesttypedef)
- [PolicyTemplateItemTypeDef](./type_defs.md#policytemplateitemtypedef)
- [OpenIdConnectAccessTokenConfigurationDetailTypeDef](./type_defs.md#openidconnectaccesstokenconfigurationdetailtypedef)
- [OpenIdConnectAccessTokenConfigurationItemTypeDef](./type_defs.md#openidconnectaccesstokenconfigurationitemtypedef)
- [OpenIdConnectAccessTokenConfigurationTypeDef](./type_defs.md#openidconnectaccesstokenconfigurationtypedef)
- [OpenIdConnectGroupConfigurationDetailTypeDef](./type_defs.md#openidconnectgroupconfigurationdetailtypedef)
- [OpenIdConnectGroupConfigurationItemTypeDef](./type_defs.md#openidconnectgroupconfigurationitemtypedef)
- [OpenIdConnectGroupConfigurationTypeDef](./type_defs.md#openidconnectgroupconfigurationtypedef)
- [OpenIdConnectIdentityTokenConfigurationDetailTypeDef](./type_defs.md#openidconnectidentitytokenconfigurationdetailtypedef)
- [OpenIdConnectIdentityTokenConfigurationItemTypeDef](./type_defs.md#openidconnectidentitytokenconfigurationitemtypedef)
- [OpenIdConnectIdentityTokenConfigurationTypeDef](./type_defs.md#openidconnectidentitytokenconfigurationtypedef)
- [StaticPolicyDefinitionDetailTypeDef](./type_defs.md#staticpolicydefinitiondetailtypedef)
- [StaticPolicyDefinitionItemTypeDef](./type_defs.md#staticpolicydefinitionitemtypedef)
- [StaticPolicyDefinitionTypeDef](./type_defs.md#staticpolicydefinitiontypedef)
- [SchemaDefinitionTypeDef](./type_defs.md#schemadefinitiontypedef)
- [UpdateCognitoGroupConfigurationTypeDef](./type_defs.md#updatecognitogroupconfigurationtypedef)
- [UpdateOpenIdConnectAccessTokenConfigurationTypeDef](./type_defs.md#updateopenidconnectaccesstokenconfigurationtypedef)
- [UpdateOpenIdConnectGroupConfigurationTypeDef](./type_defs.md#updateopenidconnectgroupconfigurationtypedef)
- [UpdateOpenIdConnectIdentityTokenConfigurationTypeDef](./type_defs.md#updateopenidconnectidentitytokenconfigurationtypedef)
- [UpdateStaticPolicyDefinitionTypeDef](./type_defs.md#updatestaticpolicydefinitiontypedef)
- [UpdatePolicyTemplateInputRequestTypeDef](./type_defs.md#updatepolicytemplateinputrequesttypedef)
- [AttributeValueOutputTypeDef](./type_defs.md#attributevalueoutputtypedef)
- [AttributeValueTypeDef](./type_defs.md#attributevaluetypedef)
- [EntityReferenceTypeDef](./type_defs.md#entityreferencetypedef)
- [TemplateLinkedPolicyDefinitionDetailTypeDef](./type_defs.md#templatelinkedpolicydefinitiondetailtypedef)
- [TemplateLinkedPolicyDefinitionItemTypeDef](./type_defs.md#templatelinkedpolicydefinitionitemtypedef)
- [TemplateLinkedPolicyDefinitionTypeDef](./type_defs.md#templatelinkedpolicydefinitiontypedef)
- [BatchGetPolicyInputRequestTypeDef](./type_defs.md#batchgetpolicyinputrequesttypedef)
- [CreateIdentitySourceOutputTypeDef](./type_defs.md#createidentitysourceoutputtypedef)
- [CreatePolicyOutputTypeDef](./type_defs.md#createpolicyoutputtypedef)
- [CreatePolicyStoreOutputTypeDef](./type_defs.md#createpolicystoreoutputtypedef)
- [CreatePolicyTemplateOutputTypeDef](./type_defs.md#createpolicytemplateoutputtypedef)
- [GetPolicyTemplateOutputTypeDef](./type_defs.md#getpolicytemplateoutputtypedef)
- [GetSchemaOutputTypeDef](./type_defs.md#getschemaoutputtypedef)
- [PutSchemaOutputTypeDef](./type_defs.md#putschemaoutputtypedef)
- [UpdateIdentitySourceOutputTypeDef](./type_defs.md#updateidentitysourceoutputtypedef)
- [UpdatePolicyOutputTypeDef](./type_defs.md#updatepolicyoutputtypedef)
- [UpdatePolicyStoreOutputTypeDef](./type_defs.md#updatepolicystoreoutputtypedef)
- [UpdatePolicyTemplateOutputTypeDef](./type_defs.md#updatepolicytemplateoutputtypedef)
- [IsAuthorizedOutputTypeDef](./type_defs.md#isauthorizedoutputtypedef)
- [IsAuthorizedWithTokenOutputTypeDef](./type_defs.md#isauthorizedwithtokenoutputtypedef)
- [CognitoUserPoolConfigurationDetailTypeDef](./type_defs.md#cognitouserpoolconfigurationdetailtypedef)
- [CognitoUserPoolConfigurationItemTypeDef](./type_defs.md#cognitouserpoolconfigurationitemtypedef)
- [CognitoUserPoolConfigurationTypeDef](./type_defs.md#cognitouserpoolconfigurationtypedef)
- [CreatePolicyStoreInputRequestTypeDef](./type_defs.md#createpolicystoreinputrequesttypedef)
- [GetPolicyStoreOutputTypeDef](./type_defs.md#getpolicystoreoutputtypedef)
- [UpdatePolicyStoreInputRequestTypeDef](./type_defs.md#updatepolicystoreinputrequesttypedef)
- [ListIdentitySourcesInputRequestTypeDef](./type_defs.md#listidentitysourcesinputrequesttypedef)
- [ListIdentitySourcesInputPaginateTypeDef](./type_defs.md#listidentitysourcesinputpaginatetypedef)
- [ListPolicyStoresInputPaginateTypeDef](./type_defs.md#listpolicystoresinputpaginatetypedef)
- [ListPolicyTemplatesInputPaginateTypeDef](./type_defs.md#listpolicytemplatesinputpaginatetypedef)
- [ListPolicyStoresOutputTypeDef](./type_defs.md#listpolicystoresoutputtypedef)
- [ListPolicyTemplatesOutputTypeDef](./type_defs.md#listpolicytemplatesoutputtypedef)
- [OpenIdConnectTokenSelectionDetailTypeDef](./type_defs.md#openidconnecttokenselectiondetailtypedef)
- [OpenIdConnectTokenSelectionItemTypeDef](./type_defs.md#openidconnecttokenselectionitemtypedef)
- [OpenIdConnectTokenSelectionTypeDef](./type_defs.md#openidconnecttokenselectiontypedef)
- [PutSchemaInputRequestTypeDef](./type_defs.md#putschemainputrequesttypedef)
- [UpdateCognitoUserPoolConfigurationTypeDef](./type_defs.md#updatecognitouserpoolconfigurationtypedef)
- [UpdateOpenIdConnectTokenSelectionTypeDef](./type_defs.md#updateopenidconnecttokenselectiontypedef)
- [UpdatePolicyDefinitionTypeDef](./type_defs.md#updatepolicydefinitiontypedef)
- [ContextDefinitionOutputTypeDef](./type_defs.md#contextdefinitionoutputtypedef)
- [AttributeValueUnionTypeDef](./type_defs.md#attributevalueuniontypedef)
- [PolicyFilterTypeDef](./type_defs.md#policyfiltertypedef)
- [PolicyDefinitionDetailTypeDef](./type_defs.md#policydefinitiondetailtypedef)
- [PolicyDefinitionItemTypeDef](./type_defs.md#policydefinitionitemtypedef)
- [PolicyDefinitionTypeDef](./type_defs.md#policydefinitiontypedef)
- [OpenIdConnectConfigurationDetailTypeDef](./type_defs.md#openidconnectconfigurationdetailtypedef)
- [OpenIdConnectConfigurationItemTypeDef](./type_defs.md#openidconnectconfigurationitemtypedef)
- [OpenIdConnectConfigurationTypeDef](./type_defs.md#openidconnectconfigurationtypedef)
- [UpdateOpenIdConnectConfigurationTypeDef](./type_defs.md#updateopenidconnectconfigurationtypedef)
- [UpdatePolicyInputRequestTypeDef](./type_defs.md#updatepolicyinputrequesttypedef)
- [BatchIsAuthorizedInputItemOutputTypeDef](./type_defs.md#batchisauthorizedinputitemoutputtypedef)
- [BatchIsAuthorizedWithTokenInputItemOutputTypeDef](./type_defs.md#batchisauthorizedwithtokeninputitemoutputtypedef)
- [ContextDefinitionTypeDef](./type_defs.md#contextdefinitiontypedef)
- [EntityItemTypeDef](./type_defs.md#entityitemtypedef)
- [ListPoliciesInputPaginateTypeDef](./type_defs.md#listpoliciesinputpaginatetypedef)
- [ListPoliciesInputRequestTypeDef](./type_defs.md#listpoliciesinputrequesttypedef)
- [BatchGetPolicyOutputItemTypeDef](./type_defs.md#batchgetpolicyoutputitemtypedef)
- [GetPolicyOutputTypeDef](./type_defs.md#getpolicyoutputtypedef)
- [PolicyItemTypeDef](./type_defs.md#policyitemtypedef)
- [CreatePolicyInputRequestTypeDef](./type_defs.md#createpolicyinputrequesttypedef)
- [ConfigurationDetailTypeDef](./type_defs.md#configurationdetailtypedef)
- [ConfigurationItemTypeDef](./type_defs.md#configurationitemtypedef)
- [ConfigurationTypeDef](./type_defs.md#configurationtypedef)
- [UpdateConfigurationTypeDef](./type_defs.md#updateconfigurationtypedef)
- [BatchIsAuthorizedOutputItemTypeDef](./type_defs.md#batchisauthorizedoutputitemtypedef)
- [BatchIsAuthorizedWithTokenOutputItemTypeDef](./type_defs.md#batchisauthorizedwithtokenoutputitemtypedef)
- [ContextDefinitionUnionTypeDef](./type_defs.md#contextdefinitionuniontypedef)
- [EntitiesDefinitionTypeDef](./type_defs.md#entitiesdefinitiontypedef)
- [BatchGetPolicyOutputTypeDef](./type_defs.md#batchgetpolicyoutputtypedef)
- [ListPoliciesOutputTypeDef](./type_defs.md#listpoliciesoutputtypedef)
- [GetIdentitySourceOutputTypeDef](./type_defs.md#getidentitysourceoutputtypedef)
- [IdentitySourceItemTypeDef](./type_defs.md#identitysourceitemtypedef)
- [CreateIdentitySourceInputRequestTypeDef](./type_defs.md#createidentitysourceinputrequesttypedef)
- [UpdateIdentitySourceInputRequestTypeDef](./type_defs.md#updateidentitysourceinputrequesttypedef)
- [BatchIsAuthorizedOutputTypeDef](./type_defs.md#batchisauthorizedoutputtypedef)
- [BatchIsAuthorizedWithTokenOutputTypeDef](./type_defs.md#batchisauthorizedwithtokenoutputtypedef)
- [BatchIsAuthorizedInputItemTypeDef](./type_defs.md#batchisauthorizedinputitemtypedef)
- [BatchIsAuthorizedWithTokenInputItemTypeDef](./type_defs.md#batchisauthorizedwithtokeninputitemtypedef)
- [IsAuthorizedInputRequestTypeDef](./type_defs.md#isauthorizedinputrequesttypedef)
- [IsAuthorizedWithTokenInputRequestTypeDef](./type_defs.md#isauthorizedwithtokeninputrequesttypedef)
- [ListIdentitySourcesOutputTypeDef](./type_defs.md#listidentitysourcesoutputtypedef)
- [BatchIsAuthorizedInputItemUnionTypeDef](./type_defs.md#batchisauthorizedinputitemuniontypedef)
- [BatchIsAuthorizedWithTokenInputItemUnionTypeDef](./type_defs.md#batchisauthorizedwithtokeninputitemuniontypedef)
- [BatchIsAuthorizedInputRequestTypeDef](./type_defs.md#batchisauthorizedinputrequesttypedef)
- [BatchIsAuthorizedWithTokenInputRequestTypeDef](./type_defs.md#batchisauthorizedwithtokeninputrequesttypedef)
