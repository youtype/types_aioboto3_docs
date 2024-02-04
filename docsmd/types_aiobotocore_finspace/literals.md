# Literals

> [Index](../README.md) > [finspace](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [finspace](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
    type annotations stubs module [types-aiobotocore-finspace](https://pypi.org/project/types-aiobotocore-finspace/).

## AutoScalingMetricType

```python
# AutoScalingMetricType usage example

from types_aiobotocore_finspace.literals import AutoScalingMetricType

def get_value() -> AutoScalingMetricType:
    return "CPU_UTILIZATION_PERCENTAGE"
```

```python
# AutoScalingMetricType definition

AutoScalingMetricType = Literal[
    "CPU_UTILIZATION_PERCENTAGE",
]
```
## ChangeTypeType

```python
# ChangeTypeType usage example

from types_aiobotocore_finspace.literals import ChangeTypeType

def get_value() -> ChangeTypeType:
    return "DELETE"
```

```python
# ChangeTypeType definition

ChangeTypeType = Literal[
    "DELETE",
    "PUT",
]
```
## ChangesetStatusType

```python
# ChangesetStatusType usage example

from types_aiobotocore_finspace.literals import ChangesetStatusType

def get_value() -> ChangesetStatusType:
    return "COMPLETED"
```

```python
# ChangesetStatusType definition

ChangesetStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "PENDING",
    "PROCESSING",
]
```
## EnvironmentStatusType

```python
# EnvironmentStatusType usage example

from types_aiobotocore_finspace.literals import EnvironmentStatusType

def get_value() -> EnvironmentStatusType:
    return "CREATED"
```

```python
# EnvironmentStatusType definition

EnvironmentStatusType = Literal[
    "CREATE_REQUESTED",
    "CREATED",
    "CREATING",
    "DELETE_REQUESTED",
    "DELETED",
    "DELETING",
    "FAILED_CREATION",
    "FAILED_DELETION",
    "FAILED_UPDATING_NETWORK",
    "RETRY_DELETION",
    "SUSPENDED",
    "UPDATE_NETWORK_REQUESTED",
    "UPDATING_NETWORK",
]
```
## ErrorDetailsType

```python
# ErrorDetailsType usage example

from types_aiobotocore_finspace.literals import ErrorDetailsType

def get_value() -> ErrorDetailsType:
    return "A user recoverable error has occurred"
```

```python
# ErrorDetailsType definition

ErrorDetailsType = Literal[
    "A user recoverable error has occurred",
    "An internal error has occurred.",
    "Cancelled",
    "Missing required permission to perform this request.",
    "One or more inputs to this request were not found.",
    "Service limits have been exceeded.",
    "The inputs to this request are invalid.",
    "The system temporarily lacks sufficient resources to process the request.",
]
```
## FederationModeType

```python
# FederationModeType usage example

from types_aiobotocore_finspace.literals import FederationModeType

def get_value() -> FederationModeType:
    return "FEDERATED"
```

```python
# FederationModeType definition

FederationModeType = Literal[
    "FEDERATED",
    "LOCAL",
]
```
## IPAddressTypeType

```python
# IPAddressTypeType usage example

from types_aiobotocore_finspace.literals import IPAddressTypeType

def get_value() -> IPAddressTypeType:
    return "IP_V4"
```

```python
# IPAddressTypeType definition

IPAddressTypeType = Literal[
    "IP_V4",
]
```
## KxAzModeType

```python
# KxAzModeType usage example

from types_aiobotocore_finspace.literals import KxAzModeType

def get_value() -> KxAzModeType:
    return "MULTI"
```

```python
# KxAzModeType definition

KxAzModeType = Literal[
    "MULTI",
    "SINGLE",
]
```
## KxClusterCodeDeploymentStrategyType

```python
# KxClusterCodeDeploymentStrategyType usage example

from types_aiobotocore_finspace.literals import KxClusterCodeDeploymentStrategyType

def get_value() -> KxClusterCodeDeploymentStrategyType:
    return "FORCE"
```

```python
# KxClusterCodeDeploymentStrategyType definition

KxClusterCodeDeploymentStrategyType = Literal[
    "FORCE",
    "NO_RESTART",
    "ROLLING",
]
```
## KxClusterStatusType

```python
# KxClusterStatusType usage example

from types_aiobotocore_finspace.literals import KxClusterStatusType

def get_value() -> KxClusterStatusType:
    return "CREATE_FAILED"
```

```python
# KxClusterStatusType definition

KxClusterStatusType = Literal[
    "CREATE_FAILED",
    "CREATING",
    "DELETE_FAILED",
    "DELETED",
    "DELETING",
    "PENDING",
    "RUNNING",
    "UPDATING",
]
```
## KxClusterTypeType

```python
# KxClusterTypeType usage example

from types_aiobotocore_finspace.literals import KxClusterTypeType

def get_value() -> KxClusterTypeType:
    return "GATEWAY"
```

```python
# KxClusterTypeType definition

KxClusterTypeType = Literal[
    "GATEWAY",
    "GP",
    "HDB",
    "RDB",
    "TICKERPLANT",
]
```
## KxDataviewStatusType

```python
# KxDataviewStatusType usage example

from types_aiobotocore_finspace.literals import KxDataviewStatusType

def get_value() -> KxDataviewStatusType:
    return "ACTIVE"
```

```python
# KxDataviewStatusType definition

KxDataviewStatusType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETING",
    "FAILED",
    "UPDATING",
]
```
## KxDeploymentStrategyType

```python
# KxDeploymentStrategyType usage example

from types_aiobotocore_finspace.literals import KxDeploymentStrategyType

def get_value() -> KxDeploymentStrategyType:
    return "NO_RESTART"
```

```python
# KxDeploymentStrategyType definition

KxDeploymentStrategyType = Literal[
    "NO_RESTART",
    "ROLLING",
]
```
## KxNAS1TypeType

```python
# KxNAS1TypeType usage example

from types_aiobotocore_finspace.literals import KxNAS1TypeType

def get_value() -> KxNAS1TypeType:
    return "HDD_12"
```

```python
# KxNAS1TypeType definition

KxNAS1TypeType = Literal[
    "HDD_12",
    "SSD_1000",
    "SSD_250",
]
```
## KxSavedownStorageTypeType

```python
# KxSavedownStorageTypeType usage example

from types_aiobotocore_finspace.literals import KxSavedownStorageTypeType

def get_value() -> KxSavedownStorageTypeType:
    return "SDS01"
```

```python
# KxSavedownStorageTypeType definition

KxSavedownStorageTypeType = Literal[
    "SDS01",
]
```
## KxScalingGroupStatusType

```python
# KxScalingGroupStatusType usage example

from types_aiobotocore_finspace.literals import KxScalingGroupStatusType

def get_value() -> KxScalingGroupStatusType:
    return "ACTIVE"
```

```python
# KxScalingGroupStatusType definition

KxScalingGroupStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATING",
    "DELETE_FAILED",
    "DELETED",
    "DELETING",
]
```
## KxVolumeStatusType

```python
# KxVolumeStatusType usage example

from types_aiobotocore_finspace.literals import KxVolumeStatusType

def get_value() -> KxVolumeStatusType:
    return "ACTIVE"
```

```python
# KxVolumeStatusType definition

KxVolumeStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATING",
    "DELETE_FAILED",
    "DELETED",
    "DELETING",
    "UPDATE_FAILED",
    "UPDATED",
    "UPDATING",
]
```
## KxVolumeTypeType

```python
# KxVolumeTypeType usage example

from types_aiobotocore_finspace.literals import KxVolumeTypeType

def get_value() -> KxVolumeTypeType:
    return "NAS_1"
```

```python
# KxVolumeTypeType definition

KxVolumeTypeType = Literal[
    "NAS_1",
]
```
## ListKxEnvironmentsPaginatorName

```python
# ListKxEnvironmentsPaginatorName usage example

from types_aiobotocore_finspace.literals import ListKxEnvironmentsPaginatorName

def get_value() -> ListKxEnvironmentsPaginatorName:
    return "list_kx_environments"
```

```python
# ListKxEnvironmentsPaginatorName definition

ListKxEnvironmentsPaginatorName = Literal[
    "list_kx_environments",
]
```
## RuleActionType

```python
# RuleActionType usage example

from types_aiobotocore_finspace.literals import RuleActionType

def get_value() -> RuleActionType:
    return "allow"
```

```python
# RuleActionType definition

RuleActionType = Literal[
    "allow",
    "deny",
]
```
## VolumeTypeType

```python
# VolumeTypeType usage example

from types_aiobotocore_finspace.literals import VolumeTypeType

def get_value() -> VolumeTypeType:
    return "NAS_1"
```

```python
# VolumeTypeType definition

VolumeTypeType = Literal[
    "NAS_1",
]
```
## dnsStatusType

```python
# dnsStatusType usage example

from types_aiobotocore_finspace.literals import dnsStatusType

def get_value() -> dnsStatusType:
    return "FAILED_UPDATE"
```

```python
# dnsStatusType definition

dnsStatusType = Literal[
    "FAILED_UPDATE",
    "NONE",
    "SUCCESSFULLY_UPDATED",
    "UPDATE_REQUESTED",
    "UPDATING",
]
```
## tgwStatusType

```python
# tgwStatusType usage example

from types_aiobotocore_finspace.literals import tgwStatusType

def get_value() -> tgwStatusType:
    return "FAILED_UPDATE"
```

```python
# tgwStatusType definition

tgwStatusType = Literal[
    "FAILED_UPDATE",
    "NONE",
    "SUCCESSFULLY_UPDATED",
    "UPDATE_REQUESTED",
    "UPDATING",
]
```
## finspaceServiceName

```python
# finspaceServiceName usage example

from types_aiobotocore_finspace.literals import finspaceServiceName

def get_value() -> finspaceServiceName:
    return "finspace"
```

```python
# finspaceServiceName definition

finspaceServiceName = Literal[
    "finspace",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_finspace.literals import ServiceName

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

from types_aiobotocore_finspace.literals import ResourceServiceName

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

from types_aiobotocore_finspace.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_kx_environments"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_kx_environments",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_finspace.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-1"
```

```python
# RegionName definition

RegionName = Literal[
    "ap-northeast-1",
    "ap-southeast-1",
    "ap-southeast-2",
    "ca-central-1",
    "eu-central-1",
    "eu-west-1",
    "eu-west-2",
    "us-east-1",
    "us-east-2",
    "us-west-2",
]
```
