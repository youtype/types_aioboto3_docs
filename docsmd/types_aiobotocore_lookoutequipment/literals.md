# Literals

> [Index](../README.md) > [LookoutEquipment](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [LookoutEquipment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#lookoutequipment)
    type annotations stubs module [types-aiobotocore-lookoutequipment](https://pypi.org/project/types-aiobotocore-lookoutequipment/).

## AutoPromotionResultType

```python
# AutoPromotionResultType usage example

from types_aiobotocore_lookoutequipment.literals import AutoPromotionResultType

def get_value() -> AutoPromotionResultType:
    return "MODEL_NOT_PROMOTED"
```

```python
# AutoPromotionResultType definition

AutoPromotionResultType = Literal[
    "MODEL_NOT_PROMOTED",
    "MODEL_PROMOTED",
    "RETRAINING_CANCELLED",
    "RETRAINING_CUSTOMER_ERROR",
    "RETRAINING_INTERNAL_ERROR",
]
```
## DataUploadFrequencyType

```python
# DataUploadFrequencyType usage example

from types_aiobotocore_lookoutequipment.literals import DataUploadFrequencyType

def get_value() -> DataUploadFrequencyType:
    return "PT10M"
```

```python
# DataUploadFrequencyType definition

DataUploadFrequencyType = Literal[
    "PT10M",
    "PT15M",
    "PT1H",
    "PT30M",
    "PT5M",
]
```
## DatasetStatusType

```python
# DatasetStatusType usage example

from types_aiobotocore_lookoutequipment.literals import DatasetStatusType

def get_value() -> DatasetStatusType:
    return "ACTIVE"
```

```python
# DatasetStatusType definition

DatasetStatusType = Literal[
    "ACTIVE",
    "CREATED",
    "IMPORT_IN_PROGRESS",
    "INGESTION_IN_PROGRESS",
]
```
## InferenceDataImportStrategyType

```python
# InferenceDataImportStrategyType usage example

from types_aiobotocore_lookoutequipment.literals import InferenceDataImportStrategyType

def get_value() -> InferenceDataImportStrategyType:
    return "ADD_WHEN_EMPTY"
```

```python
# InferenceDataImportStrategyType definition

InferenceDataImportStrategyType = Literal[
    "ADD_WHEN_EMPTY",
    "NO_IMPORT",
    "OVERWRITE",
]
```
## InferenceExecutionStatusType

```python
# InferenceExecutionStatusType usage example

from types_aiobotocore_lookoutequipment.literals import InferenceExecutionStatusType

def get_value() -> InferenceExecutionStatusType:
    return "FAILED"
```

```python
# InferenceExecutionStatusType definition

InferenceExecutionStatusType = Literal[
    "FAILED",
    "IN_PROGRESS",
    "SUCCESS",
]
```
## InferenceSchedulerStatusType

```python
# InferenceSchedulerStatusType usage example

from types_aiobotocore_lookoutequipment.literals import InferenceSchedulerStatusType

def get_value() -> InferenceSchedulerStatusType:
    return "PENDING"
```

```python
# InferenceSchedulerStatusType definition

InferenceSchedulerStatusType = Literal[
    "PENDING",
    "RUNNING",
    "STOPPED",
    "STOPPING",
]
```
## IngestionJobStatusType

```python
# IngestionJobStatusType usage example

from types_aiobotocore_lookoutequipment.literals import IngestionJobStatusType

def get_value() -> IngestionJobStatusType:
    return "FAILED"
```

```python
# IngestionJobStatusType definition

IngestionJobStatusType = Literal[
    "FAILED",
    "IMPORT_IN_PROGRESS",
    "IN_PROGRESS",
    "SUCCESS",
]
```
## LabelRatingType

```python
# LabelRatingType usage example

from types_aiobotocore_lookoutequipment.literals import LabelRatingType

def get_value() -> LabelRatingType:
    return "ANOMALY"
```

```python
# LabelRatingType definition

LabelRatingType = Literal[
    "ANOMALY",
    "NEUTRAL",
    "NO_ANOMALY",
]
```
## LatestInferenceResultType

```python
# LatestInferenceResultType usage example

from types_aiobotocore_lookoutequipment.literals import LatestInferenceResultType

def get_value() -> LatestInferenceResultType:
    return "ANOMALOUS"
```

```python
# LatestInferenceResultType definition

LatestInferenceResultType = Literal[
    "ANOMALOUS",
    "NORMAL",
]
```
## ModelPromoteModeType

```python
# ModelPromoteModeType usage example

from types_aiobotocore_lookoutequipment.literals import ModelPromoteModeType

def get_value() -> ModelPromoteModeType:
    return "MANAGED"
```

```python
# ModelPromoteModeType definition

ModelPromoteModeType = Literal[
    "MANAGED",
    "MANUAL",
]
```
## ModelQualityType

```python
# ModelQualityType usage example

from types_aiobotocore_lookoutequipment.literals import ModelQualityType

def get_value() -> ModelQualityType:
    return "CANNOT_DETERMINE_QUALITY"
```

```python
# ModelQualityType definition

ModelQualityType = Literal[
    "CANNOT_DETERMINE_QUALITY",
    "POOR_QUALITY_DETECTED",
    "QUALITY_THRESHOLD_MET",
]
```
## ModelStatusType

```python
# ModelStatusType usage example

from types_aiobotocore_lookoutequipment.literals import ModelStatusType

def get_value() -> ModelStatusType:
    return "FAILED"
```

```python
# ModelStatusType definition

ModelStatusType = Literal[
    "FAILED",
    "IMPORT_IN_PROGRESS",
    "IN_PROGRESS",
    "SUCCESS",
]
```
## ModelVersionSourceTypeType

```python
# ModelVersionSourceTypeType usage example

from types_aiobotocore_lookoutequipment.literals import ModelVersionSourceTypeType

def get_value() -> ModelVersionSourceTypeType:
    return "IMPORT"
```

```python
# ModelVersionSourceTypeType definition

ModelVersionSourceTypeType = Literal[
    "IMPORT",
    "RETRAINING",
    "TRAINING",
]
```
## ModelVersionStatusType

```python
# ModelVersionStatusType usage example

from types_aiobotocore_lookoutequipment.literals import ModelVersionStatusType

def get_value() -> ModelVersionStatusType:
    return "CANCELED"
```

```python
# ModelVersionStatusType definition

ModelVersionStatusType = Literal[
    "CANCELED",
    "FAILED",
    "IMPORT_IN_PROGRESS",
    "IN_PROGRESS",
    "SUCCESS",
]
```
## MonotonicityType

```python
# MonotonicityType usage example

from types_aiobotocore_lookoutequipment.literals import MonotonicityType

def get_value() -> MonotonicityType:
    return "DECREASING"
```

```python
# MonotonicityType definition

MonotonicityType = Literal[
    "DECREASING",
    "INCREASING",
    "STATIC",
]
```
## RetrainingSchedulerStatusType

```python
# RetrainingSchedulerStatusType usage example

from types_aiobotocore_lookoutequipment.literals import RetrainingSchedulerStatusType

def get_value() -> RetrainingSchedulerStatusType:
    return "PENDING"
```

```python
# RetrainingSchedulerStatusType definition

RetrainingSchedulerStatusType = Literal[
    "PENDING",
    "RUNNING",
    "STOPPED",
    "STOPPING",
]
```
## StatisticalIssueStatusType

```python
# StatisticalIssueStatusType usage example

from types_aiobotocore_lookoutequipment.literals import StatisticalIssueStatusType

def get_value() -> StatisticalIssueStatusType:
    return "NO_ISSUE_DETECTED"
```

```python
# StatisticalIssueStatusType definition

StatisticalIssueStatusType = Literal[
    "NO_ISSUE_DETECTED",
    "POTENTIAL_ISSUE_DETECTED",
]
```
## TargetSamplingRateType

```python
# TargetSamplingRateType usage example

from types_aiobotocore_lookoutequipment.literals import TargetSamplingRateType

def get_value() -> TargetSamplingRateType:
    return "PT10M"
```

```python
# TargetSamplingRateType definition

TargetSamplingRateType = Literal[
    "PT10M",
    "PT10S",
    "PT15M",
    "PT15S",
    "PT1H",
    "PT1M",
    "PT1S",
    "PT30M",
    "PT30S",
    "PT5M",
    "PT5S",
]
```
## LookoutEquipmentServiceName

```python
# LookoutEquipmentServiceName usage example

from types_aiobotocore_lookoutequipment.literals import LookoutEquipmentServiceName

def get_value() -> LookoutEquipmentServiceName:
    return "lookoutequipment"
```

```python
# LookoutEquipmentServiceName definition

LookoutEquipmentServiceName = Literal[
    "lookoutequipment",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_lookoutequipment.literals import ServiceName

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

from types_aiobotocore_lookoutequipment.literals import ResourceServiceName

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
## RegionName

```python
# RegionName usage example

from types_aiobotocore_lookoutequipment.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-2"
```

```python
# RegionName definition

RegionName = Literal[
    "ap-northeast-2",
    "eu-west-1",
    "us-east-1",
]
```