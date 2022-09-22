# Literals

> [Index](../README.md) > [ElasticsearchService](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [ElasticsearchService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
    type annotations stubs module [types-aiobotocore-es](https://pypi.org/project/types-aiobotocore-es/).

## AutoTuneDesiredStateType

```python title="Usage Example"
from types_aiobotocore_es.literals import AutoTuneDesiredStateType

def get_value() -> AutoTuneDesiredStateType:
    return "DISABLED"
```

```python title="Definition"
AutoTuneDesiredStateType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## AutoTuneStateType

```python title="Usage Example"
from types_aiobotocore_es.literals import AutoTuneStateType

def get_value() -> AutoTuneStateType:
    return "DISABLED"
```

```python title="Definition"
AutoTuneStateType = Literal[
    "DISABLE_IN_PROGRESS",
    "DISABLED",
    "DISABLED_AND_ROLLBACK_COMPLETE",
    "DISABLED_AND_ROLLBACK_ERROR",
    "DISABLED_AND_ROLLBACK_IN_PROGRESS",
    "DISABLED_AND_ROLLBACK_SCHEDULED",
    "ENABLE_IN_PROGRESS",
    "ENABLED",
    "ERROR",
]
```
## AutoTuneTypeType

```python title="Usage Example"
from types_aiobotocore_es.literals import AutoTuneTypeType

def get_value() -> AutoTuneTypeType:
    return "SCHEDULED_ACTION"
```

```python title="Definition"
AutoTuneTypeType = Literal[
    "SCHEDULED_ACTION",
]
```
## DeploymentStatusType

```python title="Usage Example"
from types_aiobotocore_es.literals import DeploymentStatusType

def get_value() -> DeploymentStatusType:
    return "COMPLETED"
```

```python title="Definition"
DeploymentStatusType = Literal[
    "COMPLETED",
    "ELIGIBLE",
    "IN_PROGRESS",
    "NOT_ELIGIBLE",
    "PENDING_UPDATE",
]
```
## DescribePackagesFilterNameType

```python title="Usage Example"
from types_aiobotocore_es.literals import DescribePackagesFilterNameType

def get_value() -> DescribePackagesFilterNameType:
    return "PackageID"
```

```python title="Definition"
DescribePackagesFilterNameType = Literal[
    "PackageID",
    "PackageName",
    "PackageStatus",
]
```
## DescribeReservedElasticsearchInstanceOfferingsPaginatorName

```python title="Usage Example"
from types_aiobotocore_es.literals import DescribeReservedElasticsearchInstanceOfferingsPaginatorName

def get_value() -> DescribeReservedElasticsearchInstanceOfferingsPaginatorName:
    return "describe_reserved_elasticsearch_instance_offerings"
```

```python title="Definition"
DescribeReservedElasticsearchInstanceOfferingsPaginatorName = Literal[
    "describe_reserved_elasticsearch_instance_offerings",
]
```
## DescribeReservedElasticsearchInstancesPaginatorName

```python title="Usage Example"
from types_aiobotocore_es.literals import DescribeReservedElasticsearchInstancesPaginatorName

def get_value() -> DescribeReservedElasticsearchInstancesPaginatorName:
    return "describe_reserved_elasticsearch_instances"
```

```python title="Definition"
DescribeReservedElasticsearchInstancesPaginatorName = Literal[
    "describe_reserved_elasticsearch_instances",
]
```
## DomainPackageStatusType

```python title="Usage Example"
from types_aiobotocore_es.literals import DomainPackageStatusType

def get_value() -> DomainPackageStatusType:
    return "ACTIVE"
```

```python title="Definition"
DomainPackageStatusType = Literal[
    "ACTIVE",
    "ASSOCIATING",
    "ASSOCIATION_FAILED",
    "DISSOCIATING",
    "DISSOCIATION_FAILED",
]
```
## ESPartitionInstanceTypeType

```python title="Usage Example"
from types_aiobotocore_es.literals import ESPartitionInstanceTypeType

def get_value() -> ESPartitionInstanceTypeType:
    return "c4.2xlarge.elasticsearch"
```

```python title="Definition"
ESPartitionInstanceTypeType = Literal[
    "c4.2xlarge.elasticsearch",
    "c4.4xlarge.elasticsearch",
    "c4.8xlarge.elasticsearch",
    "c4.large.elasticsearch",
    "c4.xlarge.elasticsearch",
    "c5.18xlarge.elasticsearch",
    "c5.2xlarge.elasticsearch",
    "c5.4xlarge.elasticsearch",
    "c5.9xlarge.elasticsearch",
    "c5.large.elasticsearch",
    "c5.xlarge.elasticsearch",
    "d2.2xlarge.elasticsearch",
    "d2.4xlarge.elasticsearch",
    "d2.8xlarge.elasticsearch",
    "d2.xlarge.elasticsearch",
    "i2.2xlarge.elasticsearch",
    "i2.xlarge.elasticsearch",
    "i3.16xlarge.elasticsearch",
    "i3.2xlarge.elasticsearch",
    "i3.4xlarge.elasticsearch",
    "i3.8xlarge.elasticsearch",
    "i3.large.elasticsearch",
    "i3.xlarge.elasticsearch",
    "m3.2xlarge.elasticsearch",
    "m3.large.elasticsearch",
    "m3.medium.elasticsearch",
    "m3.xlarge.elasticsearch",
    "m4.10xlarge.elasticsearch",
    "m4.2xlarge.elasticsearch",
    "m4.4xlarge.elasticsearch",
    "m4.large.elasticsearch",
    "m4.xlarge.elasticsearch",
    "m5.12xlarge.elasticsearch",
    "m5.2xlarge.elasticsearch",
    "m5.4xlarge.elasticsearch",
    "m5.large.elasticsearch",
    "m5.xlarge.elasticsearch",
    "r3.2xlarge.elasticsearch",
    "r3.4xlarge.elasticsearch",
    "r3.8xlarge.elasticsearch",
    "r3.large.elasticsearch",
    "r3.xlarge.elasticsearch",
    "r4.16xlarge.elasticsearch",
    "r4.2xlarge.elasticsearch",
    "r4.4xlarge.elasticsearch",
    "r4.8xlarge.elasticsearch",
    "r4.large.elasticsearch",
    "r4.xlarge.elasticsearch",
    "r5.12xlarge.elasticsearch",
    "r5.2xlarge.elasticsearch",
    "r5.4xlarge.elasticsearch",
    "r5.large.elasticsearch",
    "r5.xlarge.elasticsearch",
    "t2.medium.elasticsearch",
    "t2.micro.elasticsearch",
    "t2.small.elasticsearch",
    "ultrawarm1.large.elasticsearch",
    "ultrawarm1.medium.elasticsearch",
]
```
## ESWarmPartitionInstanceTypeType

```python title="Usage Example"
from types_aiobotocore_es.literals import ESWarmPartitionInstanceTypeType

def get_value() -> ESWarmPartitionInstanceTypeType:
    return "ultrawarm1.large.elasticsearch"
```

```python title="Definition"
ESWarmPartitionInstanceTypeType = Literal[
    "ultrawarm1.large.elasticsearch",
    "ultrawarm1.medium.elasticsearch",
]
```
## EngineTypeType

```python title="Usage Example"
from types_aiobotocore_es.literals import EngineTypeType

def get_value() -> EngineTypeType:
    return "Elasticsearch"
```

```python title="Definition"
EngineTypeType = Literal[
    "Elasticsearch",
    "OpenSearch",
]
```
## GetUpgradeHistoryPaginatorName

```python title="Usage Example"
from types_aiobotocore_es.literals import GetUpgradeHistoryPaginatorName

def get_value() -> GetUpgradeHistoryPaginatorName:
    return "get_upgrade_history"
```

```python title="Definition"
GetUpgradeHistoryPaginatorName = Literal[
    "get_upgrade_history",
]
```
## InboundCrossClusterSearchConnectionStatusCodeType

```python title="Usage Example"
from types_aiobotocore_es.literals import InboundCrossClusterSearchConnectionStatusCodeType

def get_value() -> InboundCrossClusterSearchConnectionStatusCodeType:
    return "APPROVED"
```

```python title="Definition"
InboundCrossClusterSearchConnectionStatusCodeType = Literal[
    "APPROVED",
    "DELETED",
    "DELETING",
    "PENDING_ACCEPTANCE",
    "REJECTED",
    "REJECTING",
]
```
## ListElasticsearchInstanceTypesPaginatorName

```python title="Usage Example"
from types_aiobotocore_es.literals import ListElasticsearchInstanceTypesPaginatorName

def get_value() -> ListElasticsearchInstanceTypesPaginatorName:
    return "list_elasticsearch_instance_types"
```

```python title="Definition"
ListElasticsearchInstanceTypesPaginatorName = Literal[
    "list_elasticsearch_instance_types",
]
```
## ListElasticsearchVersionsPaginatorName

```python title="Usage Example"
from types_aiobotocore_es.literals import ListElasticsearchVersionsPaginatorName

def get_value() -> ListElasticsearchVersionsPaginatorName:
    return "list_elasticsearch_versions"
```

```python title="Definition"
ListElasticsearchVersionsPaginatorName = Literal[
    "list_elasticsearch_versions",
]
```
## LogTypeType

```python title="Usage Example"
from types_aiobotocore_es.literals import LogTypeType

def get_value() -> LogTypeType:
    return "AUDIT_LOGS"
```

```python title="Definition"
LogTypeType = Literal[
    "AUDIT_LOGS",
    "ES_APPLICATION_LOGS",
    "INDEX_SLOW_LOGS",
    "SEARCH_SLOW_LOGS",
]
```
## OptionStateType

```python title="Usage Example"
from types_aiobotocore_es.literals import OptionStateType

def get_value() -> OptionStateType:
    return "Active"
```

```python title="Definition"
OptionStateType = Literal[
    "Active",
    "Processing",
    "RequiresIndexDocuments",
]
```
## OutboundCrossClusterSearchConnectionStatusCodeType

```python title="Usage Example"
from types_aiobotocore_es.literals import OutboundCrossClusterSearchConnectionStatusCodeType

def get_value() -> OutboundCrossClusterSearchConnectionStatusCodeType:
    return "ACTIVE"
```

```python title="Definition"
OutboundCrossClusterSearchConnectionStatusCodeType = Literal[
    "ACTIVE",
    "DELETED",
    "DELETING",
    "PENDING_ACCEPTANCE",
    "PROVISIONING",
    "REJECTED",
    "VALIDATING",
    "VALIDATION_FAILED",
]
```
## OverallChangeStatusType

```python title="Usage Example"
from types_aiobotocore_es.literals import OverallChangeStatusType

def get_value() -> OverallChangeStatusType:
    return "COMPLETED"
```

```python title="Definition"
OverallChangeStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "PENDING",
    "PROCESSING",
]
```
## PackageStatusType

```python title="Usage Example"
from types_aiobotocore_es.literals import PackageStatusType

def get_value() -> PackageStatusType:
    return "AVAILABLE"
```

```python title="Definition"
PackageStatusType = Literal[
    "AVAILABLE",
    "COPY_FAILED",
    "COPYING",
    "DELETE_FAILED",
    "DELETED",
    "DELETING",
    "VALIDATING",
    "VALIDATION_FAILED",
]
```
## PackageTypeType

```python title="Usage Example"
from types_aiobotocore_es.literals import PackageTypeType

def get_value() -> PackageTypeType:
    return "TXT-DICTIONARY"
```

```python title="Definition"
PackageTypeType = Literal[
    "TXT-DICTIONARY",
]
```
## ReservedElasticsearchInstancePaymentOptionType

```python title="Usage Example"
from types_aiobotocore_es.literals import ReservedElasticsearchInstancePaymentOptionType

def get_value() -> ReservedElasticsearchInstancePaymentOptionType:
    return "ALL_UPFRONT"
```

```python title="Definition"
ReservedElasticsearchInstancePaymentOptionType = Literal[
    "ALL_UPFRONT",
    "NO_UPFRONT",
    "PARTIAL_UPFRONT",
]
```
## RollbackOnDisableType

```python title="Usage Example"
from types_aiobotocore_es.literals import RollbackOnDisableType

def get_value() -> RollbackOnDisableType:
    return "DEFAULT_ROLLBACK"
```

```python title="Definition"
RollbackOnDisableType = Literal[
    "DEFAULT_ROLLBACK",
    "NO_ROLLBACK",
]
```
## ScheduledAutoTuneActionTypeType

```python title="Usage Example"
from types_aiobotocore_es.literals import ScheduledAutoTuneActionTypeType

def get_value() -> ScheduledAutoTuneActionTypeType:
    return "JVM_HEAP_SIZE_TUNING"
```

```python title="Definition"
ScheduledAutoTuneActionTypeType = Literal[
    "JVM_HEAP_SIZE_TUNING",
    "JVM_YOUNG_GEN_TUNING",
]
```
## ScheduledAutoTuneSeverityTypeType

```python title="Usage Example"
from types_aiobotocore_es.literals import ScheduledAutoTuneSeverityTypeType

def get_value() -> ScheduledAutoTuneSeverityTypeType:
    return "HIGH"
```

```python title="Definition"
ScheduledAutoTuneSeverityTypeType = Literal[
    "HIGH",
    "LOW",
    "MEDIUM",
]
```
## TLSSecurityPolicyType

```python title="Usage Example"
from types_aiobotocore_es.literals import TLSSecurityPolicyType

def get_value() -> TLSSecurityPolicyType:
    return "Policy-Min-TLS-1-0-2019-07"
```

```python title="Definition"
TLSSecurityPolicyType = Literal[
    "Policy-Min-TLS-1-0-2019-07",
    "Policy-Min-TLS-1-2-2019-07",
]
```
## TimeUnitType

```python title="Usage Example"
from types_aiobotocore_es.literals import TimeUnitType

def get_value() -> TimeUnitType:
    return "HOURS"
```

```python title="Definition"
TimeUnitType = Literal[
    "HOURS",
]
```
## UpgradeStatusType

```python title="Usage Example"
from types_aiobotocore_es.literals import UpgradeStatusType

def get_value() -> UpgradeStatusType:
    return "FAILED"
```

```python title="Definition"
UpgradeStatusType = Literal[
    "FAILED",
    "IN_PROGRESS",
    "SUCCEEDED",
    "SUCCEEDED_WITH_ISSUES",
]
```
## UpgradeStepType

```python title="Usage Example"
from types_aiobotocore_es.literals import UpgradeStepType

def get_value() -> UpgradeStepType:
    return "PRE_UPGRADE_CHECK"
```

```python title="Definition"
UpgradeStepType = Literal[
    "PRE_UPGRADE_CHECK",
    "SNAPSHOT",
    "UPGRADE",
]
```
## VolumeTypeType

```python title="Usage Example"
from types_aiobotocore_es.literals import VolumeTypeType

def get_value() -> VolumeTypeType:
    return "gp2"
```

```python title="Definition"
VolumeTypeType = Literal[
    "gp2",
    "gp3",
    "io1",
    "standard",
]
```
## ElasticsearchServiceServiceName

```python title="Usage Example"
from types_aiobotocore_es.literals import ElasticsearchServiceServiceName

def get_value() -> ElasticsearchServiceServiceName:
    return "es"
```

```python title="Definition"
ElasticsearchServiceServiceName = Literal[
    "es",
]
```
## ServiceName

```python title="Usage Example"
from types_aiobotocore_es.literals import ServiceName

def get_value() -> ServiceName:
    return "accessanalyzer"
```

```python title="Definition"
ServiceName = Literal[
    "accessanalyzer",
    "account",
    "acm",
    "acm-pca",
    "alexaforbusiness",
    "amp",
    "amplify",
    "amplifybackend",
    "amplifyuibuilder",
    "apigateway",
    "apigatewaymanagementapi",
    "apigatewayv2",
    "appconfig",
    "appconfigdata",
    "appflow",
    "appintegrations",
    "application-autoscaling",
    "application-insights",
    "applicationcostprofiler",
    "appmesh",
    "apprunner",
    "appstream",
    "appsync",
    "athena",
    "auditmanager",
    "autoscaling",
    "autoscaling-plans",
    "backup",
    "backup-gateway",
    "backupstorage",
    "batch",
    "billingconductor",
    "braket",
    "budgets",
    "ce",
    "chime",
    "chime-sdk-identity",
    "chime-sdk-media-pipelines",
    "chime-sdk-meetings",
    "chime-sdk-messaging",
    "cloud9",
    "cloudcontrol",
    "clouddirectory",
    "cloudformation",
    "cloudfront",
    "cloudhsm",
    "cloudhsmv2",
    "cloudsearch",
    "cloudsearchdomain",
    "cloudtrail",
    "cloudwatch",
    "codeartifact",
    "codebuild",
    "codecommit",
    "codedeploy",
    "codeguru-reviewer",
    "codeguruprofiler",
    "codepipeline",
    "codestar",
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
    "connectparticipant",
    "cur",
    "customer-profiles",
    "databrew",
    "dataexchange",
    "datapipeline",
    "datasync",
    "dax",
    "detective",
    "devicefarm",
    "devops-guru",
    "directconnect",
    "discovery",
    "dlm",
    "dms",
    "docdb",
    "drs",
    "ds",
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
    "elastic-inference",
    "elasticache",
    "elasticbeanstalk",
    "elastictranscoder",
    "elb",
    "elbv2",
    "emr",
    "emr-containers",
    "emr-serverless",
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
    "fsx",
    "gamelift",
    "gamesparks",
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
    "honeycode",
    "iam",
    "identitystore",
    "imagebuilder",
    "importexport",
    "inspector",
    "inspector2",
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
    "iotsecuretunneling",
    "iotsitewise",
    "iotthingsgraph",
    "iottwinmaker",
    "iotwireless",
    "ivs",
    "ivschat",
    "kafka",
    "kafkaconnect",
    "kendra",
    "keyspaces",
    "kinesis",
    "kinesis-video-archived-media",
    "kinesis-video-media",
    "kinesis-video-signaling",
    "kinesisanalytics",
    "kinesisanalyticsv2",
    "kinesisvideo",
    "kms",
    "lakeformation",
    "lambda",
    "lex-models",
    "lex-runtime",
    "lexv2-models",
    "lexv2-runtime",
    "license-manager",
    "license-manager-user-subscriptions",
    "lightsail",
    "location",
    "logs",
    "lookoutequipment",
    "lookoutmetrics",
    "lookoutvision",
    "m2",
    "machinelearning",
    "macie",
    "macie2",
    "managedblockchain",
    "marketplace-catalog",
    "marketplace-entitlement",
    "marketplacecommerceanalytics",
    "mediaconnect",
    "mediaconvert",
    "medialive",
    "mediapackage",
    "mediapackage-vod",
    "mediastore",
    "mediastore-data",
    "mediatailor",
    "memorydb",
    "meteringmarketplace",
    "mgh",
    "mgn",
    "migration-hub-refactor-spaces",
    "migrationhub-config",
    "migrationhubstrategy",
    "mobile",
    "mq",
    "mturk",
    "mwaa",
    "neptune",
    "network-firewall",
    "networkmanager",
    "nimble",
    "opensearch",
    "opsworks",
    "opsworkscm",
    "organizations",
    "outposts",
    "panorama",
    "personalize",
    "personalize-events",
    "personalize-runtime",
    "pi",
    "pinpoint",
    "pinpoint-email",
    "pinpoint-sms-voice",
    "pinpoint-sms-voice-v2",
    "polly",
    "pricing",
    "privatenetworks",
    "proton",
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
    "resiliencehub",
    "resource-groups",
    "resourcegroupstaggingapi",
    "robomaker",
    "rolesanywhere",
    "route53",
    "route53-recovery-cluster",
    "route53-recovery-control-config",
    "route53-recovery-readiness",
    "route53domains",
    "route53resolver",
    "rum",
    "s3",
    "s3control",
    "s3outposts",
    "sagemaker",
    "sagemaker-a2i-runtime",
    "sagemaker-edge",
    "sagemaker-featurestore-runtime",
    "sagemaker-runtime",
    "savingsplans",
    "schemas",
    "sdb",
    "secretsmanager",
    "securityhub",
    "serverlessrepo",
    "service-quotas",
    "servicecatalog",
    "servicecatalog-appregistry",
    "servicediscovery",
    "ses",
    "sesv2",
    "shield",
    "signer",
    "sms",
    "sms-voice",
    "snow-device-management",
    "snowball",
    "sns",
    "sqs",
    "ssm",
    "ssm-contacts",
    "ssm-incidents",
    "sso",
    "sso-admin",
    "sso-oidc",
    "stepfunctions",
    "storagegateway",
    "sts",
    "support",
    "support-app",
    "swf",
    "synthetics",
    "textract",
    "timestream-query",
    "timestream-write",
    "transcribe",
    "transfer",
    "translate",
    "voice-id",
    "waf",
    "waf-regional",
    "wafv2",
    "wellarchitected",
    "wisdom",
    "workdocs",
    "worklink",
    "workmail",
    "workmailmessageflow",
    "workspaces",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python title="Usage Example"
from types_aiobotocore_es.literals import ResourceServiceName

def get_value() -> ResourceServiceName:
    return "cloudformation"
```

```python title="Definition"
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

```python title="Usage Example"
from types_aiobotocore_es.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_reserved_elasticsearch_instance_offerings"
```

```python title="Definition"
PaginatorName = Literal[
    "describe_reserved_elasticsearch_instance_offerings",
    "describe_reserved_elasticsearch_instances",
    "get_upgrade_history",
    "list_elasticsearch_instance_types",
    "list_elasticsearch_versions",
]
```
## RegionName

```python title="Usage Example"
from types_aiobotocore_es.literals import RegionName

def get_value() -> RegionName:
    return "af-south-1"
```

```python title="Definition"
RegionName = Literal[
    "af-south-1",
    "ap-east-1",
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-northeast-3",
    "ap-south-1",
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
    "me-south-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
