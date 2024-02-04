# DataZoneClient

> [Index](../README.md) > [DataZone](./README.md) > DataZoneClient

!!! note ""

    Auto-generated documentation for [DataZone](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
    type annotations stubs module [types-aiobotocore-datazone](https://pypi.org/project/types-aiobotocore-datazone/).

## DataZoneClient

Type annotations and code completion for `#!python session.client("datazone")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client)

```python
# DataZoneClient usage example

from aioboto3.session import Session
from types_aiobotocore_datazone.client import DataZoneClient

session = Session()
async with session.client("datazone") as client:
    client: DataZoneClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("datazone").exceptions` structure.

```python
# DataZoneClient.exceptions usage example

async with session.client("datazone") as client:
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
        client.exceptions.UnauthorizedException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# DataZoneClient.exceptions type checking example

from types_aiobotocore_datazone.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### accept\_predictions

Accepts automatically generated business-friendly metadata for your Amazon
DataZone
assets.

Type annotations and code completion for `#!python session.client("datazone").accept_predictions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.accept_predictions)

```python
# accept_predictions method definition

await def accept_predictions(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    acceptChoices: Sequence[AcceptChoiceTypeDef] = ...,  # (1)
    acceptRule: AcceptRuleTypeDef = ...,  # (2)
    clientToken: str = ...,
    revision: str = ...,
) -> AcceptPredictionsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AcceptChoiceTypeDef](./type_defs.md#acceptchoicetypedef) 
2. See [:material-code-braces: AcceptRuleTypeDef](./type_defs.md#acceptruletypedef) 
3. See [:material-code-braces: AcceptPredictionsOutputTypeDef](./type_defs.md#acceptpredictionsoutputtypedef) 


```python
# accept_predictions method usage example with argument unpacking

kwargs: AcceptPredictionsInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.accept_predictions(**kwargs)
```

1. See [:material-code-braces: AcceptPredictionsInputRequestTypeDef](./type_defs.md#acceptpredictionsinputrequesttypedef) 

### accept\_subscription\_request

Accepts a subscription request to a specific asset.

Type annotations and code completion for `#!python session.client("datazone").accept_subscription_request` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.accept_subscription_request)

```python
# accept_subscription_request method definition

await def accept_subscription_request(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    decisionComment: str = ...,
) -> AcceptSubscriptionRequestOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AcceptSubscriptionRequestOutputTypeDef](./type_defs.md#acceptsubscriptionrequestoutputtypedef) 


```python
# accept_subscription_request method usage example with argument unpacking

kwargs: AcceptSubscriptionRequestInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.accept_subscription_request(**kwargs)
```

1. See [:material-code-braces: AcceptSubscriptionRequestInputRequestTypeDef](./type_defs.md#acceptsubscriptionrequestinputrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.client("datazone").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_subscription

Cancels the subscription to the specified asset.

Type annotations and code completion for `#!python session.client("datazone").cancel_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.cancel_subscription)

```python
# cancel_subscription method definition

await def cancel_subscription(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> CancelSubscriptionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelSubscriptionOutputTypeDef](./type_defs.md#cancelsubscriptionoutputtypedef) 


```python
# cancel_subscription method usage example with argument unpacking

kwargs: CancelSubscriptionInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.cancel_subscription(**kwargs)
```

1. See [:material-code-braces: CancelSubscriptionInputRequestTypeDef](./type_defs.md#cancelsubscriptioninputrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.client("datazone").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_asset

Creates an asset in Amazon DataZone catalog.

Type annotations and code completion for `#!python session.client("datazone").create_asset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_asset)

```python
# create_asset method definition

await def create_asset(
    self,
    *,
    domainIdentifier: str,
    name: str,
    owningProjectIdentifier: str,
    typeIdentifier: str,
    clientToken: str = ...,
    description: str = ...,
    externalIdentifier: str = ...,
    formsInput: Sequence[FormInputTypeDef] = ...,  # (1)
    glossaryTerms: Sequence[str] = ...,
    predictionConfiguration: PredictionConfigurationTypeDef = ...,  # (2)
    typeRevision: str = ...,
) -> CreateAssetOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FormInputTypeDef](./type_defs.md#forminputtypedef) 
2. See [:material-code-braces: PredictionConfigurationTypeDef](./type_defs.md#predictionconfigurationtypedef) 
3. See [:material-code-braces: CreateAssetOutputTypeDef](./type_defs.md#createassetoutputtypedef) 


```python
# create_asset method usage example with argument unpacking

kwargs: CreateAssetInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "name": ...,
    "owningProjectIdentifier": ...,
    "typeIdentifier": ...,
}

parent.create_asset(**kwargs)
```

1. See [:material-code-braces: CreateAssetInputRequestTypeDef](./type_defs.md#createassetinputrequesttypedef) 

### create\_asset\_revision

Creates a revision of the asset.

Type annotations and code completion for `#!python session.client("datazone").create_asset_revision` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_asset_revision)

```python
# create_asset_revision method definition

await def create_asset_revision(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    name: str,
    clientToken: str = ...,
    description: str = ...,
    formsInput: Sequence[FormInputTypeDef] = ...,  # (1)
    glossaryTerms: Sequence[str] = ...,
    predictionConfiguration: PredictionConfigurationTypeDef = ...,  # (2)
    typeRevision: str = ...,
) -> CreateAssetRevisionOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FormInputTypeDef](./type_defs.md#forminputtypedef) 
2. See [:material-code-braces: PredictionConfigurationTypeDef](./type_defs.md#predictionconfigurationtypedef) 
3. See [:material-code-braces: CreateAssetRevisionOutputTypeDef](./type_defs.md#createassetrevisionoutputtypedef) 


```python
# create_asset_revision method usage example with argument unpacking

kwargs: CreateAssetRevisionInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
    "name": ...,
}

parent.create_asset_revision(**kwargs)
```

1. See [:material-code-braces: CreateAssetRevisionInputRequestTypeDef](./type_defs.md#createassetrevisioninputrequesttypedef) 

### create\_asset\_type

Creates a custom asset type.

Type annotations and code completion for `#!python session.client("datazone").create_asset_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_asset_type)

```python
# create_asset_type method definition

await def create_asset_type(
    self,
    *,
    domainIdentifier: str,
    formsInput: Mapping[str, FormEntryInputTypeDef],  # (1)
    name: str,
    owningProjectIdentifier: str,
    description: str = ...,
) -> CreateAssetTypeOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FormEntryInputTypeDef](./type_defs.md#formentryinputtypedef) 
2. See [:material-code-braces: CreateAssetTypeOutputTypeDef](./type_defs.md#createassettypeoutputtypedef) 


```python
# create_asset_type method usage example with argument unpacking

kwargs: CreateAssetTypeInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "formsInput": ...,
    "name": ...,
    "owningProjectIdentifier": ...,
}

parent.create_asset_type(**kwargs)
```

1. See [:material-code-braces: CreateAssetTypeInputRequestTypeDef](./type_defs.md#createassettypeinputrequesttypedef) 

### create\_data\_source

Creates an Amazon DataZone data source.

Type annotations and code completion for `#!python session.client("datazone").create_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_data_source)

```python
# create_data_source method definition

await def create_data_source(
    self,
    *,
    domainIdentifier: str,
    environmentIdentifier: str,
    name: str,
    projectIdentifier: str,
    type: str,
    assetFormsInput: Sequence[FormInputTypeDef] = ...,  # (1)
    clientToken: str = ...,
    configuration: DataSourceConfigurationInputTypeDef = ...,  # (2)
    description: str = ...,
    enableSetting: EnableSettingType = ...,  # (3)
    publishOnImport: bool = ...,
    recommendation: RecommendationConfigurationTypeDef = ...,  # (4)
    schedule: ScheduleConfigurationTypeDef = ...,  # (5)
) -> CreateDataSourceOutputTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: FormInputTypeDef](./type_defs.md#forminputtypedef) 
2. See [:material-code-braces: DataSourceConfigurationInputTypeDef](./type_defs.md#datasourceconfigurationinputtypedef) 
3. See [:material-code-brackets: EnableSettingType](./literals.md#enablesettingtype) 
4. See [:material-code-braces: RecommendationConfigurationTypeDef](./type_defs.md#recommendationconfigurationtypedef) 
5. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
6. See [:material-code-braces: CreateDataSourceOutputTypeDef](./type_defs.md#createdatasourceoutputtypedef) 


```python
# create_data_source method usage example with argument unpacking

kwargs: CreateDataSourceInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "environmentIdentifier": ...,
    "name": ...,
    "projectIdentifier": ...,
    "type": ...,
}

parent.create_data_source(**kwargs)
```

1. See [:material-code-braces: CreateDataSourceInputRequestTypeDef](./type_defs.md#createdatasourceinputrequesttypedef) 

### create\_domain

Creates an Amazon DataZone domain.

Type annotations and code completion for `#!python session.client("datazone").create_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_domain)

```python
# create_domain method definition

await def create_domain(
    self,
    *,
    domainExecutionRole: str,
    name: str,
    clientToken: str = ...,
    description: str = ...,
    kmsKeyIdentifier: str = ...,
    singleSignOn: SingleSignOnTypeDef = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> CreateDomainOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SingleSignOnTypeDef](./type_defs.md#singlesignontypedef) 
2. See [:material-code-braces: CreateDomainOutputTypeDef](./type_defs.md#createdomainoutputtypedef) 


```python
# create_domain method usage example with argument unpacking

kwargs: CreateDomainInputRequestTypeDef = {  # (1)
    "domainExecutionRole": ...,
    "name": ...,
}

parent.create_domain(**kwargs)
```

1. See [:material-code-braces: CreateDomainInputRequestTypeDef](./type_defs.md#createdomaininputrequesttypedef) 

### create\_environment

Create an Amazon DataZone environment.

Type annotations and code completion for `#!python session.client("datazone").create_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_environment)

```python
# create_environment method definition

await def create_environment(
    self,
    *,
    domainIdentifier: str,
    environmentProfileIdentifier: str,
    name: str,
    projectIdentifier: str,
    description: str = ...,
    glossaryTerms: Sequence[str] = ...,
    userParameters: Sequence[EnvironmentParameterTypeDef] = ...,  # (1)
) -> CreateEnvironmentOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EnvironmentParameterTypeDef](./type_defs.md#environmentparametertypedef) 
2. See [:material-code-braces: CreateEnvironmentOutputTypeDef](./type_defs.md#createenvironmentoutputtypedef) 


```python
# create_environment method usage example with argument unpacking

kwargs: CreateEnvironmentInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "environmentProfileIdentifier": ...,
    "name": ...,
    "projectIdentifier": ...,
}

