# Typed dictionaries

> [Index](../README.md) > [MQ](./README.md) > Typed dictionaries

!!! note ""

    Auto-generated documentation for [MQ](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
    type annotations stubs module [types-aiobotocore-mq](https://pypi.org/project/types-aiobotocore-mq/).

## ActionRequiredTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import ActionRequiredTypeDef

def get_value() -> ActionRequiredTypeDef:
    return {
        "ActionRequiredCode": ...,
    }
```

```python title="Definition"
class ActionRequiredTypeDef(TypedDict):
    ActionRequiredCode: NotRequired[str],
    ActionRequiredInfo: NotRequired[str],
```

## AvailabilityZoneTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import AvailabilityZoneTypeDef

def get_value() -> AvailabilityZoneTypeDef:
    return {
        "Name": ...,
    }
```

```python title="Definition"
class AvailabilityZoneTypeDef(TypedDict):
    Name: NotRequired[str],
```

## EngineVersionTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import EngineVersionTypeDef

def get_value() -> EngineVersionTypeDef:
    return {
        "Name": ...,
    }
```

```python title="Definition"
class EngineVersionTypeDef(TypedDict):
    Name: NotRequired[str],
```

## BrokerInstanceTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import BrokerInstanceTypeDef

def get_value() -> BrokerInstanceTypeDef:
    return {
        "ConsoleURL": ...,
    }
```

```python title="Definition"
class BrokerInstanceTypeDef(TypedDict):
    ConsoleURL: NotRequired[str],
    Endpoints: NotRequired[List[str]],
    IpAddress: NotRequired[str],
```

## BrokerSummaryTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import BrokerSummaryTypeDef

def get_value() -> BrokerSummaryTypeDef:
    return {
        "DeploymentMode": ...,
        "EngineType": ...,
    }
```

```python title="Definition"
class BrokerSummaryTypeDef(TypedDict):
    DeploymentMode: DeploymentModeType,  # (2)
    EngineType: EngineTypeType,  # (3)
    BrokerArn: NotRequired[str],
    BrokerId: NotRequired[str],
    BrokerName: NotRequired[str],
    BrokerState: NotRequired[BrokerStateType],  # (1)
    Created: NotRequired[datetime],
    HostInstanceType: NotRequired[str],
```

1. See [:material-code-brackets: BrokerStateType](./literals.md#brokerstatetype) 
2. See [:material-code-brackets: DeploymentModeType](./literals.md#deploymentmodetype) 
3. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
## ConfigurationIdTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import ConfigurationIdTypeDef

def get_value() -> ConfigurationIdTypeDef:
    return {
        "Id": ...,
    }
```

```python title="Definition"
class ConfigurationIdTypeDef(TypedDict):
    Id: str,
    Revision: NotRequired[int],
```

## ConfigurationRevisionTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import ConfigurationRevisionTypeDef

def get_value() -> ConfigurationRevisionTypeDef:
    return {
        "Created": ...,
        "Revision": ...,
    }
```

```python title="Definition"
class ConfigurationRevisionTypeDef(TypedDict):
    Created: datetime,
    Revision: int,
    Description: NotRequired[str],
```

## EncryptionOptionsTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import EncryptionOptionsTypeDef

def get_value() -> EncryptionOptionsTypeDef:
    return {
        "UseAwsOwnedKey": ...,
    }
```

```python title="Definition"
class EncryptionOptionsTypeDef(TypedDict):
    UseAwsOwnedKey: bool,
    KmsKeyId: NotRequired[str],
```

## LdapServerMetadataInputTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import LdapServerMetadataInputTypeDef

def get_value() -> LdapServerMetadataInputTypeDef:
    return {
        "Hosts": ...,
        "RoleBase": ...,
        "RoleSearchMatching": ...,
        "ServiceAccountPassword": ...,
        "ServiceAccountUsername": ...,
        "UserBase": ...,
        "UserSearchMatching": ...,
    }
```

```python title="Definition"
class LdapServerMetadataInputTypeDef(TypedDict):
    Hosts: Sequence[str],
    RoleBase: str,
    RoleSearchMatching: str,
    ServiceAccountPassword: str,
    ServiceAccountUsername: str,
    UserBase: str,
    UserSearchMatching: str,
    RoleName: NotRequired[str],
    RoleSearchSubtree: NotRequired[bool],
    UserRoleName: NotRequired[str],
    UserSearchSubtree: NotRequired[bool],
```

## LogsTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import LogsTypeDef

def get_value() -> LogsTypeDef:
    return {
        "Audit": ...,
    }
```

```python title="Definition"
class LogsTypeDef(TypedDict):
    Audit: NotRequired[bool],
    General: NotRequired[bool],
```

## UserTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import UserTypeDef

def get_value() -> UserTypeDef:
    return {
        "Password": ...,
        "Username": ...,
    }
```

```python title="Definition"
class UserTypeDef(TypedDict):
    Password: str,
    Username: str,
    ConsoleAccess: NotRequired[bool],
    Groups: NotRequired[Sequence[str]],
```

## WeeklyStartTimeTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import WeeklyStartTimeTypeDef

def get_value() -> WeeklyStartTimeTypeDef:
    return {
        "DayOfWeek": ...,
        "TimeOfDay": ...,
    }
```

```python title="Definition"
class WeeklyStartTimeTypeDef(TypedDict):
    DayOfWeek: DayOfWeekType,  # (1)
    TimeOfDay: str,
    TimeZone: NotRequired[str],
```

1. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) 
## ResponseMetadataTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import ResponseMetadataTypeDef

def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
        "HostId": ...,
        "HTTPStatusCode": ...,
        "HTTPHeaders": ...,
        "RetryAttempts": ...,
    }
