# AuditManagerClient

> [Index](../README.md) > [AuditManager](./README.md) > AuditManagerClient

!!! note ""

    Auto-generated documentation for [AuditManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#auditmanager)
    type annotations stubs module [types-aiobotocore-auditmanager](https://pypi.org/project/types-aiobotocore-auditmanager/).

## AuditManagerClient

Type annotations and code completion for `#!python session.client("auditmanager")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# AuditManagerClient usage example

from aioboto3.session import Session
from types_aiobotocore_auditmanager.client import AuditManagerClient

session = Session()
async with session.client("auditmanager") as client:
    client: AuditManagerClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("auditmanager").exceptions` structure.

```python
# AuditManagerClient.exceptions usage example

async with session.client("auditmanager") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# AuditManagerClient.exceptions type checking example

from types_aiobotocore_auditmanager.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("auditmanager").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("auditmanager").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

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


### associate\_assessment\_report\_evidence\_folder

Associates an evidence folder to an assessment report in an Audit Manager
assessment.

Type annotations and code completion for `#!python session.client("auditmanager").associate_assessment_report_evidence_folder` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# associate_assessment_report_evidence_folder method definition

await def associate_assessment_report_evidence_folder(
    self,
    *,
    assessmentId: str,
    evidenceFolderId: str,
) -> dict[str, Any]:
    ...
```



```python
# associate_assessment_report_evidence_folder method usage example with argument unpacking

kwargs: AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
    "evidenceFolderId": ...,
}

parent.associate_assessment_report_evidence_folder(**kwargs)
```

1. See [:material-code-braces: AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef](./type_defs.md#associateassessmentreportevidencefolderrequestrequesttypedef) 

### batch\_associate\_assessment\_report\_evidence

Associates a list of evidence to an assessment report in an Audit Manager
assessment.

Type annotations and code completion for `#!python session.client("auditmanager").batch_associate_assessment_report_evidence` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# batch_associate_assessment_report_evidence method definition

await def batch_associate_assessment_report_evidence(
    self,
    *,
    assessmentId: str,
    evidenceFolderId: str,
    evidenceIds: Sequence[str],
) -> BatchAssociateAssessmentReportEvidenceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchAssociateAssessmentReportEvidenceResponseTypeDef](./type_defs.md#batchassociateassessmentreportevidenceresponsetypedef) 


```python
# batch_associate_assessment_report_evidence method usage example with argument unpacking

kwargs: BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
    "evidenceFolderId": ...,
    "evidenceIds": ...,
}

parent.batch_associate_assessment_report_evidence(**kwargs)
```

1. See [:material-code-braces: BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef](./type_defs.md#batchassociateassessmentreportevidencerequestrequesttypedef) 

### batch\_create\_delegation\_by\_assessment

Creates a batch of delegations for an assessment in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").batch_create_delegation_by_assessment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# batch_create_delegation_by_assessment method definition

await def batch_create_delegation_by_assessment(
    self,
    *,
    createDelegationRequests: Sequence[CreateDelegationRequestTypeDef],  # (1)
    assessmentId: str,
) -> BatchCreateDelegationByAssessmentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CreateDelegationRequestTypeDef](./type_defs.md#createdelegationrequesttypedef) 
2. See [:material-code-braces: BatchCreateDelegationByAssessmentResponseTypeDef](./type_defs.md#batchcreatedelegationbyassessmentresponsetypedef) 


```python
# batch_create_delegation_by_assessment method usage example with argument unpacking

kwargs: BatchCreateDelegationByAssessmentRequestRequestTypeDef = {  # (1)
    "createDelegationRequests": ...,
    "assessmentId": ...,
}

parent.batch_create_delegation_by_assessment(**kwargs)
```

1. See [:material-code-braces: BatchCreateDelegationByAssessmentRequestRequestTypeDef](./type_defs.md#batchcreatedelegationbyassessmentrequestrequesttypedef) 

### batch\_delete\_delegation\_by\_assessment

Deletes a batch of delegations for an assessment in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").batch_delete_delegation_by_assessment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# batch_delete_delegation_by_assessment method definition

await def batch_delete_delegation_by_assessment(
    self,
    *,
    delegationIds: Sequence[str],
    assessmentId: str,
) -> BatchDeleteDelegationByAssessmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDeleteDelegationByAssessmentResponseTypeDef](./type_defs.md#batchdeletedelegationbyassessmentresponsetypedef) 


```python
# batch_delete_delegation_by_assessment method usage example with argument unpacking

kwargs: BatchDeleteDelegationByAssessmentRequestRequestTypeDef = {  # (1)
    "delegationIds": ...,
    "assessmentId": ...,
}

parent.batch_delete_delegation_by_assessment(**kwargs)
```

1. See [:material-code-braces: BatchDeleteDelegationByAssessmentRequestRequestTypeDef](./type_defs.md#batchdeletedelegationbyassessmentrequestrequesttypedef) 

### batch\_disassociate\_assessment\_report\_evidence

Disassociates a list of evidence from an assessment report in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").batch_disassociate_assessment_report_evidence` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# batch_disassociate_assessment_report_evidence method definition

await def batch_disassociate_assessment_report_evidence(
    self,
    *,
    assessmentId: str,
    evidenceFolderId: str,
    evidenceIds: Sequence[str],
) -> BatchDisassociateAssessmentReportEvidenceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDisassociateAssessmentReportEvidenceResponseTypeDef](./type_defs.md#batchdisassociateassessmentreportevidenceresponsetypedef) 


```python
# batch_disassociate_assessment_report_evidence method usage example with argument unpacking

kwargs: BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
    "evidenceFolderId": ...,
    "evidenceIds": ...,
}

parent.batch_disassociate_assessment_report_evidence(**kwargs)
```

1. See [:material-code-braces: BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef](./type_defs.md#batchdisassociateassessmentreportevidencerequestrequesttypedef) 

### batch\_import\_evidence\_to\_assessment\_control

Adds one or more pieces of evidence to a control in an Audit Manager assessment.

Type annotations and code completion for `#!python session.client("auditmanager").batch_import_evidence_to_assessment_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# batch_import_evidence_to_assessment_control method definition

await def batch_import_evidence_to_assessment_control(
    self,
    *,
    assessmentId: str,
    controlSetId: str,
    controlId: str,
    manualEvidence: Sequence[ManualEvidenceTypeDef],  # (1)
) -> BatchImportEvidenceToAssessmentControlResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ManualEvidenceTypeDef](./type_defs.md#manualevidencetypedef) 
2. See [:material-code-braces: BatchImportEvidenceToAssessmentControlResponseTypeDef](./type_defs.md#batchimportevidencetoassessmentcontrolresponsetypedef) 


```python
# batch_import_evidence_to_assessment_control method usage example with argument unpacking

kwargs: BatchImportEvidenceToAssessmentControlRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
    "controlSetId": ...,
    "controlId": ...,
    "manualEvidence": ...,
}

parent.batch_import_evidence_to_assessment_control(**kwargs)
```

1. See [:material-code-braces: BatchImportEvidenceToAssessmentControlRequestRequestTypeDef](./type_defs.md#batchimportevidencetoassessmentcontrolrequestrequesttypedef) 

### create\_assessment

Creates an assessment in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").create_assessment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# create_assessment method definition

await def create_assessment(
    self,
    *,
    name: str,
    assessmentReportsDestination: AssessmentReportsDestinationTypeDef,  # (1)
    scope: ScopeTypeDef,  # (2)
    roles: Sequence[RoleTypeDef],  # (3)
    frameworkId: str,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateAssessmentResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: AssessmentReportsDestinationTypeDef](./type_defs.md#assessmentreportsdestinationtypedef) 
2. See [:material-code-braces: ScopeTypeDef](./type_defs.md#scopetypedef) 
3. See [:material-code-braces: RoleTypeDef](./type_defs.md#roletypedef) 
4. See [:material-code-braces: CreateAssessmentResponseTypeDef](./type_defs.md#createassessmentresponsetypedef) 


```python
# create_assessment method usage example with argument unpacking

kwargs: CreateAssessmentRequestRequestTypeDef = {  # (1)
    "name": ...,
    "assessmentReportsDestination": ...,
    "scope": ...,
    "roles": ...,
    "frameworkId": ...,
}

parent.create_assessment(**kwargs)
```

1. See [:material-code-braces: CreateAssessmentRequestRequestTypeDef](./type_defs.md#createassessmentrequestrequesttypedef) 

### create\_assessment\_framework

Creates a custom framework in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").create_assessment_framework` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# create_assessment_framework method definition

await def create_assessment_framework(
    self,
    *,
    name: str,
    controlSets: Sequence[CreateAssessmentFrameworkControlSetTypeDef],  # (1)
    description: str = ...,
    complianceType: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateAssessmentFrameworkResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CreateAssessmentFrameworkControlSetTypeDef](./type_defs.md#createassessmentframeworkcontrolsettypedef) 
2. See [:material-code-braces: CreateAssessmentFrameworkResponseTypeDef](./type_defs.md#createassessmentframeworkresponsetypedef) 


```python
# create_assessment_framework method usage example with argument unpacking

kwargs: CreateAssessmentFrameworkRequestRequestTypeDef = {  # (1)
    "name": ...,
    "controlSets": ...,
}

parent.create_assessment_framework(**kwargs)
```

1. See [:material-code-braces: CreateAssessmentFrameworkRequestRequestTypeDef](./type_defs.md#createassessmentframeworkrequestrequesttypedef) 

### create\_assessment\_report

Creates an assessment report for the specified assessment.

Type annotations and code completion for `#!python session.client("auditmanager").create_assessment_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# create_assessment_report method definition

await def create_assessment_report(
    self,
    *,
    name: str,
    assessmentId: str,
    description: str = ...,
    queryStatement: str = ...,
) -> CreateAssessmentReportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateAssessmentReportResponseTypeDef](./type_defs.md#createassessmentreportresponsetypedef) 


```python
# create_assessment_report method usage example with argument unpacking

kwargs: CreateAssessmentReportRequestRequestTypeDef = {  # (1)
    "name": ...,
    "assessmentId": ...,
}

parent.create_assessment_report(**kwargs)
```

1. See [:material-code-braces: CreateAssessmentReportRequestRequestTypeDef](./type_defs.md#createassessmentreportrequestrequesttypedef) 

### create\_control

Creates a new custom control in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").create_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# create_control method definition

await def create_control(
    self,
    *,
    name: str,
    controlMappingSources: Sequence[CreateControlMappingSourceTypeDef],  # (1)
    description: str = ...,
    testingInformation: str = ...,
    actionPlanTitle: str = ...,
    actionPlanInstructions: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateControlResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CreateControlMappingSourceTypeDef](./type_defs.md#createcontrolmappingsourcetypedef) 
2. See [:material-code-braces: CreateControlResponseTypeDef](./type_defs.md#createcontrolresponsetypedef) 


```python
# create_control method usage example with argument unpacking

kwargs: CreateControlRequestRequestTypeDef = {  # (1)
    "name": ...,
    "controlMappingSources": ...,
}

parent.create_control(**kwargs)
```

1. See [:material-code-braces: CreateControlRequestRequestTypeDef](./type_defs.md#createcontrolrequestrequesttypedef) 

### delete\_assessment

Deletes an assessment in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").delete_assessment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# delete_assessment method definition

await def delete_assessment(
    self,
    *,
    assessmentId: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_assessment method usage example with argument unpacking

kwargs: DeleteAssessmentRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
}

parent.delete_assessment(**kwargs)
```

1. See [:material-code-braces: DeleteAssessmentRequestRequestTypeDef](./type_defs.md#deleteassessmentrequestrequesttypedef) 

### delete\_assessment\_framework

Deletes a custom framework in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").delete_assessment_framework` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# delete_assessment_framework method definition

await def delete_assessment_framework(
    self,
    *,
    frameworkId: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_assessment_framework method usage example with argument unpacking

kwargs: DeleteAssessmentFrameworkRequestRequestTypeDef = {  # (1)
    "frameworkId": ...,
}

parent.delete_assessment_framework(**kwargs)
```

1. See [:material-code-braces: DeleteAssessmentFrameworkRequestRequestTypeDef](./type_defs.md#deleteassessmentframeworkrequestrequesttypedef) 

### delete\_assessment\_framework\_share

Deletes a share request for a custom framework in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").delete_assessment_framework_share` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# delete_assessment_framework_share method definition

await def delete_assessment_framework_share(
    self,
    *,
    requestId: str,
    requestType: ShareRequestTypeType,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ShareRequestTypeType](./literals.md#sharerequesttypetype) 


```python
# delete_assessment_framework_share method usage example with argument unpacking

kwargs: DeleteAssessmentFrameworkShareRequestRequestTypeDef = {  # (1)
    "requestId": ...,
    "requestType": ...,
}

parent.delete_assessment_framework_share(**kwargs)
```

1. See [:material-code-braces: DeleteAssessmentFrameworkShareRequestRequestTypeDef](./type_defs.md#deleteassessmentframeworksharerequestrequesttypedef) 

### delete\_assessment\_report

Deletes an assessment report in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").delete_assessment_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# delete_assessment_report method definition

await def delete_assessment_report(
    self,
    *,
    assessmentId: str,
    assessmentReportId: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_assessment_report method usage example with argument unpacking

kwargs: DeleteAssessmentReportRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
    "assessmentReportId": ...,
}

parent.delete_assessment_report(**kwargs)
```

1. See [:material-code-braces: DeleteAssessmentReportRequestRequestTypeDef](./type_defs.md#deleteassessmentreportrequestrequesttypedef) 

### delete\_control

Deletes a custom control in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").delete_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# delete_control method definition

await def delete_control(
    self,
    *,
    controlId: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_control method usage example with argument unpacking

kwargs: DeleteControlRequestRequestTypeDef = {  # (1)
    "controlId": ...,
}

parent.delete_control(**kwargs)
```

1. See [:material-code-braces: DeleteControlRequestRequestTypeDef](./type_defs.md#deletecontrolrequestrequesttypedef) 

### deregister\_account

Deregisters an account in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").deregister_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# deregister_account method definition

await def deregister_account(
    self,
) -> DeregisterAccountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeregisterAccountResponseTypeDef](./type_defs.md#deregisteraccountresponsetypedef) 

### deregister\_organization\_admin\_account

Removes the specified Amazon Web Services account as a delegated administrator
for Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").deregister_organization_admin_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# deregister_organization_admin_account method definition

await def deregister_organization_admin_account(
    self,
    *,
    adminAccountId: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# deregister_organization_admin_account method usage example with argument unpacking

kwargs: DeregisterOrganizationAdminAccountRequestRequestTypeDef = {  # (1)
    "adminAccountId": ...,
}

parent.deregister_organization_admin_account(**kwargs)
```

1. See [:material-code-braces: DeregisterOrganizationAdminAccountRequestRequestTypeDef](./type_defs.md#deregisterorganizationadminaccountrequestrequesttypedef) 

### disassociate\_assessment\_report\_evidence\_folder

Disassociates an evidence folder from the specified assessment report in Audit
Manager.

Type annotations and code completion for `#!python session.client("auditmanager").disassociate_assessment_report_evidence_folder` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# disassociate_assessment_report_evidence_folder method definition

await def disassociate_assessment_report_evidence_folder(
    self,
    *,
    assessmentId: str,
    evidenceFolderId: str,
) -> dict[str, Any]:
    ...
```



```python
# disassociate_assessment_report_evidence_folder method usage example with argument unpacking

kwargs: DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
    "evidenceFolderId": ...,
}

parent.disassociate_assessment_report_evidence_folder(**kwargs)
```

1. See [:material-code-braces: DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef](./type_defs.md#disassociateassessmentreportevidencefolderrequestrequesttypedef) 

### get\_account\_status

Gets the registration status of an account in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").get_account_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# get_account_status method definition

await def get_account_status(
    self,
) -> GetAccountStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccountStatusResponseTypeDef](./type_defs.md#getaccountstatusresponsetypedef) 

### get\_assessment

Gets information about a specified assessment.

Type annotations and code completion for `#!python session.client("auditmanager").get_assessment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# get_assessment method definition

await def get_assessment(
    self,
    *,
    assessmentId: str,
) -> GetAssessmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAssessmentResponseTypeDef](./type_defs.md#getassessmentresponsetypedef) 


```python
# get_assessment method usage example with argument unpacking

kwargs: GetAssessmentRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
}

parent.get_assessment(**kwargs)
```

1. See [:material-code-braces: GetAssessmentRequestRequestTypeDef](./type_defs.md#getassessmentrequestrequesttypedef) 

### get\_assessment\_framework

Gets information about a specified framework.

Type annotations and code completion for `#!python session.client("auditmanager").get_assessment_framework` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# get_assessment_framework method definition

await def get_assessment_framework(
    self,
    *,
    frameworkId: str,
) -> GetAssessmentFrameworkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAssessmentFrameworkResponseTypeDef](./type_defs.md#getassessmentframeworkresponsetypedef) 


```python
# get_assessment_framework method usage example with argument unpacking

kwargs: GetAssessmentFrameworkRequestRequestTypeDef = {  # (1)
    "frameworkId": ...,
}

parent.get_assessment_framework(**kwargs)
```

1. See [:material-code-braces: GetAssessmentFrameworkRequestRequestTypeDef](./type_defs.md#getassessmentframeworkrequestrequesttypedef) 

### get\_assessment\_report\_url

Gets the URL of an assessment report in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").get_assessment_report_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# get_assessment_report_url method definition

await def get_assessment_report_url(
    self,
    *,
    assessmentReportId: str,
    assessmentId: str,
) -> GetAssessmentReportUrlResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAssessmentReportUrlResponseTypeDef](./type_defs.md#getassessmentreporturlresponsetypedef) 


```python
# get_assessment_report_url method usage example with argument unpacking

kwargs: GetAssessmentReportUrlRequestRequestTypeDef = {  # (1)
    "assessmentReportId": ...,
    "assessmentId": ...,
}

parent.get_assessment_report_url(**kwargs)
```

1. See [:material-code-braces: GetAssessmentReportUrlRequestRequestTypeDef](./type_defs.md#getassessmentreporturlrequestrequesttypedef) 

### get\_change\_logs

Gets a list of changelogs from Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").get_change_logs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# get_change_logs method definition

await def get_change_logs(
    self,
    *,
    assessmentId: str,
    controlSetId: str = ...,
    controlId: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> GetChangeLogsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetChangeLogsResponseTypeDef](./type_defs.md#getchangelogsresponsetypedef) 


```python
# get_change_logs method usage example with argument unpacking

kwargs: GetChangeLogsRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
}

parent.get_change_logs(**kwargs)
```

1. See [:material-code-braces: GetChangeLogsRequestRequestTypeDef](./type_defs.md#getchangelogsrequestrequesttypedef) 

### get\_control

Gets information about a specified control.

Type annotations and code completion for `#!python session.client("auditmanager").get_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# get_control method definition

await def get_control(
    self,
    *,
    controlId: str,
) -> GetControlResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetControlResponseTypeDef](./type_defs.md#getcontrolresponsetypedef) 


```python
# get_control method usage example with argument unpacking

kwargs: GetControlRequestRequestTypeDef = {  # (1)
    "controlId": ...,
}

parent.get_control(**kwargs)
```

1. See [:material-code-braces: GetControlRequestRequestTypeDef](./type_defs.md#getcontrolrequestrequesttypedef) 

### get\_delegations

Gets a list of delegations from an audit owner to a delegate.

Type annotations and code completion for `#!python session.client("auditmanager").get_delegations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# get_delegations method definition

await def get_delegations(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> GetDelegationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDelegationsResponseTypeDef](./type_defs.md#getdelegationsresponsetypedef) 


```python
# get_delegations method usage example with argument unpacking

kwargs: GetDelegationsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.get_delegations(**kwargs)
```

1. See [:material-code-braces: GetDelegationsRequestRequestTypeDef](./type_defs.md#getdelegationsrequestrequesttypedef) 

### get\_evidence

Gets information about a specified evidence item.

Type annotations and code completion for `#!python session.client("auditmanager").get_evidence` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# get_evidence method definition

await def get_evidence(
    self,
    *,
    assessmentId: str,
    controlSetId: str,
    evidenceFolderId: str,
    evidenceId: str,
) -> GetEvidenceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEvidenceResponseTypeDef](./type_defs.md#getevidenceresponsetypedef) 


```python
# get_evidence method usage example with argument unpacking

kwargs: GetEvidenceRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
    "controlSetId": ...,
    "evidenceFolderId": ...,
    "evidenceId": ...,
}

parent.get_evidence(**kwargs)
```

1. See [:material-code-braces: GetEvidenceRequestRequestTypeDef](./type_defs.md#getevidencerequestrequesttypedef) 

### get\_evidence\_by\_evidence\_folder

Gets all evidence from a specified evidence folder in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").get_evidence_by_evidence_folder` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# get_evidence_by_evidence_folder method definition

await def get_evidence_by_evidence_folder(
    self,
    *,
    assessmentId: str,
    controlSetId: str,
    evidenceFolderId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> GetEvidenceByEvidenceFolderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEvidenceByEvidenceFolderResponseTypeDef](./type_defs.md#getevidencebyevidencefolderresponsetypedef) 


```python
# get_evidence_by_evidence_folder method usage example with argument unpacking

kwargs: GetEvidenceByEvidenceFolderRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
    "controlSetId": ...,
    "evidenceFolderId": ...,
}

parent.get_evidence_by_evidence_folder(**kwargs)
```

1. See [:material-code-braces: GetEvidenceByEvidenceFolderRequestRequestTypeDef](./type_defs.md#getevidencebyevidencefolderrequestrequesttypedef) 

### get\_evidence\_file\_upload\_url

Creates a presigned Amazon S3 URL that can be used to upload a file as manual
evidence.

Type annotations and code completion for `#!python session.client("auditmanager").get_evidence_file_upload_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# get_evidence_file_upload_url method definition

await def get_evidence_file_upload_url(
    self,
    *,
    fileName: str,
) -> GetEvidenceFileUploadUrlResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEvidenceFileUploadUrlResponseTypeDef](./type_defs.md#getevidencefileuploadurlresponsetypedef) 


```python
# get_evidence_file_upload_url method usage example with argument unpacking

kwargs: GetEvidenceFileUploadUrlRequestRequestTypeDef = {  # (1)
    "fileName": ...,
}

parent.get_evidence_file_upload_url(**kwargs)
```

1. See [:material-code-braces: GetEvidenceFileUploadUrlRequestRequestTypeDef](./type_defs.md#getevidencefileuploadurlrequestrequesttypedef) 

### get\_evidence\_folder

Gets an evidence folder from a specified assessment in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").get_evidence_folder` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# get_evidence_folder method definition

await def get_evidence_folder(
    self,
    *,
    assessmentId: str,
    controlSetId: str,
    evidenceFolderId: str,
) -> GetEvidenceFolderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEvidenceFolderResponseTypeDef](./type_defs.md#getevidencefolderresponsetypedef) 


```python
# get_evidence_folder method usage example with argument unpacking

kwargs: GetEvidenceFolderRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
    "controlSetId": ...,
    "evidenceFolderId": ...,
}

parent.get_evidence_folder(**kwargs)
```

1. See [:material-code-braces: GetEvidenceFolderRequestRequestTypeDef](./type_defs.md#getevidencefolderrequestrequesttypedef) 

### get\_evidence\_folders\_by\_assessment

Gets the evidence folders from a specified assessment in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").get_evidence_folders_by_assessment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# get_evidence_folders_by_assessment method definition

await def get_evidence_folders_by_assessment(
    self,
    *,
    assessmentId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> GetEvidenceFoldersByAssessmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEvidenceFoldersByAssessmentResponseTypeDef](./type_defs.md#getevidencefoldersbyassessmentresponsetypedef) 


```python
# get_evidence_folders_by_assessment method usage example with argument unpacking

kwargs: GetEvidenceFoldersByAssessmentRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
}

parent.get_evidence_folders_by_assessment(**kwargs)
```

1. See [:material-code-braces: GetEvidenceFoldersByAssessmentRequestRequestTypeDef](./type_defs.md#getevidencefoldersbyassessmentrequestrequesttypedef) 

### get\_evidence\_folders\_by\_assessment\_control

Gets a list of evidence folders that are associated with a specified control in
an Audit Manager assessment.

Type annotations and code completion for `#!python session.client("auditmanager").get_evidence_folders_by_assessment_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# get_evidence_folders_by_assessment_control method definition

await def get_evidence_folders_by_assessment_control(
    self,
    *,
    assessmentId: str,
    controlSetId: str,
    controlId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> GetEvidenceFoldersByAssessmentControlResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEvidenceFoldersByAssessmentControlResponseTypeDef](./type_defs.md#getevidencefoldersbyassessmentcontrolresponsetypedef) 


```python
# get_evidence_folders_by_assessment_control method usage example with argument unpacking

kwargs: GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
    "controlSetId": ...,
    "controlId": ...,
}

parent.get_evidence_folders_by_assessment_control(**kwargs)
```

1. See [:material-code-braces: GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef](./type_defs.md#getevidencefoldersbyassessmentcontrolrequestrequesttypedef) 

### get\_insights

Gets the latest analytics data for all your current active assessments.

Type annotations and code completion for `#!python session.client("auditmanager").get_insights` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# get_insights method definition

await def get_insights(
    self,
) -> GetInsightsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInsightsResponseTypeDef](./type_defs.md#getinsightsresponsetypedef) 

### get\_insights\_by\_assessment

Gets the latest analytics data for a specific active assessment.

Type annotations and code completion for `#!python session.client("auditmanager").get_insights_by_assessment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# get_insights_by_assessment method definition

await def get_insights_by_assessment(
    self,
    *,
    assessmentId: str,
) -> GetInsightsByAssessmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInsightsByAssessmentResponseTypeDef](./type_defs.md#getinsightsbyassessmentresponsetypedef) 


```python
# get_insights_by_assessment method usage example with argument unpacking

kwargs: GetInsightsByAssessmentRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
}

parent.get_insights_by_assessment(**kwargs)
```

1. See [:material-code-braces: GetInsightsByAssessmentRequestRequestTypeDef](./type_defs.md#getinsightsbyassessmentrequestrequesttypedef) 

### get\_organization\_admin\_account

Gets the name of the delegated Amazon Web Services administrator account for a
specified organization.

Type annotations and code completion for `#!python session.client("auditmanager").get_organization_admin_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# get_organization_admin_account method definition

await def get_organization_admin_account(
    self,
) -> GetOrganizationAdminAccountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOrganizationAdminAccountResponseTypeDef](./type_defs.md#getorganizationadminaccountresponsetypedef) 

### get\_services\_in\_scope

Gets a list of the Amazon Web Services from which Audit Manager can collect
evidence.

Type annotations and code completion for `#!python session.client("auditmanager").get_services_in_scope` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# get_services_in_scope method definition

await def get_services_in_scope(
    self,
) -> GetServicesInScopeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServicesInScopeResponseTypeDef](./type_defs.md#getservicesinscoperesponsetypedef) 

### get\_settings

Gets the settings for a specified Amazon Web Services account.

Type annotations and code completion for `#!python session.client("auditmanager").get_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# get_settings method definition

await def get_settings(
    self,
    *,
    attribute: SettingAttributeType,  # (1)
) -> GetSettingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SettingAttributeType](./literals.md#settingattributetype) 
2. See [:material-code-braces: GetSettingsResponseTypeDef](./type_defs.md#getsettingsresponsetypedef) 


```python
# get_settings method usage example with argument unpacking

kwargs: GetSettingsRequestRequestTypeDef = {  # (1)
    "attribute": ...,
}

parent.get_settings(**kwargs)
```

1. See [:material-code-braces: GetSettingsRequestRequestTypeDef](./type_defs.md#getsettingsrequestrequesttypedef) 

### list\_assessment\_control\_insights\_by\_control\_domain

Lists the latest analytics data for controls within a specific control domain
and a specific active assessment.

Type annotations and code completion for `#!python session.client("auditmanager").list_assessment_control_insights_by_control_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# list_assessment_control_insights_by_control_domain method definition

await def list_assessment_control_insights_by_control_domain(
    self,
    *,
    controlDomainId: str,
    assessmentId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAssessmentControlInsightsByControlDomainResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAssessmentControlInsightsByControlDomainResponseTypeDef](./type_defs.md#listassessmentcontrolinsightsbycontroldomainresponsetypedef) 


```python
# list_assessment_control_insights_by_control_domain method usage example with argument unpacking

kwargs: ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef = {  # (1)
    "controlDomainId": ...,
    "assessmentId": ...,
}

parent.list_assessment_control_insights_by_control_domain(**kwargs)
```

1. See [:material-code-braces: ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef](./type_defs.md#listassessmentcontrolinsightsbycontroldomainrequestrequesttypedef) 

### list\_assessment\_framework\_share\_requests

Returns a list of sent or received share requests for custom frameworks in
Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").list_assessment_framework_share_requests` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# list_assessment_framework_share_requests method definition

await def list_assessment_framework_share_requests(
    self,
    *,
    requestType: ShareRequestTypeType,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAssessmentFrameworkShareRequestsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ShareRequestTypeType](./literals.md#sharerequesttypetype) 
2. See [:material-code-braces: ListAssessmentFrameworkShareRequestsResponseTypeDef](./type_defs.md#listassessmentframeworksharerequestsresponsetypedef) 


```python
# list_assessment_framework_share_requests method usage example with argument unpacking

kwargs: ListAssessmentFrameworkShareRequestsRequestRequestTypeDef = {  # (1)
    "requestType": ...,
}

parent.list_assessment_framework_share_requests(**kwargs)
```

1. See [:material-code-braces: ListAssessmentFrameworkShareRequestsRequestRequestTypeDef](./type_defs.md#listassessmentframeworksharerequestsrequestrequesttypedef) 

### list\_assessment\_frameworks

Returns a list of the frameworks that are available in the Audit Manager
framework library.

Type annotations and code completion for `#!python session.client("auditmanager").list_assessment_frameworks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# list_assessment_frameworks method definition

await def list_assessment_frameworks(
    self,
    *,
    frameworkType: FrameworkTypeType,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAssessmentFrameworksResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: FrameworkTypeType](./literals.md#frameworktypetype) 
2. See [:material-code-braces: ListAssessmentFrameworksResponseTypeDef](./type_defs.md#listassessmentframeworksresponsetypedef) 


```python
# list_assessment_frameworks method usage example with argument unpacking

kwargs: ListAssessmentFrameworksRequestRequestTypeDef = {  # (1)
    "frameworkType": ...,
}

parent.list_assessment_frameworks(**kwargs)
```

1. See [:material-code-braces: ListAssessmentFrameworksRequestRequestTypeDef](./type_defs.md#listassessmentframeworksrequestrequesttypedef) 

### list\_assessment\_reports

Returns a list of assessment reports created in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").list_assessment_reports` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# list_assessment_reports method definition

await def list_assessment_reports(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAssessmentReportsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAssessmentReportsResponseTypeDef](./type_defs.md#listassessmentreportsresponsetypedef) 


```python
# list_assessment_reports method usage example with argument unpacking

kwargs: ListAssessmentReportsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_assessment_reports(**kwargs)
```

1. See [:material-code-braces: ListAssessmentReportsRequestRequestTypeDef](./type_defs.md#listassessmentreportsrequestrequesttypedef) 

### list\_assessments

Returns a list of current and past assessments from Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").list_assessments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# list_assessments method definition

await def list_assessments(
    self,
    *,
    status: AssessmentStatusType = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAssessmentsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AssessmentStatusType](./literals.md#assessmentstatustype) 
2. See [:material-code-braces: ListAssessmentsResponseTypeDef](./type_defs.md#listassessmentsresponsetypedef) 


```python
# list_assessments method usage example with argument unpacking

kwargs: ListAssessmentsRequestRequestTypeDef = {  # (1)
    "status": ...,
}

parent.list_assessments(**kwargs)
```

1. See [:material-code-braces: ListAssessmentsRequestRequestTypeDef](./type_defs.md#listassessmentsrequestrequesttypedef) 

### list\_control\_domain\_insights

Lists the latest analytics data for control domains across all of your active
assessments.

Type annotations and code completion for `#!python session.client("auditmanager").list_control_domain_insights` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# list_control_domain_insights method definition

await def list_control_domain_insights(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListControlDomainInsightsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListControlDomainInsightsResponseTypeDef](./type_defs.md#listcontroldomaininsightsresponsetypedef) 


```python
# list_control_domain_insights method usage example with argument unpacking

kwargs: ListControlDomainInsightsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_control_domain_insights(**kwargs)
```

1. See [:material-code-braces: ListControlDomainInsightsRequestRequestTypeDef](./type_defs.md#listcontroldomaininsightsrequestrequesttypedef) 

### list\_control\_domain\_insights\_by\_assessment

Lists analytics data for control domains within a specified active assessment.

Type annotations and code completion for `#!python session.client("auditmanager").list_control_domain_insights_by_assessment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# list_control_domain_insights_by_assessment method definition

await def list_control_domain_insights_by_assessment(
    self,
    *,
    assessmentId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListControlDomainInsightsByAssessmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListControlDomainInsightsByAssessmentResponseTypeDef](./type_defs.md#listcontroldomaininsightsbyassessmentresponsetypedef) 


```python
# list_control_domain_insights_by_assessment method usage example with argument unpacking

kwargs: ListControlDomainInsightsByAssessmentRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
}

parent.list_control_domain_insights_by_assessment(**kwargs)
```

1. See [:material-code-braces: ListControlDomainInsightsByAssessmentRequestRequestTypeDef](./type_defs.md#listcontroldomaininsightsbyassessmentrequestrequesttypedef) 

### list\_control\_insights\_by\_control\_domain

Lists the latest analytics data for controls within a specific control domain
across all active assessments.

Type annotations and code completion for `#!python session.client("auditmanager").list_control_insights_by_control_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# list_control_insights_by_control_domain method definition

await def list_control_insights_by_control_domain(
    self,
    *,
    controlDomainId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListControlInsightsByControlDomainResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListControlInsightsByControlDomainResponseTypeDef](./type_defs.md#listcontrolinsightsbycontroldomainresponsetypedef) 


```python
# list_control_insights_by_control_domain method usage example with argument unpacking

kwargs: ListControlInsightsByControlDomainRequestRequestTypeDef = {  # (1)
    "controlDomainId": ...,
}

parent.list_control_insights_by_control_domain(**kwargs)
```

1. See [:material-code-braces: ListControlInsightsByControlDomainRequestRequestTypeDef](./type_defs.md#listcontrolinsightsbycontroldomainrequestrequesttypedef) 

### list\_controls

Returns a list of controls from Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").list_controls` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# list_controls method definition

await def list_controls(
    self,
    *,
    controlType: ControlTypeType,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
    controlCatalogId: str = ...,
) -> ListControlsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ControlTypeType](./literals.md#controltypetype) 
2. See [:material-code-braces: ListControlsResponseTypeDef](./type_defs.md#listcontrolsresponsetypedef) 


```python
# list_controls method usage example with argument unpacking

kwargs: ListControlsRequestRequestTypeDef = {  # (1)
    "controlType": ...,
}

parent.list_controls(**kwargs)
```

1. See [:material-code-braces: ListControlsRequestRequestTypeDef](./type_defs.md#listcontrolsrequestrequesttypedef) 

### list\_keywords\_for\_data\_source

Returns a list of keywords that are pre-mapped to the specified control data
source.

Type annotations and code completion for `#!python session.client("auditmanager").list_keywords_for_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# list_keywords_for_data_source method definition

await def list_keywords_for_data_source(
    self,
    *,
    source: DataSourceTypeType,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListKeywordsForDataSourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
2. See [:material-code-braces: ListKeywordsForDataSourceResponseTypeDef](./type_defs.md#listkeywordsfordatasourceresponsetypedef) 


```python
# list_keywords_for_data_source method usage example with argument unpacking

kwargs: ListKeywordsForDataSourceRequestRequestTypeDef = {  # (1)
    "source": ...,
}

parent.list_keywords_for_data_source(**kwargs)
```

1. See [:material-code-braces: ListKeywordsForDataSourceRequestRequestTypeDef](./type_defs.md#listkeywordsfordatasourcerequestrequesttypedef) 

### list\_notifications

Returns a list of all Audit Manager notifications.

Type annotations and code completion for `#!python session.client("auditmanager").list_notifications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# list_notifications method definition

await def list_notifications(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListNotificationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListNotificationsResponseTypeDef](./type_defs.md#listnotificationsresponsetypedef) 


```python
# list_notifications method usage example with argument unpacking

kwargs: ListNotificationsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_notifications(**kwargs)
```

1. See [:material-code-braces: ListNotificationsRequestRequestTypeDef](./type_defs.md#listnotificationsrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of tags for the specified resource in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

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

### register\_account

Enables Audit Manager for the specified Amazon Web Services account.

Type annotations and code completion for `#!python session.client("auditmanager").register_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# register_account method definition

await def register_account(
    self,
    *,
    kmsKey: str = ...,
    delegatedAdminAccount: str = ...,
) -> RegisterAccountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RegisterAccountResponseTypeDef](./type_defs.md#registeraccountresponsetypedef) 


```python
# register_account method usage example with argument unpacking

kwargs: RegisterAccountRequestRequestTypeDef = {  # (1)
    "kmsKey": ...,
}

parent.register_account(**kwargs)
```

1. See [:material-code-braces: RegisterAccountRequestRequestTypeDef](./type_defs.md#registeraccountrequestrequesttypedef) 

### register\_organization\_admin\_account

Enables an Amazon Web Services account within the organization as the delegated
administrator for Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").register_organization_admin_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# register_organization_admin_account method definition

await def register_organization_admin_account(
    self,
    *,
    adminAccountId: str,
) -> RegisterOrganizationAdminAccountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RegisterOrganizationAdminAccountResponseTypeDef](./type_defs.md#registerorganizationadminaccountresponsetypedef) 


```python
# register_organization_admin_account method usage example with argument unpacking

kwargs: RegisterOrganizationAdminAccountRequestRequestTypeDef = {  # (1)
    "adminAccountId": ...,
}

parent.register_organization_admin_account(**kwargs)
```

1. See [:material-code-braces: RegisterOrganizationAdminAccountRequestRequestTypeDef](./type_defs.md#registerorganizationadminaccountrequestrequesttypedef) 

### start\_assessment\_framework\_share

Creates a share request for a custom framework in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").start_assessment_framework_share` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# start_assessment_framework_share method definition

await def start_assessment_framework_share(
    self,
    *,
    frameworkId: str,
    destinationAccount: str,
    destinationRegion: str,
    comment: str = ...,
) -> StartAssessmentFrameworkShareResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartAssessmentFrameworkShareResponseTypeDef](./type_defs.md#startassessmentframeworkshareresponsetypedef) 


```python
# start_assessment_framework_share method usage example with argument unpacking

kwargs: StartAssessmentFrameworkShareRequestRequestTypeDef = {  # (1)
    "frameworkId": ...,
    "destinationAccount": ...,
    "destinationRegion": ...,
}

parent.start_assessment_framework_share(**kwargs)
```

1. See [:material-code-braces: StartAssessmentFrameworkShareRequestRequestTypeDef](./type_defs.md#startassessmentframeworksharerequestrequesttypedef) 

### tag\_resource

Tags the specified resource in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> dict[str, Any]:
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

Removes a tag from a resource in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> dict[str, Any]:
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

### update\_assessment

Edits an Audit Manager assessment.

Type annotations and code completion for `#!python session.client("auditmanager").update_assessment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# update_assessment method definition

await def update_assessment(
    self,
    *,
    assessmentId: str,
    scope: ScopeTypeDef,  # (1)
    assessmentName: str = ...,
    assessmentDescription: str = ...,
    assessmentReportsDestination: AssessmentReportsDestinationTypeDef = ...,  # (2)
    roles: Sequence[RoleTypeDef] = ...,  # (3)
) -> UpdateAssessmentResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ScopeTypeDef](./type_defs.md#scopetypedef) 
2. See [:material-code-braces: AssessmentReportsDestinationTypeDef](./type_defs.md#assessmentreportsdestinationtypedef) 
3. See [:material-code-braces: RoleTypeDef](./type_defs.md#roletypedef) 
4. See [:material-code-braces: UpdateAssessmentResponseTypeDef](./type_defs.md#updateassessmentresponsetypedef) 


```python
# update_assessment method usage example with argument unpacking

kwargs: UpdateAssessmentRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
    "scope": ...,
}

parent.update_assessment(**kwargs)
```

1. See [:material-code-braces: UpdateAssessmentRequestRequestTypeDef](./type_defs.md#updateassessmentrequestrequesttypedef) 

### update\_assessment\_control

Updates a control within an assessment in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").update_assessment_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# update_assessment_control method definition

await def update_assessment_control(
    self,
    *,
    assessmentId: str,
    controlSetId: str,
    controlId: str,
    controlStatus: ControlStatusType = ...,  # (1)
    commentBody: str = ...,
) -> UpdateAssessmentControlResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ControlStatusType](./literals.md#controlstatustype) 
2. See [:material-code-braces: UpdateAssessmentControlResponseTypeDef](./type_defs.md#updateassessmentcontrolresponsetypedef) 


```python
# update_assessment_control method usage example with argument unpacking

kwargs: UpdateAssessmentControlRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
    "controlSetId": ...,
    "controlId": ...,
}

parent.update_assessment_control(**kwargs)
```

1. See [:material-code-braces: UpdateAssessmentControlRequestRequestTypeDef](./type_defs.md#updateassessmentcontrolrequestrequesttypedef) 

### update\_assessment\_control\_set\_status

Updates the status of a control set in an Audit Manager assessment.

Type annotations and code completion for `#!python session.client("auditmanager").update_assessment_control_set_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# update_assessment_control_set_status method definition

await def update_assessment_control_set_status(
    self,
    *,
    assessmentId: str,
    controlSetId: str,
    status: ControlSetStatusType,  # (1)
    comment: str,
) -> UpdateAssessmentControlSetStatusResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ControlSetStatusType](./literals.md#controlsetstatustype) 
2. See [:material-code-braces: UpdateAssessmentControlSetStatusResponseTypeDef](./type_defs.md#updateassessmentcontrolsetstatusresponsetypedef) 


```python
# update_assessment_control_set_status method usage example with argument unpacking

kwargs: UpdateAssessmentControlSetStatusRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
    "controlSetId": ...,
    "status": ...,
    "comment": ...,
}

parent.update_assessment_control_set_status(**kwargs)
```

1. See [:material-code-braces: UpdateAssessmentControlSetStatusRequestRequestTypeDef](./type_defs.md#updateassessmentcontrolsetstatusrequestrequesttypedef) 

### update\_assessment\_framework

Updates a custom framework in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").update_assessment_framework` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# update_assessment_framework method definition

await def update_assessment_framework(
    self,
    *,
    frameworkId: str,
    name: str,
    controlSets: Sequence[UpdateAssessmentFrameworkControlSetTypeDef],  # (1)
    description: str = ...,
    complianceType: str = ...,
) -> UpdateAssessmentFrameworkResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UpdateAssessmentFrameworkControlSetTypeDef](./type_defs.md#updateassessmentframeworkcontrolsettypedef) 
2. See [:material-code-braces: UpdateAssessmentFrameworkResponseTypeDef](./type_defs.md#updateassessmentframeworkresponsetypedef) 


```python
# update_assessment_framework method usage example with argument unpacking

kwargs: UpdateAssessmentFrameworkRequestRequestTypeDef = {  # (1)
    "frameworkId": ...,
    "name": ...,
    "controlSets": ...,
}

parent.update_assessment_framework(**kwargs)
```

1. See [:material-code-braces: UpdateAssessmentFrameworkRequestRequestTypeDef](./type_defs.md#updateassessmentframeworkrequestrequesttypedef) 

### update\_assessment\_framework\_share

Updates a share request for a custom framework in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").update_assessment_framework_share` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# update_assessment_framework_share method definition

await def update_assessment_framework_share(
    self,
    *,
    requestId: str,
    requestType: ShareRequestTypeType,  # (1)
    action: ShareRequestActionType,  # (2)
) -> UpdateAssessmentFrameworkShareResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ShareRequestTypeType](./literals.md#sharerequesttypetype) 
2. See [:material-code-brackets: ShareRequestActionType](./literals.md#sharerequestactiontype) 
3. See [:material-code-braces: UpdateAssessmentFrameworkShareResponseTypeDef](./type_defs.md#updateassessmentframeworkshareresponsetypedef) 


```python
# update_assessment_framework_share method usage example with argument unpacking

kwargs: UpdateAssessmentFrameworkShareRequestRequestTypeDef = {  # (1)
    "requestId": ...,
    "requestType": ...,
    "action": ...,
}

parent.update_assessment_framework_share(**kwargs)
```

1. See [:material-code-braces: UpdateAssessmentFrameworkShareRequestRequestTypeDef](./type_defs.md#updateassessmentframeworksharerequestrequesttypedef) 

### update\_assessment\_status

Updates the status of an assessment in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").update_assessment_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# update_assessment_status method definition

await def update_assessment_status(
    self,
    *,
    assessmentId: str,
    status: AssessmentStatusType,  # (1)
) -> UpdateAssessmentStatusResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AssessmentStatusType](./literals.md#assessmentstatustype) 
2. See [:material-code-braces: UpdateAssessmentStatusResponseTypeDef](./type_defs.md#updateassessmentstatusresponsetypedef) 


```python
# update_assessment_status method usage example with argument unpacking

kwargs: UpdateAssessmentStatusRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
    "status": ...,
}

parent.update_assessment_status(**kwargs)
```

1. See [:material-code-braces: UpdateAssessmentStatusRequestRequestTypeDef](./type_defs.md#updateassessmentstatusrequestrequesttypedef) 

### update\_control

Updates a custom control in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").update_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# update_control method definition

await def update_control(
    self,
    *,
    controlId: str,
    name: str,
    controlMappingSources: Sequence[ControlMappingSourceTypeDef],  # (1)
    description: str = ...,
    testingInformation: str = ...,
    actionPlanTitle: str = ...,
    actionPlanInstructions: str = ...,
) -> UpdateControlResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ControlMappingSourceTypeDef](./type_defs.md#controlmappingsourcetypedef) 
2. See [:material-code-braces: UpdateControlResponseTypeDef](./type_defs.md#updatecontrolresponsetypedef) 


```python
# update_control method usage example with argument unpacking

kwargs: UpdateControlRequestRequestTypeDef = {  # (1)
    "controlId": ...,
    "name": ...,
    "controlMappingSources": ...,
}

parent.update_control(**kwargs)
```

1. See [:material-code-braces: UpdateControlRequestRequestTypeDef](./type_defs.md#updatecontrolrequestrequesttypedef) 

### update\_settings

Updates Audit Manager settings for the current account.

Type annotations and code completion for `#!python session.client("auditmanager").update_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# update_settings method definition

await def update_settings(
    self,
    *,
    snsTopic: str = ...,
    defaultAssessmentReportsDestination: AssessmentReportsDestinationTypeDef = ...,  # (1)
    defaultProcessOwners: Sequence[RoleTypeDef] = ...,  # (2)
    kmsKey: str = ...,
    evidenceFinderEnabled: bool = ...,
    deregistrationPolicy: DeregistrationPolicyTypeDef = ...,  # (3)
    defaultExportDestination: DefaultExportDestinationTypeDef = ...,  # (4)
) -> UpdateSettingsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: AssessmentReportsDestinationTypeDef](./type_defs.md#assessmentreportsdestinationtypedef) 
2. See [:material-code-braces: RoleTypeDef](./type_defs.md#roletypedef) 
3. See [:material-code-braces: DeregistrationPolicyTypeDef](./type_defs.md#deregistrationpolicytypedef) 
4. See [:material-code-braces: DefaultExportDestinationTypeDef](./type_defs.md#defaultexportdestinationtypedef) 
5. See [:material-code-braces: UpdateSettingsResponseTypeDef](./type_defs.md#updatesettingsresponsetypedef) 


```python
# update_settings method usage example with argument unpacking

kwargs: UpdateSettingsRequestRequestTypeDef = {  # (1)
    "snsTopic": ...,
}

parent.update_settings(**kwargs)
```

1. See [:material-code-braces: UpdateSettingsRequestRequestTypeDef](./type_defs.md#updatesettingsrequestrequesttypedef) 

### validate\_assessment\_report\_integrity

Validates the integrity of an assessment report in Audit Manager.

Type annotations and code completion for `#!python session.client("auditmanager").validate_assessment_report_integrity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# validate_assessment_report_integrity method definition

await def validate_assessment_report_integrity(
    self,
    *,
    s3RelativePath: str,
) -> ValidateAssessmentReportIntegrityResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ValidateAssessmentReportIntegrityResponseTypeDef](./type_defs.md#validateassessmentreportintegrityresponsetypedef) 


```python
# validate_assessment_report_integrity method usage example with argument unpacking

kwargs: ValidateAssessmentReportIntegrityRequestRequestTypeDef = {  # (1)
    "s3RelativePath": ...,
}

parent.validate_assessment_report_integrity(**kwargs)
```

1. See [:material-code-braces: ValidateAssessmentReportIntegrityRequestRequestTypeDef](./type_defs.md#validateassessmentreportintegrityrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("auditmanager").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("auditmanager").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




