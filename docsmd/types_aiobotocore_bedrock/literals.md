# Literals

> [Index](../README.md) > [Bedrock](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Bedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock)
    type annotations stubs module [types-aiobotocore-bedrock](https://pypi.org/project/types-aiobotocore-bedrock/).

## CommitmentDurationType

```python
# CommitmentDurationType usage example

from types_aiobotocore_bedrock.literals import CommitmentDurationType

def get_value() -> CommitmentDurationType:
    return "OneMonth"
```

```python
# CommitmentDurationType definition

CommitmentDurationType = Literal[
    "OneMonth",
    "SixMonths",
]
```
## CustomizationTypeType

```python
# CustomizationTypeType usage example

from types_aiobotocore_bedrock.literals import CustomizationTypeType

def get_value() -> CustomizationTypeType:
    return "CONTINUED_PRE_TRAINING"
```

```python
# CustomizationTypeType definition

CustomizationTypeType = Literal[
    "CONTINUED_PRE_TRAINING",
    "FINE_TUNING",
]
```
## FineTuningJobStatusType

```python
# FineTuningJobStatusType usage example

from types_aiobotocore_bedrock.literals import FineTuningJobStatusType

def get_value() -> FineTuningJobStatusType:
    return "Completed"
```

```python
# FineTuningJobStatusType definition

FineTuningJobStatusType = Literal[
    "Completed",
    "Failed",
    "InProgress",
    "Stopped",
    "Stopping",
]
```
## FoundationModelLifecycleStatusType

```python
# FoundationModelLifecycleStatusType usage example

from types_aiobotocore_bedrock.literals import FoundationModelLifecycleStatusType

def get_value() -> FoundationModelLifecycleStatusType:
    return "ACTIVE"
```

```python
# FoundationModelLifecycleStatusType definition

FoundationModelLifecycleStatusType = Literal[
    "ACTIVE",
    "LEGACY",
]
```
## InferenceTypeType

```python
# InferenceTypeType usage example

from types_aiobotocore_bedrock.literals import InferenceTypeType

def get_value() -> InferenceTypeType:
    return "ON_DEMAND"
```

```python
# InferenceTypeType definition

InferenceTypeType = Literal[
    "ON_DEMAND",
    "PROVISIONED",
]
```
## ListCustomModelsPaginatorName

```python
# ListCustomModelsPaginatorName usage example

from types_aiobotocore_bedrock.literals import ListCustomModelsPaginatorName

def get_value() -> ListCustomModelsPaginatorName:
    return "list_custom_models"
```

```python
# ListCustomModelsPaginatorName definition

ListCustomModelsPaginatorName = Literal[
    "list_custom_models",
]
```
## ListModelCustomizationJobsPaginatorName

```python
# ListModelCustomizationJobsPaginatorName usage example

from types_aiobotocore_bedrock.literals import ListModelCustomizationJobsPaginatorName

def get_value() -> ListModelCustomizationJobsPaginatorName:
    return "list_model_customization_jobs"
```

```python
# ListModelCustomizationJobsPaginatorName definition

ListModelCustomizationJobsPaginatorName = Literal[
    "list_model_customization_jobs",
]
```
## ListProvisionedModelThroughputsPaginatorName

```python
# ListProvisionedModelThroughputsPaginatorName usage example

from types_aiobotocore_bedrock.literals import ListProvisionedModelThroughputsPaginatorName

def get_value() -> ListProvisionedModelThroughputsPaginatorName:
    return "list_provisioned_model_throughputs"
```

```python
# ListProvisionedModelThroughputsPaginatorName definition

ListProvisionedModelThroughputsPaginatorName = Literal[
    "list_provisioned_model_throughputs",
]
```
## ModelCustomizationJobStatusType

```python
# ModelCustomizationJobStatusType usage example

from types_aiobotocore_bedrock.literals import ModelCustomizationJobStatusType

def get_value() -> ModelCustomizationJobStatusType:
    return "Completed"
```

```python
# ModelCustomizationJobStatusType definition

ModelCustomizationJobStatusType = Literal[
    "Completed",
    "Failed",
    "InProgress",
    "Stopped",
    "Stopping",
]
```
## ModelCustomizationType

```python
# ModelCustomizationType usage example

from types_aiobotocore_bedrock.literals import ModelCustomizationType

def get_value() -> ModelCustomizationType:
    return "CONTINUED_PRE_TRAINING"
```

```python
# ModelCustomizationType definition

ModelCustomizationType = Literal[
    "CONTINUED_PRE_TRAINING",
    "FINE_TUNING",
]
```
## ModelModalityType

```python
# ModelModalityType usage example

from types_aiobotocore_bedrock.literals import ModelModalityType

def get_value() -> ModelModalityType:
    return "EMBEDDING"
```

```python
# ModelModalityType definition

ModelModalityType = Literal[
    "EMBEDDING",
    "IMAGE",
    "TEXT",
]
```
## ProvisionedModelStatusType

```python
# ProvisionedModelStatusType usage example

from types_aiobotocore_bedrock.literals import ProvisionedModelStatusType

def get_value() -> ProvisionedModelStatusType:
    return "Creating"
```

```python
# ProvisionedModelStatusType definition

ProvisionedModelStatusType = Literal[
    "Creating",
    "Failed",
    "InService",
    "Updating",
]
```
## SortByProvisionedModelsType

```python
# SortByProvisionedModelsType usage example

from types_aiobotocore_bedrock.literals import SortByProvisionedModelsType

def get_value() -> SortByProvisionedModelsType:
    return "CreationTime"
```

```python
# SortByProvisionedModelsType definition

SortByProvisionedModelsType = Literal[
    "CreationTime",
]
```
## SortJobsByType

```python
# SortJobsByType usage example

from types_aiobotocore_bedrock.literals import SortJobsByType

def get_value() -> SortJobsByType:
    return "CreationTime"
```

```python
# SortJobsByType definition

SortJobsByType = Literal[
    "CreationTime",
]
```
## SortModelsByType

```python
# SortModelsByType usage example

from types_aiobotocore_bedrock.literals import SortModelsByType

def get_value() -> SortModelsByType:
    return "CreationTime"
```

```python
# SortModelsByType definition

SortModelsByType = Literal[
    "CreationTime",
]
```
## SortOrderType

```python
# SortOrderType usage example

from types_aiobotocore_bedrock.literals import SortOrderType

def get_value() -> SortOrderType:
    return "Ascending"
```

```python
# SortOrderType definition

SortOrderType = Literal[
    "Ascending",
    "Descending",
]
```
## BedrockServiceName

```python
# BedrockServiceName usage example

from types_aiobotocore_bedrock.literals import BedrockServiceName

def get_value() -> BedrockServiceName:
    return "bedrock"
```

```python
# BedrockServiceName definition

BedrockServiceName = Literal[
    "bedrock",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_bedrock.literals import ServiceName

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
    "appfabric",
    "appflow",
    "appintegrations",
    "application-autoscaling",
    "application-insights",
    "applicationcostprofiler",
    "appmesh",
    "apprunner",
    "appstream",
    "appsync",
    "arc-zonal-shift",
    "athena",
    "auditmanager",
    "autoscaling",
    "autoscaling-plans",
    "b2bi",
    "backup",
    "backup-gateway",
    "backupstorage",
    "batch",
    "bcm-data-exports",
    "bedrock",
    "bedrock-agent",
    "bedrock-agent-runtime",
    "bedrock-runtime",
    "billingconductor",
    "braket",
    "budgets",
    "ce",
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
    "codedeploy",
    "codeguru-reviewer",
    "codeguru-security",
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
    "connectcases",
    "connectparticipant",
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
    "inspector-scan",
    "inspector2",
    "internetmonitor",
    "iot",
    "iot-data",
    "iot-jobs-data",
    "iot-roborunner",
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
    "managedblockchain",
    "managedblockchain-query",
    "marketplace-agreement",
    "marketplace-catalog",
    "marketplace-deployment",
    "marketplace-entitlement",
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
    "mobile",
    "mq",
    "mturk",
    "mwaa",
    "neptune",
    "neptune-graph",
    "neptunedata",
    "network-firewall",
    "networkmanager",
    "networkmonitor",
    "nimble",
    "oam",
    "omics",
    "opensearch",
    "opensearchserverless",
    "opsworks",
    "opsworkscm",
    "organizations",
    "osis",
    "outposts",
    "panorama",
    "payment-cryptography",
    "payment-cryptography-data",
    "pca-connector-ad",
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
    "route53resolver",
    "rum",
    "s3",
    "s3control",
    "s3outposts",
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
    "sqs",
    "ssm",
    "ssm-contacts",
    "ssm-incidents",
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
    "textract",
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
    "worklink",
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

from types_aiobotocore_bedrock.literals import ResourceServiceName

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

from types_aiobotocore_bedrock.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_custom_models"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_custom_models",
    "list_model_customization_jobs",
    "list_provisioned_model_throughputs",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_bedrock.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-1"
```

```python
# RegionName definition

RegionName = Literal[
    "ap-northeast-1",
    "ap-southeast-1",
    "eu-central-1",
    "us-east-1",
    "us-west-2",
]
```
