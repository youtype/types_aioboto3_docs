# Literals

> [Index](../README.md) > [CodeCommit](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [CodeCommit](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#codecommit)
    type annotations stubs module [types-aiobotocore-codecommit](https://pypi.org/project/types-aiobotocore-codecommit/).

## ApprovalStateType

```python
# ApprovalStateType usage example

from types_aiobotocore_codecommit.literals import ApprovalStateType

def get_value() -> ApprovalStateType:
    return "APPROVE"
```

```python
# ApprovalStateType definition

ApprovalStateType = Literal[
    "APPROVE",
    "REVOKE",
]
```
## BatchGetRepositoriesErrorCodeEnumType

```python
# BatchGetRepositoriesErrorCodeEnumType usage example

from types_aiobotocore_codecommit.literals import BatchGetRepositoriesErrorCodeEnumType

def get_value() -> BatchGetRepositoriesErrorCodeEnumType:
    return "EncryptionIntegrityChecksFailedException"
```

```python
# BatchGetRepositoriesErrorCodeEnumType definition

BatchGetRepositoriesErrorCodeEnumType = Literal[
    "EncryptionIntegrityChecksFailedException",
    "EncryptionKeyAccessDeniedException",
    "EncryptionKeyDisabledException",
    "EncryptionKeyNotFoundException",
    "EncryptionKeyUnavailableException",
    "RepositoryDoesNotExistException",
]
```
## ChangeTypeEnumType

```python
# ChangeTypeEnumType usage example

from types_aiobotocore_codecommit.literals import ChangeTypeEnumType

def get_value() -> ChangeTypeEnumType:
    return "A"
```

```python
# ChangeTypeEnumType definition

ChangeTypeEnumType = Literal[
    "A",
    "D",
    "M",
]
```
## ConflictDetailLevelTypeEnumType

```python
# ConflictDetailLevelTypeEnumType usage example

from types_aiobotocore_codecommit.literals import ConflictDetailLevelTypeEnumType

def get_value() -> ConflictDetailLevelTypeEnumType:
    return "FILE_LEVEL"
```

```python
# ConflictDetailLevelTypeEnumType definition

ConflictDetailLevelTypeEnumType = Literal[
    "FILE_LEVEL",
    "LINE_LEVEL",
]
```
## ConflictResolutionStrategyTypeEnumType

```python
# ConflictResolutionStrategyTypeEnumType usage example

from types_aiobotocore_codecommit.literals import ConflictResolutionStrategyTypeEnumType

def get_value() -> ConflictResolutionStrategyTypeEnumType:
    return "ACCEPT_DESTINATION"
```

```python
# ConflictResolutionStrategyTypeEnumType definition

ConflictResolutionStrategyTypeEnumType = Literal[
    "ACCEPT_DESTINATION",
    "ACCEPT_SOURCE",
    "AUTOMERGE",
    "NONE",
]
```
## DescribePullRequestEventsPaginatorName

```python
# DescribePullRequestEventsPaginatorName usage example

from types_aiobotocore_codecommit.literals import DescribePullRequestEventsPaginatorName

def get_value() -> DescribePullRequestEventsPaginatorName:
    return "describe_pull_request_events"
```

```python
# DescribePullRequestEventsPaginatorName definition

DescribePullRequestEventsPaginatorName = Literal[
    "describe_pull_request_events",
]
```
## FileModeTypeEnumType

```python
# FileModeTypeEnumType usage example

from types_aiobotocore_codecommit.literals import FileModeTypeEnumType

def get_value() -> FileModeTypeEnumType:
    return "EXECUTABLE"
```

```python
# FileModeTypeEnumType definition

FileModeTypeEnumType = Literal[
    "EXECUTABLE",
    "NORMAL",
    "SYMLINK",
]
```
## GetCommentsForComparedCommitPaginatorName

```python
# GetCommentsForComparedCommitPaginatorName usage example

from types_aiobotocore_codecommit.literals import GetCommentsForComparedCommitPaginatorName

def get_value() -> GetCommentsForComparedCommitPaginatorName:
    return "get_comments_for_compared_commit"
```

```python
# GetCommentsForComparedCommitPaginatorName definition

GetCommentsForComparedCommitPaginatorName = Literal[
    "get_comments_for_compared_commit",
]
```
## GetCommentsForPullRequestPaginatorName

```python
# GetCommentsForPullRequestPaginatorName usage example

from types_aiobotocore_codecommit.literals import GetCommentsForPullRequestPaginatorName

def get_value() -> GetCommentsForPullRequestPaginatorName:
    return "get_comments_for_pull_request"
```

```python
# GetCommentsForPullRequestPaginatorName definition

GetCommentsForPullRequestPaginatorName = Literal[
    "get_comments_for_pull_request",
]
```
## GetDifferencesPaginatorName

```python
# GetDifferencesPaginatorName usage example

from types_aiobotocore_codecommit.literals import GetDifferencesPaginatorName

def get_value() -> GetDifferencesPaginatorName:
    return "get_differences"
```

```python
# GetDifferencesPaginatorName definition

GetDifferencesPaginatorName = Literal[
    "get_differences",
]
```
## ListBranchesPaginatorName

```python
# ListBranchesPaginatorName usage example

from types_aiobotocore_codecommit.literals import ListBranchesPaginatorName

def get_value() -> ListBranchesPaginatorName:
    return "list_branches"
```

```python
# ListBranchesPaginatorName definition

ListBranchesPaginatorName = Literal[
    "list_branches",
]
```
## ListPullRequestsPaginatorName

```python
# ListPullRequestsPaginatorName usage example

from types_aiobotocore_codecommit.literals import ListPullRequestsPaginatorName

def get_value() -> ListPullRequestsPaginatorName:
    return "list_pull_requests"
```

```python
# ListPullRequestsPaginatorName definition

ListPullRequestsPaginatorName = Literal[
    "list_pull_requests",
]
```
## ListRepositoriesPaginatorName

```python
# ListRepositoriesPaginatorName usage example

from types_aiobotocore_codecommit.literals import ListRepositoriesPaginatorName

def get_value() -> ListRepositoriesPaginatorName:
    return "list_repositories"
```

```python
# ListRepositoriesPaginatorName definition

ListRepositoriesPaginatorName = Literal[
    "list_repositories",
]
```
## MergeOptionTypeEnumType

```python
# MergeOptionTypeEnumType usage example

from types_aiobotocore_codecommit.literals import MergeOptionTypeEnumType

def get_value() -> MergeOptionTypeEnumType:
    return "FAST_FORWARD_MERGE"
```

```python
# MergeOptionTypeEnumType definition

MergeOptionTypeEnumType = Literal[
    "FAST_FORWARD_MERGE",
    "SQUASH_MERGE",
    "THREE_WAY_MERGE",
]
```
## ObjectTypeEnumType

```python
# ObjectTypeEnumType usage example

from types_aiobotocore_codecommit.literals import ObjectTypeEnumType

def get_value() -> ObjectTypeEnumType:
    return "DIRECTORY"
```

```python
# ObjectTypeEnumType definition

ObjectTypeEnumType = Literal[
    "DIRECTORY",
    "FILE",
    "GIT_LINK",
    "SYMBOLIC_LINK",
]
```
## OrderEnumType

```python
# OrderEnumType usage example

from types_aiobotocore_codecommit.literals import OrderEnumType

def get_value() -> OrderEnumType:
    return "ascending"
```

```python
# OrderEnumType definition

OrderEnumType = Literal[
    "ascending",
    "descending",
]
```
## OverrideStatusType

```python
# OverrideStatusType usage example

from types_aiobotocore_codecommit.literals import OverrideStatusType

def get_value() -> OverrideStatusType:
    return "OVERRIDE"
```

```python
# OverrideStatusType definition

OverrideStatusType = Literal[
    "OVERRIDE",
    "REVOKE",
]
```
## PullRequestEventTypeType

```python
# PullRequestEventTypeType usage example

from types_aiobotocore_codecommit.literals import PullRequestEventTypeType

def get_value() -> PullRequestEventTypeType:
    return "PULL_REQUEST_APPROVAL_RULE_CREATED"
```

```python
# PullRequestEventTypeType definition

PullRequestEventTypeType = Literal[
    "PULL_REQUEST_APPROVAL_RULE_CREATED",
    "PULL_REQUEST_APPROVAL_RULE_DELETED",
    "PULL_REQUEST_APPROVAL_RULE_OVERRIDDEN",
    "PULL_REQUEST_APPROVAL_RULE_UPDATED",
    "PULL_REQUEST_APPROVAL_STATE_CHANGED",
    "PULL_REQUEST_CREATED",
    "PULL_REQUEST_MERGE_STATE_CHANGED",
    "PULL_REQUEST_SOURCE_REFERENCE_UPDATED",
    "PULL_REQUEST_STATUS_CHANGED",
]
```
## PullRequestStatusEnumType

```python
# PullRequestStatusEnumType usage example

from types_aiobotocore_codecommit.literals import PullRequestStatusEnumType

def get_value() -> PullRequestStatusEnumType:
    return "CLOSED"
```

```python
# PullRequestStatusEnumType definition

PullRequestStatusEnumType = Literal[
    "CLOSED",
    "OPEN",
]
```
## RelativeFileVersionEnumType

```python
# RelativeFileVersionEnumType usage example

from types_aiobotocore_codecommit.literals import RelativeFileVersionEnumType

def get_value() -> RelativeFileVersionEnumType:
    return "AFTER"
```

```python
# RelativeFileVersionEnumType definition

RelativeFileVersionEnumType = Literal[
    "AFTER",
    "BEFORE",
]
```
## ReplacementTypeEnumType

```python
# ReplacementTypeEnumType usage example

from types_aiobotocore_codecommit.literals import ReplacementTypeEnumType

def get_value() -> ReplacementTypeEnumType:
    return "KEEP_BASE"
```

```python
# ReplacementTypeEnumType definition

ReplacementTypeEnumType = Literal[
    "KEEP_BASE",
    "KEEP_DESTINATION",
    "KEEP_SOURCE",
    "USE_NEW_CONTENT",
]
```
## RepositoryTriggerEventEnumType

```python
# RepositoryTriggerEventEnumType usage example

from types_aiobotocore_codecommit.literals import RepositoryTriggerEventEnumType

def get_value() -> RepositoryTriggerEventEnumType:
    return "all"
```

```python
# RepositoryTriggerEventEnumType definition

RepositoryTriggerEventEnumType = Literal[
    "all",
    "createReference",
    "deleteReference",
    "updateReference",
]
```
## SortByEnumType

```python
# SortByEnumType usage example

from types_aiobotocore_codecommit.literals import SortByEnumType

def get_value() -> SortByEnumType:
    return "lastModifiedDate"
```

```python
# SortByEnumType definition

SortByEnumType = Literal[
    "lastModifiedDate",
    "repositoryName",
]
```
## CodeCommitServiceName

```python
# CodeCommitServiceName usage example

from types_aiobotocore_codecommit.literals import CodeCommitServiceName

def get_value() -> CodeCommitServiceName:
    return "codecommit"
```

```python
# CodeCommitServiceName definition

CodeCommitServiceName = Literal[
    "codecommit",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_codecommit.literals import ServiceName

def get_value() -> ServiceName:
    return "accessanalyzer"
```

```python
# ServiceName definition

ServiceName = Literal[
    "accessanalyzer",
    "account",
    "acm",
    "acm-pca",
    "amp",
    "amplify",
    "amplifybackend",
    "amplifyuibuilder",
    "apigateway",
    "apigatewaymanagementapi",
    "apigatewayv2",
    "appconfig",
    "appconfigdata",
    "appfabric",
    "appflow",
    "appintegrations",
    "application-autoscaling",
    "application-insights",
    "application-signals",
    "applicationcostprofiler",
    "appmesh",
    "apprunner",
    "appstream",
    "appsync",
    "apptest",
    "arc-zonal-shift",
    "artifact",
    "athena",
    "auditmanager",
    "autoscaling",
    "autoscaling-plans",
    "b2bi",
    "backup",
    "backup-gateway",
    "batch",
    "bcm-data-exports",
    "bcm-pricing-calculator",
    "bedrock",
    "bedrock-agent",
    "bedrock-agent-runtime",
    "bedrock-data-automation",
    "bedrock-data-automation-runtime",
    "bedrock-runtime",
    "billing",
    "billingconductor",
    "braket",
    "budgets",
    "ce",
    "chatbot",
    "chime",
    "chime-sdk-identity",
    "chime-sdk-media-pipelines",
    "chime-sdk-meetings",
    "chime-sdk-messaging",
    "chime-sdk-voice",
    "cleanrooms",
    "cleanroomsml",
    "cloud9",
    "cloudcontrol",
    "clouddirectory",
    "cloudformation",
    "cloudfront",
    "cloudfront-keyvaluestore",
    "cloudhsm",
    "cloudhsmv2",
    "cloudsearch",
    "cloudsearchdomain",
    "cloudtrail",
    "cloudtrail-data",
    "cloudwatch",
    "codeartifact",
    "codebuild",
    "codecatalyst",
    "codecommit",
    "codeconnections",
    "codedeploy",
    "codeguru-reviewer",
    "codeguru-security",
    "codeguruprofiler",
    "codepipeline",
    "codestar-connections",
    "codestar-notifications",
    "cognito-identity",
    "cognito-idp",
    "cognito-sync",
    "comprehend",
    "comprehendmedical",
    "compute-optimizer",
    "config",
    "connect",
    "connect-contact-lens",
    "connectcampaigns",
    "connectcampaignsv2",
    "connectcases",
    "connectparticipant",
    "controlcatalog",
    "controltower",
    "cost-optimization-hub",
    "cur",
    "customer-profiles",
    "databrew",
    "dataexchange",
    "datapipeline",
    "datasync",
    "datazone",
    "dax",
    "deadline",
    "detective",
    "devicefarm",
    "devops-guru",
    "directconnect",
    "discovery",
    "dlm",
    "dms",
    "docdb",
    "docdb-elastic",
    "drs",
    "ds",
    "ds-data",
    "dsql",
    "dynamodb",
    "dynamodbstreams",
    "ebs",
    "ec2",
    "ec2-instance-connect",
    "ecr",
    "ecr-public",
    "ecs",
    "efs",
    "eks",
    "eks-auth",
    "elastic-inference",
    "elasticache",
    "elasticbeanstalk",
    "elastictranscoder",
    "elb",
    "elbv2",
    "emr",
    "emr-containers",
    "emr-serverless",
    "entityresolution",
    "es",
    "events",
    "evidently",
    "finspace",
    "finspace-data",
    "firehose",
    "fis",
    "fms",
    "forecast",
    "forecastquery",
    "frauddetector",
    "freetier",
    "fsx",
    "gamelift",
    "geo-maps",
    "geo-places",
    "geo-routes",
    "glacier",
    "globalaccelerator",
    "glue",
    "grafana",
    "greengrass",
    "greengrassv2",
    "groundstation",
    "guardduty",
    "health",
    "healthlake",
    "iam",
    "identitystore",
    "imagebuilder",
    "importexport",
    "inspector",
    "inspector-scan",
    "inspector2",
    "internetmonitor",
    "invoicing",
    "iot",
    "iot-data",
    "iot-jobs-data",
    "iot1click-devices",
    "iot1click-projects",
    "iotanalytics",
    "iotdeviceadvisor",
    "iotevents",
    "iotevents-data",
    "iotfleethub",
    "iotfleetwise",
    "iotsecuretunneling",
    "iotsitewise",
    "iotthingsgraph",
    "iottwinmaker",
    "iotwireless",
    "ivs",
    "ivs-realtime",
    "ivschat",
    "kafka",
    "kafkaconnect",
    "kendra",
    "kendra-ranking",
    "keyspaces",
    "kinesis",
    "kinesis-video-archived-media",
    "kinesis-video-media",
    "kinesis-video-signaling",
    "kinesis-video-webrtc-storage",
    "kinesisanalytics",
    "kinesisanalyticsv2",
    "kinesisvideo",
    "kms",
    "lakeformation",
    "lambda",
    "launch-wizard",
    "lex-models",
    "lex-runtime",
    "lexv2-models",
    "lexv2-runtime",
    "license-manager",
    "license-manager-linux-subscriptions",
    "license-manager-user-subscriptions",
    "lightsail",
    "location",
    "logs",
    "lookoutequipment",
    "lookoutmetrics",
    "lookoutvision",
    "m2",
    "machinelearning",
    "macie2",
    "mailmanager",
    "managedblockchain",
    "managedblockchain-query",
    "marketplace-agreement",
    "marketplace-catalog",
    "marketplace-deployment",
    "marketplace-entitlement",
    "marketplace-reporting",
    "marketplacecommerceanalytics",
    "mediaconnect",
    "mediaconvert",
    "medialive",
    "mediapackage",
    "mediapackage-vod",
    "mediapackagev2",
    "mediastore",
    "mediastore-data",
    "mediatailor",
    "medical-imaging",
    "memorydb",
    "meteringmarketplace",
    "mgh",
    "mgn",
    "migration-hub-refactor-spaces",
    "migrationhub-config",
    "migrationhuborchestrator",
    "migrationhubstrategy",
    "mq",
    "mturk",
    "mwaa",
    "neptune",
    "neptune-graph",
    "neptunedata",
    "network-firewall",
    "networkflowmonitor",
    "networkmanager",
    "networkmonitor",
    "notifications",
    "notificationscontacts",
    "oam",
    "observabilityadmin",
    "omics",
    "opensearch",
    "opensearchserverless",
    "opsworks",
    "opsworkscm",
    "organizations",
    "osis",
    "outposts",
    "panorama",
    "partnercentral-selling",
    "payment-cryptography",
    "payment-cryptography-data",
    "pca-connector-ad",
    "pca-connector-scep",
    "pcs",
    "personalize",
    "personalize-events",
    "personalize-runtime",
    "pi",
    "pinpoint",
    "pinpoint-email",
    "pinpoint-sms-voice",
    "pinpoint-sms-voice-v2",
    "pipes",
    "polly",
    "pricing",
    "privatenetworks",
    "proton",
    "qapps",
    "qbusiness",
    "qconnect",
    "qldb",
    "qldb-session",
    "quicksight",
    "ram",
    "rbin",
    "rds",
    "rds-data",
    "redshift",
    "redshift-data",
    "redshift-serverless",
    "rekognition",
    "repostspace",
    "resiliencehub",
    "resource-explorer-2",
    "resource-groups",
    "resourcegroupstaggingapi",
    "robomaker",
    "rolesanywhere",
    "route53",
    "route53-recovery-cluster",
    "route53-recovery-control-config",
    "route53-recovery-readiness",
    "route53domains",
    "route53profiles",
    "route53resolver",
    "rum",
    "s3",
    "s3control",
    "s3outposts",
    "s3tables",
    "sagemaker",
    "sagemaker-a2i-runtime",
    "sagemaker-edge",
    "sagemaker-featurestore-runtime",
    "sagemaker-geospatial",
    "sagemaker-metrics",
    "sagemaker-runtime",
    "savingsplans",
    "scheduler",
    "schemas",
    "sdb",
    "secretsmanager",
    "security-ir",
    "securityhub",
    "securitylake",
    "serverlessrepo",
    "service-quotas",
    "servicecatalog",
    "servicecatalog-appregistry",
    "servicediscovery",
    "ses",
    "sesv2",
    "shield",
    "signer",
    "simspaceweaver",
    "sms",
    "sms-voice",
    "snow-device-management",
    "snowball",
    "sns",
    "socialmessaging",
    "sqs",
    "ssm",
    "ssm-contacts",
    "ssm-incidents",
    "ssm-quicksetup",
    "ssm-sap",
    "sso",
    "sso-admin",
    "sso-oidc",
    "stepfunctions",
    "storagegateway",
    "sts",
    "supplychain",
    "support",
    "support-app",
    "swf",
    "synthetics",
    "taxsettings",
    "textract",
    "timestream-influxdb",
    "timestream-query",
    "timestream-write",
    "tnb",
    "transcribe",
    "transfer",
    "translate",
    "trustedadvisor",
    "verifiedpermissions",
    "voice-id",
    "vpc-lattice",
    "waf",
    "waf-regional",
    "wafv2",
    "wellarchitected",
    "wisdom",
    "workdocs",
    "workmail",
    "workmailmessageflow",
    "workspaces",
    "workspaces-thin-client",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python
# ResourceServiceName usage example

from types_aiobotocore_codecommit.literals import ResourceServiceName

def get_value() -> ResourceServiceName:
    return "cloudformation"
```

```python
# ResourceServiceName definition

ResourceServiceName = Literal[
    "cloudformation",
    "cloudwatch",
    "dynamodb",
    "ec2",
    "glacier",
    "iam",
    "opsworks",
    "s3",
    "sns",
    "sqs",
]
```
## PaginatorName

```python
# PaginatorName usage example

from types_aiobotocore_codecommit.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_pull_request_events"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "describe_pull_request_events",
    "get_comments_for_compared_commit",
    "get_comments_for_pull_request",
    "get_differences",
    "list_branches",
    "list_pull_requests",
    "list_repositories",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_codecommit.literals import RegionName

def get_value() -> RegionName:
    return "af-south-1"
```

```python
# RegionName definition

RegionName = Literal[
    "af-south-1",
    "ap-east-1",
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-northeast-3",
    "ap-south-1",
    "ap-south-2",
    "ap-southeast-1",
    "ap-southeast-2",
    "ap-southeast-3",
    "ca-central-1",
    "eu-central-1",
    "eu-north-1",
    "eu-south-1",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "il-central-1",
    "me-central-1",
    "me-south-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```