# Literals

> [Index](../README.md) > [AppConfig](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [AppConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#appconfig)
    type annotations stubs module [types-aiobotocore-appconfig](https://pypi.org/project/types-aiobotocore-appconfig/).

## ActionPointType

```python
# ActionPointType usage example

from types_aiobotocore_appconfig.literals import ActionPointType

def get_value() -> ActionPointType:
    return "AT_DEPLOYMENT_TICK"
```

```python
# ActionPointType definition

ActionPointType = Literal[
    "AT_DEPLOYMENT_TICK",
    "ON_DEPLOYMENT_BAKING",
    "ON_DEPLOYMENT_COMPLETE",
    "ON_DEPLOYMENT_ROLLED_BACK",
    "ON_DEPLOYMENT_START",
    "ON_DEPLOYMENT_STEP",
    "PRE_CREATE_HOSTED_CONFIGURATION_VERSION",
    "PRE_START_DEPLOYMENT",
]
```
## DeletionProtectionCheckType

```python
# DeletionProtectionCheckType usage example

from types_aiobotocore_appconfig.literals import DeletionProtectionCheckType

def get_value() -> DeletionProtectionCheckType:
    return "ACCOUNT_DEFAULT"
```

```python
# DeletionProtectionCheckType definition

DeletionProtectionCheckType = Literal[
    "ACCOUNT_DEFAULT",
    "APPLY",
    "BYPASS",
]
```
## DeploymentEventTypeType

```python
# DeploymentEventTypeType usage example

from types_aiobotocore_appconfig.literals import DeploymentEventTypeType

def get_value() -> DeploymentEventTypeType:
    return "BAKE_TIME_STARTED"
```

```python
# DeploymentEventTypeType definition

DeploymentEventTypeType = Literal[
    "BAKE_TIME_STARTED",
    "DEPLOYMENT_COMPLETED",
    "DEPLOYMENT_STARTED",
    "PERCENTAGE_UPDATED",
    "REVERT_COMPLETED",
    "ROLLBACK_COMPLETED",
    "ROLLBACK_STARTED",
]
```
## DeploymentStateType

```python
# DeploymentStateType usage example

from types_aiobotocore_appconfig.literals import DeploymentStateType

def get_value() -> DeploymentStateType:
    return "BAKING"
```

```python
# DeploymentStateType definition

DeploymentStateType = Literal[
    "BAKING",
    "COMPLETE",
    "DEPLOYING",
    "REVERTED",
    "ROLLED_BACK",
    "ROLLING_BACK",
    "VALIDATING",
]
```
## EnvironmentStateType

```python
# EnvironmentStateType usage example

from types_aiobotocore_appconfig.literals import EnvironmentStateType

def get_value() -> EnvironmentStateType:
    return "DEPLOYING"
```

```python
# EnvironmentStateType definition

EnvironmentStateType = Literal[
    "DEPLOYING",
    "READY_FOR_DEPLOYMENT",
    "REVERTED",
    "ROLLED_BACK",
    "ROLLING_BACK",
]
```
## GrowthTypeType

```python
# GrowthTypeType usage example

from types_aiobotocore_appconfig.literals import GrowthTypeType

def get_value() -> GrowthTypeType:
    return "EXPONENTIAL"
```

```python
# GrowthTypeType definition

GrowthTypeType = Literal[
    "EXPONENTIAL",
    "LINEAR",
]
```
## ListApplicationsPaginatorName

```python
# ListApplicationsPaginatorName usage example

from types_aiobotocore_appconfig.literals import ListApplicationsPaginatorName

def get_value() -> ListApplicationsPaginatorName:
    return "list_applications"
```

```python
# ListApplicationsPaginatorName definition

ListApplicationsPaginatorName = Literal[
    "list_applications",
]
```
## ListConfigurationProfilesPaginatorName

```python
# ListConfigurationProfilesPaginatorName usage example

from types_aiobotocore_appconfig.literals import ListConfigurationProfilesPaginatorName

def get_value() -> ListConfigurationProfilesPaginatorName:
    return "list_configuration_profiles"
```

```python
# ListConfigurationProfilesPaginatorName definition

ListConfigurationProfilesPaginatorName = Literal[
    "list_configuration_profiles",
]
```
## ListDeploymentStrategiesPaginatorName

```python
# ListDeploymentStrategiesPaginatorName usage example

from types_aiobotocore_appconfig.literals import ListDeploymentStrategiesPaginatorName

def get_value() -> ListDeploymentStrategiesPaginatorName:
    return "list_deployment_strategies"
```

```python
# ListDeploymentStrategiesPaginatorName definition

ListDeploymentStrategiesPaginatorName = Literal[
    "list_deployment_strategies",
]
```
## ListDeploymentsPaginatorName

```python
# ListDeploymentsPaginatorName usage example

from types_aiobotocore_appconfig.literals import ListDeploymentsPaginatorName

def get_value() -> ListDeploymentsPaginatorName:
    return "list_deployments"
```

```python
# ListDeploymentsPaginatorName definition

ListDeploymentsPaginatorName = Literal[
    "list_deployments",
]
```
## ListEnvironmentsPaginatorName

```python
# ListEnvironmentsPaginatorName usage example

from types_aiobotocore_appconfig.literals import ListEnvironmentsPaginatorName

def get_value() -> ListEnvironmentsPaginatorName:
    return "list_environments"
```

```python
# ListEnvironmentsPaginatorName definition

ListEnvironmentsPaginatorName = Literal[
    "list_environments",
]
```
## ListExtensionAssociationsPaginatorName

```python
# ListExtensionAssociationsPaginatorName usage example

from types_aiobotocore_appconfig.literals import ListExtensionAssociationsPaginatorName

def get_value() -> ListExtensionAssociationsPaginatorName:
    return "list_extension_associations"
```

```python
# ListExtensionAssociationsPaginatorName definition

ListExtensionAssociationsPaginatorName = Literal[
    "list_extension_associations",
]
```
## ListExtensionsPaginatorName

```python
# ListExtensionsPaginatorName usage example

from types_aiobotocore_appconfig.literals import ListExtensionsPaginatorName

def get_value() -> ListExtensionsPaginatorName:
    return "list_extensions"
```

```python
# ListExtensionsPaginatorName definition

ListExtensionsPaginatorName = Literal[
    "list_extensions",
]
```
## ListHostedConfigurationVersionsPaginatorName

```python
# ListHostedConfigurationVersionsPaginatorName usage example

from types_aiobotocore_appconfig.literals import ListHostedConfigurationVersionsPaginatorName

def get_value() -> ListHostedConfigurationVersionsPaginatorName:
    return "list_hosted_configuration_versions"
```

```python
# ListHostedConfigurationVersionsPaginatorName definition

ListHostedConfigurationVersionsPaginatorName = Literal[
    "list_hosted_configuration_versions",
]
```
## ReplicateToType

```python
# ReplicateToType usage example

from types_aiobotocore_appconfig.literals import ReplicateToType

def get_value() -> ReplicateToType:
    return "NONE"
```

```python
# ReplicateToType definition

ReplicateToType = Literal[
    "NONE",
    "SSM_DOCUMENT",
]
```
## TriggeredByType

```python
# TriggeredByType usage example

from types_aiobotocore_appconfig.literals import TriggeredByType

def get_value() -> TriggeredByType:
    return "APPCONFIG"
```

```python
# TriggeredByType definition

TriggeredByType = Literal[
    "APPCONFIG",
    "CLOUDWATCH_ALARM",
    "INTERNAL_ERROR",
    "USER",
]
```
## ValidatorTypeType

```python
# ValidatorTypeType usage example

from types_aiobotocore_appconfig.literals import ValidatorTypeType

def get_value() -> ValidatorTypeType:
    return "JSON_SCHEMA"
```

```python
# ValidatorTypeType definition

ValidatorTypeType = Literal[
    "JSON_SCHEMA",
    "LAMBDA",
]
```
## AppConfigServiceName

```python
# AppConfigServiceName usage example

from types_aiobotocore_appconfig.literals import AppConfigServiceName

def get_value() -> AppConfigServiceName:
    return "appconfig"
```

```python
# AppConfigServiceName definition

AppConfigServiceName = Literal[
    "appconfig",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_appconfig.literals import ServiceName

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

from types_aiobotocore_appconfig.literals import ResourceServiceName

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

from types_aiobotocore_appconfig.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_applications"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_applications",
    "list_configuration_profiles",
    "list_deployment_strategies",
    "list_deployments",
    "list_environments",
    "list_extension_associations",
    "list_extensions",
    "list_hosted_configuration_versions",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_appconfig.literals import RegionName

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
    "ap-southeast-4",
    "ap-southeast-5",
    "ca-central-1",
    "ca-west-1",
    "eu-central-1",
    "eu-central-2",
    "eu-north-1",
    "eu-south-1",
    "eu-south-2",
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