# Literals

> [Index](../README.md) > [MailManager](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [MailManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager.html#mailmanager)
    type annotations stubs module [types-aiobotocore-mailmanager](https://pypi.org/project/types-aiobotocore-mailmanager/).

## AcceptActionType

```python
# AcceptActionType usage example

from types_aiobotocore_mailmanager.literals import AcceptActionType

def get_value() -> AcceptActionType:
    return "ALLOW"
```

```python
# AcceptActionType definition

AcceptActionType = Literal[
    "ALLOW",
    "DENY",
]
```
## ActionFailurePolicyType

```python
# ActionFailurePolicyType usage example

from types_aiobotocore_mailmanager.literals import ActionFailurePolicyType

def get_value() -> ActionFailurePolicyType:
    return "CONTINUE"
```

```python
# ActionFailurePolicyType definition

ActionFailurePolicyType = Literal[
    "CONTINUE",
    "DROP",
]
```
## ArchiveBooleanEmailAttributeType

```python
# ArchiveBooleanEmailAttributeType usage example

from types_aiobotocore_mailmanager.literals import ArchiveBooleanEmailAttributeType

def get_value() -> ArchiveBooleanEmailAttributeType:
    return "HAS_ATTACHMENTS"
```

```python
# ArchiveBooleanEmailAttributeType definition

ArchiveBooleanEmailAttributeType = Literal[
    "HAS_ATTACHMENTS",
]
```
## ArchiveBooleanOperatorType

```python
# ArchiveBooleanOperatorType usage example

from types_aiobotocore_mailmanager.literals import ArchiveBooleanOperatorType

def get_value() -> ArchiveBooleanOperatorType:
    return "IS_FALSE"
```

```python
# ArchiveBooleanOperatorType definition

ArchiveBooleanOperatorType = Literal[
    "IS_FALSE",
    "IS_TRUE",
]
```
## ArchiveStateType

```python
# ArchiveStateType usage example

from types_aiobotocore_mailmanager.literals import ArchiveStateType

def get_value() -> ArchiveStateType:
    return "ACTIVE"
```

```python
# ArchiveStateType definition

ArchiveStateType = Literal[
    "ACTIVE",
    "PENDING_DELETION",
]
```
## ArchiveStringEmailAttributeType

```python
# ArchiveStringEmailAttributeType usage example

from types_aiobotocore_mailmanager.literals import ArchiveStringEmailAttributeType

def get_value() -> ArchiveStringEmailAttributeType:
    return "CC"
```

```python
# ArchiveStringEmailAttributeType definition

ArchiveStringEmailAttributeType = Literal[
    "CC",
    "ENVELOPE_FROM",
    "ENVELOPE_TO",
    "FROM",
    "SUBJECT",
    "TO",
]
```
## ArchiveStringOperatorType

```python
# ArchiveStringOperatorType usage example

from types_aiobotocore_mailmanager.literals import ArchiveStringOperatorType

def get_value() -> ArchiveStringOperatorType:
    return "CONTAINS"
```

```python
# ArchiveStringOperatorType definition

ArchiveStringOperatorType = Literal[
    "CONTAINS",
]
```
## ExportStateType

```python
# ExportStateType usage example

from types_aiobotocore_mailmanager.literals import ExportStateType

def get_value() -> ExportStateType:
    return "CANCELLED"
```

```python
# ExportStateType definition

ExportStateType = Literal[
    "CANCELLED",
    "COMPLETED",
    "FAILED",
    "PREPROCESSING",
    "PROCESSING",
    "QUEUED",
]
```
## IngressBooleanOperatorType

```python
# IngressBooleanOperatorType usage example

from types_aiobotocore_mailmanager.literals import IngressBooleanOperatorType

def get_value() -> IngressBooleanOperatorType:
    return "IS_FALSE"
```

```python
# IngressBooleanOperatorType definition

IngressBooleanOperatorType = Literal[
    "IS_FALSE",
    "IS_TRUE",
]
```
## IngressIpOperatorType

```python
# IngressIpOperatorType usage example

from types_aiobotocore_mailmanager.literals import IngressIpOperatorType

def get_value() -> IngressIpOperatorType:
    return "CIDR_MATCHES"
```

```python
# IngressIpOperatorType definition

IngressIpOperatorType = Literal[
    "CIDR_MATCHES",
    "NOT_CIDR_MATCHES",
]
```
## IngressIpv4AttributeType

```python
# IngressIpv4AttributeType usage example

from types_aiobotocore_mailmanager.literals import IngressIpv4AttributeType

def get_value() -> IngressIpv4AttributeType:
    return "SENDER_IP"
```

```python
# IngressIpv4AttributeType definition

IngressIpv4AttributeType = Literal[
    "SENDER_IP",
]
```
## IngressPointStatusToUpdateType

```python
# IngressPointStatusToUpdateType usage example

from types_aiobotocore_mailmanager.literals import IngressPointStatusToUpdateType

def get_value() -> IngressPointStatusToUpdateType:
    return "ACTIVE"
```

```python
# IngressPointStatusToUpdateType definition

IngressPointStatusToUpdateType = Literal[
    "ACTIVE",
    "CLOSED",
]
```
## IngressPointStatusType

```python
# IngressPointStatusType usage example

from types_aiobotocore_mailmanager.literals import IngressPointStatusType

def get_value() -> IngressPointStatusType:
    return "ACTIVE"
```

```python
# IngressPointStatusType definition

IngressPointStatusType = Literal[
    "ACTIVE",
    "CLOSED",
    "DEPROVISIONING",
    "FAILED",
    "PROVISIONING",
    "UPDATING",
]
```
## IngressPointTypeType

```python
# IngressPointTypeType usage example

from types_aiobotocore_mailmanager.literals import IngressPointTypeType

def get_value() -> IngressPointTypeType:
    return "AUTH"
```

```python
# IngressPointTypeType definition

IngressPointTypeType = Literal[
    "AUTH",
    "OPEN",
]
```
## IngressStringEmailAttributeType

```python
# IngressStringEmailAttributeType usage example

from types_aiobotocore_mailmanager.literals import IngressStringEmailAttributeType

def get_value() -> IngressStringEmailAttributeType:
    return "RECIPIENT"
```

```python
# IngressStringEmailAttributeType definition

IngressStringEmailAttributeType = Literal[
    "RECIPIENT",
]
```
## IngressStringOperatorType

```python
# IngressStringOperatorType usage example

from types_aiobotocore_mailmanager.literals import IngressStringOperatorType

def get_value() -> IngressStringOperatorType:
    return "CONTAINS"
```

```python
# IngressStringOperatorType definition

IngressStringOperatorType = Literal[
    "CONTAINS",
    "ENDS_WITH",
    "EQUALS",
    "NOT_EQUALS",
    "STARTS_WITH",
]
```
## IngressTlsAttributeType

```python
# IngressTlsAttributeType usage example

from types_aiobotocore_mailmanager.literals import IngressTlsAttributeType

def get_value() -> IngressTlsAttributeType:
    return "TLS_PROTOCOL"
```

```python
# IngressTlsAttributeType definition

IngressTlsAttributeType = Literal[
    "TLS_PROTOCOL",
]
```
## IngressTlsProtocolAttributeType

```python
# IngressTlsProtocolAttributeType usage example

from types_aiobotocore_mailmanager.literals import IngressTlsProtocolAttributeType

def get_value() -> IngressTlsProtocolAttributeType:
    return "TLS1_2"
```

```python
# IngressTlsProtocolAttributeType definition

IngressTlsProtocolAttributeType = Literal[
    "TLS1_2",
    "TLS1_3",
]
```
## IngressTlsProtocolOperatorType

```python
# IngressTlsProtocolOperatorType usage example

from types_aiobotocore_mailmanager.literals import IngressTlsProtocolOperatorType

def get_value() -> IngressTlsProtocolOperatorType:
    return "IS"
```

```python
# IngressTlsProtocolOperatorType definition

IngressTlsProtocolOperatorType = Literal[
    "IS",
    "MINIMUM_TLS_VERSION",
]
```
## ListAddonInstancesPaginatorName

```python
# ListAddonInstancesPaginatorName usage example

from types_aiobotocore_mailmanager.literals import ListAddonInstancesPaginatorName

def get_value() -> ListAddonInstancesPaginatorName:
    return "list_addon_instances"
```

```python
# ListAddonInstancesPaginatorName definition

ListAddonInstancesPaginatorName = Literal[
    "list_addon_instances",
]
```
## ListAddonSubscriptionsPaginatorName

```python
# ListAddonSubscriptionsPaginatorName usage example

from types_aiobotocore_mailmanager.literals import ListAddonSubscriptionsPaginatorName

def get_value() -> ListAddonSubscriptionsPaginatorName:
    return "list_addon_subscriptions"
```

```python
# ListAddonSubscriptionsPaginatorName definition

ListAddonSubscriptionsPaginatorName = Literal[
    "list_addon_subscriptions",
]
```
## ListArchiveExportsPaginatorName

```python
# ListArchiveExportsPaginatorName usage example

from types_aiobotocore_mailmanager.literals import ListArchiveExportsPaginatorName

def get_value() -> ListArchiveExportsPaginatorName:
    return "list_archive_exports"
```

```python
# ListArchiveExportsPaginatorName definition

ListArchiveExportsPaginatorName = Literal[
    "list_archive_exports",
]
```
## ListArchiveSearchesPaginatorName

```python
# ListArchiveSearchesPaginatorName usage example

from types_aiobotocore_mailmanager.literals import ListArchiveSearchesPaginatorName

def get_value() -> ListArchiveSearchesPaginatorName:
    return "list_archive_searches"
```

```python
# ListArchiveSearchesPaginatorName definition

ListArchiveSearchesPaginatorName = Literal[
    "list_archive_searches",
]
```
## ListArchivesPaginatorName

```python
# ListArchivesPaginatorName usage example

from types_aiobotocore_mailmanager.literals import ListArchivesPaginatorName

def get_value() -> ListArchivesPaginatorName:
    return "list_archives"
```

```python
# ListArchivesPaginatorName definition

ListArchivesPaginatorName = Literal[
    "list_archives",
]
```
## ListIngressPointsPaginatorName

```python
# ListIngressPointsPaginatorName usage example

from types_aiobotocore_mailmanager.literals import ListIngressPointsPaginatorName

def get_value() -> ListIngressPointsPaginatorName:
    return "list_ingress_points"
```

```python
# ListIngressPointsPaginatorName definition

ListIngressPointsPaginatorName = Literal[
    "list_ingress_points",
]
```
## ListRelaysPaginatorName

```python
# ListRelaysPaginatorName usage example

from types_aiobotocore_mailmanager.literals import ListRelaysPaginatorName

def get_value() -> ListRelaysPaginatorName:
    return "list_relays"
```

```python
# ListRelaysPaginatorName definition

ListRelaysPaginatorName = Literal[
    "list_relays",
]
```
## ListRuleSetsPaginatorName

```python
# ListRuleSetsPaginatorName usage example

from types_aiobotocore_mailmanager.literals import ListRuleSetsPaginatorName

def get_value() -> ListRuleSetsPaginatorName:
    return "list_rule_sets"
```

```python
# ListRuleSetsPaginatorName definition

ListRuleSetsPaginatorName = Literal[
    "list_rule_sets",
]
```
## ListTrafficPoliciesPaginatorName

```python
# ListTrafficPoliciesPaginatorName usage example

from types_aiobotocore_mailmanager.literals import ListTrafficPoliciesPaginatorName

def get_value() -> ListTrafficPoliciesPaginatorName:
    return "list_traffic_policies"
```

```python
# ListTrafficPoliciesPaginatorName definition

ListTrafficPoliciesPaginatorName = Literal[
    "list_traffic_policies",
]
```
## MailFromType

```python
# MailFromType usage example

from types_aiobotocore_mailmanager.literals import MailFromType

def get_value() -> MailFromType:
    return "PRESERVE"
```

```python
# MailFromType definition

MailFromType = Literal[
    "PRESERVE",
    "REPLACE",
]
```
## RetentionPeriodType

```python
# RetentionPeriodType usage example

from types_aiobotocore_mailmanager.literals import RetentionPeriodType

def get_value() -> RetentionPeriodType:
    return "EIGHTEEN_MONTHS"
```

```python
# RetentionPeriodType definition

RetentionPeriodType = Literal[
    "EIGHT_YEARS",
    "EIGHTEEN_MONTHS",
    "FIVE_YEARS",
    "FOUR_YEARS",
    "NINE_MONTHS",
    "NINE_YEARS",
    "ONE_YEAR",
    "PERMANENT",
    "SEVEN_YEARS",
    "SIX_MONTHS",
    "SIX_YEARS",
    "TEN_YEARS",
    "THIRTY_MONTHS",
    "THREE_MONTHS",
    "THREE_YEARS",
    "TWO_YEARS",
]
```
## RuleBooleanEmailAttributeType

```python
# RuleBooleanEmailAttributeType usage example

from types_aiobotocore_mailmanager.literals import RuleBooleanEmailAttributeType

def get_value() -> RuleBooleanEmailAttributeType:
    return "READ_RECEIPT_REQUESTED"
```

```python
# RuleBooleanEmailAttributeType definition

RuleBooleanEmailAttributeType = Literal[
    "READ_RECEIPT_REQUESTED",
    "TLS",
    "TLS_WRAPPED",
]
```
## RuleBooleanOperatorType

```python
# RuleBooleanOperatorType usage example

from types_aiobotocore_mailmanager.literals import RuleBooleanOperatorType

def get_value() -> RuleBooleanOperatorType:
    return "IS_FALSE"
```

```python
# RuleBooleanOperatorType definition

RuleBooleanOperatorType = Literal[
    "IS_FALSE",
    "IS_TRUE",
]
```
## RuleDmarcOperatorType

```python
# RuleDmarcOperatorType usage example

from types_aiobotocore_mailmanager.literals import RuleDmarcOperatorType

def get_value() -> RuleDmarcOperatorType:
    return "EQUALS"
```

```python
# RuleDmarcOperatorType definition

RuleDmarcOperatorType = Literal[
    "EQUALS",
    "NOT_EQUALS",
]
```
## RuleDmarcPolicyType

```python
# RuleDmarcPolicyType usage example

from types_aiobotocore_mailmanager.literals import RuleDmarcPolicyType

def get_value() -> RuleDmarcPolicyType:
    return "NONE"
```

```python
# RuleDmarcPolicyType definition

RuleDmarcPolicyType = Literal[
    "NONE",
    "QUARANTINE",
    "REJECT",
]
```
## RuleIpEmailAttributeType

```python
# RuleIpEmailAttributeType usage example

from types_aiobotocore_mailmanager.literals import RuleIpEmailAttributeType

def get_value() -> RuleIpEmailAttributeType:
    return "SOURCE_IP"
```

```python
# RuleIpEmailAttributeType definition

RuleIpEmailAttributeType = Literal[
    "SOURCE_IP",
]
```
## RuleIpOperatorType

```python
# RuleIpOperatorType usage example

from types_aiobotocore_mailmanager.literals import RuleIpOperatorType

def get_value() -> RuleIpOperatorType:
    return "CIDR_MATCHES"
```

```python
# RuleIpOperatorType definition

RuleIpOperatorType = Literal[
    "CIDR_MATCHES",
    "NOT_CIDR_MATCHES",
]
```
## RuleNumberEmailAttributeType

```python
# RuleNumberEmailAttributeType usage example

from types_aiobotocore_mailmanager.literals import RuleNumberEmailAttributeType

def get_value() -> RuleNumberEmailAttributeType:
    return "MESSAGE_SIZE"
```

```python
# RuleNumberEmailAttributeType definition

RuleNumberEmailAttributeType = Literal[
    "MESSAGE_SIZE",
]
```
## RuleNumberOperatorType

```python
# RuleNumberOperatorType usage example

from types_aiobotocore_mailmanager.literals import RuleNumberOperatorType

def get_value() -> RuleNumberOperatorType:
    return "EQUALS"
```

```python
# RuleNumberOperatorType definition

RuleNumberOperatorType = Literal[
    "EQUALS",
    "GREATER_THAN",
    "GREATER_THAN_OR_EQUAL",
    "LESS_THAN",
    "LESS_THAN_OR_EQUAL",
    "NOT_EQUALS",
]
```
## RuleStringEmailAttributeType

```python
# RuleStringEmailAttributeType usage example

from types_aiobotocore_mailmanager.literals import RuleStringEmailAttributeType

def get_value() -> RuleStringEmailAttributeType:
    return "CC"
```

```python
# RuleStringEmailAttributeType definition

RuleStringEmailAttributeType = Literal[
    "CC",
    "FROM",
    "HELO",
    "MAIL_FROM",
    "RECIPIENT",
    "SENDER",
    "SUBJECT",
    "TO",
]
```
## RuleStringOperatorType

```python
# RuleStringOperatorType usage example

from types_aiobotocore_mailmanager.literals import RuleStringOperatorType

def get_value() -> RuleStringOperatorType:
    return "CONTAINS"
```

```python
# RuleStringOperatorType definition

RuleStringOperatorType = Literal[
    "CONTAINS",
    "ENDS_WITH",
    "EQUALS",
    "NOT_EQUALS",
    "STARTS_WITH",
]
```
## RuleVerdictAttributeType

```python
# RuleVerdictAttributeType usage example

from types_aiobotocore_mailmanager.literals import RuleVerdictAttributeType

def get_value() -> RuleVerdictAttributeType:
    return "DKIM"
```

```python
# RuleVerdictAttributeType definition

RuleVerdictAttributeType = Literal[
    "DKIM",
    "SPF",
]
```
## RuleVerdictOperatorType

```python
# RuleVerdictOperatorType usage example

from types_aiobotocore_mailmanager.literals import RuleVerdictOperatorType

def get_value() -> RuleVerdictOperatorType:
    return "EQUALS"
```

```python
# RuleVerdictOperatorType definition

RuleVerdictOperatorType = Literal[
    "EQUALS",
    "NOT_EQUALS",
]
```
## RuleVerdictType

```python
# RuleVerdictType usage example

from types_aiobotocore_mailmanager.literals import RuleVerdictType

def get_value() -> RuleVerdictType:
    return "FAIL"
```

```python
# RuleVerdictType definition

RuleVerdictType = Literal[
    "FAIL",
    "GRAY",
    "PASS",
    "PROCESSING_FAILED",
]
```
## SearchStateType

```python
# SearchStateType usage example

from types_aiobotocore_mailmanager.literals import SearchStateType

def get_value() -> SearchStateType:
    return "CANCELLED"
```

```python
# SearchStateType definition

SearchStateType = Literal[
    "CANCELLED",
    "COMPLETED",
    "FAILED",
    "QUEUED",
    "RUNNING",
]
```
## MailManagerServiceName

```python
# MailManagerServiceName usage example

from types_aiobotocore_mailmanager.literals import MailManagerServiceName

def get_value() -> MailManagerServiceName:
    return "mailmanager"
```

```python
# MailManagerServiceName definition

MailManagerServiceName = Literal[
    "mailmanager",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_mailmanager.literals import ServiceName

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

from types_aiobotocore_mailmanager.literals import ResourceServiceName

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

from types_aiobotocore_mailmanager.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_addon_instances"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_addon_instances",
    "list_addon_subscriptions",
    "list_archive_exports",
    "list_archive_searches",
    "list_archives",
    "list_ingress_points",
    "list_relays",
    "list_rule_sets",
    "list_traffic_policies",
]
```