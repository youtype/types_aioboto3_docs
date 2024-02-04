# Literals

> [Index](../README.md) > [CostOptimizationHub](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [CostOptimizationHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub)
    type annotations stubs module [types-aiobotocore-cost-optimization-hub](https://pypi.org/project/types-aiobotocore-cost-optimization-hub/).

## ActionTypeType

```python
# ActionTypeType usage example

from types_aiobotocore_cost_optimization_hub.literals import ActionTypeType

def get_value() -> ActionTypeType:
    return "MigrateToGraviton"
```

```python
# ActionTypeType definition

ActionTypeType = Literal[
    "MigrateToGraviton",
    "PurchaseReservedInstances",
    "PurchaseSavingsPlans",
    "Rightsize",
    "Stop",
    "Upgrade",
]
```
## EnrollmentStatusType

```python
# EnrollmentStatusType usage example

from types_aiobotocore_cost_optimization_hub.literals import EnrollmentStatusType

def get_value() -> EnrollmentStatusType:
    return "Active"
```

```python
# EnrollmentStatusType definition

EnrollmentStatusType = Literal[
    "Active",
    "Inactive",
]
```
## ImplementationEffortType

```python
# ImplementationEffortType usage example

from types_aiobotocore_cost_optimization_hub.literals import ImplementationEffortType

def get_value() -> ImplementationEffortType:
    return "High"
```

```python
# ImplementationEffortType definition

ImplementationEffortType = Literal[
    "High",
    "Low",
    "Medium",
    "VeryHigh",
    "VeryLow",
]
```
## ListEnrollmentStatusesPaginatorName

```python
# ListEnrollmentStatusesPaginatorName usage example

from types_aiobotocore_cost_optimization_hub.literals import ListEnrollmentStatusesPaginatorName

def get_value() -> ListEnrollmentStatusesPaginatorName:
    return "list_enrollment_statuses"
```

```python
# ListEnrollmentStatusesPaginatorName definition

ListEnrollmentStatusesPaginatorName = Literal[
    "list_enrollment_statuses",
]
```
## ListRecommendationSummariesPaginatorName

```python
# ListRecommendationSummariesPaginatorName usage example

from types_aiobotocore_cost_optimization_hub.literals import ListRecommendationSummariesPaginatorName

def get_value() -> ListRecommendationSummariesPaginatorName:
    return "list_recommendation_summaries"
```

```python
# ListRecommendationSummariesPaginatorName definition

ListRecommendationSummariesPaginatorName = Literal[
    "list_recommendation_summaries",
]
```
## ListRecommendationsPaginatorName

```python
# ListRecommendationsPaginatorName usage example

from types_aiobotocore_cost_optimization_hub.literals import ListRecommendationsPaginatorName

def get_value() -> ListRecommendationsPaginatorName:
    return "list_recommendations"
```

```python
# ListRecommendationsPaginatorName definition

ListRecommendationsPaginatorName = Literal[
    "list_recommendations",
]
```
## MemberAccountDiscountVisibilityType

```python
# MemberAccountDiscountVisibilityType usage example

from types_aiobotocore_cost_optimization_hub.literals import MemberAccountDiscountVisibilityType

def get_value() -> MemberAccountDiscountVisibilityType:
    return "All"
```

```python
# MemberAccountDiscountVisibilityType definition

MemberAccountDiscountVisibilityType = Literal[
    "All",
    "None",
]
```
## OrderType

```python
# OrderType usage example

from types_aiobotocore_cost_optimization_hub.literals import OrderType

def get_value() -> OrderType:
    return "Asc"
```

```python
# OrderType definition

OrderType = Literal[
    "Asc",
    "Desc",
]
```
## ResourceTypeType

```python
# ResourceTypeType usage example

from types_aiobotocore_cost_optimization_hub.literals import ResourceTypeType

def get_value() -> ResourceTypeType:
    return "ComputeSavingsPlans"
```

```python
# ResourceTypeType definition

ResourceTypeType = Literal[
    "ComputeSavingsPlans",
    "EbsVolume",
    "Ec2AutoScalingGroup",
    "Ec2Instance",
    "Ec2InstanceSavingsPlans",
    "Ec2ReservedInstances",
    "EcsService",
    "ElastiCacheReservedInstances",
    "LambdaFunction",
    "OpenSearchReservedInstances",
    "RdsReservedInstances",
    "RedshiftReservedInstances",
    "SageMakerSavingsPlans",
]
```
## SavingsEstimationModeType

```python
# SavingsEstimationModeType usage example

from types_aiobotocore_cost_optimization_hub.literals import SavingsEstimationModeType

def get_value() -> SavingsEstimationModeType:
    return "AfterDiscounts"
```

```python
# SavingsEstimationModeType definition

SavingsEstimationModeType = Literal[
    "AfterDiscounts",
    "BeforeDiscounts",
]
```
## SourceType

```python
# SourceType usage example

from types_aiobotocore_cost_optimization_hub.literals import SourceType

def get_value() -> SourceType:
    return "ComputeOptimizer"
```

```python
# SourceType definition

SourceType = Literal[
    "ComputeOptimizer",
    "CostExplorer",
]
```
## CostOptimizationHubServiceName

```python
# CostOptimizationHubServiceName usage example

from types_aiobotocore_cost_optimization_hub.literals import CostOptimizationHubServiceName

def get_value() -> CostOptimizationHubServiceName:
    return "cost-optimization-hub"
```

```python
# CostOptimizationHubServiceName definition

CostOptimizationHubServiceName = Literal[
    "cost-optimization-hub",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_cost_optimization_hub.literals import ServiceName

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

from types_aiobotocore_cost_optimization_hub.literals import ResourceServiceName

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

from types_aiobotocore_cost_optimization_hub.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_enrollment_statuses"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_enrollment_statuses",
    "list_recommendation_summaries",
    "list_recommendations",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_cost_optimization_hub.literals import RegionName

def get_value() -> RegionName:
    return "us-east-1"
```

```python
# RegionName definition

RegionName = Literal[
    "us-east-1",
]
```
