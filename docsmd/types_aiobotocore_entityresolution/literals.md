# Literals

> [Index](../README.md) > [EntityResolution](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [EntityResolution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
    type annotations stubs module [types-aiobotocore-entityresolution](https://pypi.org/project/types-aiobotocore-entityresolution/).

## AttributeMatchingModelType

```python
# AttributeMatchingModelType usage example

from types_aiobotocore_entityresolution.literals import AttributeMatchingModelType

def get_value() -> AttributeMatchingModelType:
    return "MANY_TO_MANY"
```

```python
# AttributeMatchingModelType definition

AttributeMatchingModelType = Literal[
    "MANY_TO_MANY",
    "ONE_TO_ONE",
]
```
## IdMappingTypeType

```python
# IdMappingTypeType usage example

from types_aiobotocore_entityresolution.literals import IdMappingTypeType

def get_value() -> IdMappingTypeType:
    return "PROVIDER"
```

```python
# IdMappingTypeType definition

IdMappingTypeType = Literal[
    "PROVIDER",
]
```
## IncrementalRunTypeType

```python
# IncrementalRunTypeType usage example

from types_aiobotocore_entityresolution.literals import IncrementalRunTypeType

def get_value() -> IncrementalRunTypeType:
    return "IMMEDIATE"
```

```python
# IncrementalRunTypeType definition

IncrementalRunTypeType = Literal[
    "IMMEDIATE",
]
```
## JobStatusType

```python
# JobStatusType usage example

from types_aiobotocore_entityresolution.literals import JobStatusType

def get_value() -> JobStatusType:
    return "FAILED"
```

```python
# JobStatusType definition

JobStatusType = Literal[
    "FAILED",
    "QUEUED",
    "RUNNING",
    "SUCCEEDED",
]
```
## ListIdMappingJobsPaginatorName

```python
# ListIdMappingJobsPaginatorName usage example

from types_aiobotocore_entityresolution.literals import ListIdMappingJobsPaginatorName

def get_value() -> ListIdMappingJobsPaginatorName:
    return "list_id_mapping_jobs"
```

```python
# ListIdMappingJobsPaginatorName definition

ListIdMappingJobsPaginatorName = Literal[
    "list_id_mapping_jobs",
]
```
## ListIdMappingWorkflowsPaginatorName

```python
# ListIdMappingWorkflowsPaginatorName usage example

from types_aiobotocore_entityresolution.literals import ListIdMappingWorkflowsPaginatorName

def get_value() -> ListIdMappingWorkflowsPaginatorName:
    return "list_id_mapping_workflows"
```

```python
# ListIdMappingWorkflowsPaginatorName definition

ListIdMappingWorkflowsPaginatorName = Literal[
    "list_id_mapping_workflows",
]
```
## ListMatchingJobsPaginatorName

```python
# ListMatchingJobsPaginatorName usage example

from types_aiobotocore_entityresolution.literals import ListMatchingJobsPaginatorName

def get_value() -> ListMatchingJobsPaginatorName:
    return "list_matching_jobs"
```

```python
# ListMatchingJobsPaginatorName definition

ListMatchingJobsPaginatorName = Literal[
    "list_matching_jobs",
]
```
## ListMatchingWorkflowsPaginatorName

```python
# ListMatchingWorkflowsPaginatorName usage example

from types_aiobotocore_entityresolution.literals import ListMatchingWorkflowsPaginatorName

def get_value() -> ListMatchingWorkflowsPaginatorName:
    return "list_matching_workflows"
```

```python
# ListMatchingWorkflowsPaginatorName definition

ListMatchingWorkflowsPaginatorName = Literal[
    "list_matching_workflows",
]
```
## ListProviderServicesPaginatorName

```python
# ListProviderServicesPaginatorName usage example

from types_aiobotocore_entityresolution.literals import ListProviderServicesPaginatorName

def get_value() -> ListProviderServicesPaginatorName:
    return "list_provider_services"
```

```python
# ListProviderServicesPaginatorName definition

ListProviderServicesPaginatorName = Literal[
    "list_provider_services",
]
```
## ListSchemaMappingsPaginatorName

```python
# ListSchemaMappingsPaginatorName usage example

from types_aiobotocore_entityresolution.literals import ListSchemaMappingsPaginatorName

def get_value() -> ListSchemaMappingsPaginatorName:
    return "list_schema_mappings"
```

```python
# ListSchemaMappingsPaginatorName definition

ListSchemaMappingsPaginatorName = Literal[
    "list_schema_mappings",
]
```
## ResolutionTypeType

```python
# ResolutionTypeType usage example

from types_aiobotocore_entityresolution.literals import ResolutionTypeType

def get_value() -> ResolutionTypeType:
    return "ML_MATCHING"
```

```python
# ResolutionTypeType definition

ResolutionTypeType = Literal[
    "ML_MATCHING",
    "PROVIDER",
    "RULE_MATCHING",
]
```
## SchemaAttributeTypeType

```python
# SchemaAttributeTypeType usage example

from types_aiobotocore_entityresolution.literals import SchemaAttributeTypeType

def get_value() -> SchemaAttributeTypeType:
    return "ADDRESS"
```

```python
# SchemaAttributeTypeType definition

SchemaAttributeTypeType = Literal[
    "ADDRESS",
    "ADDRESS_CITY",
    "ADDRESS_COUNTRY",
    "ADDRESS_POSTALCODE",
    "ADDRESS_STATE",
    "ADDRESS_STREET1",
    "ADDRESS_STREET2",
    "ADDRESS_STREET3",
    "DATE",
    "EMAIL_ADDRESS",
    "NAME",
    "NAME_FIRST",
    "NAME_LAST",
    "NAME_MIDDLE",
    "PHONE",
    "PHONE_COUNTRYCODE",
    "PHONE_NUMBER",
    "PROVIDER_ID",
    "STRING",
    "UNIQUE_ID",
]
```
## ServiceTypeType

```python
# ServiceTypeType usage example

from types_aiobotocore_entityresolution.literals import ServiceTypeType

def get_value() -> ServiceTypeType:
    return "ASSIGNMENT"
```

```python
# ServiceTypeType definition

ServiceTypeType = Literal[
    "ASSIGNMENT",
    "ID_MAPPING",
]
```
## EntityResolutionServiceName

```python
# EntityResolutionServiceName usage example

from types_aiobotocore_entityresolution.literals import EntityResolutionServiceName

def get_value() -> EntityResolutionServiceName:
    return "entityresolution"
```

```python
# EntityResolutionServiceName definition

EntityResolutionServiceName = Literal[
    "entityresolution",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_entityresolution.literals import ServiceName

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

from types_aiobotocore_entityresolution.literals import ResourceServiceName

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

from types_aiobotocore_entityresolution.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_id_mapping_jobs"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_id_mapping_jobs",
    "list_id_mapping_workflows",
    "list_matching_jobs",
    "list_matching_workflows",
    "list_provider_services",
    "list_schema_mappings",
]
```
