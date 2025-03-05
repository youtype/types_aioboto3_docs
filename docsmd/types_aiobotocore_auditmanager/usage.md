# Examples

> [Index](../README.md) > [AuditManager](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AuditManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#auditmanager)
    type annotations stubs module [types-aiobotocore-auditmanager](https://pypi.org/project/types-aiobotocore-auditmanager/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[auditmanager]` package installed.

Write your `AuditManager` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# AuditManagerClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("auditmanager") as client:  # (1)
    result = await client.batch_associate_assessment_report_evidence()  # (2)
```

1. client: [AuditManagerClient](./client.md)
2. result: [:material-code-braces: BatchAssociateAssessmentReportEvidenceResponseTypeDef](./type_defs.md#batchassociateassessmentreportevidenceresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[auditmanager]`
or a standalone `types_aiobotocore_auditmanager` package, you have to explicitly specify
`client: AuditManagerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# AuditManagerClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_auditmanager.client import AuditManagerClient
from types_aiobotocore_auditmanager.type_defs import BatchAssociateAssessmentReportEvidenceResponseTypeDef
from types_aiobotocore_auditmanager.type_defs import BatchAssociateAssessmentReportEvidenceRequestTypeDef


session = Session()

client: AuditManagerClient
async with session.client("auditmanager") as client:  # (1)
    kwargs: BatchAssociateAssessmentReportEvidenceRequestTypeDef = {...}  # (2)
    result: BatchAssociateAssessmentReportEvidenceResponseTypeDef = await client.batch_associate_assessment_report_evidence(**kwargs)  # (3)
```

1. client: [AuditManagerClient](./client.md)
2. kwargs: [:material-code-braces: BatchAssociateAssessmentReportEvidenceRequestTypeDef](./type_defs.md#batchassociateassessmentreportevidencerequesttypedef)
3. result: [:material-code-braces: BatchAssociateAssessmentReportEvidenceResponseTypeDef](./type_defs.md#batchassociateassessmentreportevidenceresponsetypedef)