parent.create_environment(**kwargs)
```

1. See [:material-code-braces: CreateEnvironmentInputRequestTypeDef](./type_defs.md#createenvironmentinputrequesttypedef) 

### create\_environment\_profile

Creates an Amazon DataZone environment profile.

Type annotations and code completion for `#!python session.client("datazone").create_environment_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_environment_profile)

```python
# create_environment_profile method definition

await def create_environment_profile(
    self,
    *,
    domainIdentifier: str,
    environmentBlueprintIdentifier: str,
    name: str,
    projectIdentifier: str,
    awsAccountId: str = ...,
    awsAccountRegion: str = ...,
    description: str = ...,
    userParameters: Sequence[EnvironmentParameterTypeDef] = ...,  # (1)
) -> CreateEnvironmentProfileOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EnvironmentParameterTypeDef](./type_defs.md#environmentparametertypedef) 
2. See [:material-code-braces: CreateEnvironmentProfileOutputTypeDef](./type_defs.md#createenvironmentprofileoutputtypedef) 


```python
# create_environment_profile method usage example with argument unpacking

kwargs: CreateEnvironmentProfileInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "environmentBlueprintIdentifier": ...,
    "name": ...,
    "projectIdentifier": ...,
}

parent.create_environment_profile(**kwargs)
```

1. See [:material-code-braces: CreateEnvironmentProfileInputRequestTypeDef](./type_defs.md#createenvironmentprofileinputrequesttypedef) 

### create\_form\_type

Creates a metadata form type.

Type annotations and code completion for `#!python session.client("datazone").create_form_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_form_type)

```python
# create_form_type method definition

await def create_form_type(
    self,
    *,
    domainIdentifier: str,
    model: ModelTypeDef,  # (1)
    name: str,
    owningProjectIdentifier: str,
    description: str = ...,
    status: FormTypeStatusType = ...,  # (2)
) -> CreateFormTypeOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ModelTypeDef](./type_defs.md#modeltypedef) 
2. See [:material-code-brackets: FormTypeStatusType](./literals.md#formtypestatustype) 
3. See [:material-code-braces: CreateFormTypeOutputTypeDef](./type_defs.md#createformtypeoutputtypedef) 


```python
# create_form_type method usage example with argument unpacking

kwargs: CreateFormTypeInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "model": ...,
    "name": ...,
    "owningProjectIdentifier": ...,
}

parent.create_form_type(**kwargs)
```

1. See [:material-code-braces: CreateFormTypeInputRequestTypeDef](./type_defs.md#createformtypeinputrequesttypedef) 

### create\_glossary

Creates an Amazon DataZone business glossary.

Type annotations and code completion for `#!python session.client("datazone").create_glossary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_glossary)

```python
# create_glossary method definition

await def create_glossary(
    self,
    *,
    domainIdentifier: str,
    name: str,
    owningProjectIdentifier: str,
    clientToken: str = ...,
    description: str = ...,
    status: GlossaryStatusType = ...,  # (1)
) -> CreateGlossaryOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: GlossaryStatusType](./literals.md#glossarystatustype) 
2. See [:material-code-braces: CreateGlossaryOutputTypeDef](./type_defs.md#createglossaryoutputtypedef) 


```python
# create_glossary method usage example with argument unpacking

kwargs: CreateGlossaryInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "name": ...,
    "owningProjectIdentifier": ...,
}

parent.create_glossary(**kwargs)
```

1. See [:material-code-braces: CreateGlossaryInputRequestTypeDef](./type_defs.md#createglossaryinputrequesttypedef) 

### create\_glossary\_term

Creates a business glossary term.

Type annotations and code completion for `#!python session.client("datazone").create_glossary_term` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_glossary_term)

```python
# create_glossary_term method definition

await def create_glossary_term(
    self,
    *,
    domainIdentifier: str,
    glossaryIdentifier: str,
    name: str,
    clientToken: str = ...,
    longDescription: str = ...,
    shortDescription: str = ...,
    status: GlossaryTermStatusType = ...,  # (1)
    termRelations: TermRelationsTypeDef = ...,  # (2)
) -> CreateGlossaryTermOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: GlossaryTermStatusType](./literals.md#glossarytermstatustype) 
2. See [:material-code-braces: TermRelationsTypeDef](./type_defs.md#termrelationstypedef) 
3. See [:material-code-braces: CreateGlossaryTermOutputTypeDef](./type_defs.md#createglossarytermoutputtypedef) 


```python
# create_glossary_term method usage example with argument unpacking

kwargs: CreateGlossaryTermInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "glossaryIdentifier": ...,
    "name": ...,
}

parent.create_glossary_term(**kwargs)
```

1. See [:material-code-braces: CreateGlossaryTermInputRequestTypeDef](./type_defs.md#createglossaryterminputrequesttypedef) 

### create\_group\_profile

Creates a group profile in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").create_group_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_group_profile)

```python
# create_group_profile method definition

