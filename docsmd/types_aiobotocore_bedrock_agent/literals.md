# Literals

> [Index](../README.md) > [AgentsforBedrock](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [AgentsforBedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
    type annotations stubs module [types-aiobotocore-bedrock-agent](https://pypi.org/project/types-aiobotocore-bedrock-agent/).

## ActionGroupSignatureType

```python
# ActionGroupSignatureType usage example

from types_aiobotocore_bedrock_agent.literals import ActionGroupSignatureType

def get_value() -> ActionGroupSignatureType:
    return "AMAZON.UserInput"
```

```python
# ActionGroupSignatureType definition

ActionGroupSignatureType = Literal[
    "AMAZON.UserInput",
]
```
## ActionGroupStateType

```python
# ActionGroupStateType usage example

from types_aiobotocore_bedrock_agent.literals import ActionGroupStateType

def get_value() -> ActionGroupStateType:
    return "DISABLED"
```

```python
# ActionGroupStateType definition

ActionGroupStateType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## AgentAliasStatusType

```python
# AgentAliasStatusType usage example

from types_aiobotocore_bedrock_agent.literals import AgentAliasStatusType

def get_value() -> AgentAliasStatusType:
    return "CREATING"
```

```python
# AgentAliasStatusType definition

AgentAliasStatusType = Literal[
    "CREATING",
    "DELETING",
    "FAILED",
    "PREPARED",
    "UPDATING",
]
```
## AgentStatusType

```python
# AgentStatusType usage example

from types_aiobotocore_bedrock_agent.literals import AgentStatusType

def get_value() -> AgentStatusType:
    return "CREATING"
```

```python
# AgentStatusType definition

AgentStatusType = Literal[
    "CREATING",
    "DELETING",
    "FAILED",
    "NOT_PREPARED",
    "PREPARED",
    "PREPARING",
    "UPDATING",
    "VERSIONING",
]
```
## ChunkingStrategyType

```python
# ChunkingStrategyType usage example

from types_aiobotocore_bedrock_agent.literals import ChunkingStrategyType

def get_value() -> ChunkingStrategyType:
    return "FIXED_SIZE"
```

```python
# ChunkingStrategyType definition

ChunkingStrategyType = Literal[
    "FIXED_SIZE",
    "NONE",
]
```
## CreationModeType

```python
# CreationModeType usage example

from types_aiobotocore_bedrock_agent.literals import CreationModeType

def get_value() -> CreationModeType:
    return "DEFAULT"
```

```python
# CreationModeType definition

CreationModeType = Literal[
    "DEFAULT",
    "OVERRIDDEN",
]
```
## DataSourceStatusType

```python
# DataSourceStatusType usage example

from types_aiobotocore_bedrock_agent.literals import DataSourceStatusType

def get_value() -> DataSourceStatusType:
    return "AVAILABLE"
```

```python
# DataSourceStatusType definition

DataSourceStatusType = Literal[
    "AVAILABLE",
    "DELETING",
]
```
## DataSourceTypeType

```python
# DataSourceTypeType usage example

from types_aiobotocore_bedrock_agent.literals import DataSourceTypeType

def get_value() -> DataSourceTypeType:
    return "S3"
```

```python
# DataSourceTypeType definition

DataSourceTypeType = Literal[
    "S3",
]
```
## IngestionJobFilterAttributeType

```python
# IngestionJobFilterAttributeType usage example

from types_aiobotocore_bedrock_agent.literals import IngestionJobFilterAttributeType

def get_value() -> IngestionJobFilterAttributeType:
    return "STATUS"
```

```python
# IngestionJobFilterAttributeType definition

IngestionJobFilterAttributeType = Literal[
    "STATUS",
]
```
## IngestionJobFilterOperatorType

```python
# IngestionJobFilterOperatorType usage example

from types_aiobotocore_bedrock_agent.literals import IngestionJobFilterOperatorType

def get_value() -> IngestionJobFilterOperatorType:
    return "EQ"
```

```python
# IngestionJobFilterOperatorType definition

IngestionJobFilterOperatorType = Literal[
    "EQ",
]
```
## IngestionJobSortByAttributeType

```python
# IngestionJobSortByAttributeType usage example

from types_aiobotocore_bedrock_agent.literals import IngestionJobSortByAttributeType

def get_value() -> IngestionJobSortByAttributeType:
    return "STARTED_AT"
```

```python
# IngestionJobSortByAttributeType definition

IngestionJobSortByAttributeType = Literal[
    "STARTED_AT",
    "STATUS",
]
```
## IngestionJobStatusType

```python
# IngestionJobStatusType usage example

from types_aiobotocore_bedrock_agent.literals import IngestionJobStatusType

def get_value() -> IngestionJobStatusType:
    return "COMPLETE"
```

```python
# IngestionJobStatusType definition

IngestionJobStatusType = Literal[
    "COMPLETE",
    "FAILED",
    "IN_PROGRESS",
    "STARTING",
]
```
## KnowledgeBaseStateType

```python
# KnowledgeBaseStateType usage example

from types_aiobotocore_bedrock_agent.literals import KnowledgeBaseStateType

def get_value() -> KnowledgeBaseStateType:
    return "DISABLED"
```

```python
# KnowledgeBaseStateType definition

KnowledgeBaseStateType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## KnowledgeBaseStatusType

```python
# KnowledgeBaseStatusType usage example

from types_aiobotocore_bedrock_agent.literals import KnowledgeBaseStatusType

def get_value() -> KnowledgeBaseStatusType:
    return "ACTIVE"
```

```python
# KnowledgeBaseStatusType definition

KnowledgeBaseStatusType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETING",
    "FAILED",
    "UPDATING",
]
```
## KnowledgeBaseStorageTypeType

```python
# KnowledgeBaseStorageTypeType usage example

from types_aiobotocore_bedrock_agent.literals import KnowledgeBaseStorageTypeType

def get_value() -> KnowledgeBaseStorageTypeType:
    return "OPENSEARCH_SERVERLESS"
```

```python
# KnowledgeBaseStorageTypeType definition

KnowledgeBaseStorageTypeType = Literal[
    "OPENSEARCH_SERVERLESS",
    "PINECONE",
    "RDS",
    "REDIS_ENTERPRISE_CLOUD",
]
```
## KnowledgeBaseTypeType

```python
# KnowledgeBaseTypeType usage example

from types_aiobotocore_bedrock_agent.literals import KnowledgeBaseTypeType

def get_value() -> KnowledgeBaseTypeType:
    return "VECTOR"
```

```python
# KnowledgeBaseTypeType definition

KnowledgeBaseTypeType = Literal[
    "VECTOR",
]
```
## ListAgentActionGroupsPaginatorName

```python
# ListAgentActionGroupsPaginatorName usage example

from types_aiobotocore_bedrock_agent.literals import ListAgentActionGroupsPaginatorName

def get_value() -> ListAgentActionGroupsPaginatorName:
    return "list_agent_action_groups"
```

```python
# ListAgentActionGroupsPaginatorName definition

ListAgentActionGroupsPaginatorName = Literal[
    "list_agent_action_groups",
]
```
## ListAgentAliasesPaginatorName

```python
# ListAgentAliasesPaginatorName usage example

from types_aiobotocore_bedrock_agent.literals import ListAgentAliasesPaginatorName

def get_value() -> ListAgentAliasesPaginatorName:
    return "list_agent_aliases"
```

```python
# ListAgentAliasesPaginatorName definition

ListAgentAliasesPaginatorName = Literal[
    "list_agent_aliases",
]
```
## ListAgentKnowledgeBasesPaginatorName

```python
# ListAgentKnowledgeBasesPaginatorName usage example

from types_aiobotocore_bedrock_agent.literals import ListAgentKnowledgeBasesPaginatorName

def get_value() -> ListAgentKnowledgeBasesPaginatorName:
    return "list_agent_knowledge_bases"
```

```python
# ListAgentKnowledgeBasesPaginatorName definition

ListAgentKnowledgeBasesPaginatorName = Literal[
    "list_agent_knowledge_bases",
]
```
## ListAgentVersionsPaginatorName

```python
# ListAgentVersionsPaginatorName usage example

from types_aiobotocore_bedrock_agent.literals import ListAgentVersionsPaginatorName

def get_value() -> ListAgentVersionsPaginatorName:
    return "list_agent_versions"
```

```python
# ListAgentVersionsPaginatorName definition

ListAgentVersionsPaginatorName = Literal[
    "list_agent_versions",
]
```
## ListAgentsPaginatorName

```python
# ListAgentsPaginatorName usage example

from types_aiobotocore_bedrock_agent.literals import ListAgentsPaginatorName

def get_value() -> ListAgentsPaginatorName:
    return "list_agents"
```

```python
# ListAgentsPaginatorName definition

ListAgentsPaginatorName = Literal[
    "list_agents",
]
```
## ListDataSourcesPaginatorName

```python
# ListDataSourcesPaginatorName usage example

from types_aiobotocore_bedrock_agent.literals import ListDataSourcesPaginatorName

def get_value() -> ListDataSourcesPaginatorName:
    return "list_data_sources"
```

```python
# ListDataSourcesPaginatorName definition

ListDataSourcesPaginatorName = Literal[
    "list_data_sources",
]
```
## ListIngestionJobsPaginatorName

```python
# ListIngestionJobsPaginatorName usage example

from types_aiobotocore_bedrock_agent.literals import ListIngestionJobsPaginatorName

def get_value() -> ListIngestionJobsPaginatorName:
    return "list_ingestion_jobs"
```

```python
# ListIngestionJobsPaginatorName definition

ListIngestionJobsPaginatorName = Literal[
    "list_ingestion_jobs",
]
```
## ListKnowledgeBasesPaginatorName

```python
# ListKnowledgeBasesPaginatorName usage example

from types_aiobotocore_bedrock_agent.literals import ListKnowledgeBasesPaginatorName

def get_value() -> ListKnowledgeBasesPaginatorName:
    return "list_knowledge_bases"
```

```python
# ListKnowledgeBasesPaginatorName definition

ListKnowledgeBasesPaginatorName = Literal[
    "list_knowledge_bases",
]
```
## PromptStateType

```python
# PromptStateType usage example

from types_aiobotocore_bedrock_agent.literals import PromptStateType

def get_value() -> PromptStateType:
    return "DISABLED"
```

```python
# PromptStateType definition

PromptStateType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## PromptTypeType

```python
# PromptTypeType usage example

from types_aiobotocore_bedrock_agent.literals import PromptTypeType

def get_value() -> PromptTypeType:
    return "KNOWLEDGE_BASE_RESPONSE_GENERATION"
```

```python
# PromptTypeType definition

PromptTypeType = Literal[
    "KNOWLEDGE_BASE_RESPONSE_GENERATION",
    "ORCHESTRATION",
    "POST_PROCESSING",
    "PRE_PROCESSING",
]
```
## SortOrderType

```python
# SortOrderType usage example

from types_aiobotocore_bedrock_agent.literals import SortOrderType

def get_value() -> SortOrderType:
    return "ASCENDING"
```

```python
# SortOrderType definition

SortOrderType = Literal[
    "ASCENDING",
    "DESCENDING",
]
```
## AgentsforBedrockServiceName

```python
# AgentsforBedrockServiceName usage example

from types_aiobotocore_bedrock_agent.literals import AgentsforBedrockServiceName

def get_value() -> AgentsforBedrockServiceName:
    return "bedrock-agent"
```

```python
# AgentsforBedrockServiceName definition

AgentsforBedrockServiceName = Literal[
    "bedrock-agent",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_bedrock_agent.literals import ServiceName

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

from types_aiobotocore_bedrock_agent.literals import ResourceServiceName

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

from types_aiobotocore_bedrock_agent.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_agent_action_groups"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_agent_action_groups",
    "list_agent_aliases",
    "list_agent_knowledge_bases",
    "list_agent_versions",
    "list_agents",
    "list_data_sources",
    "list_ingestion_jobs",
    "list_knowledge_bases",
]
```
