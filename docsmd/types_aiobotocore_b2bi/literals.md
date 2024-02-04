# Literals

> [Index](../README.md) > [B2BI](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [B2BI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI)
    type annotations stubs module [types-aiobotocore-b2bi](https://pypi.org/project/types-aiobotocore-b2bi/).

## CapabilityTypeType

```python
# CapabilityTypeType usage example

from types_aiobotocore_b2bi.literals import CapabilityTypeType

def get_value() -> CapabilityTypeType:
    return "edi"
```

```python
# CapabilityTypeType definition

CapabilityTypeType = Literal[
    "edi",
]
```
## FileFormatType

```python
# FileFormatType usage example

from types_aiobotocore_b2bi.literals import FileFormatType

def get_value() -> FileFormatType:
    return "JSON"
```

```python
# FileFormatType definition

FileFormatType = Literal[
    "JSON",
    "XML",
]
```
## ListCapabilitiesPaginatorName

```python
# ListCapabilitiesPaginatorName usage example

from types_aiobotocore_b2bi.literals import ListCapabilitiesPaginatorName

def get_value() -> ListCapabilitiesPaginatorName:
    return "list_capabilities"
```

```python
# ListCapabilitiesPaginatorName definition

ListCapabilitiesPaginatorName = Literal[
    "list_capabilities",
]
```
## ListPartnershipsPaginatorName

```python
# ListPartnershipsPaginatorName usage example

from types_aiobotocore_b2bi.literals import ListPartnershipsPaginatorName

def get_value() -> ListPartnershipsPaginatorName:
    return "list_partnerships"
```

```python
# ListPartnershipsPaginatorName definition

ListPartnershipsPaginatorName = Literal[
    "list_partnerships",
]
```
## ListProfilesPaginatorName

```python
# ListProfilesPaginatorName usage example

from types_aiobotocore_b2bi.literals import ListProfilesPaginatorName

def get_value() -> ListProfilesPaginatorName:
    return "list_profiles"
```

```python
# ListProfilesPaginatorName definition

ListProfilesPaginatorName = Literal[
    "list_profiles",
]
```
## ListTransformersPaginatorName

```python
# ListTransformersPaginatorName usage example

from types_aiobotocore_b2bi.literals import ListTransformersPaginatorName

def get_value() -> ListTransformersPaginatorName:
    return "list_transformers"
```

```python
# ListTransformersPaginatorName definition

ListTransformersPaginatorName = Literal[
    "list_transformers",
]
```
## LoggingType

```python
# LoggingType usage example

from types_aiobotocore_b2bi.literals import LoggingType

def get_value() -> LoggingType:
    return "DISABLED"
```

```python
# LoggingType definition

LoggingType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## TransformerJobStatusType

```python
# TransformerJobStatusType usage example

from types_aiobotocore_b2bi.literals import TransformerJobStatusType

def get_value() -> TransformerJobStatusType:
    return "failed"
```

```python
# TransformerJobStatusType definition

TransformerJobStatusType = Literal[
    "failed",
    "running",
    "succeeded",
]
```
## TransformerStatusType

```python
# TransformerStatusType usage example

from types_aiobotocore_b2bi.literals import TransformerStatusType

def get_value() -> TransformerStatusType:
    return "active"
```

```python
# TransformerStatusType definition

TransformerStatusType = Literal[
    "active",
    "inactive",
]
```
## X12TransactionSetType

```python
# X12TransactionSetType usage example

from types_aiobotocore_b2bi.literals import X12TransactionSetType

def get_value() -> X12TransactionSetType:
    return "X12_110"
```

```python
# X12TransactionSetType definition

X12TransactionSetType = Literal[
    "X12_110",
    "X12_180",
    "X12_204",
    "X12_210",
    "X12_214",
    "X12_215",
    "X12_310",
    "X12_315",
    "X12_322",
    "X12_404",
    "X12_410",
    "X12_820",
    "X12_824",
    "X12_830",
    "X12_846",
    "X12_850",
    "X12_852",
    "X12_855",
    "X12_856",
    "X12_860",
    "X12_861",
    "X12_864",
    "X12_940",
    "X12_990",
    "X12_997",
]
```
## X12VersionType

```python
# X12VersionType usage example

from types_aiobotocore_b2bi.literals import X12VersionType

def get_value() -> X12VersionType:
    return "VERSION_4010"
```

```python
# X12VersionType definition

X12VersionType = Literal[
    "VERSION_4010",
    "VERSION_4030",
    "VERSION_5010",
]
```
## B2BIServiceName

```python
# B2BIServiceName usage example

from types_aiobotocore_b2bi.literals import B2BIServiceName

def get_value() -> B2BIServiceName:
    return "b2bi"
```

```python
# B2BIServiceName definition

B2BIServiceName = Literal[
    "b2bi",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_b2bi.literals import ServiceName

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

from types_aiobotocore_b2bi.literals import ResourceServiceName

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

from types_aiobotocore_b2bi.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_capabilities"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_capabilities",
    "list_partnerships",
    "list_profiles",
    "list_transformers",
]
```
