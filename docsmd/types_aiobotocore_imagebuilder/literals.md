# Literals

> [Index](../README.md) > [Imagebuilder](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Imagebuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
    type annotations stubs module [types-aiobotocore-imagebuilder](https://pypi.org/project/types-aiobotocore-imagebuilder/).

## BuildTypeType

```python
# BuildTypeType usage example

from types_aiobotocore_imagebuilder.literals import BuildTypeType

def get_value() -> BuildTypeType:
    return "IMPORT"
```

```python
# BuildTypeType definition

BuildTypeType = Literal[
    "IMPORT",
    "SCHEDULED",
    "USER_INITIATED",
]
```
## ComponentFormatType

```python
# ComponentFormatType usage example

from types_aiobotocore_imagebuilder.literals import ComponentFormatType

def get_value() -> ComponentFormatType:
    return "SHELL"
```

```python
# ComponentFormatType definition

ComponentFormatType = Literal[
    "SHELL",
]
```
## ComponentStatusType

```python
# ComponentStatusType usage example

from types_aiobotocore_imagebuilder.literals import ComponentStatusType

def get_value() -> ComponentStatusType:
    return "ACTIVE"
```

```python
# ComponentStatusType definition

ComponentStatusType = Literal[
    "ACTIVE",
    "DEPRECATED",
    "DISABLED",
]
```
## ComponentTypeType

```python
# ComponentTypeType usage example

from types_aiobotocore_imagebuilder.literals import ComponentTypeType

def get_value() -> ComponentTypeType:
    return "BUILD"
```

```python
# ComponentTypeType definition

ComponentTypeType = Literal[
    "BUILD",
    "TEST",
]
```
## ContainerRepositoryServiceType

```python
# ContainerRepositoryServiceType usage example

from types_aiobotocore_imagebuilder.literals import ContainerRepositoryServiceType

def get_value() -> ContainerRepositoryServiceType:
    return "ECR"
```

```python
# ContainerRepositoryServiceType definition

ContainerRepositoryServiceType = Literal[
    "ECR",
]
```
## ContainerTypeType

```python
# ContainerTypeType usage example

from types_aiobotocore_imagebuilder.literals import ContainerTypeType

def get_value() -> ContainerTypeType:
    return "DOCKER"
```

```python
# ContainerTypeType definition

ContainerTypeType = Literal[
    "DOCKER",
]
```
## DiskImageFormatType

```python
# DiskImageFormatType usage example

from types_aiobotocore_imagebuilder.literals import DiskImageFormatType

def get_value() -> DiskImageFormatType:
    return "RAW"
```

```python
# DiskImageFormatType definition

DiskImageFormatType = Literal[
    "RAW",
    "VHD",
    "VMDK",
]
```
## EbsVolumeTypeType

```python
# EbsVolumeTypeType usage example

from types_aiobotocore_imagebuilder.literals import EbsVolumeTypeType

def get_value() -> EbsVolumeTypeType:
    return "gp2"
```

```python
# EbsVolumeTypeType definition

EbsVolumeTypeType = Literal[
    "gp2",
    "gp3",
    "io1",
    "io2",
    "sc1",
    "st1",
    "standard",
]
```
## ImageScanStatusType

```python
# ImageScanStatusType usage example

from types_aiobotocore_imagebuilder.literals import ImageScanStatusType

def get_value() -> ImageScanStatusType:
    return "ABANDONED"
```

```python
# ImageScanStatusType definition

ImageScanStatusType = Literal[
    "ABANDONED",
    "COLLECTING",
    "COMPLETED",
    "FAILED",
    "PENDING",
    "SCANNING",
    "TIMED_OUT",
]
```
## ImageSourceType

```python
# ImageSourceType usage example

from types_aiobotocore_imagebuilder.literals import ImageSourceType

def get_value() -> ImageSourceType:
    return "AMAZON_MANAGED"
```

```python
# ImageSourceType definition

ImageSourceType = Literal[
    "AMAZON_MANAGED",
    "AWS_MARKETPLACE",
    "CUSTOM",
    "IMPORTED",
]
```
## ImageStatusType

```python
# ImageStatusType usage example

from types_aiobotocore_imagebuilder.literals import ImageStatusType

def get_value() -> ImageStatusType:
    return "AVAILABLE"
```

```python
# ImageStatusType definition

ImageStatusType = Literal[
    "AVAILABLE",
    "BUILDING",
    "CANCELLED",
    "CREATING",
    "DELETED",
    "DEPRECATED",
    "DISABLED",
    "DISTRIBUTING",
    "FAILED",
    "INTEGRATING",
    "PENDING",
    "TESTING",
]
```
## ImageTypeType

```python
# ImageTypeType usage example

from types_aiobotocore_imagebuilder.literals import ImageTypeType

def get_value() -> ImageTypeType:
    return "AMI"
```

```python
# ImageTypeType definition

ImageTypeType = Literal[
    "AMI",
    "DOCKER",
]
```
## LifecycleExecutionResourceActionNameType

```python
# LifecycleExecutionResourceActionNameType usage example

from types_aiobotocore_imagebuilder.literals import LifecycleExecutionResourceActionNameType

def get_value() -> LifecycleExecutionResourceActionNameType:
    return "AVAILABLE"
```

```python
# LifecycleExecutionResourceActionNameType definition

LifecycleExecutionResourceActionNameType = Literal[
    "AVAILABLE",
    "DELETE",
    "DEPRECATE",
    "DISABLE",
]
```
## LifecycleExecutionResourceStatusType

```python
# LifecycleExecutionResourceStatusType usage example

from types_aiobotocore_imagebuilder.literals import LifecycleExecutionResourceStatusType

def get_value() -> LifecycleExecutionResourceStatusType:
    return "FAILED"
```

```python
# LifecycleExecutionResourceStatusType definition

LifecycleExecutionResourceStatusType = Literal[
    "FAILED",
    "IN_PROGRESS",
    "SKIPPED",
    "SUCCESS",
]
```
## LifecycleExecutionStatusType

```python
# LifecycleExecutionStatusType usage example

from types_aiobotocore_imagebuilder.literals import LifecycleExecutionStatusType

def get_value() -> LifecycleExecutionStatusType:
    return "CANCELLED"
```

```python
# LifecycleExecutionStatusType definition

LifecycleExecutionStatusType = Literal[
    "CANCELLED",
    "CANCELLING",
    "FAILED",
    "IN_PROGRESS",
    "PENDING",
    "SUCCESS",
]
```
## LifecyclePolicyDetailActionTypeType

```python
# LifecyclePolicyDetailActionTypeType usage example

from types_aiobotocore_imagebuilder.literals import LifecyclePolicyDetailActionTypeType

def get_value() -> LifecyclePolicyDetailActionTypeType:
    return "DELETE"
```

```python
# LifecyclePolicyDetailActionTypeType definition

LifecyclePolicyDetailActionTypeType = Literal[
    "DELETE",
    "DEPRECATE",
    "DISABLE",
]
```
## LifecyclePolicyDetailFilterTypeType

```python
# LifecyclePolicyDetailFilterTypeType usage example

from types_aiobotocore_imagebuilder.literals import LifecyclePolicyDetailFilterTypeType

def get_value() -> LifecyclePolicyDetailFilterTypeType:
    return "AGE"
```

```python
# LifecyclePolicyDetailFilterTypeType definition

LifecyclePolicyDetailFilterTypeType = Literal[
    "AGE",
    "COUNT",
]
```
## LifecyclePolicyResourceTypeType

```python
# LifecyclePolicyResourceTypeType usage example

from types_aiobotocore_imagebuilder.literals import LifecyclePolicyResourceTypeType

def get_value() -> LifecyclePolicyResourceTypeType:
    return "AMI_IMAGE"
```

```python
# LifecyclePolicyResourceTypeType definition

LifecyclePolicyResourceTypeType = Literal[
    "AMI_IMAGE",
    "CONTAINER_IMAGE",
]
```
## LifecyclePolicyStatusType

```python
# LifecyclePolicyStatusType usage example

from types_aiobotocore_imagebuilder.literals import LifecyclePolicyStatusType

def get_value() -> LifecyclePolicyStatusType:
    return "DISABLED"
```

```python
# LifecyclePolicyStatusType definition

LifecyclePolicyStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## LifecyclePolicyTimeUnitType

```python
# LifecyclePolicyTimeUnitType usage example

from types_aiobotocore_imagebuilder.literals import LifecyclePolicyTimeUnitType

def get_value() -> LifecyclePolicyTimeUnitType:
    return "DAYS"
```

```python
# LifecyclePolicyTimeUnitType definition

LifecyclePolicyTimeUnitType = Literal[
    "DAYS",
    "MONTHS",
    "WEEKS",
    "YEARS",
]
```
## MarketplaceResourceTypeType

```python
# MarketplaceResourceTypeType usage example

from types_aiobotocore_imagebuilder.literals import MarketplaceResourceTypeType

def get_value() -> MarketplaceResourceTypeType:
    return "COMPONENT_ARTIFACT"
```

```python
# MarketplaceResourceTypeType definition

MarketplaceResourceTypeType = Literal[
    "COMPONENT_ARTIFACT",
    "COMPONENT_DATA",
]
```
## OnWorkflowFailureType

```python
# OnWorkflowFailureType usage example

from types_aiobotocore_imagebuilder.literals import OnWorkflowFailureType

def get_value() -> OnWorkflowFailureType:
    return "ABORT"
```

```python
# OnWorkflowFailureType definition

OnWorkflowFailureType = Literal[
    "ABORT",
    "CONTINUE",
]
```
## OwnershipType

```python
# OwnershipType usage example

from types_aiobotocore_imagebuilder.literals import OwnershipType

def get_value() -> OwnershipType:
    return "AWSMarketplace"
```

```python
# OwnershipType definition

OwnershipType = Literal[
    "Amazon",
    "AWSMarketplace",
    "Self",
    "Shared",
    "ThirdParty",
]
```
## PipelineExecutionStartConditionType

```python
# PipelineExecutionStartConditionType usage example

from types_aiobotocore_imagebuilder.literals import PipelineExecutionStartConditionType

def get_value() -> PipelineExecutionStartConditionType:
    return "EXPRESSION_MATCH_AND_DEPENDENCY_UPDATES_AVAILABLE"
```

```python
# PipelineExecutionStartConditionType definition

PipelineExecutionStartConditionType = Literal[
    "EXPRESSION_MATCH_AND_DEPENDENCY_UPDATES_AVAILABLE",
    "EXPRESSION_MATCH_ONLY",
]
```
## PipelineStatusType

```python
# PipelineStatusType usage example

from types_aiobotocore_imagebuilder.literals import PipelineStatusType

def get_value() -> PipelineStatusType:
    return "DISABLED"
```

```python
# PipelineStatusType definition

PipelineStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## PlatformType

```python
# PlatformType usage example

from types_aiobotocore_imagebuilder.literals import PlatformType

def get_value() -> PlatformType:
    return "Linux"
```

```python
# PlatformType definition

PlatformType = Literal[
    "Linux",
    "macOS",
    "Windows",
]
```
## ProductCodeTypeType

```python
# ProductCodeTypeType usage example

from types_aiobotocore_imagebuilder.literals import ProductCodeTypeType

def get_value() -> ProductCodeTypeType:
    return "marketplace"
```

```python
# ProductCodeTypeType definition

ProductCodeTypeType = Literal[
    "marketplace",
]
```
## ResourceStatusType

```python
# ResourceStatusType usage example

from types_aiobotocore_imagebuilder.literals import ResourceStatusType

def get_value() -> ResourceStatusType:
    return "AVAILABLE"
```

```python
# ResourceStatusType definition

ResourceStatusType = Literal[
    "AVAILABLE",
    "DELETED",
    "DEPRECATED",
    "DISABLED",
]
```
## TenancyTypeType

```python
# TenancyTypeType usage example

from types_aiobotocore_imagebuilder.literals import TenancyTypeType

def get_value() -> TenancyTypeType:
    return "dedicated"
```

```python
# TenancyTypeType definition

TenancyTypeType = Literal[
    "dedicated",
    "default",
    "host",
]
```
## WorkflowExecutionStatusType

```python
# WorkflowExecutionStatusType usage example

from types_aiobotocore_imagebuilder.literals import WorkflowExecutionStatusType

def get_value() -> WorkflowExecutionStatusType:
    return "CANCELLED"
```

```python
# WorkflowExecutionStatusType definition

WorkflowExecutionStatusType = Literal[
    "CANCELLED",
    "COMPLETED",
    "FAILED",
    "PENDING",
    "ROLLBACK_COMPLETED",
    "ROLLBACK_IN_PROGRESS",
    "RUNNING",
    "SKIPPED",
]
```
## WorkflowStatusType

```python
# WorkflowStatusType usage example

from types_aiobotocore_imagebuilder.literals import WorkflowStatusType

def get_value() -> WorkflowStatusType:
    return "DEPRECATED"
```

```python
# WorkflowStatusType definition

WorkflowStatusType = Literal[
    "DEPRECATED",
]
```
## WorkflowStepActionTypeType

```python
# WorkflowStepActionTypeType usage example

from types_aiobotocore_imagebuilder.literals import WorkflowStepActionTypeType

def get_value() -> WorkflowStepActionTypeType:
    return "RESUME"
```

```python
# WorkflowStepActionTypeType definition

WorkflowStepActionTypeType = Literal[
    "RESUME",
    "STOP",
]
```
## WorkflowStepExecutionRollbackStatusType

```python
# WorkflowStepExecutionRollbackStatusType usage example

from types_aiobotocore_imagebuilder.literals import WorkflowStepExecutionRollbackStatusType

def get_value() -> WorkflowStepExecutionRollbackStatusType:
    return "COMPLETED"
```

```python
# WorkflowStepExecutionRollbackStatusType definition

WorkflowStepExecutionRollbackStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "RUNNING",
    "SKIPPED",
]
```
## WorkflowStepExecutionStatusType

```python
# WorkflowStepExecutionStatusType usage example

from types_aiobotocore_imagebuilder.literals import WorkflowStepExecutionStatusType

def get_value() -> WorkflowStepExecutionStatusType:
    return "CANCELLED"
```

```python
# WorkflowStepExecutionStatusType definition

WorkflowStepExecutionStatusType = Literal[
    "CANCELLED",
    "COMPLETED",
    "FAILED",
    "PENDING",
    "RUNNING",
    "SKIPPED",
]
```
## WorkflowTypeType

```python
# WorkflowTypeType usage example

from types_aiobotocore_imagebuilder.literals import WorkflowTypeType

def get_value() -> WorkflowTypeType:
    return "BUILD"
```

```python
# WorkflowTypeType definition

WorkflowTypeType = Literal[
    "BUILD",
    "DISTRIBUTION",
    "TEST",
]
```
## ImagebuilderServiceName

```python
# ImagebuilderServiceName usage example

from types_aiobotocore_imagebuilder.literals import ImagebuilderServiceName

def get_value() -> ImagebuilderServiceName:
    return "imagebuilder"
```

```python
# ImagebuilderServiceName definition

ImagebuilderServiceName = Literal[
    "imagebuilder",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_imagebuilder.literals import ServiceName

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

from types_aiobotocore_imagebuilder.literals import ResourceServiceName

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