# Literals

> [Index](../README.md) > [EMRContainers](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [EMRContainers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
    type annotations stubs module [types-aiobotocore-emr-containers](https://pypi.org/project/types-aiobotocore-emr-containers/).

## ContainerProviderTypeType

```python title="Usage Example"
from types_aiobotocore_emr_containers.literals import ContainerProviderTypeType

def get_value() -> ContainerProviderTypeType:
    return "EKS"
```

```python title="Definition"
ContainerProviderTypeType = Literal[
    "EKS",
]
```
## EndpointStateType

```python title="Usage Example"
from types_aiobotocore_emr_containers.literals import EndpointStateType

def get_value() -> EndpointStateType:
    return "ACTIVE"
```

```python title="Definition"
EndpointStateType = Literal[
    "ACTIVE",
    "CREATING",
    "TERMINATED",
    "TERMINATED_WITH_ERRORS",
    "TERMINATING",
]
```
## FailureReasonType

```python title="Usage Example"
from types_aiobotocore_emr_containers.literals import FailureReasonType

def get_value() -> FailureReasonType:
    return "CLUSTER_UNAVAILABLE"
```

```python title="Definition"
FailureReasonType = Literal[
    "CLUSTER_UNAVAILABLE",
    "INTERNAL_ERROR",
    "USER_ERROR",
    "VALIDATION_ERROR",
]
```
## JobRunStateType

```python title="Usage Example"
from types_aiobotocore_emr_containers.literals import JobRunStateType

def get_value() -> JobRunStateType:
    return "CANCELLED"
```

```python title="Definition"
JobRunStateType = Literal[
    "CANCEL_PENDING",
    "CANCELLED",
    "COMPLETED",
    "FAILED",
    "PENDING",
    "RUNNING",
    "SUBMITTED",
]
```
## ListJobRunsPaginatorName

```python title="Usage Example"
from types_aiobotocore_emr_containers.literals import ListJobRunsPaginatorName

def get_value() -> ListJobRunsPaginatorName:
    return "list_job_runs"
```

```python title="Definition"
ListJobRunsPaginatorName = Literal[
    "list_job_runs",
]
```
## ListManagedEndpointsPaginatorName

```python title="Usage Example"
from types_aiobotocore_emr_containers.literals import ListManagedEndpointsPaginatorName

def get_value() -> ListManagedEndpointsPaginatorName:
    return "list_managed_endpoints"
```

```python title="Definition"
ListManagedEndpointsPaginatorName = Literal[
    "list_managed_endpoints",
]
```
## ListVirtualClustersPaginatorName

```python title="Usage Example"
from types_aiobotocore_emr_containers.literals import ListVirtualClustersPaginatorName

def get_value() -> ListVirtualClustersPaginatorName:
    return "list_virtual_clusters"
```

```python title="Definition"
ListVirtualClustersPaginatorName = Literal[
    "list_virtual_clusters",
]
```
## PersistentAppUIType

```python title="Usage Example"
from types_aiobotocore_emr_containers.literals import PersistentAppUIType

def get_value() -> PersistentAppUIType:
    return "DISABLED"
```

```python title="Definition"
PersistentAppUIType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## VirtualClusterStateType

```python title="Usage Example"
from types_aiobotocore_emr_containers.literals import VirtualClusterStateType

def get_value() -> VirtualClusterStateType:
    return "ARRESTED"
```

```python title="Definition"
VirtualClusterStateType = Literal[
    "ARRESTED",
    "RUNNING",
    "TERMINATED",
    "TERMINATING",
]
```
## EMRContainersServiceName

```python title="Usage Example"
from types_aiobotocore_emr_containers.literals import EMRContainersServiceName

def get_value() -> EMRContainersServiceName:
    return "emr-containers"
```

```python title="Definition"
EMRContainersServiceName = Literal[
    "emr-containers",
]
```
## ServiceName

```python title="Usage Example"
from types_aiobotocore_emr_containers.literals import ServiceName

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
from types_aiobotocore_emr_containers.literals import ResourceServiceName

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
from types_aiobotocore_emr_containers.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_job_runs"
```

```python title="Definition"
PaginatorName = Literal[
    "list_job_runs",
    "list_managed_endpoints",
    "list_virtual_clusters",
]
```
## RegionName

```python title="Usage Example"
from types_aiobotocore_emr_containers.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-1"
```

```python title="Definition"
RegionName = Literal[
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-south-1",
    "ap-southeast-1",
    "ap-southeast-2",
    "ca-central-1",
    "eu-central-1",
    "eu-north-1",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
