# Literals

> [Index](../README.md) > [AppRegistry](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [AppRegistry](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
    type annotations stubs module [types-aiobotocore-servicecatalog-appregistry](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry/).

## ListApplicationsPaginatorName

```python title="Usage Example"
from types_aiobotocore_servicecatalog_appregistry.literals import ListApplicationsPaginatorName

def get_value() -> ListApplicationsPaginatorName:
    return "list_applications"
```

```python title="Definition"
ListApplicationsPaginatorName = Literal[
    "list_applications",
]
```
## ListAssociatedAttributeGroupsPaginatorName

```python title="Usage Example"
from types_aiobotocore_servicecatalog_appregistry.literals import ListAssociatedAttributeGroupsPaginatorName

def get_value() -> ListAssociatedAttributeGroupsPaginatorName:
    return "list_associated_attribute_groups"
```

```python title="Definition"
ListAssociatedAttributeGroupsPaginatorName = Literal[
    "list_associated_attribute_groups",
]
```
## ListAssociatedResourcesPaginatorName

```python title="Usage Example"
from types_aiobotocore_servicecatalog_appregistry.literals import ListAssociatedResourcesPaginatorName

def get_value() -> ListAssociatedResourcesPaginatorName:
    return "list_associated_resources"
```

```python title="Definition"
ListAssociatedResourcesPaginatorName = Literal[
    "list_associated_resources",
]
```
## ListAttributeGroupsForApplicationPaginatorName

```python title="Usage Example"
from types_aiobotocore_servicecatalog_appregistry.literals import ListAttributeGroupsForApplicationPaginatorName

def get_value() -> ListAttributeGroupsForApplicationPaginatorName:
    return "list_attribute_groups_for_application"
```

```python title="Definition"
ListAttributeGroupsForApplicationPaginatorName = Literal[
    "list_attribute_groups_for_application",
]
```
## ListAttributeGroupsPaginatorName

```python title="Usage Example"
from types_aiobotocore_servicecatalog_appregistry.literals import ListAttributeGroupsPaginatorName

def get_value() -> ListAttributeGroupsPaginatorName:
    return "list_attribute_groups"
```

```python title="Definition"
ListAttributeGroupsPaginatorName = Literal[
    "list_attribute_groups",
]
```
## ResourceGroupStateType

```python title="Usage Example"
from types_aiobotocore_servicecatalog_appregistry.literals import ResourceGroupStateType

def get_value() -> ResourceGroupStateType:
    return "CREATE_COMPLETE"
```

```python title="Definition"
ResourceGroupStateType = Literal[
    "CREATE_COMPLETE",
    "CREATE_FAILED",
    "CREATING",
    "UPDATE_COMPLETE",
    "UPDATE_FAILED",
    "UPDATING",
]
```
## ResourceTypeType

```python title="Usage Example"
from types_aiobotocore_servicecatalog_appregistry.literals import ResourceTypeType

def get_value() -> ResourceTypeType:
    return "CFN_STACK"
```

```python title="Definition"
ResourceTypeType = Literal[
    "CFN_STACK",
]
```
## SyncActionType

```python title="Usage Example"
from types_aiobotocore_servicecatalog_appregistry.literals import SyncActionType

def get_value() -> SyncActionType:
    return "NO_ACTION"
```

```python title="Definition"
SyncActionType = Literal[
    "NO_ACTION",
    "START_SYNC",
]
```
## AppRegistryServiceName

```python title="Usage Example"
from types_aiobotocore_servicecatalog_appregistry.literals import AppRegistryServiceName

def get_value() -> AppRegistryServiceName:
    return "servicecatalog-appregistry"
```

```python title="Definition"
AppRegistryServiceName = Literal[
    "servicecatalog-appregistry",
]
```
## ServiceName

```python title="Usage Example"
from types_aiobotocore_servicecatalog_appregistry.literals import ServiceName

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
from types_aiobotocore_servicecatalog_appregistry.literals import ResourceServiceName

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
from types_aiobotocore_servicecatalog_appregistry.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_applications"
```

```python title="Definition"
PaginatorName = Literal[
    "list_applications",
    "list_associated_attribute_groups",
    "list_associated_resources",
    "list_attribute_groups",
    "list_attribute_groups_for_application",
]
```
## RegionName

```python title="Usage Example"
from types_aiobotocore_servicecatalog_appregistry.literals import RegionName

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
