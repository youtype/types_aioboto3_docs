# Literals

> [Index](../README.md) > [QConnect](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [QConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect)
    type annotations stubs module [types-aiobotocore-qconnect](https://pypi.org/project/types-aiobotocore-qconnect/).

## AssistantCapabilityTypeType

```python
# AssistantCapabilityTypeType usage example

from types_aiobotocore_qconnect.literals import AssistantCapabilityTypeType

def get_value() -> AssistantCapabilityTypeType:
    return "V1"
```

```python
# AssistantCapabilityTypeType definition

AssistantCapabilityTypeType = Literal[
    "V1",
    "V2",
]
```
## AssistantStatusType

```python
# AssistantStatusType usage example

from types_aiobotocore_qconnect.literals import AssistantStatusType

def get_value() -> AssistantStatusType:
    return "ACTIVE"
```

```python
# AssistantStatusType definition

AssistantStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATE_IN_PROGRESS",
    "DELETE_FAILED",
    "DELETE_IN_PROGRESS",
    "DELETED",
]
```
## AssistantTypeType

```python
# AssistantTypeType usage example

from types_aiobotocore_qconnect.literals import AssistantTypeType

def get_value() -> AssistantTypeType:
    return "AGENT"
```

```python
# AssistantTypeType definition

AssistantTypeType = Literal[
    "AGENT",
]
```
## AssociationTypeType

```python
# AssociationTypeType usage example

from types_aiobotocore_qconnect.literals import AssociationTypeType

def get_value() -> AssociationTypeType:
    return "KNOWLEDGE_BASE"
```

```python
# AssociationTypeType definition

AssociationTypeType = Literal[
    "KNOWLEDGE_BASE",
]
```
## ContentStatusType

```python
# ContentStatusType usage example

from types_aiobotocore_qconnect.literals import ContentStatusType

def get_value() -> ContentStatusType:
    return "ACTIVE"
```

```python
# ContentStatusType definition

ContentStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATE_IN_PROGRESS",
    "DELETE_FAILED",
    "DELETE_IN_PROGRESS",
    "DELETED",
    "UPDATE_FAILED",
]
```
## ExternalSourceType

```python
# ExternalSourceType usage example

from types_aiobotocore_qconnect.literals import ExternalSourceType

def get_value() -> ExternalSourceType:
    return "AMAZON_CONNECT"
```

```python
# ExternalSourceType definition

ExternalSourceType = Literal[
    "AMAZON_CONNECT",
]
```
## FilterFieldType

```python
# FilterFieldType usage example

from types_aiobotocore_qconnect.literals import FilterFieldType

def get_value() -> FilterFieldType:
    return "NAME"
```

```python
# FilterFieldType definition

FilterFieldType = Literal[
    "NAME",
]
```
## FilterOperatorType

```python
# FilterOperatorType usage example

from types_aiobotocore_qconnect.literals import FilterOperatorType

def get_value() -> FilterOperatorType:
    return "EQUALS"
```

```python
# FilterOperatorType definition

FilterOperatorType = Literal[
    "EQUALS",
]
```
## ImportJobStatusType

```python
# ImportJobStatusType usage example

from types_aiobotocore_qconnect.literals import ImportJobStatusType

def get_value() -> ImportJobStatusType:
    return "COMPLETE"
```

```python
# ImportJobStatusType definition

ImportJobStatusType = Literal[
    "COMPLETE",
    "DELETE_FAILED",
    "DELETE_IN_PROGRESS",
    "DELETED",
    "FAILED",
    "START_IN_PROGRESS",
]
```
## ImportJobTypeType

```python
# ImportJobTypeType usage example

from types_aiobotocore_qconnect.literals import ImportJobTypeType

def get_value() -> ImportJobTypeType:
    return "QUICK_RESPONSES"
```

```python
# ImportJobTypeType definition

ImportJobTypeType = Literal[
    "QUICK_RESPONSES",
]
```
## KnowledgeBaseStatusType

```python
# KnowledgeBaseStatusType usage example

from types_aiobotocore_qconnect.literals import KnowledgeBaseStatusType

def get_value() -> KnowledgeBaseStatusType:
    return "ACTIVE"
```

```python
# KnowledgeBaseStatusType definition

KnowledgeBaseStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATE_IN_PROGRESS",
    "DELETE_FAILED",
    "DELETE_IN_PROGRESS",
    "DELETED",
]
```
## KnowledgeBaseTypeType

```python
# KnowledgeBaseTypeType usage example

from types_aiobotocore_qconnect.literals import KnowledgeBaseTypeType

def get_value() -> KnowledgeBaseTypeType:
    return "CUSTOM"
```

```python
# KnowledgeBaseTypeType definition

KnowledgeBaseTypeType = Literal[
    "CUSTOM",
    "EXTERNAL",
    "QUICK_RESPONSES",
]
```
## ListAssistantAssociationsPaginatorName

```python
# ListAssistantAssociationsPaginatorName usage example

from types_aiobotocore_qconnect.literals import ListAssistantAssociationsPaginatorName

def get_value() -> ListAssistantAssociationsPaginatorName:
    return "list_assistant_associations"
```

```python
# ListAssistantAssociationsPaginatorName definition

ListAssistantAssociationsPaginatorName = Literal[
    "list_assistant_associations",
]
```
## ListAssistantsPaginatorName

```python
# ListAssistantsPaginatorName usage example

from types_aiobotocore_qconnect.literals import ListAssistantsPaginatorName

def get_value() -> ListAssistantsPaginatorName:
    return "list_assistants"
```

```python
# ListAssistantsPaginatorName definition

ListAssistantsPaginatorName = Literal[
    "list_assistants",
]
```
## ListContentsPaginatorName

```python
# ListContentsPaginatorName usage example

from types_aiobotocore_qconnect.literals import ListContentsPaginatorName

def get_value() -> ListContentsPaginatorName:
    return "list_contents"
```

```python
# ListContentsPaginatorName definition

ListContentsPaginatorName = Literal[
    "list_contents",
]
```
## ListImportJobsPaginatorName

```python
# ListImportJobsPaginatorName usage example

from types_aiobotocore_qconnect.literals import ListImportJobsPaginatorName

def get_value() -> ListImportJobsPaginatorName:
    return "list_import_jobs"
```

```python
# ListImportJobsPaginatorName definition

ListImportJobsPaginatorName = Literal[
    "list_import_jobs",
]
```
## ListKnowledgeBasesPaginatorName

```python
# ListKnowledgeBasesPaginatorName usage example

from types_aiobotocore_qconnect.literals import ListKnowledgeBasesPaginatorName

def get_value() -> ListKnowledgeBasesPaginatorName:
    return "list_knowledge_bases"
```

```python
# ListKnowledgeBasesPaginatorName definition

ListKnowledgeBasesPaginatorName = Literal[
    "list_knowledge_bases",
]
```
## ListQuickResponsesPaginatorName

```python
# ListQuickResponsesPaginatorName usage example

from types_aiobotocore_qconnect.literals import ListQuickResponsesPaginatorName

def get_value() -> ListQuickResponsesPaginatorName:
    return "list_quick_responses"
```

```python
# ListQuickResponsesPaginatorName definition

ListQuickResponsesPaginatorName = Literal[
    "list_quick_responses",
]
```
## OrderType

```python
# OrderType usage example

from types_aiobotocore_qconnect.literals import OrderType

def get_value() -> OrderType:
    return "ASC"
```

```python
# OrderType definition

OrderType = Literal[
    "ASC",
    "DESC",
]
```
## PriorityType

```python
# PriorityType usage example

from types_aiobotocore_qconnect.literals import PriorityType

def get_value() -> PriorityType:
    return "HIGH"
```

```python
# PriorityType definition

PriorityType = Literal[
    "HIGH",
    "LOW",
    "MEDIUM",
]
```
## QueryAssistantPaginatorName

```python
# QueryAssistantPaginatorName usage example

from types_aiobotocore_qconnect.literals import QueryAssistantPaginatorName

def get_value() -> QueryAssistantPaginatorName:
    return "query_assistant"
```

```python
# QueryAssistantPaginatorName definition

QueryAssistantPaginatorName = Literal[
    "query_assistant",
]
```
## QueryConditionComparisonOperatorType

```python
# QueryConditionComparisonOperatorType usage example

from types_aiobotocore_qconnect.literals import QueryConditionComparisonOperatorType

def get_value() -> QueryConditionComparisonOperatorType:
    return "EQUALS"
```

```python
# QueryConditionComparisonOperatorType definition

QueryConditionComparisonOperatorType = Literal[
    "EQUALS",
]
```
## QueryConditionFieldNameType

```python
# QueryConditionFieldNameType usage example

from types_aiobotocore_qconnect.literals import QueryConditionFieldNameType

def get_value() -> QueryConditionFieldNameType:
    return "RESULT_TYPE"
```

```python
# QueryConditionFieldNameType definition

QueryConditionFieldNameType = Literal[
    "RESULT_TYPE",
]
```
## QueryResultTypeType

```python
# QueryResultTypeType usage example

from types_aiobotocore_qconnect.literals import QueryResultTypeType

def get_value() -> QueryResultTypeType:
    return "GENERATIVE_ANSWER"
```

```python
# QueryResultTypeType definition

QueryResultTypeType = Literal[
    "GENERATIVE_ANSWER",
    "KNOWLEDGE_CONTENT",
]
```
## QuickResponseFilterOperatorType

```python
# QuickResponseFilterOperatorType usage example

from types_aiobotocore_qconnect.literals import QuickResponseFilterOperatorType

def get_value() -> QuickResponseFilterOperatorType:
    return "EQUALS"
```

```python
# QuickResponseFilterOperatorType definition

QuickResponseFilterOperatorType = Literal[
    "EQUALS",
    "PREFIX",
]
```
## QuickResponseQueryOperatorType

```python
# QuickResponseQueryOperatorType usage example

from types_aiobotocore_qconnect.literals import QuickResponseQueryOperatorType

def get_value() -> QuickResponseQueryOperatorType:
    return "CONTAINS"
```

```python
# QuickResponseQueryOperatorType definition

QuickResponseQueryOperatorType = Literal[
    "CONTAINS",
    "CONTAINS_AND_PREFIX",
]
```
## QuickResponseStatusType

```python
# QuickResponseStatusType usage example

from types_aiobotocore_qconnect.literals import QuickResponseStatusType

def get_value() -> QuickResponseStatusType:
    return "CREATED"
```

```python
# QuickResponseStatusType definition

QuickResponseStatusType = Literal[
    "CREATE_FAILED",
    "CREATE_IN_PROGRESS",
    "CREATED",
    "DELETE_FAILED",
    "DELETE_IN_PROGRESS",
    "DELETED",
    "UPDATE_FAILED",
    "UPDATE_IN_PROGRESS",
]
```
## RecommendationSourceTypeType

```python
# RecommendationSourceTypeType usage example

from types_aiobotocore_qconnect.literals import RecommendationSourceTypeType

def get_value() -> RecommendationSourceTypeType:
    return "ISSUE_DETECTION"
```

```python
# RecommendationSourceTypeType definition

RecommendationSourceTypeType = Literal[
    "ISSUE_DETECTION",
    "OTHER",
    "RULE_EVALUATION",
]
```
## RecommendationTriggerTypeType

```python
# RecommendationTriggerTypeType usage example

from types_aiobotocore_qconnect.literals import RecommendationTriggerTypeType

def get_value() -> RecommendationTriggerTypeType:
    return "GENERATIVE"
```

```python
# RecommendationTriggerTypeType definition

RecommendationTriggerTypeType = Literal[
    "GENERATIVE",
    "QUERY",
]
```
## RecommendationTypeType

```python
# RecommendationTypeType usage example

from types_aiobotocore_qconnect.literals import RecommendationTypeType

def get_value() -> RecommendationTypeType:
    return "GENERATIVE_ANSWER"
```

```python
# RecommendationTypeType definition

RecommendationTypeType = Literal[
    "GENERATIVE_ANSWER",
    "GENERATIVE_RESPONSE",
    "KNOWLEDGE_CONTENT",
]
```
## RelevanceLevelType

```python
# RelevanceLevelType usage example

from types_aiobotocore_qconnect.literals import RelevanceLevelType

def get_value() -> RelevanceLevelType:
    return "HIGH"
```

```python
# RelevanceLevelType definition

RelevanceLevelType = Literal[
    "HIGH",
    "LOW",
    "MEDIUM",
]
```
## RelevanceType

```python
# RelevanceType usage example

from types_aiobotocore_qconnect.literals import RelevanceType

def get_value() -> RelevanceType:
    return "HELPFUL"
```

```python
# RelevanceType definition

RelevanceType = Literal[
    "HELPFUL",
    "NOT_HELPFUL",
]
```
## SearchContentPaginatorName

```python
# SearchContentPaginatorName usage example

from types_aiobotocore_qconnect.literals import SearchContentPaginatorName

def get_value() -> SearchContentPaginatorName:
    return "search_content"
```

```python
# SearchContentPaginatorName definition

SearchContentPaginatorName = Literal[
    "search_content",
]
```
## SearchQuickResponsesPaginatorName

```python
# SearchQuickResponsesPaginatorName usage example

from types_aiobotocore_qconnect.literals import SearchQuickResponsesPaginatorName

def get_value() -> SearchQuickResponsesPaginatorName:
    return "search_quick_responses"
```

```python
# SearchQuickResponsesPaginatorName definition

SearchQuickResponsesPaginatorName = Literal[
    "search_quick_responses",
]
```
## SearchSessionsPaginatorName

```python
# SearchSessionsPaginatorName usage example

from types_aiobotocore_qconnect.literals import SearchSessionsPaginatorName

def get_value() -> SearchSessionsPaginatorName:
    return "search_sessions"
```

```python
# SearchSessionsPaginatorName definition

SearchSessionsPaginatorName = Literal[
    "search_sessions",
]
```
## SourceContentTypeType

```python
# SourceContentTypeType usage example

from types_aiobotocore_qconnect.literals import SourceContentTypeType

def get_value() -> SourceContentTypeType:
    return "KNOWLEDGE_CONTENT"
```

```python
# SourceContentTypeType definition

SourceContentTypeType = Literal[
    "KNOWLEDGE_CONTENT",
]
```
## TargetTypeType

```python
# TargetTypeType usage example

from types_aiobotocore_qconnect.literals import TargetTypeType

def get_value() -> TargetTypeType:
    return "RECOMMENDATION"
```

```python
# TargetTypeType definition

TargetTypeType = Literal[
    "RECOMMENDATION",
    "RESULT",
]
```
## QConnectServiceName

```python
# QConnectServiceName usage example

from types_aiobotocore_qconnect.literals import QConnectServiceName

def get_value() -> QConnectServiceName:
    return "qconnect"
```

```python
# QConnectServiceName definition

QConnectServiceName = Literal[
    "qconnect",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_qconnect.literals import ServiceName

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

from types_aiobotocore_qconnect.literals import ResourceServiceName

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

from types_aiobotocore_qconnect.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_assistant_associations"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_assistant_associations",
    "list_assistants",
    "list_contents",
    "list_import_jobs",
    "list_knowledge_bases",
    "list_quick_responses",
    "query_assistant",
    "search_content",
    "search_quick_responses",
    "search_sessions",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_qconnect.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-1"
```

```python
# RegionName definition

RegionName = Literal[
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-southeast-1",
    "ap-southeast-2",
    "ca-central-1",
    "eu-central-1",
    "eu-west-2",
    "us-east-1",
    "us-west-2",
]
```