```

```python title="Definition"
class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## CreateConfigurationRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import CreateConfigurationRequestRequestTypeDef

def get_value() -> CreateConfigurationRequestRequestTypeDef:
    return {
        "EngineType": ...,
        "EngineVersion": ...,
        "Name": ...,
    }
```

```python title="Definition"
class CreateConfigurationRequestRequestTypeDef(TypedDict):
    EngineType: EngineTypeType,  # (1)
    EngineVersion: str,
    Name: str,
    AuthenticationStrategy: NotRequired[AuthenticationStrategyType],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
2. See [:material-code-brackets: AuthenticationStrategyType](./literals.md#authenticationstrategytype) 
## CreateTagsRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import CreateTagsRequestRequestTypeDef

def get_value() -> CreateTagsRequestRequestTypeDef:
    return {
        "ResourceArn": ...,
    }
```

```python title="Definition"
class CreateTagsRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: NotRequired[Mapping[str, str]],
```

## CreateUserRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import CreateUserRequestRequestTypeDef

def get_value() -> CreateUserRequestRequestTypeDef:
    return {
        "BrokerId": ...,
        "Password": ...,
        "Username": ...,
    }
```

```python title="Definition"
class CreateUserRequestRequestTypeDef(TypedDict):
    BrokerId: str,
    Password: str,
    Username: str,
    ConsoleAccess: NotRequired[bool],
    Groups: NotRequired[Sequence[str]],
```

## DeleteBrokerRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import DeleteBrokerRequestRequestTypeDef

def get_value() -> DeleteBrokerRequestRequestTypeDef:
    return {
        "BrokerId": ...,
    }
```

```python title="Definition"
class DeleteBrokerRequestRequestTypeDef(TypedDict):
    BrokerId: str,
```

## DeleteTagsRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import DeleteTagsRequestRequestTypeDef

def get_value() -> DeleteTagsRequestRequestTypeDef:
    return {
        "ResourceArn": ...,
        "TagKeys": ...,
    }
```

```python title="Definition"
class DeleteTagsRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## DeleteUserRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import DeleteUserRequestRequestTypeDef

def get_value() -> DeleteUserRequestRequestTypeDef:
    return {
        "BrokerId": ...,
        "Username": ...,
    }
```

```python title="Definition"
class DeleteUserRequestRequestTypeDef(TypedDict):
    BrokerId: str,
    Username: str,
```

## DescribeBrokerEngineTypesRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import DescribeBrokerEngineTypesRequestRequestTypeDef

def get_value() -> DescribeBrokerEngineTypesRequestRequestTypeDef:
    return {
        "EngineType": ...,
    }
```

```python title="Definition"
class DescribeBrokerEngineTypesRequestRequestTypeDef(TypedDict):
    EngineType: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeBrokerInstanceOptionsRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import DescribeBrokerInstanceOptionsRequestRequestTypeDef

def get_value() -> DescribeBrokerInstanceOptionsRequestRequestTypeDef:
    return {
        "EngineType": ...,
    }
```

```python title="Definition"
class DescribeBrokerInstanceOptionsRequestRequestTypeDef(TypedDict):
    EngineType: NotRequired[str],
    HostInstanceType: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    StorageType: NotRequired[str],
```

## DescribeBrokerRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import DescribeBrokerRequestRequestTypeDef

def get_value() -> DescribeBrokerRequestRequestTypeDef:
    return {
        "BrokerId": ...,
    }
```

```python title="Definition"
class DescribeBrokerRequestRequestTypeDef(TypedDict):
    BrokerId: str,
```

## LdapServerMetadataOutputTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import LdapServerMetadataOutputTypeDef

def get_value() -> LdapServerMetadataOutputTypeDef:
    return {
        "Hosts": ...,
        "RoleBase": ...,
        "RoleSearchMatching": ...,
        "ServiceAccountUsername": ...,
        "UserBase": ...,
        "UserSearchMatching": ...,
    }
```

```python title="Definition"
class LdapServerMetadataOutputTypeDef(TypedDict):
    Hosts: List[str],
    RoleBase: str,
    RoleSearchMatching: str,
    ServiceAccountUsername: str,
    UserBase: str,
    UserSearchMatching: str,
    RoleName: NotRequired[str],
    RoleSearchSubtree: NotRequired[bool],
    UserRoleName: NotRequired[str],
    UserSearchSubtree: NotRequired[bool],
```

## UserSummaryTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import UserSummaryTypeDef

def get_value() -> UserSummaryTypeDef:
    return {
        "Username": ...,
    }
```

```python title="Definition"
class UserSummaryTypeDef(TypedDict):
    Username: str,
    PendingChange: NotRequired[ChangeTypeType],  # (1)
```

1. See [:material-code-brackets: ChangeTypeType](./literals.md#changetypetype) 
## DescribeConfigurationRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import DescribeConfigurationRequestRequestTypeDef

def get_value() -> DescribeConfigurationRequestRequestTypeDef:
    return {
        "ConfigurationId": ...,
    }
```

```python title="Definition"
class DescribeConfigurationRequestRequestTypeDef(TypedDict):
    ConfigurationId: str,
```

## DescribeConfigurationRevisionRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import DescribeConfigurationRevisionRequestRequestTypeDef

def get_value() -> DescribeConfigurationRevisionRequestRequestTypeDef:
    return {
        "ConfigurationId": ...,
        "ConfigurationRevision": ...,
    }
```

```python title="Definition"
class DescribeConfigurationRevisionRequestRequestTypeDef(TypedDict):
    ConfigurationId: str,
    ConfigurationRevision: str,
```

## DescribeUserRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import DescribeUserRequestRequestTypeDef

def get_value() -> DescribeUserRequestRequestTypeDef:
    return {
        "BrokerId": ...,
        "Username": ...,
    }
```

```python title="Definition"
class DescribeUserRequestRequestTypeDef(TypedDict):
    BrokerId: str,
    Username: str,
```

## UserPendingChangesTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import UserPendingChangesTypeDef

def get_value() -> UserPendingChangesTypeDef:
    return {
        "PendingChange": ...,
    }
```

```python title="Definition"
class UserPendingChangesTypeDef(TypedDict):
    PendingChange: ChangeTypeType,  # (1)
    ConsoleAccess: NotRequired[bool],
    Groups: NotRequired[List[str]],
```

1. See [:material-code-brackets: ChangeTypeType](./literals.md#changetypetype) 
## PaginatorConfigTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import PaginatorConfigTypeDef

def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }
```

```python title="Definition"
class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListBrokersRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import ListBrokersRequestRequestTypeDef

def get_value() -> ListBrokersRequestRequestTypeDef:
    return {
        "MaxResults": ...,
    }
```

```python title="Definition"
class ListBrokersRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListConfigurationRevisionsRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import ListConfigurationRevisionsRequestRequestTypeDef

def get_value() -> ListConfigurationRevisionsRequestRequestTypeDef:
    return {
        "ConfigurationId": ...,
    }
```

```python title="Definition"
class ListConfigurationRevisionsRequestRequestTypeDef(TypedDict):
    ConfigurationId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListConfigurationsRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import ListConfigurationsRequestRequestTypeDef

def get_value() -> ListConfigurationsRequestRequestTypeDef:
    return {
        "MaxResults": ...,
    }
```

```python title="Definition"
class ListConfigurationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import ListTagsRequestRequestTypeDef

def get_value() -> ListTagsRequestRequestTypeDef:
    return {
        "ResourceArn": ...,
    }
```

```python title="Definition"
class ListTagsRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListUsersRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import ListUsersRequestRequestTypeDef

def get_value() -> ListUsersRequestRequestTypeDef:
    return {
        "BrokerId": ...,
    }
```

```python title="Definition"
class ListUsersRequestRequestTypeDef(TypedDict):
    BrokerId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## PendingLogsTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import PendingLogsTypeDef

def get_value() -> PendingLogsTypeDef:
    return {
        "Audit": ...,
    }
```

```python title="Definition"
class PendingLogsTypeDef(TypedDict):
    Audit: NotRequired[bool],
    General: NotRequired[bool],
```

## RebootBrokerRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import RebootBrokerRequestRequestTypeDef

def get_value() -> RebootBrokerRequestRequestTypeDef:
    return {
        "BrokerId": ...,
    }
```

```python title="Definition"
class RebootBrokerRequestRequestTypeDef(TypedDict):
    BrokerId: str,
```

## SanitizationWarningTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import SanitizationWarningTypeDef

def get_value() -> SanitizationWarningTypeDef:
    return {
        "Reason": ...,
    }
```

```python title="Definition"
class SanitizationWarningTypeDef(TypedDict):
    Reason: SanitizationWarningReasonType,  # (1)
    AttributeName: NotRequired[str],
    ElementName: NotRequired[str],
```

1. See [:material-code-brackets: SanitizationWarningReasonType](./literals.md#sanitizationwarningreasontype) 
## UpdateConfigurationRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import UpdateConfigurationRequestRequestTypeDef

def get_value() -> UpdateConfigurationRequestRequestTypeDef:
    return {
        "ConfigurationId": ...,
        "Data": ...,
    }
```

```python title="Definition"
class UpdateConfigurationRequestRequestTypeDef(TypedDict):
    ConfigurationId: str,
    Data: str,
    Description: NotRequired[str],
```

## UpdateUserRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import UpdateUserRequestRequestTypeDef

def get_value() -> UpdateUserRequestRequestTypeDef:
    return {
        "BrokerId": ...,
        "Username": ...,
    }
```

```python title="Definition"
class UpdateUserRequestRequestTypeDef(TypedDict):
    BrokerId: str,
    Username: str,
    ConsoleAccess: NotRequired[bool],
    Groups: NotRequired[Sequence[str]],
    Password: NotRequired[str],
```

## BrokerInstanceOptionTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import BrokerInstanceOptionTypeDef

def get_value() -> BrokerInstanceOptionTypeDef:
    return {
        "AvailabilityZones": ...,
    }
```

```python title="Definition"
class BrokerInstanceOptionTypeDef(TypedDict):
    AvailabilityZones: NotRequired[List[AvailabilityZoneTypeDef]],  # (1)
    EngineType: NotRequired[EngineTypeType],  # (2)
    HostInstanceType: NotRequired[str],
    StorageType: NotRequired[BrokerStorageTypeType],  # (3)
    SupportedDeploymentModes: NotRequired[List[DeploymentModeType]],  # (4)
    SupportedEngineVersions: NotRequired[List[str]],
```

1. See [:material-code-braces: AvailabilityZoneTypeDef](./type_defs.md#availabilityzonetypedef) 
2. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
3. See [:material-code-brackets: BrokerStorageTypeType](./literals.md#brokerstoragetypetype) 
4. See [:material-code-brackets: DeploymentModeType](./literals.md#deploymentmodetype) 
## BrokerEngineTypeTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import BrokerEngineTypeTypeDef

def get_value() -> BrokerEngineTypeTypeDef:
    return {
        "EngineType": ...,
    }
```

```python title="Definition"
class BrokerEngineTypeTypeDef(TypedDict):
    EngineType: NotRequired[EngineTypeType],  # (1)
    EngineVersions: NotRequired[List[EngineVersionTypeDef]],  # (2)
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
2. See [:material-code-braces: EngineVersionTypeDef](./type_defs.md#engineversiontypedef) 
## ConfigurationsTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import ConfigurationsTypeDef

def get_value() -> ConfigurationsTypeDef:
    return {
        "Current": ...,
    }
```

```python title="Definition"
class ConfigurationsTypeDef(TypedDict):
    Current: NotRequired[ConfigurationIdTypeDef],  # (1)
    History: NotRequired[List[ConfigurationIdTypeDef]],  # (2)
    Pending: NotRequired[ConfigurationIdTypeDef],  # (1)
```

1. See [:material-code-braces: ConfigurationIdTypeDef](./type_defs.md#configurationidtypedef) 
2. See [:material-code-braces: ConfigurationIdTypeDef](./type_defs.md#configurationidtypedef) 
3. See [:material-code-braces: ConfigurationIdTypeDef](./type_defs.md#configurationidtypedef) 
## ConfigurationTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import ConfigurationTypeDef

def get_value() -> ConfigurationTypeDef:
    return {
        "Arn": ...,
        "AuthenticationStrategy": ...,
        "Created": ...,
        "Description": ...,
        "EngineType": ...,
        "EngineVersion": ...,
        "Id": ...,
        "LatestRevision": ...,
        "Name": ...,
    }
```

```python title="Definition"
class ConfigurationTypeDef(TypedDict):
    Arn: str,
    AuthenticationStrategy: AuthenticationStrategyType,  # (1)
    Created: datetime,
    Description: str,
    EngineType: EngineTypeType,  # (2)
    EngineVersion: str,
    Id: str,
    LatestRevision: ConfigurationRevisionTypeDef,  # (3)
    Name: str,
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: AuthenticationStrategyType](./literals.md#authenticationstrategytype) 
2. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
3. See [:material-code-braces: ConfigurationRevisionTypeDef](./type_defs.md#configurationrevisiontypedef) 
## CreateBrokerRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import CreateBrokerRequestRequestTypeDef

def get_value() -> CreateBrokerRequestRequestTypeDef:
    return {
        "AutoMinorVersionUpgrade": ...,
        "BrokerName": ...,
        "DeploymentMode": ...,
        "EngineType": ...,
        "EngineVersion": ...,
        "HostInstanceType": ...,
        "PubliclyAccessible": ...,
        "Users": ...,
    }
```

```python title="Definition"
class CreateBrokerRequestRequestTypeDef(TypedDict):
    AutoMinorVersionUpgrade: bool,
    BrokerName: str,
    DeploymentMode: DeploymentModeType,  # (1)
    EngineType: EngineTypeType,  # (2)
    EngineVersion: str,
    HostInstanceType: str,
    PubliclyAccessible: bool,
    Users: Sequence[UserTypeDef],  # (3)
    AuthenticationStrategy: NotRequired[AuthenticationStrategyType],  # (4)
    Configuration: NotRequired[ConfigurationIdTypeDef],  # (5)
    CreatorRequestId: NotRequired[str],
    EncryptionOptions: NotRequired[EncryptionOptionsTypeDef],  # (6)
    LdapServerMetadata: NotRequired[LdapServerMetadataInputTypeDef],  # (7)
    Logs: NotRequired[LogsTypeDef],  # (8)
    MaintenanceWindowStartTime: NotRequired[WeeklyStartTimeTypeDef],  # (9)
    SecurityGroups: NotRequired[Sequence[str]],
    StorageType: NotRequired[BrokerStorageTypeType],  # (10)
    SubnetIds: NotRequired[Sequence[str]],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: DeploymentModeType](./literals.md#deploymentmodetype) 
2. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
3. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
4. See [:material-code-brackets: AuthenticationStrategyType](./literals.md#authenticationstrategytype) 
5. See [:material-code-braces: ConfigurationIdTypeDef](./type_defs.md#configurationidtypedef) 
6. See [:material-code-braces: EncryptionOptionsTypeDef](./type_defs.md#encryptionoptionstypedef) 
7. See [:material-code-braces: LdapServerMetadataInputTypeDef](./type_defs.md#ldapservermetadatainputtypedef) 
8. See [:material-code-braces: LogsTypeDef](./type_defs.md#logstypedef) 
9. See [:material-code-braces: WeeklyStartTimeTypeDef](./type_defs.md#weeklystarttimetypedef) 
10. See [:material-code-brackets: BrokerStorageTypeType](./literals.md#brokerstoragetypetype) 
## UpdateBrokerRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import UpdateBrokerRequestRequestTypeDef

def get_value() -> UpdateBrokerRequestRequestTypeDef:
    return {
        "BrokerId": ...,
    }
```

```python title="Definition"
class UpdateBrokerRequestRequestTypeDef(TypedDict):
    BrokerId: str,
    AuthenticationStrategy: NotRequired[AuthenticationStrategyType],  # (1)
    AutoMinorVersionUpgrade: NotRequired[bool],
    Configuration: NotRequired[ConfigurationIdTypeDef],  # (2)
    EngineVersion: NotRequired[str],
    HostInstanceType: NotRequired[str],
    LdapServerMetadata: NotRequired[LdapServerMetadataInputTypeDef],  # (3)
    Logs: NotRequired[LogsTypeDef],  # (4)
    MaintenanceWindowStartTime: NotRequired[WeeklyStartTimeTypeDef],  # (5)
    SecurityGroups: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: AuthenticationStrategyType](./literals.md#authenticationstrategytype) 
2. See [:material-code-braces: ConfigurationIdTypeDef](./type_defs.md#configurationidtypedef) 
3. See [:material-code-braces: LdapServerMetadataInputTypeDef](./type_defs.md#ldapservermetadatainputtypedef) 
4. See [:material-code-braces: LogsTypeDef](./type_defs.md#logstypedef) 
5. See [:material-code-braces: WeeklyStartTimeTypeDef](./type_defs.md#weeklystarttimetypedef) 
## CreateBrokerResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import CreateBrokerResponseTypeDef

def get_value() -> CreateBrokerResponseTypeDef:
    return {
        "BrokerArn": ...,
        "BrokerId": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class CreateBrokerResponseTypeDef(TypedDict):
    BrokerArn: str,
    BrokerId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfigurationResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import CreateConfigurationResponseTypeDef

def get_value() -> CreateConfigurationResponseTypeDef:
    return {
        "Arn": ...,
        "AuthenticationStrategy": ...,
        "Created": ...,
        "Id": ...,
        "LatestRevision": ...,
        "Name": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class CreateConfigurationResponseTypeDef(TypedDict):
    Arn: str,
    AuthenticationStrategy: AuthenticationStrategyType,  # (1)
    Created: datetime,
    Id: str,
    LatestRevision: ConfigurationRevisionTypeDef,  # (2)
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AuthenticationStrategyType](./literals.md#authenticationstrategytype) 
2. See [:material-code-braces: ConfigurationRevisionTypeDef](./type_defs.md#configurationrevisiontypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBrokerResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import DeleteBrokerResponseTypeDef

def get_value() -> DeleteBrokerResponseTypeDef:
    return {
        "BrokerId": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DeleteBrokerResponseTypeDef(TypedDict):
    BrokerId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConfigurationResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import DescribeConfigurationResponseTypeDef

def get_value() -> DescribeConfigurationResponseTypeDef:
    return {
        "Arn": ...,
        "AuthenticationStrategy": ...,
        "Created": ...,
        "Description": ...,
        "EngineType": ...,
        "EngineVersion": ...,
        "Id": ...,
        "LatestRevision": ...,
        "Name": ...,
        "Tags": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DescribeConfigurationResponseTypeDef(TypedDict):
    Arn: str,
    AuthenticationStrategy: AuthenticationStrategyType,  # (1)
    Created: datetime,
    Description: str,
    EngineType: EngineTypeType,  # (2)
    EngineVersion: str,
    Id: str,
    LatestRevision: ConfigurationRevisionTypeDef,  # (3)
    Name: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: AuthenticationStrategyType](./literals.md#authenticationstrategytype) 
2. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
3. See [:material-code-braces: ConfigurationRevisionTypeDef](./type_defs.md#configurationrevisiontypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConfigurationRevisionResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import DescribeConfigurationRevisionResponseTypeDef

def get_value() -> DescribeConfigurationRevisionResponseTypeDef:
    return {
        "ConfigurationId": ...,
        "Created": ...,
        "Data": ...,
        "Description": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DescribeConfigurationRevisionResponseTypeDef(TypedDict):
    ConfigurationId: str,
    Created: datetime,
    Data: str,
    Description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import EmptyResponseMetadataTypeDef

def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBrokersResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import ListBrokersResponseTypeDef

def get_value() -> ListBrokersResponseTypeDef:
    return {
        "BrokerSummaries": ...,
        "NextToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListBrokersResponseTypeDef(TypedDict):
    BrokerSummaries: List[BrokerSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BrokerSummaryTypeDef](./type_defs.md#brokersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfigurationRevisionsResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import ListConfigurationRevisionsResponseTypeDef

def get_value() -> ListConfigurationRevisionsResponseTypeDef:
    return {
        "ConfigurationId": ...,
        "MaxResults": ...,
        "NextToken": ...,
        "Revisions": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListConfigurationRevisionsResponseTypeDef(TypedDict):
    ConfigurationId: str,
    MaxResults: int,
    NextToken: str,
    Revisions: List[ConfigurationRevisionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfigurationRevisionTypeDef](./type_defs.md#configurationrevisiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import ListTagsResponseTypeDef

def get_value() -> ListTagsResponseTypeDef:
    return {
        "Tags": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListTagsResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBrokerResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import UpdateBrokerResponseTypeDef

def get_value() -> UpdateBrokerResponseTypeDef:
    return {
        "AuthenticationStrategy": ...,
        "AutoMinorVersionUpgrade": ...,
        "BrokerId": ...,
        "Configuration": ...,
        "EngineVersion": ...,
        "HostInstanceType": ...,
        "LdapServerMetadata": ...,
        "Logs": ...,
        "MaintenanceWindowStartTime": ...,
        "SecurityGroups": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateBrokerResponseTypeDef(TypedDict):
    AuthenticationStrategy: AuthenticationStrategyType,  # (1)
    AutoMinorVersionUpgrade: bool,
    BrokerId: str,
    Configuration: ConfigurationIdTypeDef,  # (2)
    EngineVersion: str,
    HostInstanceType: str,
    LdapServerMetadata: LdapServerMetadataOutputTypeDef,  # (3)
    Logs: LogsTypeDef,  # (4)
    MaintenanceWindowStartTime: WeeklyStartTimeTypeDef,  # (5)
    SecurityGroups: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: AuthenticationStrategyType](./literals.md#authenticationstrategytype) 
2. See [:material-code-braces: ConfigurationIdTypeDef](./type_defs.md#configurationidtypedef) 
3. See [:material-code-braces: LdapServerMetadataOutputTypeDef](./type_defs.md#ldapservermetadataoutputtypedef) 
4. See [:material-code-braces: LogsTypeDef](./type_defs.md#logstypedef) 
5. See [:material-code-braces: WeeklyStartTimeTypeDef](./type_defs.md#weeklystarttimetypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUsersResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import ListUsersResponseTypeDef

def get_value() -> ListUsersResponseTypeDef:
    return {
        "BrokerId": ...,
        "MaxResults": ...,
        "NextToken": ...,
        "Users": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListUsersResponseTypeDef(TypedDict):
    BrokerId: str,
    MaxResults: int,
    NextToken: str,
    Users: List[UserSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserSummaryTypeDef](./type_defs.md#usersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUserResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import DescribeUserResponseTypeDef

def get_value() -> DescribeUserResponseTypeDef:
    return {
        "BrokerId": ...,
        "ConsoleAccess": ...,
        "Groups": ...,
        "Pending": ...,
        "Username": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DescribeUserResponseTypeDef(TypedDict):
    BrokerId: str,
    ConsoleAccess: bool,
    Groups: List[str],
    Pending: UserPendingChangesTypeDef,  # (1)
    Username: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserPendingChangesTypeDef](./type_defs.md#userpendingchangestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBrokersRequestListBrokersPaginateTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import ListBrokersRequestListBrokersPaginateTypeDef

def get_value() -> ListBrokersRequestListBrokersPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }
```

```python title="Definition"
class ListBrokersRequestListBrokersPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## LogsSummaryTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import LogsSummaryTypeDef

def get_value() -> LogsSummaryTypeDef:
    return {
        "General": ...,
        "GeneralLogGroup": ...,
    }
```

```python title="Definition"
class LogsSummaryTypeDef(TypedDict):
    General: bool,
    GeneralLogGroup: str,
    Audit: NotRequired[bool],
    AuditLogGroup: NotRequired[str],
    Pending: NotRequired[PendingLogsTypeDef],  # (1)
```

1. See [:material-code-braces: PendingLogsTypeDef](./type_defs.md#pendinglogstypedef) 
## UpdateConfigurationResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import UpdateConfigurationResponseTypeDef

def get_value() -> UpdateConfigurationResponseTypeDef:
    return {
        "Arn": ...,
        "Created": ...,
        "Id": ...,
        "LatestRevision": ...,
        "Name": ...,
        "Warnings": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateConfigurationResponseTypeDef(TypedDict):
    Arn: str,
    Created: datetime,
    Id: str,
    LatestRevision: ConfigurationRevisionTypeDef,  # (1)
    Name: str,
    Warnings: List[SanitizationWarningTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConfigurationRevisionTypeDef](./type_defs.md#configurationrevisiontypedef) 
2. See [:material-code-braces: SanitizationWarningTypeDef](./type_defs.md#sanitizationwarningtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBrokerInstanceOptionsResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import DescribeBrokerInstanceOptionsResponseTypeDef

def get_value() -> DescribeBrokerInstanceOptionsResponseTypeDef:
    return {
        "BrokerInstanceOptions": ...,
        "MaxResults": ...,
        "NextToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DescribeBrokerInstanceOptionsResponseTypeDef(TypedDict):
    BrokerInstanceOptions: List[BrokerInstanceOptionTypeDef],  # (1)
    MaxResults: int,
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BrokerInstanceOptionTypeDef](./type_defs.md#brokerinstanceoptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBrokerEngineTypesResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import DescribeBrokerEngineTypesResponseTypeDef

def get_value() -> DescribeBrokerEngineTypesResponseTypeDef:
    return {
        "BrokerEngineTypes": ...,
        "MaxResults": ...,
        "NextToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DescribeBrokerEngineTypesResponseTypeDef(TypedDict):
    BrokerEngineTypes: List[BrokerEngineTypeTypeDef],  # (1)
    MaxResults: int,
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BrokerEngineTypeTypeDef](./type_defs.md#brokerenginetypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfigurationsResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import ListConfigurationsResponseTypeDef

def get_value() -> ListConfigurationsResponseTypeDef:
    return {
        "Configurations": ...,
        "MaxResults": ...,
        "NextToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListConfigurationsResponseTypeDef(TypedDict):
    Configurations: List[ConfigurationTypeDef],  # (1)
    MaxResults: int,
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBrokerResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_mq.type_defs import DescribeBrokerResponseTypeDef

def get_value() -> DescribeBrokerResponseTypeDef:
    return {
        "ActionsRequired": ...,
        "AuthenticationStrategy": ...,
        "AutoMinorVersionUpgrade": ...,
        "BrokerArn": ...,
        "BrokerId": ...,
        "BrokerInstances": ...,
        "BrokerName": ...,
        "BrokerState": ...,
        "Configurations": ...,
        "Created": ...,
        "DeploymentMode": ...,
        "EncryptionOptions": ...,
        "EngineType": ...,
        "EngineVersion": ...,
        "HostInstanceType": ...,
        "LdapServerMetadata": ...,
        "Logs": ...,
        "MaintenanceWindowStartTime": ...,
        "PendingAuthenticationStrategy": ...,
        "PendingEngineVersion": ...,
        "PendingHostInstanceType": ...,
        "PendingLdapServerMetadata": ...,
        "PendingSecurityGroups": ...,
        "PubliclyAccessible": ...,
        "SecurityGroups": ...,
        "StorageType": ...,
        "SubnetIds": ...,
        "Tags": ...,
        "Users": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DescribeBrokerResponseTypeDef(TypedDict):
    ActionsRequired: List[ActionRequiredTypeDef],  # (1)
    AuthenticationStrategy: AuthenticationStrategyType,  # (2)
    AutoMinorVersionUpgrade: bool,
    BrokerArn: str,
    BrokerId: str,
    BrokerInstances: List[BrokerInstanceTypeDef],  # (3)
    BrokerName: str,
    BrokerState: BrokerStateType,  # (4)
    Configurations: ConfigurationsTypeDef,  # (5)
    Created: datetime,
    DeploymentMode: DeploymentModeType,  # (6)
    EncryptionOptions: EncryptionOptionsTypeDef,  # (7)
    EngineType: EngineTypeType,  # (8)
    EngineVersion: str,
    HostInstanceType: str,
    LdapServerMetadata: LdapServerMetadataOutputTypeDef,  # (9)
    Logs: LogsSummaryTypeDef,  # (10)
    MaintenanceWindowStartTime: WeeklyStartTimeTypeDef,  # (11)
    PendingAuthenticationStrategy: AuthenticationStrategyType,  # (2)
    PendingEngineVersion: str,
    PendingHostInstanceType: str,
    PendingLdapServerMetadata: LdapServerMetadataOutputTypeDef,  # (9)
    PendingSecurityGroups: List[str],
    PubliclyAccessible: bool,
    SecurityGroups: List[str],
    StorageType: BrokerStorageTypeType,  # (14)
    SubnetIds: List[str],
    Tags: Dict[str, str],
    Users: List[UserSummaryTypeDef],  # (15)
    ResponseMetadata: ResponseMetadataTypeDef,  # (16)
```

1. See [:material-code-braces: ActionRequiredTypeDef](./type_defs.md#actionrequiredtypedef) 
2. See [:material-code-brackets: AuthenticationStrategyType](./literals.md#authenticationstrategytype) 
3. See [:material-code-braces: BrokerInstanceTypeDef](./type_defs.md#brokerinstancetypedef) 
4. See [:material-code-brackets: BrokerStateType](./literals.md#brokerstatetype) 
5. See [:material-code-braces: ConfigurationsTypeDef](./type_defs.md#configurationstypedef) 
6. See [:material-code-brackets: DeploymentModeType](./literals.md#deploymentmodetype) 
7. See [:material-code-braces: EncryptionOptionsTypeDef](./type_defs.md#encryptionoptionstypedef) 
8. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
9. See [:material-code-braces: LdapServerMetadataOutputTypeDef](./type_defs.md#ldapservermetadataoutputtypedef) 
10. See [:material-code-braces: LogsSummaryTypeDef](./type_defs.md#logssummarytypedef) 
11. See [:material-code-braces: WeeklyStartTimeTypeDef](./type_defs.md#weeklystarttimetypedef) 
12. See [:material-code-brackets: AuthenticationStrategyType](./literals.md#authenticationstrategytype) 
13. See [:material-code-braces: LdapServerMetadataOutputTypeDef](./type_defs.md#ldapservermetadataoutputtypedef) 
14. See [:material-code-brackets: BrokerStorageTypeType](./literals.md#brokerstoragetypetype) 
15. See [:material-code-braces: UserSummaryTypeDef](./type_defs.md#usersummarytypedef) 
16. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