await def create_group_profile(
    self,
    *,
    domainIdentifier: str,
    groupIdentifier: str,
    clientToken: str = ...,
) -> CreateGroupProfileOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateGroupProfileOutputTypeDef](./type_defs.md#creategroupprofileoutputtypedef) 


```python
# create_group_profile method usage example with argument unpacking

kwargs: CreateGroupProfileInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "groupIdentifier": ...,
}

parent.create_group_profile(**kwargs)
```

1. See [:material-code-braces: CreateGroupProfileInputRequestTypeDef](./type_defs.md#creategroupprofileinputrequesttypedef) 

### create\_listing\_change\_set

See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/datazone-2018-05-10/CreateListingChangeSet).

Type annotations and code completion for `#!python session.client("datazone").create_listing_change_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_listing_change_set)

```python
# create_listing_change_set method definition

await def create_listing_change_set(
    self,
    *,
    action: ChangeActionType,  # (1)
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: EntityTypeType,  # (2)
    clientToken: str = ...,
    entityRevision: str = ...,
) -> CreateListingChangeSetOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
3. See [:material-code-braces: CreateListingChangeSetOutputTypeDef](./type_defs.md#createlistingchangesetoutputtypedef) 


```python
# create_listing_change_set method usage example with argument unpacking

kwargs: CreateListingChangeSetInputRequestTypeDef = {  # (1)
    "action": ...,
    "domainIdentifier": ...,
    "entityIdentifier": ...,
    "entityType": ...,
}

parent.create_listing_change_set(**kwargs)
```

1. See [:material-code-braces: CreateListingChangeSetInputRequestTypeDef](./type_defs.md#createlistingchangesetinputrequesttypedef) 

### create\_project

Creates an Amazon DataZone project.

Type annotations and code completion for `#!python session.client("datazone").create_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_project)

```python
# create_project method definition

await def create_project(
    self,
    *,
    domainIdentifier: str,
    name: str,
    description: str = ...,
    glossaryTerms: Sequence[str] = ...,
) -> CreateProjectOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateProjectOutputTypeDef](./type_defs.md#createprojectoutputtypedef) 


```python
# create_project method usage example with argument unpacking

kwargs: CreateProjectInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "name": ...,
}

parent.create_project(**kwargs)
```

1. See [:material-code-braces: CreateProjectInputRequestTypeDef](./type_defs.md#createprojectinputrequesttypedef) 

### create\_project\_membership

Creates a project membership in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").create_project_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_project_membership)

```python
# create_project_membership method definition

await def create_project_membership(
    self,
    *,
    designation: UserDesignationType,  # (1)
    domainIdentifier: str,
    member: MemberTypeDef,  # (2)
    projectIdentifier: str,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: UserDesignationType](./literals.md#userdesignationtype) 
2. See [:material-code-braces: MemberTypeDef](./type_defs.md#membertypedef) 


```python
# create_project_membership method usage example with argument unpacking

kwargs: CreateProjectMembershipInputRequestTypeDef = {  # (1)
    "designation": ...,
    "domainIdentifier": ...,
    "member": ...,
    "projectIdentifier": ...,
}

parent.create_project_membership(**kwargs)
```

1. See [:material-code-braces: CreateProjectMembershipInputRequestTypeDef](./type_defs.md#createprojectmembershipinputrequesttypedef) 

### create\_subscription\_grant

Creates a subsscription grant in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").create_subscription_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_subscription_grant)

```python
# create_subscription_grant method definition

await def create_subscription_grant(
    self,
    *,
    domainIdentifier: str,
    environmentIdentifier: str,
    grantedEntity: GrantedEntityInputTypeDef,  # (1)
    subscriptionTargetIdentifier: str,
    assetTargetNames: Sequence[AssetTargetNameMapTypeDef] = ...,  # (2)
    clientToken: str = ...,
) -> CreateSubscriptionGrantOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: GrantedEntityInputTypeDef](./type_defs.md#grantedentityinputtypedef) 
2. See [:material-code-braces: AssetTargetNameMapTypeDef](./type_defs.md#assettargetnamemaptypedef) 
3. See [:material-code-braces: CreateSubscriptionGrantOutputTypeDef](./type_defs.md#createsubscriptiongrantoutputtypedef) 


```python
# create_subscription_grant method usage example with argument unpacking

kwargs: CreateSubscriptionGrantInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "environmentIdentifier": ...,
    "grantedEntity": ...,
    "subscriptionTargetIdentifier": ...,
}

parent.create_subscription_grant(**kwargs)
```

1. See [:material-code-braces: CreateSubscriptionGrantInputRequestTypeDef](./type_defs.md#createsubscriptiongrantinputrequesttypedef) 

### create\_subscription\_request

Creates a subscription request in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").create_subscription_request` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_subscription_request)

```python
# create_subscription_request method definition

await def create_subscription_request(
    self,
    *,
    domainIdentifier: str,
    requestReason: str,
    subscribedListings: Sequence[SubscribedListingInputTypeDef],  # (1)
    subscribedPrincipals: Sequence[SubscribedPrincipalInputTypeDef],  # (2)
    clientToken: str = ...,
) -> CreateSubscriptionRequestOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SubscribedListingInputTypeDef](./type_defs.md#subscribedlistinginputtypedef) 
2. See [:material-code-braces: SubscribedPrincipalInputTypeDef](./type_defs.md#subscribedprincipalinputtypedef) 
3. See [:material-code-braces: CreateSubscriptionRequestOutputTypeDef](./type_defs.md#createsubscriptionrequestoutputtypedef) 


```python
# create_subscription_request method usage example with argument unpacking

kwargs: CreateSubscriptionRequestInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "requestReason": ...,
    "subscribedListings": ...,
    "subscribedPrincipals": ...,
}

parent.create_subscription_request(**kwargs)
```

1. See [:material-code-braces: CreateSubscriptionRequestInputRequestTypeDef](./type_defs.md#createsubscriptionrequestinputrequesttypedef) 

### create\_subscription\_target

Creates a subscription target in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").create_subscription_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_subscription_target)

```python
# create_subscription_target method definition

await def create_subscription_target(
    self,
    *,
    applicableAssetTypes: Sequence[str],
    authorizedPrincipals: Sequence[str],
    domainIdentifier: str,
    environmentIdentifier: str,
    manageAccessRole: str,
    name: str,
    subscriptionTargetConfig: Sequence[SubscriptionTargetFormTypeDef],  # (1)
    type: str,
    clientToken: str = ...,
    provider: str = ...,
) -> CreateSubscriptionTargetOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SubscriptionTargetFormTypeDef](./type_defs.md#subscriptiontargetformtypedef) 
2. See [:material-code-braces: CreateSubscriptionTargetOutputTypeDef](./type_defs.md#createsubscriptiontargetoutputtypedef) 


```python
# create_subscription_target method usage example with argument unpacking

kwargs: CreateSubscriptionTargetInputRequestTypeDef = {  # (1)
    "applicableAssetTypes": ...,
    "authorizedPrincipals": ...,
    "domainIdentifier": ...,
    "environmentIdentifier": ...,
    "manageAccessRole": ...,
    "name": ...,
    "subscriptionTargetConfig": ...,
    "type": ...,
}

parent.create_subscription_target(**kwargs)
```

1. See [:material-code-braces: CreateSubscriptionTargetInputRequestTypeDef](./type_defs.md#createsubscriptiontargetinputrequesttypedef) 

### create\_user\_profile

Creates a user profile in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").create_user_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_user_profile)

```python
# create_user_profile method definition

await def create_user_profile(
    self,
    *,
    domainIdentifier: str,
    userIdentifier: str,
    clientToken: str = ...,
    userType: UserTypeType = ...,  # (1)
) -> CreateUserProfileOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
2. See [:material-code-braces: CreateUserProfileOutputTypeDef](./type_defs.md#createuserprofileoutputtypedef) 


```python
# create_user_profile method usage example with argument unpacking

kwargs: CreateUserProfileInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "userIdentifier": ...,
}

parent.create_user_profile(**kwargs)
```

1. See [:material-code-braces: CreateUserProfileInputRequestTypeDef](./type_defs.md#createuserprofileinputrequesttypedef) 

### delete\_asset

Delets an asset in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").delete_asset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_asset)

```python
# delete_asset method definition

await def delete_asset(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_asset method usage example with argument unpacking

kwargs: DeleteAssetInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.delete_asset(**kwargs)
```

1. See [:material-code-braces: DeleteAssetInputRequestTypeDef](./type_defs.md#deleteassetinputrequesttypedef) 

### delete\_asset\_type

Deletes an asset type in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").delete_asset_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_asset_type)

```python
# delete_asset_type method definition

await def delete_asset_type(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_asset_type method usage example with argument unpacking

kwargs: DeleteAssetTypeInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.delete_asset_type(**kwargs)
```

1. See [:material-code-braces: DeleteAssetTypeInputRequestTypeDef](./type_defs.md#deleteassettypeinputrequesttypedef) 

### delete\_data\_source

Deletes a data source in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").delete_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_data_source)

```python
# delete_data_source method definition

await def delete_data_source(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    clientToken: str = ...,
) -> DeleteDataSourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDataSourceOutputTypeDef](./type_defs.md#deletedatasourceoutputtypedef) 


```python
# delete_data_source method usage example with argument unpacking

kwargs: DeleteDataSourceInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.delete_data_source(**kwargs)
```

1. See [:material-code-braces: DeleteDataSourceInputRequestTypeDef](./type_defs.md#deletedatasourceinputrequesttypedef) 

### delete\_domain

Deletes a Amazon DataZone domain.

Type annotations and code completion for `#!python session.client("datazone").delete_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_domain)

```python
# delete_domain method definition

await def delete_domain(
    self,
    *,
    identifier: str,
    clientToken: str = ...,
    skipDeletionCheck: bool = ...,
) -> DeleteDomainOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDomainOutputTypeDef](./type_defs.md#deletedomainoutputtypedef) 


```python
# delete_domain method usage example with argument unpacking

kwargs: DeleteDomainInputRequestTypeDef = {  # (1)
    "identifier": ...,
}

parent.delete_domain(**kwargs)
```

1. See [:material-code-braces: DeleteDomainInputRequestTypeDef](./type_defs.md#deletedomaininputrequesttypedef) 

### delete\_environment

Deletes an environment in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").delete_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_environment)

```python
# delete_environment method definition

await def delete_environment(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_environment method usage example with argument unpacking

kwargs: DeleteEnvironmentInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.delete_environment(**kwargs)
```

1. See [:material-code-braces: DeleteEnvironmentInputRequestTypeDef](./type_defs.md#deleteenvironmentinputrequesttypedef) 

### delete\_environment\_blueprint\_configuration

Deletes the blueprint configuration in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").delete_environment_blueprint_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_environment_blueprint_configuration)

```python
# delete_environment_blueprint_configuration method definition

await def delete_environment_blueprint_configuration(
    self,
    *,
    domainIdentifier: str,
    environmentBlueprintIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_environment_blueprint_configuration method usage example with argument unpacking

kwargs: DeleteEnvironmentBlueprintConfigurationInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "environmentBlueprintIdentifier": ...,
}

parent.delete_environment_blueprint_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteEnvironmentBlueprintConfigurationInputRequestTypeDef](./type_defs.md#deleteenvironmentblueprintconfigurationinputrequesttypedef) 

### delete\_environment\_profile

Deletes an environment profile in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").delete_environment_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_environment_profile)

```python
# delete_environment_profile method definition

await def delete_environment_profile(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_environment_profile method usage example with argument unpacking

kwargs: DeleteEnvironmentProfileInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.delete_environment_profile(**kwargs)
```

1. See [:material-code-braces: DeleteEnvironmentProfileInputRequestTypeDef](./type_defs.md#deleteenvironmentprofileinputrequesttypedef) 

### delete\_form\_type

Delets and metadata form type in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").delete_form_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_form_type)

```python
# delete_form_type method definition

await def delete_form_type(
    self,
    *,
    domainIdentifier: str,
    formTypeIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_form_type method usage example with argument unpacking

kwargs: DeleteFormTypeInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "formTypeIdentifier": ...,
}

parent.delete_form_type(**kwargs)
```

1. See [:material-code-braces: DeleteFormTypeInputRequestTypeDef](./type_defs.md#deleteformtypeinputrequesttypedef) 

### delete\_glossary

Deletes a business glossary in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").delete_glossary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_glossary)

```python
# delete_glossary method definition

await def delete_glossary(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_glossary method usage example with argument unpacking

kwargs: DeleteGlossaryInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.delete_glossary(**kwargs)
```

1. See [:material-code-braces: DeleteGlossaryInputRequestTypeDef](./type_defs.md#deleteglossaryinputrequesttypedef) 

### delete\_glossary\_term

Deletes a business glossary term in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").delete_glossary_term` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_glossary_term)

```python
# delete_glossary_term method definition

await def delete_glossary_term(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_glossary_term method usage example with argument unpacking

kwargs: DeleteGlossaryTermInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.delete_glossary_term(**kwargs)
```

1. See [:material-code-braces: DeleteGlossaryTermInputRequestTypeDef](./type_defs.md#deleteglossaryterminputrequesttypedef) 

### delete\_listing

See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/datazone-2018-05-10/DeleteListing).

Type annotations and code completion for `#!python session.client("datazone").delete_listing` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_listing)

```python
# delete_listing method definition

await def delete_listing(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_listing method usage example with argument unpacking

kwargs: DeleteListingInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.delete_listing(**kwargs)
```

1. See [:material-code-braces: DeleteListingInputRequestTypeDef](./type_defs.md#deletelistinginputrequesttypedef) 

### delete\_project

Deletes a project in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").delete_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_project)

```python
# delete_project method definition

await def delete_project(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    skipDeletionCheck: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_project method usage example with argument unpacking

kwargs: DeleteProjectInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.delete_project(**kwargs)
```

1. See [:material-code-braces: DeleteProjectInputRequestTypeDef](./type_defs.md#deleteprojectinputrequesttypedef) 

### delete\_project\_membership

Deletes project membership in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").delete_project_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_project_membership)

```python
# delete_project_membership method definition

await def delete_project_membership(
    self,
    *,
    domainIdentifier: str,
    member: MemberTypeDef,  # (1)
    projectIdentifier: str,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: MemberTypeDef](./type_defs.md#membertypedef) 


```python
# delete_project_membership method usage example with argument unpacking

kwargs: DeleteProjectMembershipInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "member": ...,
    "projectIdentifier": ...,
}

parent.delete_project_membership(**kwargs)
```

1. See [:material-code-braces: DeleteProjectMembershipInputRequestTypeDef](./type_defs.md#deleteprojectmembershipinputrequesttypedef) 

### delete\_subscription\_grant

Deletes and subscription grant in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").delete_subscription_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_subscription_grant)

```python
# delete_subscription_grant method definition

await def delete_subscription_grant(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> DeleteSubscriptionGrantOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteSubscriptionGrantOutputTypeDef](./type_defs.md#deletesubscriptiongrantoutputtypedef) 


```python
# delete_subscription_grant method usage example with argument unpacking

kwargs: DeleteSubscriptionGrantInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.delete_subscription_grant(**kwargs)
```

1. See [:material-code-braces: DeleteSubscriptionGrantInputRequestTypeDef](./type_defs.md#deletesubscriptiongrantinputrequesttypedef) 

### delete\_subscription\_request

Deletes a subscription request in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").delete_subscription_request` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_subscription_request)

```python
# delete_subscription_request method definition

await def delete_subscription_request(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_subscription_request method usage example with argument unpacking

kwargs: DeleteSubscriptionRequestInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.delete_subscription_request(**kwargs)
```

1. See [:material-code-braces: DeleteSubscriptionRequestInputRequestTypeDef](./type_defs.md#deletesubscriptionrequestinputrequesttypedef) 

### delete\_subscription\_target

Deletes a subscription target in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").delete_subscription_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_subscription_target)

```python
# delete_subscription_target method definition

await def delete_subscription_target(
    self,
    *,
    domainIdentifier: str,
    environmentIdentifier: str,
    identifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_subscription_target method usage example with argument unpacking

kwargs: DeleteSubscriptionTargetInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "environmentIdentifier": ...,
    "identifier": ...,
}

parent.delete_subscription_target(**kwargs)
```

1. See [:material-code-braces: DeleteSubscriptionTargetInputRequestTypeDef](./type_defs.md#deletesubscriptiontargetinputrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.client("datazone").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.generate_presigned_url)

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


### get\_asset

Gets an Amazon DataZone asset.

Type annotations and code completion for `#!python session.client("datazone").get_asset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_asset)

```python
# get_asset method definition

await def get_asset(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    revision: str = ...,
) -> GetAssetOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAssetOutputTypeDef](./type_defs.md#getassetoutputtypedef) 


```python
# get_asset method usage example with argument unpacking

kwargs: GetAssetInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.get_asset(**kwargs)
```

1. See [:material-code-braces: GetAssetInputRequestTypeDef](./type_defs.md#getassetinputrequesttypedef) 

### get\_asset\_type

Gets an Amazon DataZone asset type.

Type annotations and code completion for `#!python session.client("datazone").get_asset_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_asset_type)

```python
# get_asset_type method definition

await def get_asset_type(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    revision: str = ...,
) -> GetAssetTypeOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAssetTypeOutputTypeDef](./type_defs.md#getassettypeoutputtypedef) 


```python
# get_asset_type method usage example with argument unpacking

kwargs: GetAssetTypeInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.get_asset_type(**kwargs)
```

1. See [:material-code-braces: GetAssetTypeInputRequestTypeDef](./type_defs.md#getassettypeinputrequesttypedef) 

### get\_data\_source

Gets an Amazon DataZone data source.

Type annotations and code completion for `#!python session.client("datazone").get_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_data_source)

```python
# get_data_source method definition

await def get_data_source(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> GetDataSourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataSourceOutputTypeDef](./type_defs.md#getdatasourceoutputtypedef) 


```python
# get_data_source method usage example with argument unpacking

kwargs: GetDataSourceInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.get_data_source(**kwargs)
```

1. See [:material-code-braces: GetDataSourceInputRequestTypeDef](./type_defs.md#getdatasourceinputrequesttypedef) 

### get\_data\_source\_run

Gets an Amazon DataZone data source run.

Type annotations and code completion for `#!python session.client("datazone").get_data_source_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_data_source_run)

```python
# get_data_source_run method definition

await def get_data_source_run(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> GetDataSourceRunOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataSourceRunOutputTypeDef](./type_defs.md#getdatasourcerunoutputtypedef) 


```python
# get_data_source_run method usage example with argument unpacking

kwargs: GetDataSourceRunInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.get_data_source_run(**kwargs)
```

1. See [:material-code-braces: GetDataSourceRunInputRequestTypeDef](./type_defs.md#getdatasourceruninputrequesttypedef) 

### get\_domain

Gets an Amazon DataZone domain.

Type annotations and code completion for `#!python session.client("datazone").get_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_domain)

```python
# get_domain method definition

await def get_domain(
    self,
    *,
    identifier: str,
) -> GetDomainOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDomainOutputTypeDef](./type_defs.md#getdomainoutputtypedef) 


```python
# get_domain method usage example with argument unpacking

kwargs: GetDomainInputRequestTypeDef = {  # (1)
    "identifier": ...,
}

parent.get_domain(**kwargs)
```

1. See [:material-code-braces: GetDomainInputRequestTypeDef](./type_defs.md#getdomaininputrequesttypedef) 

### get\_environment

Gets an Amazon DataZone environment.

Type annotations and code completion for `#!python session.client("datazone").get_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_environment)

```python
# get_environment method definition

await def get_environment(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> GetEnvironmentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEnvironmentOutputTypeDef](./type_defs.md#getenvironmentoutputtypedef) 


```python
# get_environment method usage example with argument unpacking

kwargs: GetEnvironmentInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.get_environment(**kwargs)
```

1. See [:material-code-braces: GetEnvironmentInputRequestTypeDef](./type_defs.md#getenvironmentinputrequesttypedef) 

### get\_environment\_blueprint

Gets an Amazon DataZone blueprint.

Type annotations and code completion for `#!python session.client("datazone").get_environment_blueprint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_environment_blueprint)

```python
# get_environment_blueprint method definition

await def get_environment_blueprint(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> GetEnvironmentBlueprintOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEnvironmentBlueprintOutputTypeDef](./type_defs.md#getenvironmentblueprintoutputtypedef) 


```python
# get_environment_blueprint method usage example with argument unpacking

kwargs: GetEnvironmentBlueprintInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.get_environment_blueprint(**kwargs)
```

1. See [:material-code-braces: GetEnvironmentBlueprintInputRequestTypeDef](./type_defs.md#getenvironmentblueprintinputrequesttypedef) 

### get\_environment\_blueprint\_configuration

Gets the blueprint configuration in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").get_environment_blueprint_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_environment_blueprint_configuration)

```python
# get_environment_blueprint_configuration method definition

await def get_environment_blueprint_configuration(
    self,
    *,
    domainIdentifier: str,
    environmentBlueprintIdentifier: str,
) -> GetEnvironmentBlueprintConfigurationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEnvironmentBlueprintConfigurationOutputTypeDef](./type_defs.md#getenvironmentblueprintconfigurationoutputtypedef) 


```python
# get_environment_blueprint_configuration method usage example with argument unpacking

kwargs: GetEnvironmentBlueprintConfigurationInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "environmentBlueprintIdentifier": ...,
}

parent.get_environment_blueprint_configuration(**kwargs)
```

1. See [:material-code-braces: GetEnvironmentBlueprintConfigurationInputRequestTypeDef](./type_defs.md#getenvironmentblueprintconfigurationinputrequesttypedef) 

### get\_environment\_profile

Gets an evinronment profile in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").get_environment_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_environment_profile)

```python
# get_environment_profile method definition

await def get_environment_profile(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> GetEnvironmentProfileOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEnvironmentProfileOutputTypeDef](./type_defs.md#getenvironmentprofileoutputtypedef) 


```python
# get_environment_profile method usage example with argument unpacking

kwargs: GetEnvironmentProfileInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.get_environment_profile(**kwargs)
```

1. See [:material-code-braces: GetEnvironmentProfileInputRequestTypeDef](./type_defs.md#getenvironmentprofileinputrequesttypedef) 

### get\_form\_type

Gets a metadata form type in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").get_form_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_form_type)

```python
# get_form_type method definition

await def get_form_type(
    self,
    *,
    domainIdentifier: str,
    formTypeIdentifier: str,
    revision: str = ...,
) -> GetFormTypeOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFormTypeOutputTypeDef](./type_defs.md#getformtypeoutputtypedef) 


```python
# get_form_type method usage example with argument unpacking

kwargs: GetFormTypeInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "formTypeIdentifier": ...,
}

parent.get_form_type(**kwargs)
```

1. See [:material-code-braces: GetFormTypeInputRequestTypeDef](./type_defs.md#getformtypeinputrequesttypedef) 

### get\_glossary

Gets a business glossary in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").get_glossary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_glossary)

```python
# get_glossary method definition

await def get_glossary(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> GetGlossaryOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGlossaryOutputTypeDef](./type_defs.md#getglossaryoutputtypedef) 


```python
# get_glossary method usage example with argument unpacking

kwargs: GetGlossaryInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.get_glossary(**kwargs)
```

1. See [:material-code-braces: GetGlossaryInputRequestTypeDef](./type_defs.md#getglossaryinputrequesttypedef) 

### get\_glossary\_term

Gets a business glossary term in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").get_glossary_term` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_glossary_term)

```python
# get_glossary_term method definition

await def get_glossary_term(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> GetGlossaryTermOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGlossaryTermOutputTypeDef](./type_defs.md#getglossarytermoutputtypedef) 


```python
# get_glossary_term method usage example with argument unpacking

kwargs: GetGlossaryTermInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.get_glossary_term(**kwargs)
```

1. See [:material-code-braces: GetGlossaryTermInputRequestTypeDef](./type_defs.md#getglossaryterminputrequesttypedef) 

### get\_group\_profile

Gets a group profile in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").get_group_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_group_profile)

```python
# get_group_profile method definition

await def get_group_profile(
    self,
    *,
    domainIdentifier: str,
    groupIdentifier: str,
) -> GetGroupProfileOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGroupProfileOutputTypeDef](./type_defs.md#getgroupprofileoutputtypedef) 


```python
# get_group_profile method usage example with argument unpacking

kwargs: GetGroupProfileInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "groupIdentifier": ...,
}

parent.get_group_profile(**kwargs)
```

1. See [:material-code-braces: GetGroupProfileInputRequestTypeDef](./type_defs.md#getgroupprofileinputrequesttypedef) 

### get\_iam\_portal\_login\_url

Gets the data portal URL for the specified Amazon DataZone domain.

Type annotations and code completion for `#!python session.client("datazone").get_iam_portal_login_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_iam_portal_login_url)

```python
# get_iam_portal_login_url method definition

await def get_iam_portal_login_url(
    self,
    *,
    domainIdentifier: str,
) -> GetIamPortalLoginUrlOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIamPortalLoginUrlOutputTypeDef](./type_defs.md#getiamportalloginurloutputtypedef) 


```python
# get_iam_portal_login_url method usage example with argument unpacking

kwargs: GetIamPortalLoginUrlInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
}

parent.get_iam_portal_login_url(**kwargs)
```

1. See [:material-code-braces: GetIamPortalLoginUrlInputRequestTypeDef](./type_defs.md#getiamportalloginurlinputrequesttypedef) 

### get\_listing

See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/datazone-2018-05-10/GetListing).

Type annotations and code completion for `#!python session.client("datazone").get_listing` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_listing)

```python
# get_listing method definition

await def get_listing(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    listingRevision: str = ...,
) -> GetListingOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetListingOutputTypeDef](./type_defs.md#getlistingoutputtypedef) 


```python
# get_listing method usage example with argument unpacking

kwargs: GetListingInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.get_listing(**kwargs)
```

1. See [:material-code-braces: GetListingInputRequestTypeDef](./type_defs.md#getlistinginputrequesttypedef) 

### get\_project

Gets a project in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").get_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_project)

```python
# get_project method definition

await def get_project(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> GetProjectOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetProjectOutputTypeDef](./type_defs.md#getprojectoutputtypedef) 


```python
# get_project method usage example with argument unpacking

kwargs: GetProjectInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.get_project(**kwargs)
```

1. See [:material-code-braces: GetProjectInputRequestTypeDef](./type_defs.md#getprojectinputrequesttypedef) 

### get\_subscription

Gets a subscription in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").get_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_subscription)

```python
# get_subscription method definition

await def get_subscription(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> GetSubscriptionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSubscriptionOutputTypeDef](./type_defs.md#getsubscriptionoutputtypedef) 


```python
# get_subscription method usage example with argument unpacking

kwargs: GetSubscriptionInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.get_subscription(**kwargs)
```

1. See [:material-code-braces: GetSubscriptionInputRequestTypeDef](./type_defs.md#getsubscriptioninputrequesttypedef) 

### get\_subscription\_grant

Gets the subscription grant in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").get_subscription_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_subscription_grant)

```python
# get_subscription_grant method definition

await def get_subscription_grant(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> GetSubscriptionGrantOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSubscriptionGrantOutputTypeDef](./type_defs.md#getsubscriptiongrantoutputtypedef) 


```python
# get_subscription_grant method usage example with argument unpacking

kwargs: GetSubscriptionGrantInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.get_subscription_grant(**kwargs)
```

1. See [:material-code-braces: GetSubscriptionGrantInputRequestTypeDef](./type_defs.md#getsubscriptiongrantinputrequesttypedef) 

### get\_subscription\_request\_details

Gets the details of the specified subscription request.

Type annotations and code completion for `#!python session.client("datazone").get_subscription_request_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_subscription_request_details)

```python
# get_subscription_request_details method definition

await def get_subscription_request_details(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
) -> GetSubscriptionRequestDetailsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSubscriptionRequestDetailsOutputTypeDef](./type_defs.md#getsubscriptionrequestdetailsoutputtypedef) 


```python
# get_subscription_request_details method usage example with argument unpacking

kwargs: GetSubscriptionRequestDetailsInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.get_subscription_request_details(**kwargs)
```

1. See [:material-code-braces: GetSubscriptionRequestDetailsInputRequestTypeDef](./type_defs.md#getsubscriptionrequestdetailsinputrequesttypedef) 

### get\_subscription\_target

Gets the subscription target in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").get_subscription_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_subscription_target)

```python
# get_subscription_target method definition

await def get_subscription_target(
    self,
    *,
    domainIdentifier: str,
    environmentIdentifier: str,
    identifier: str,
) -> GetSubscriptionTargetOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSubscriptionTargetOutputTypeDef](./type_defs.md#getsubscriptiontargetoutputtypedef) 


```python
# get_subscription_target method usage example with argument unpacking

kwargs: GetSubscriptionTargetInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "environmentIdentifier": ...,
    "identifier": ...,
}

parent.get_subscription_target(**kwargs)
```

1. See [:material-code-braces: GetSubscriptionTargetInputRequestTypeDef](./type_defs.md#getsubscriptiontargetinputrequesttypedef) 

### get\_user\_profile

Gets a user profile in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").get_user_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_user_profile)

```python
# get_user_profile method definition

await def get_user_profile(
    self,
    *,
    domainIdentifier: str,
    userIdentifier: str,
    type: UserProfileTypeType = ...,  # (1)
) -> GetUserProfileOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: UserProfileTypeType](./literals.md#userprofiletypetype) 
2. See [:material-code-braces: GetUserProfileOutputTypeDef](./type_defs.md#getuserprofileoutputtypedef) 


```python
# get_user_profile method usage example with argument unpacking

kwargs: GetUserProfileInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "userIdentifier": ...,
}

parent.get_user_profile(**kwargs)
```

1. See [:material-code-braces: GetUserProfileInputRequestTypeDef](./type_defs.md#getuserprofileinputrequesttypedef) 

### list\_asset\_revisions

Lists the revisions for the asset.

Type annotations and code completion for `#!python session.client("datazone").list_asset_revisions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_asset_revisions)

```python
# list_asset_revisions method definition

await def list_asset_revisions(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAssetRevisionsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAssetRevisionsOutputTypeDef](./type_defs.md#listassetrevisionsoutputtypedef) 


```python
# list_asset_revisions method usage example with argument unpacking

kwargs: ListAssetRevisionsInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.list_asset_revisions(**kwargs)
```

1. See [:material-code-braces: ListAssetRevisionsInputRequestTypeDef](./type_defs.md#listassetrevisionsinputrequesttypedef) 

### list\_data\_source\_run\_activities

Lists data source run activities.

Type annotations and code completion for `#!python session.client("datazone").list_data_source_run_activities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_data_source_run_activities)

```python
# list_data_source_run_activities method definition

await def list_data_source_run_activities(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    maxResults: int = ...,
    nextToken: str = ...,
    status: DataAssetActivityStatusType = ...,  # (1)
) -> ListDataSourceRunActivitiesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DataAssetActivityStatusType](./literals.md#dataassetactivitystatustype) 
2. See [:material-code-braces: ListDataSourceRunActivitiesOutputTypeDef](./type_defs.md#listdatasourcerunactivitiesoutputtypedef) 


```python
# list_data_source_run_activities method usage example with argument unpacking

kwargs: ListDataSourceRunActivitiesInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.list_data_source_run_activities(**kwargs)
```

1. See [:material-code-braces: ListDataSourceRunActivitiesInputRequestTypeDef](./type_defs.md#listdatasourcerunactivitiesinputrequesttypedef) 

### list\_data\_source\_runs

Lists data source runs in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").list_data_source_runs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_data_source_runs)

```python
# list_data_source_runs method definition

await def list_data_source_runs(
    self,
    *,
    dataSourceIdentifier: str,
    domainIdentifier: str,
    maxResults: int = ...,
    nextToken: str = ...,
    status: DataSourceRunStatusType = ...,  # (1)
) -> ListDataSourceRunsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DataSourceRunStatusType](./literals.md#datasourcerunstatustype) 
2. See [:material-code-braces: ListDataSourceRunsOutputTypeDef](./type_defs.md#listdatasourcerunsoutputtypedef) 


```python
# list_data_source_runs method usage example with argument unpacking

kwargs: ListDataSourceRunsInputRequestTypeDef = {  # (1)
    "dataSourceIdentifier": ...,
    "domainIdentifier": ...,
}

parent.list_data_source_runs(**kwargs)
```

1. See [:material-code-braces: ListDataSourceRunsInputRequestTypeDef](./type_defs.md#listdatasourcerunsinputrequesttypedef) 

### list\_data\_sources

Lists data sources in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").list_data_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_data_sources)

```python
# list_data_sources method definition

await def list_data_sources(
    self,
    *,
    domainIdentifier: str,
    projectIdentifier: str,
    environmentIdentifier: str = ...,
    maxResults: int = ...,
    name: str = ...,
    nextToken: str = ...,
    status: DataSourceStatusType = ...,  # (1)
    type: str = ...,
) -> ListDataSourcesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
2. See [:material-code-braces: ListDataSourcesOutputTypeDef](./type_defs.md#listdatasourcesoutputtypedef) 


```python
# list_data_sources method usage example with argument unpacking

kwargs: ListDataSourcesInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "projectIdentifier": ...,
}

parent.list_data_sources(**kwargs)
```

1. See [:material-code-braces: ListDataSourcesInputRequestTypeDef](./type_defs.md#listdatasourcesinputrequesttypedef) 

### list\_domains

Lists Amazon DataZone domains.

Type annotations and code completion for `#!python session.client("datazone").list_domains` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_domains)

```python
# list_domains method definition

await def list_domains(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    status: DomainStatusType = ...,  # (1)
) -> ListDomainsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
2. See [:material-code-braces: ListDomainsOutputTypeDef](./type_defs.md#listdomainsoutputtypedef) 


```python
# list_domains method usage example with argument unpacking

kwargs: ListDomainsInputRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_domains(**kwargs)
```

1. See [:material-code-braces: ListDomainsInputRequestTypeDef](./type_defs.md#listdomainsinputrequesttypedef) 

### list\_environment\_blueprint\_configurations

Lists blueprint configurations for a Amazon DataZone environment.

Type annotations and code completion for `#!python session.client("datazone").list_environment_blueprint_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_environment_blueprint_configurations)

```python
# list_environment_blueprint_configurations method definition

await def list_environment_blueprint_configurations(
    self,
    *,
    domainIdentifier: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListEnvironmentBlueprintConfigurationsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEnvironmentBlueprintConfigurationsOutputTypeDef](./type_defs.md#listenvironmentblueprintconfigurationsoutputtypedef) 


```python
# list_environment_blueprint_configurations method usage example with argument unpacking

kwargs: ListEnvironmentBlueprintConfigurationsInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
}

parent.list_environment_blueprint_configurations(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentBlueprintConfigurationsInputRequestTypeDef](./type_defs.md#listenvironmentblueprintconfigurationsinputrequesttypedef) 

### list\_environment\_blueprints

Lists blueprints in an Amazon DataZone environment.

Type annotations and code completion for `#!python session.client("datazone").list_environment_blueprints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_environment_blueprints)

```python
# list_environment_blueprints method definition

await def list_environment_blueprints(
    self,
    *,
    domainIdentifier: str,
    managed: bool = ...,
    maxResults: int = ...,
    name: str = ...,
    nextToken: str = ...,
) -> ListEnvironmentBlueprintsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEnvironmentBlueprintsOutputTypeDef](./type_defs.md#listenvironmentblueprintsoutputtypedef) 


```python
# list_environment_blueprints method usage example with argument unpacking

kwargs: ListEnvironmentBlueprintsInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
}

parent.list_environment_blueprints(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentBlueprintsInputRequestTypeDef](./type_defs.md#listenvironmentblueprintsinputrequesttypedef) 

### list\_environment\_profiles

Lists Amazon DataZone environment profiles.

Type annotations and code completion for `#!python session.client("datazone").list_environment_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_environment_profiles)

```python
# list_environment_profiles method definition

await def list_environment_profiles(
    self,
    *,
    domainIdentifier: str,
    awsAccountId: str = ...,
    awsAccountRegion: str = ...,
    environmentBlueprintIdentifier: str = ...,
    maxResults: int = ...,
    name: str = ...,
    nextToken: str = ...,
    projectIdentifier: str = ...,
) -> ListEnvironmentProfilesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEnvironmentProfilesOutputTypeDef](./type_defs.md#listenvironmentprofilesoutputtypedef) 


```python
# list_environment_profiles method usage example with argument unpacking

kwargs: ListEnvironmentProfilesInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
}

parent.list_environment_profiles(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentProfilesInputRequestTypeDef](./type_defs.md#listenvironmentprofilesinputrequesttypedef) 

### list\_environments

Lists Amazon DataZone environments.

Type annotations and code completion for `#!python session.client("datazone").list_environments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_environments)

```python
# list_environments method definition

await def list_environments(
    self,
    *,
    domainIdentifier: str,
    projectIdentifier: str,
    awsAccountId: str = ...,
    awsAccountRegion: str = ...,
    environmentBlueprintIdentifier: str = ...,
    environmentProfileIdentifier: str = ...,
    maxResults: int = ...,
    name: str = ...,
    nextToken: str = ...,
    provider: str = ...,
    status: EnvironmentStatusType = ...,  # (1)
) -> ListEnvironmentsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
2. See [:material-code-braces: ListEnvironmentsOutputTypeDef](./type_defs.md#listenvironmentsoutputtypedef) 


```python
# list_environments method usage example with argument unpacking

kwargs: ListEnvironmentsInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "projectIdentifier": ...,
}

parent.list_environments(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentsInputRequestTypeDef](./type_defs.md#listenvironmentsinputrequesttypedef) 

### list\_notifications

Lists all Amazon DataZone notifications.

Type annotations and code completion for `#!python session.client("datazone").list_notifications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_notifications)

```python
# list_notifications method definition

await def list_notifications(
    self,
    *,
    domainIdentifier: str,
    type: NotificationTypeType,  # (1)
    afterTimestamp: Union[datetime, str] = ...,
    beforeTimestamp: Union[datetime, str] = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    subjects: Sequence[str] = ...,
    taskStatus: TaskStatusType = ...,  # (2)
) -> ListNotificationsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
2. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
3. See [:material-code-braces: ListNotificationsOutputTypeDef](./type_defs.md#listnotificationsoutputtypedef) 


```python
# list_notifications method usage example with argument unpacking

kwargs: ListNotificationsInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "type": ...,
}

parent.list_notifications(**kwargs)
```

1. See [:material-code-braces: ListNotificationsInputRequestTypeDef](./type_defs.md#listnotificationsinputrequesttypedef) 

### list\_project\_memberships

Lists all members of the specified project.

Type annotations and code completion for `#!python session.client("datazone").list_project_memberships` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_project_memberships)

```python
# list_project_memberships method definition

await def list_project_memberships(
    self,
    *,
    domainIdentifier: str,
    projectIdentifier: str,
    maxResults: int = ...,
    nextToken: str = ...,
    sortBy: SortFieldProjectType = ...,  # (1)
    sortOrder: SortOrderType = ...,  # (2)
) -> ListProjectMembershipsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SortFieldProjectType](./literals.md#sortfieldprojecttype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListProjectMembershipsOutputTypeDef](./type_defs.md#listprojectmembershipsoutputtypedef) 


```python
# list_project_memberships method usage example with argument unpacking

kwargs: ListProjectMembershipsInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "projectIdentifier": ...,
}

parent.list_project_memberships(**kwargs)
```

1. See [:material-code-braces: ListProjectMembershipsInputRequestTypeDef](./type_defs.md#listprojectmembershipsinputrequesttypedef) 

### list\_projects

Lists Amazon DataZone projects.

Type annotations and code completion for `#!python session.client("datazone").list_projects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_projects)

```python
# list_projects method definition

await def list_projects(
    self,
    *,
    domainIdentifier: str,
    groupIdentifier: str = ...,
    maxResults: int = ...,
    name: str = ...,
    nextToken: str = ...,
    userIdentifier: str = ...,
) -> ListProjectsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListProjectsOutputTypeDef](./type_defs.md#listprojectsoutputtypedef) 


```python
# list_projects method usage example with argument unpacking

kwargs: ListProjectsInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
}

parent.list_projects(**kwargs)
```

1. See [:material-code-braces: ListProjectsInputRequestTypeDef](./type_defs.md#listprojectsinputrequesttypedef) 

### list\_subscription\_grants

Lists subscription grants.

Type annotations and code completion for `#!python session.client("datazone").list_subscription_grants` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_subscription_grants)

```python
# list_subscription_grants method definition

await def list_subscription_grants(
    self,
    *,
    domainIdentifier: str,
    environmentId: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    sortBy: SortKeyType = ...,  # (1)
    sortOrder: SortOrderType = ...,  # (2)
    subscribedListingId: str = ...,
    subscriptionId: str = ...,
    subscriptionTargetId: str = ...,
) -> ListSubscriptionGrantsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SortKeyType](./literals.md#sortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListSubscriptionGrantsOutputTypeDef](./type_defs.md#listsubscriptiongrantsoutputtypedef) 


```python
# list_subscription_grants method usage example with argument unpacking

kwargs: ListSubscriptionGrantsInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
}

parent.list_subscription_grants(**kwargs)
```

1. See [:material-code-braces: ListSubscriptionGrantsInputRequestTypeDef](./type_defs.md#listsubscriptiongrantsinputrequesttypedef) 

### list\_subscription\_requests

Lists Amazon DataZone subscription requests.

Type annotations and code completion for `#!python session.client("datazone").list_subscription_requests` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_subscription_requests)

```python
# list_subscription_requests method definition

await def list_subscription_requests(
    self,
    *,
    domainIdentifier: str,
    approverProjectId: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    owningProjectId: str = ...,
    sortBy: SortKeyType = ...,  # (1)
    sortOrder: SortOrderType = ...,  # (2)
    status: SubscriptionRequestStatusType = ...,  # (3)
    subscribedListingId: str = ...,
) -> ListSubscriptionRequestsOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: SortKeyType](./literals.md#sortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: SubscriptionRequestStatusType](./literals.md#subscriptionrequeststatustype) 
4. See [:material-code-braces: ListSubscriptionRequestsOutputTypeDef](./type_defs.md#listsubscriptionrequestsoutputtypedef) 


```python
# list_subscription_requests method usage example with argument unpacking

kwargs: ListSubscriptionRequestsInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
}

parent.list_subscription_requests(**kwargs)
```

1. See [:material-code-braces: ListSubscriptionRequestsInputRequestTypeDef](./type_defs.md#listsubscriptionrequestsinputrequesttypedef) 

### list\_subscription\_targets

Lists subscription targets in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").list_subscription_targets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_subscription_targets)

```python
# list_subscription_targets method definition

await def list_subscription_targets(
    self,
    *,
    domainIdentifier: str,
    environmentIdentifier: str,
    maxResults: int = ...,
    nextToken: str = ...,
    sortBy: SortKeyType = ...,  # (1)
    sortOrder: SortOrderType = ...,  # (2)
) -> ListSubscriptionTargetsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SortKeyType](./literals.md#sortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListSubscriptionTargetsOutputTypeDef](./type_defs.md#listsubscriptiontargetsoutputtypedef) 


```python
# list_subscription_targets method usage example with argument unpacking

kwargs: ListSubscriptionTargetsInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "environmentIdentifier": ...,
}

parent.list_subscription_targets(**kwargs)
```

1. See [:material-code-braces: ListSubscriptionTargetsInputRequestTypeDef](./type_defs.md#listsubscriptiontargetsinputrequesttypedef) 

### list\_subscriptions

Lists subscriptions in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").list_subscriptions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_subscriptions)

```python
# list_subscriptions method definition

await def list_subscriptions(
    self,
    *,
    domainIdentifier: str,
    approverProjectId: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    owningProjectId: str = ...,
    sortBy: SortKeyType = ...,  # (1)
    sortOrder: SortOrderType = ...,  # (2)
    status: SubscriptionStatusType = ...,  # (3)
    subscribedListingId: str = ...,
    subscriptionRequestIdentifier: str = ...,
) -> ListSubscriptionsOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: SortKeyType](./literals.md#sortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: SubscriptionStatusType](./literals.md#subscriptionstatustype) 
4. See [:material-code-braces: ListSubscriptionsOutputTypeDef](./type_defs.md#listsubscriptionsoutputtypedef) 


```python
# list_subscriptions method usage example with argument unpacking

kwargs: ListSubscriptionsInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
}

parent.list_subscriptions(**kwargs)
```

1. See [:material-code-braces: ListSubscriptionsInputRequestTypeDef](./type_defs.md#listsubscriptionsinputrequesttypedef) 

### list\_tags\_for\_resource

Lists tags for the specified resource in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### put\_environment\_blueprint\_configuration

Writes the configuration for the specified environment blueprint in Amazon
DataZone.

Type annotations and code completion for `#!python session.client("datazone").put_environment_blueprint_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.put_environment_blueprint_configuration)

```python
# put_environment_blueprint_configuration method definition

await def put_environment_blueprint_configuration(
    self,
    *,
    domainIdentifier: str,
    enabledRegions: Sequence[str],
    environmentBlueprintIdentifier: str,
    manageAccessRoleArn: str = ...,
    provisioningRoleArn: str = ...,
    regionalParameters: Mapping[str, Mapping[str, str]] = ...,
) -> PutEnvironmentBlueprintConfigurationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutEnvironmentBlueprintConfigurationOutputTypeDef](./type_defs.md#putenvironmentblueprintconfigurationoutputtypedef) 


```python
# put_environment_blueprint_configuration method usage example with argument unpacking

kwargs: PutEnvironmentBlueprintConfigurationInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "enabledRegions": ...,
    "environmentBlueprintIdentifier": ...,
}

parent.put_environment_blueprint_configuration(**kwargs)
```

1. See [:material-code-braces: PutEnvironmentBlueprintConfigurationInputRequestTypeDef](./type_defs.md#putenvironmentblueprintconfigurationinputrequesttypedef) 

### reject\_predictions

Rejects automatically generated business-friendly metadata for your Amazon
DataZone
assets.

Type annotations and code completion for `#!python session.client("datazone").reject_predictions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.reject_predictions)

```python
# reject_predictions method definition

await def reject_predictions(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    clientToken: str = ...,
    rejectChoices: Sequence[RejectChoiceTypeDef] = ...,  # (1)
    rejectRule: RejectRuleTypeDef = ...,  # (2)
    revision: str = ...,
) -> RejectPredictionsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RejectChoiceTypeDef](./type_defs.md#rejectchoicetypedef) 
2. See [:material-code-braces: RejectRuleTypeDef](./type_defs.md#rejectruletypedef) 
3. See [:material-code-braces: RejectPredictionsOutputTypeDef](./type_defs.md#rejectpredictionsoutputtypedef) 


```python
# reject_predictions method usage example with argument unpacking

kwargs: RejectPredictionsInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.reject_predictions(**kwargs)
```

1. See [:material-code-braces: RejectPredictionsInputRequestTypeDef](./type_defs.md#rejectpredictionsinputrequesttypedef) 

### reject\_subscription\_request

Rejects the specified subscription request.

Type annotations and code completion for `#!python session.client("datazone").reject_subscription_request` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.reject_subscription_request)

```python
# reject_subscription_request method definition

await def reject_subscription_request(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    decisionComment: str = ...,
) -> RejectSubscriptionRequestOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RejectSubscriptionRequestOutputTypeDef](./type_defs.md#rejectsubscriptionrequestoutputtypedef) 


```python
# reject_subscription_request method usage example with argument unpacking

kwargs: RejectSubscriptionRequestInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.reject_subscription_request(**kwargs)
```

1. See [:material-code-braces: RejectSubscriptionRequestInputRequestTypeDef](./type_defs.md#rejectsubscriptionrequestinputrequesttypedef) 

### revoke\_subscription

Revokes a specified subscription in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").revoke_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.revoke_subscription)

```python
# revoke_subscription method definition

await def revoke_subscription(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    retainPermissions: bool = ...,
) -> RevokeSubscriptionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RevokeSubscriptionOutputTypeDef](./type_defs.md#revokesubscriptionoutputtypedef) 


```python
# revoke_subscription method usage example with argument unpacking

kwargs: RevokeSubscriptionInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.revoke_subscription(**kwargs)
```

1. See [:material-code-braces: RevokeSubscriptionInputRequestTypeDef](./type_defs.md#revokesubscriptioninputrequesttypedef) 

### search

Searches for assets in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").search` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.search)

```python
# search method definition

await def search(
    self,
    *,
    domainIdentifier: str,
    searchScope: InventorySearchScopeType,  # (1)
    additionalAttributes: Sequence[SearchOutputAdditionalAttributeType] = ...,  # (2)
    filters: FilterClauseTypeDef = ...,  # (3)
    maxResults: int = ...,
    nextToken: str = ...,
    owningProjectIdentifier: str = ...,
    searchIn: Sequence[SearchInItemTypeDef] = ...,  # (4)
    searchText: str = ...,
    sort: SearchSortTypeDef = ...,  # (5)
) -> SearchOutputTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: InventorySearchScopeType](./literals.md#inventorysearchscopetype) 
2. See [:material-code-brackets: SearchOutputAdditionalAttributeType](./literals.md#searchoutputadditionalattributetype) 
3. See [:material-code-braces: FilterClauseTypeDef](./type_defs.md#filterclausetypedef) 
4. See [:material-code-braces: SearchInItemTypeDef](./type_defs.md#searchinitemtypedef) 
5. See [:material-code-braces: SearchSortTypeDef](./type_defs.md#searchsorttypedef) 
6. See [:material-code-braces: SearchOutputTypeDef](./type_defs.md#searchoutputtypedef) 


```python
# search method usage example with argument unpacking

kwargs: SearchInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "searchScope": ...,
}

parent.search(**kwargs)
```

1. See [:material-code-braces: SearchInputRequestTypeDef](./type_defs.md#searchinputrequesttypedef) 

### search\_group\_profiles

Searches group profiles in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").search_group_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.search_group_profiles)

```python
# search_group_profiles method definition

await def search_group_profiles(
    self,
    *,
    domainIdentifier: str,
    groupType: GroupSearchTypeType,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
    searchText: str = ...,
) -> SearchGroupProfilesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: GroupSearchTypeType](./literals.md#groupsearchtypetype) 
2. See [:material-code-braces: SearchGroupProfilesOutputTypeDef](./type_defs.md#searchgroupprofilesoutputtypedef) 


```python
# search_group_profiles method usage example with argument unpacking

kwargs: SearchGroupProfilesInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "groupType": ...,
}

parent.search_group_profiles(**kwargs)
```

1. See [:material-code-braces: SearchGroupProfilesInputRequestTypeDef](./type_defs.md#searchgroupprofilesinputrequesttypedef) 

### search\_listings

Searches listings in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").search_listings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.search_listings)

```python
# search_listings method definition

await def search_listings(
    self,
    *,
    domainIdentifier: str,
    additionalAttributes: Sequence[SearchOutputAdditionalAttributeType] = ...,  # (1)
    filters: FilterClauseTypeDef = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
    searchIn: Sequence[SearchInItemTypeDef] = ...,  # (3)
    searchText: str = ...,
    sort: SearchSortTypeDef = ...,  # (4)
) -> SearchListingsOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: SearchOutputAdditionalAttributeType](./literals.md#searchoutputadditionalattributetype) 
2. See [:material-code-braces: FilterClauseTypeDef](./type_defs.md#filterclausetypedef) 
3. See [:material-code-braces: SearchInItemTypeDef](./type_defs.md#searchinitemtypedef) 
4. See [:material-code-braces: SearchSortTypeDef](./type_defs.md#searchsorttypedef) 
5. See [:material-code-braces: SearchListingsOutputTypeDef](./type_defs.md#searchlistingsoutputtypedef) 


```python
# search_listings method usage example with argument unpacking

kwargs: SearchListingsInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
}

parent.search_listings(**kwargs)
```

1. See [:material-code-braces: SearchListingsInputRequestTypeDef](./type_defs.md#searchlistingsinputrequesttypedef) 

### search\_types

Searches for types in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").search_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.search_types)

```python
# search_types method definition

await def search_types(
    self,
    *,
    domainIdentifier: str,
    managed: bool,
    searchScope: TypesSearchScopeType,  # (1)
    filters: FilterClauseTypeDef = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
    searchIn: Sequence[SearchInItemTypeDef] = ...,  # (3)
    searchText: str = ...,
    sort: SearchSortTypeDef = ...,  # (4)
) -> SearchTypesOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: TypesSearchScopeType](./literals.md#typessearchscopetype) 
2. See [:material-code-braces: FilterClauseTypeDef](./type_defs.md#filterclausetypedef) 
3. See [:material-code-braces: SearchInItemTypeDef](./type_defs.md#searchinitemtypedef) 
4. See [:material-code-braces: SearchSortTypeDef](./type_defs.md#searchsorttypedef) 
5. See [:material-code-braces: SearchTypesOutputTypeDef](./type_defs.md#searchtypesoutputtypedef) 


```python
# search_types method usage example with argument unpacking

kwargs: SearchTypesInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "managed": ...,
    "searchScope": ...,
}

parent.search_types(**kwargs)
```

1. See [:material-code-braces: SearchTypesInputRequestTypeDef](./type_defs.md#searchtypesinputrequesttypedef) 

### search\_user\_profiles

Searches user profiles in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").search_user_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.search_user_profiles)

```python
# search_user_profiles method definition

await def search_user_profiles(
    self,
    *,
    domainIdentifier: str,
    userType: UserSearchTypeType,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
    searchText: str = ...,
) -> SearchUserProfilesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: UserSearchTypeType](./literals.md#usersearchtypetype) 
2. See [:material-code-braces: SearchUserProfilesOutputTypeDef](./type_defs.md#searchuserprofilesoutputtypedef) 


```python
# search_user_profiles method usage example with argument unpacking

kwargs: SearchUserProfilesInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "userType": ...,
}

parent.search_user_profiles(**kwargs)
```

1. See [:material-code-braces: SearchUserProfilesInputRequestTypeDef](./type_defs.md#searchuserprofilesinputrequesttypedef) 

### start\_data\_source\_run

Start the run of the specified data source in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").start_data_source_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.start_data_source_run)

```python
# start_data_source_run method definition

await def start_data_source_run(
    self,
    *,
    dataSourceIdentifier: str,
    domainIdentifier: str,
    clientToken: str = ...,
) -> StartDataSourceRunOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartDataSourceRunOutputTypeDef](./type_defs.md#startdatasourcerunoutputtypedef) 


```python
# start_data_source_run method usage example with argument unpacking

kwargs: StartDataSourceRunInputRequestTypeDef = {  # (1)
    "dataSourceIdentifier": ...,
    "domainIdentifier": ...,
}

parent.start_data_source_run(**kwargs)
```

1. See [:material-code-braces: StartDataSourceRunInputRequestTypeDef](./type_defs.md#startdatasourceruninputrequesttypedef) 

### tag\_resource

Tags a resource in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Untags a resource in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_data\_source

Updates the specified data source in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").update_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_data_source)

```python
# update_data_source method definition

await def update_data_source(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    assetFormsInput: Sequence[FormInputTypeDef] = ...,  # (1)
    configuration: DataSourceConfigurationInputTypeDef = ...,  # (2)
    description: str = ...,
    enableSetting: EnableSettingType = ...,  # (3)
    name: str = ...,
    publishOnImport: bool = ...,
    recommendation: RecommendationConfigurationTypeDef = ...,  # (4)
    schedule: ScheduleConfigurationTypeDef = ...,  # (5)
) -> UpdateDataSourceOutputTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: FormInputTypeDef](./type_defs.md#forminputtypedef) 
2. See [:material-code-braces: DataSourceConfigurationInputTypeDef](./type_defs.md#datasourceconfigurationinputtypedef) 
3. See [:material-code-brackets: EnableSettingType](./literals.md#enablesettingtype) 
4. See [:material-code-braces: RecommendationConfigurationTypeDef](./type_defs.md#recommendationconfigurationtypedef) 
5. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
6. See [:material-code-braces: UpdateDataSourceOutputTypeDef](./type_defs.md#updatedatasourceoutputtypedef) 


```python
# update_data_source method usage example with argument unpacking

kwargs: UpdateDataSourceInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.update_data_source(**kwargs)
```

1. See [:material-code-braces: UpdateDataSourceInputRequestTypeDef](./type_defs.md#updatedatasourceinputrequesttypedef) 

### update\_domain

Updates a Amazon DataZone domain.

Type annotations and code completion for `#!python session.client("datazone").update_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_domain)

```python
# update_domain method definition

await def update_domain(
    self,
    *,
    identifier: str,
    clientToken: str = ...,
    description: str = ...,
    domainExecutionRole: str = ...,
    name: str = ...,
    singleSignOn: SingleSignOnTypeDef = ...,  # (1)
) -> UpdateDomainOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SingleSignOnTypeDef](./type_defs.md#singlesignontypedef) 
2. See [:material-code-braces: UpdateDomainOutputTypeDef](./type_defs.md#updatedomainoutputtypedef) 


```python
# update_domain method usage example with argument unpacking

kwargs: UpdateDomainInputRequestTypeDef = {  # (1)
    "identifier": ...,
}

parent.update_domain(**kwargs)
```

1. See [:material-code-braces: UpdateDomainInputRequestTypeDef](./type_defs.md#updatedomaininputrequesttypedef) 

### update\_environment

Updates the specified environment in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").update_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_environment)

```python
# update_environment method definition

await def update_environment(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    description: str = ...,
    glossaryTerms: Sequence[str] = ...,
    name: str = ...,
) -> UpdateEnvironmentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateEnvironmentOutputTypeDef](./type_defs.md#updateenvironmentoutputtypedef) 


```python
# update_environment method usage example with argument unpacking

kwargs: UpdateEnvironmentInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.update_environment(**kwargs)
```

1. See [:material-code-braces: UpdateEnvironmentInputRequestTypeDef](./type_defs.md#updateenvironmentinputrequesttypedef) 

### update\_environment\_profile

Updates the specified environment profile in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").update_environment_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_environment_profile)

```python
# update_environment_profile method definition

await def update_environment_profile(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    awsAccountId: str = ...,
    awsAccountRegion: str = ...,
    description: str = ...,
    name: str = ...,
    userParameters: Sequence[EnvironmentParameterTypeDef] = ...,  # (1)
) -> UpdateEnvironmentProfileOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EnvironmentParameterTypeDef](./type_defs.md#environmentparametertypedef) 
2. See [:material-code-braces: UpdateEnvironmentProfileOutputTypeDef](./type_defs.md#updateenvironmentprofileoutputtypedef) 


```python
# update_environment_profile method usage example with argument unpacking

kwargs: UpdateEnvironmentProfileInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.update_environment_profile(**kwargs)
```

1. See [:material-code-braces: UpdateEnvironmentProfileInputRequestTypeDef](./type_defs.md#updateenvironmentprofileinputrequesttypedef) 

### update\_glossary

Updates the business glossary in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").update_glossary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_glossary)

```python
# update_glossary method definition

await def update_glossary(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    clientToken: str = ...,
    description: str = ...,
    name: str = ...,
    status: GlossaryStatusType = ...,  # (1)
) -> UpdateGlossaryOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: GlossaryStatusType](./literals.md#glossarystatustype) 
2. See [:material-code-braces: UpdateGlossaryOutputTypeDef](./type_defs.md#updateglossaryoutputtypedef) 


```python
# update_glossary method usage example with argument unpacking

kwargs: UpdateGlossaryInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.update_glossary(**kwargs)
```

1. See [:material-code-braces: UpdateGlossaryInputRequestTypeDef](./type_defs.md#updateglossaryinputrequesttypedef) 

### update\_glossary\_term

Updates a business glossary term in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").update_glossary_term` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_glossary_term)

```python
# update_glossary_term method definition

await def update_glossary_term(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    glossaryIdentifier: str = ...,
    longDescription: str = ...,
    name: str = ...,
    shortDescription: str = ...,
    status: GlossaryTermStatusType = ...,  # (1)
    termRelations: TermRelationsTypeDef = ...,  # (2)
) -> UpdateGlossaryTermOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: GlossaryTermStatusType](./literals.md#glossarytermstatustype) 
2. See [:material-code-braces: TermRelationsTypeDef](./type_defs.md#termrelationstypedef) 
3. See [:material-code-braces: UpdateGlossaryTermOutputTypeDef](./type_defs.md#updateglossarytermoutputtypedef) 


```python
# update_glossary_term method usage example with argument unpacking

kwargs: UpdateGlossaryTermInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.update_glossary_term(**kwargs)
```

1. See [:material-code-braces: UpdateGlossaryTermInputRequestTypeDef](./type_defs.md#updateglossaryterminputrequesttypedef) 

### update\_group\_profile

Updates the specified group profile in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").update_group_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_group_profile)

```python
# update_group_profile method definition

await def update_group_profile(
    self,
    *,
    domainIdentifier: str,
    groupIdentifier: str,
    status: GroupProfileStatusType,  # (1)
) -> UpdateGroupProfileOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: GroupProfileStatusType](./literals.md#groupprofilestatustype) 
2. See [:material-code-braces: UpdateGroupProfileOutputTypeDef](./type_defs.md#updategroupprofileoutputtypedef) 


```python
# update_group_profile method usage example with argument unpacking

kwargs: UpdateGroupProfileInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "groupIdentifier": ...,
    "status": ...,
}

parent.update_group_profile(**kwargs)
```

1. See [:material-code-braces: UpdateGroupProfileInputRequestTypeDef](./type_defs.md#updategroupprofileinputrequesttypedef) 

### update\_project

Updates the specified project in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").update_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_project)

```python
# update_project method definition

await def update_project(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    description: str = ...,
    glossaryTerms: Sequence[str] = ...,
    name: str = ...,
) -> UpdateProjectOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateProjectOutputTypeDef](./type_defs.md#updateprojectoutputtypedef) 


```python
# update_project method usage example with argument unpacking

kwargs: UpdateProjectInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.update_project(**kwargs)
```

1. See [:material-code-braces: UpdateProjectInputRequestTypeDef](./type_defs.md#updateprojectinputrequesttypedef) 

### update\_subscription\_grant\_status

Updates the status of the specified subscription grant status in Amazon
DataZone.

Type annotations and code completion for `#!python session.client("datazone").update_subscription_grant_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_subscription_grant_status)

```python
# update_subscription_grant_status method definition

await def update_subscription_grant_status(
    self,
    *,
    assetIdentifier: str,
    domainIdentifier: str,
    identifier: str,
    status: SubscriptionGrantStatusType,  # (1)
    failureCause: FailureCauseTypeDef = ...,  # (2)
    targetName: str = ...,
) -> UpdateSubscriptionGrantStatusOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SubscriptionGrantStatusType](./literals.md#subscriptiongrantstatustype) 
2. See [:material-code-braces: FailureCauseTypeDef](./type_defs.md#failurecausetypedef) 
3. See [:material-code-braces: UpdateSubscriptionGrantStatusOutputTypeDef](./type_defs.md#updatesubscriptiongrantstatusoutputtypedef) 


```python
# update_subscription_grant_status method usage example with argument unpacking

kwargs: UpdateSubscriptionGrantStatusInputRequestTypeDef = {  # (1)
    "assetIdentifier": ...,
    "domainIdentifier": ...,
    "identifier": ...,
    "status": ...,
}

parent.update_subscription_grant_status(**kwargs)
```

1. See [:material-code-braces: UpdateSubscriptionGrantStatusInputRequestTypeDef](./type_defs.md#updatesubscriptiongrantstatusinputrequesttypedef) 

### update\_subscription\_request

Updates a specified subscription request in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").update_subscription_request` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_subscription_request)

```python
# update_subscription_request method definition

await def update_subscription_request(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    requestReason: str,
) -> UpdateSubscriptionRequestOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateSubscriptionRequestOutputTypeDef](./type_defs.md#updatesubscriptionrequestoutputtypedef) 


```python
# update_subscription_request method usage example with argument unpacking

kwargs: UpdateSubscriptionRequestInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
    "requestReason": ...,
}

parent.update_subscription_request(**kwargs)
```

1. See [:material-code-braces: UpdateSubscriptionRequestInputRequestTypeDef](./type_defs.md#updatesubscriptionrequestinputrequesttypedef) 

### update\_subscription\_target

Updates the specified subscription target in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").update_subscription_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_subscription_target)

```python
# update_subscription_target method definition

await def update_subscription_target(
    self,
    *,
    domainIdentifier: str,
    environmentIdentifier: str,
    identifier: str,
    applicableAssetTypes: Sequence[str] = ...,
    authorizedPrincipals: Sequence[str] = ...,
    manageAccessRole: str = ...,
    name: str = ...,
    provider: str = ...,
    subscriptionTargetConfig: Sequence[SubscriptionTargetFormTypeDef] = ...,  # (1)
) -> UpdateSubscriptionTargetOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SubscriptionTargetFormTypeDef](./type_defs.md#subscriptiontargetformtypedef) 
2. See [:material-code-braces: UpdateSubscriptionTargetOutputTypeDef](./type_defs.md#updatesubscriptiontargetoutputtypedef) 


```python
# update_subscription_target method usage example with argument unpacking

kwargs: UpdateSubscriptionTargetInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "environmentIdentifier": ...,
    "identifier": ...,
}

parent.update_subscription_target(**kwargs)
```

1. See [:material-code-braces: UpdateSubscriptionTargetInputRequestTypeDef](./type_defs.md#updatesubscriptiontargetinputrequesttypedef) 

### update\_user\_profile

Updates the specified user profile in Amazon DataZone.

Type annotations and code completion for `#!python session.client("datazone").update_user_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.update_user_profile)

```python
# update_user_profile method definition

await def update_user_profile(
    self,
    *,
    domainIdentifier: str,
    status: UserProfileStatusType,  # (1)
    userIdentifier: str,
    type: UserProfileTypeType = ...,  # (2)
) -> UpdateUserProfileOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: UserProfileStatusType](./literals.md#userprofilestatustype) 
2. See [:material-code-brackets: UserProfileTypeType](./literals.md#userprofiletypetype) 
3. See [:material-code-braces: UpdateUserProfileOutputTypeDef](./type_defs.md#updateuserprofileoutputtypedef) 


```python
# update_user_profile method usage example with argument unpacking

kwargs: UpdateUserProfileInputRequestTypeDef = {  # (1)
    "domainIdentifier": ...,
    "status": ...,
    "userIdentifier": ...,
}

parent.update_user_profile(**kwargs)
```

1. See [:material-code-braces: UpdateUserProfileInputRequestTypeDef](./type_defs.md#updateuserprofileinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("datazone").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> DataZoneClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("datazone").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.__aexit__)

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




### get_paginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator` method with overloads.

- `client.get_paginator("list_asset_revisions")` -> [ListAssetRevisionsPaginator](./paginators.md#listassetrevisionspaginator)
- `client.get_paginator("list_data_source_run_activities")` -> [ListDataSourceRunActivitiesPaginator](./paginators.md#listdatasourcerunactivitiespaginator)
- `client.get_paginator("list_data_source_runs")` -> [ListDataSourceRunsPaginator](./paginators.md#listdatasourcerunspaginator)
- `client.get_paginator("list_data_sources")` -> [ListDataSourcesPaginator](./paginators.md#listdatasourcespaginator)
- `client.get_paginator("list_domains")` -> [ListDomainsPaginator](./paginators.md#listdomainspaginator)
- `client.get_paginator("list_environment_blueprint_configurations")` -> [ListEnvironmentBlueprintConfigurationsPaginator](./paginators.md#listenvironmentblueprintconfigurationspaginator)
- `client.get_paginator("list_environment_blueprints")` -> [ListEnvironmentBlueprintsPaginator](./paginators.md#listenvironmentblueprintspaginator)
- `client.get_paginator("list_environment_profiles")` -> [ListEnvironmentProfilesPaginator](./paginators.md#listenvironmentprofilespaginator)
- `client.get_paginator("list_environments")` -> [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
- `client.get_paginator("list_notifications")` -> [ListNotificationsPaginator](./paginators.md#listnotificationspaginator)
- `client.get_paginator("list_project_memberships")` -> [ListProjectMembershipsPaginator](./paginators.md#listprojectmembershipspaginator)
- `client.get_paginator("list_projects")` -> [ListProjectsPaginator](./paginators.md#listprojectspaginator)
- `client.get_paginator("list_subscription_grants")` -> [ListSubscriptionGrantsPaginator](./paginators.md#listsubscriptiongrantspaginator)
- `client.get_paginator("list_subscription_requests")` -> [ListSubscriptionRequestsPaginator](./paginators.md#listsubscriptionrequestspaginator)
- `client.get_paginator("list_subscription_targets")` -> [ListSubscriptionTargetsPaginator](./paginators.md#listsubscriptiontargetspaginator)
- `client.get_paginator("list_subscriptions")` -> [ListSubscriptionsPaginator](./paginators.md#listsubscriptionspaginator)
- `client.get_paginator("search")` -> [SearchPaginator](./paginators.md#searchpaginator)
- `client.get_paginator("search_group_profiles")` -> [SearchGroupProfilesPaginator](./paginators.md#searchgroupprofilespaginator)
- `client.get_paginator("search_listings")` -> [SearchListingsPaginator](./paginators.md#searchlistingspaginator)
- `client.get_paginator("search_types")` -> [SearchTypesPaginator](./paginators.md#searchtypespaginator)
- `client.get_paginator("search_user_profiles")` -> [SearchUserProfilesPaginator](./paginators.md#searchuserprofilespaginator)



