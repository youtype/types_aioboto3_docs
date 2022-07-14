# Typed dictionaries

> [Index](../README.md) > [WAFRegional](./README.md) > Typed dictionaries

!!! note ""

    Auto-generated documentation for [WAFRegional](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
    type annotations stubs module [types-aiobotocore-waf-regional](https://pypi.org/project/types-aiobotocore-waf-regional/).

## ExcludedRuleTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ExcludedRuleTypeDef

def get_value() -> ExcludedRuleTypeDef:
    return {
        "RuleId": ...,
    }
```

```python title="Definition"
class ExcludedRuleTypeDef(TypedDict):
    RuleId: str,
```

## WafActionTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import WafActionTypeDef

def get_value() -> WafActionTypeDef:
    return {
        "Type": ...,
    }
```

```python title="Definition"
class WafActionTypeDef(TypedDict):
    Type: WafActionTypeType,  # (1)
```

1. See [:material-code-brackets: WafActionTypeType](./literals.md#wafactiontypetype) 
## WafOverrideActionTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import WafOverrideActionTypeDef

def get_value() -> WafOverrideActionTypeDef:
    return {
        "Type": ...,
    }
```

```python title="Definition"
class WafOverrideActionTypeDef(TypedDict):
    Type: WafOverrideActionTypeType,  # (1)
```

1. See [:material-code-brackets: WafOverrideActionTypeType](./literals.md#wafoverrideactiontypetype) 
## AssociateWebACLRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import AssociateWebACLRequestRequestTypeDef

def get_value() -> AssociateWebACLRequestRequestTypeDef:
    return {
        "WebACLId": ...,
        "ResourceArn": ...,
    }
```

```python title="Definition"
class AssociateWebACLRequestRequestTypeDef(TypedDict):
    WebACLId: str,
    ResourceArn: str,
```

## ByteMatchSetSummaryTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ByteMatchSetSummaryTypeDef

def get_value() -> ByteMatchSetSummaryTypeDef:
    return {
        "ByteMatchSetId": ...,
        "Name": ...,
    }
```

```python title="Definition"
class ByteMatchSetSummaryTypeDef(TypedDict):
    ByteMatchSetId: str,
    Name: str,
```

## FieldToMatchTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import FieldToMatchTypeDef

def get_value() -> FieldToMatchTypeDef:
    return {
        "Type": ...,
    }
```

```python title="Definition"
class FieldToMatchTypeDef(TypedDict):
    Type: MatchFieldTypeType,  # (1)
    Data: NotRequired[str],
```

1. See [:material-code-brackets: MatchFieldTypeType](./literals.md#matchfieldtypetype) 
## CreateByteMatchSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateByteMatchSetRequestRequestTypeDef

def get_value() -> CreateByteMatchSetRequestRequestTypeDef:
    return {
        "Name": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class CreateByteMatchSetRequestRequestTypeDef(TypedDict):
    Name: str,
    ChangeToken: str,
```

## ResponseMetadataTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ResponseMetadataTypeDef

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

## CreateGeoMatchSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateGeoMatchSetRequestRequestTypeDef

def get_value() -> CreateGeoMatchSetRequestRequestTypeDef:
    return {
        "Name": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class CreateGeoMatchSetRequestRequestTypeDef(TypedDict):
    Name: str,
    ChangeToken: str,
```

## CreateIPSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateIPSetRequestRequestTypeDef

def get_value() -> CreateIPSetRequestRequestTypeDef:
    return {
        "Name": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class CreateIPSetRequestRequestTypeDef(TypedDict):
    Name: str,
    ChangeToken: str,
```

## TagTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import TagTypeDef

def get_value() -> TagTypeDef:
    return {
        "Key": ...,
        "Value": ...,
    }
```

```python title="Definition"
class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CreateRegexMatchSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateRegexMatchSetRequestRequestTypeDef

def get_value() -> CreateRegexMatchSetRequestRequestTypeDef:
    return {
        "Name": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class CreateRegexMatchSetRequestRequestTypeDef(TypedDict):
    Name: str,
    ChangeToken: str,
```

## CreateRegexPatternSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateRegexPatternSetRequestRequestTypeDef

def get_value() -> CreateRegexPatternSetRequestRequestTypeDef:
    return {
        "Name": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class CreateRegexPatternSetRequestRequestTypeDef(TypedDict):
    Name: str,
    ChangeToken: str,
```

## RegexPatternSetTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import RegexPatternSetTypeDef

def get_value() -> RegexPatternSetTypeDef:
    return {
        "RegexPatternSetId": ...,
        "RegexPatternStrings": ...,
    }
```

```python title="Definition"
class RegexPatternSetTypeDef(TypedDict):
    RegexPatternSetId: str,
    RegexPatternStrings: List[str],
    Name: NotRequired[str],
```

## RuleGroupTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import RuleGroupTypeDef

def get_value() -> RuleGroupTypeDef:
    return {
        "RuleGroupId": ...,
    }
```

```python title="Definition"
class RuleGroupTypeDef(TypedDict):
    RuleGroupId: str,
    Name: NotRequired[str],
    MetricName: NotRequired[str],
```

## CreateSizeConstraintSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateSizeConstraintSetRequestRequestTypeDef

def get_value() -> CreateSizeConstraintSetRequestRequestTypeDef:
    return {
        "Name": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class CreateSizeConstraintSetRequestRequestTypeDef(TypedDict):
    Name: str,
    ChangeToken: str,
```

## CreateSqlInjectionMatchSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateSqlInjectionMatchSetRequestRequestTypeDef

def get_value() -> CreateSqlInjectionMatchSetRequestRequestTypeDef:
    return {
        "Name": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class CreateSqlInjectionMatchSetRequestRequestTypeDef(TypedDict):
    Name: str,
    ChangeToken: str,
```

## CreateWebACLMigrationStackRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateWebACLMigrationStackRequestRequestTypeDef

def get_value() -> CreateWebACLMigrationStackRequestRequestTypeDef:
    return {
        "WebACLId": ...,
        "S3BucketName": ...,
        "IgnoreUnsupportedType": ...,
    }
```

```python title="Definition"
class CreateWebACLMigrationStackRequestRequestTypeDef(TypedDict):
    WebACLId: str,
    S3BucketName: str,
    IgnoreUnsupportedType: bool,
```

## CreateXssMatchSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateXssMatchSetRequestRequestTypeDef

def get_value() -> CreateXssMatchSetRequestRequestTypeDef:
    return {
        "Name": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class CreateXssMatchSetRequestRequestTypeDef(TypedDict):
    Name: str,
    ChangeToken: str,
```

## DeleteByteMatchSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteByteMatchSetRequestRequestTypeDef

def get_value() -> DeleteByteMatchSetRequestRequestTypeDef:
    return {
        "ByteMatchSetId": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class DeleteByteMatchSetRequestRequestTypeDef(TypedDict):
    ByteMatchSetId: str,
    ChangeToken: str,
```

## DeleteGeoMatchSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteGeoMatchSetRequestRequestTypeDef

def get_value() -> DeleteGeoMatchSetRequestRequestTypeDef:
    return {
        "GeoMatchSetId": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class DeleteGeoMatchSetRequestRequestTypeDef(TypedDict):
    GeoMatchSetId: str,
    ChangeToken: str,
```

## DeleteIPSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteIPSetRequestRequestTypeDef

def get_value() -> DeleteIPSetRequestRequestTypeDef:
    return {
        "IPSetId": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class DeleteIPSetRequestRequestTypeDef(TypedDict):
    IPSetId: str,
    ChangeToken: str,
```

## DeleteLoggingConfigurationRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteLoggingConfigurationRequestRequestTypeDef

def get_value() -> DeleteLoggingConfigurationRequestRequestTypeDef:
    return {
        "ResourceArn": ...,
    }
```

```python title="Definition"
class DeleteLoggingConfigurationRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## DeletePermissionPolicyRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeletePermissionPolicyRequestRequestTypeDef

def get_value() -> DeletePermissionPolicyRequestRequestTypeDef:
    return {
        "ResourceArn": ...,
    }
```

```python title="Definition"
class DeletePermissionPolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## DeleteRateBasedRuleRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteRateBasedRuleRequestRequestTypeDef

def get_value() -> DeleteRateBasedRuleRequestRequestTypeDef:
    return {
        "RuleId": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class DeleteRateBasedRuleRequestRequestTypeDef(TypedDict):
    RuleId: str,
    ChangeToken: str,
```

## DeleteRegexMatchSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteRegexMatchSetRequestRequestTypeDef

def get_value() -> DeleteRegexMatchSetRequestRequestTypeDef:
    return {
        "RegexMatchSetId": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class DeleteRegexMatchSetRequestRequestTypeDef(TypedDict):
    RegexMatchSetId: str,
    ChangeToken: str,
```

## DeleteRegexPatternSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteRegexPatternSetRequestRequestTypeDef

def get_value() -> DeleteRegexPatternSetRequestRequestTypeDef:
    return {
        "RegexPatternSetId": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class DeleteRegexPatternSetRequestRequestTypeDef(TypedDict):
    RegexPatternSetId: str,
    ChangeToken: str,
```

## DeleteRuleGroupRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteRuleGroupRequestRequestTypeDef

def get_value() -> DeleteRuleGroupRequestRequestTypeDef:
    return {
        "RuleGroupId": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class DeleteRuleGroupRequestRequestTypeDef(TypedDict):
    RuleGroupId: str,
    ChangeToken: str,
```

## DeleteRuleRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteRuleRequestRequestTypeDef

def get_value() -> DeleteRuleRequestRequestTypeDef:
    return {
        "RuleId": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class DeleteRuleRequestRequestTypeDef(TypedDict):
    RuleId: str,
    ChangeToken: str,
```

## DeleteSizeConstraintSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteSizeConstraintSetRequestRequestTypeDef

def get_value() -> DeleteSizeConstraintSetRequestRequestTypeDef:
    return {
        "SizeConstraintSetId": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class DeleteSizeConstraintSetRequestRequestTypeDef(TypedDict):
    SizeConstraintSetId: str,
    ChangeToken: str,
```

## DeleteSqlInjectionMatchSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteSqlInjectionMatchSetRequestRequestTypeDef

def get_value() -> DeleteSqlInjectionMatchSetRequestRequestTypeDef:
    return {
        "SqlInjectionMatchSetId": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class DeleteSqlInjectionMatchSetRequestRequestTypeDef(TypedDict):
    SqlInjectionMatchSetId: str,
    ChangeToken: str,
```

## DeleteWebACLRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteWebACLRequestRequestTypeDef

def get_value() -> DeleteWebACLRequestRequestTypeDef:
    return {
        "WebACLId": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class DeleteWebACLRequestRequestTypeDef(TypedDict):
    WebACLId: str,
    ChangeToken: str,
```

## DeleteXssMatchSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteXssMatchSetRequestRequestTypeDef

def get_value() -> DeleteXssMatchSetRequestRequestTypeDef:
    return {
        "XssMatchSetId": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class DeleteXssMatchSetRequestRequestTypeDef(TypedDict):
    XssMatchSetId: str,
    ChangeToken: str,
```

## DisassociateWebACLRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DisassociateWebACLRequestRequestTypeDef

def get_value() -> DisassociateWebACLRequestRequestTypeDef:
    return {
        "ResourceArn": ...,
    }
```

```python title="Definition"
class DisassociateWebACLRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## GeoMatchConstraintTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GeoMatchConstraintTypeDef

def get_value() -> GeoMatchConstraintTypeDef:
    return {
        "Type": ...,
        "Value": ...,
    }
```

```python title="Definition"
class GeoMatchConstraintTypeDef(TypedDict):
    Type: GeoMatchConstraintTypeType,  # (1)
    Value: GeoMatchConstraintValueType,  # (2)
```

1. See [:material-code-brackets: GeoMatchConstraintTypeType](./literals.md#geomatchconstrainttypetype) 
2. See [:material-code-brackets: GeoMatchConstraintValueType](./literals.md#geomatchconstraintvaluetype) 
## GeoMatchSetSummaryTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GeoMatchSetSummaryTypeDef

def get_value() -> GeoMatchSetSummaryTypeDef:
    return {
        "GeoMatchSetId": ...,
        "Name": ...,
    }
```

```python title="Definition"
class GeoMatchSetSummaryTypeDef(TypedDict):
    GeoMatchSetId: str,
    Name: str,
```

## GetByteMatchSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetByteMatchSetRequestRequestTypeDef

def get_value() -> GetByteMatchSetRequestRequestTypeDef:
    return {
        "ByteMatchSetId": ...,
    }
```

```python title="Definition"
class GetByteMatchSetRequestRequestTypeDef(TypedDict):
    ByteMatchSetId: str,
```

## GetChangeTokenStatusRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetChangeTokenStatusRequestRequestTypeDef

def get_value() -> GetChangeTokenStatusRequestRequestTypeDef:
    return {
        "ChangeToken": ...,
    }
```

```python title="Definition"
class GetChangeTokenStatusRequestRequestTypeDef(TypedDict):
    ChangeToken: str,
```

## GetGeoMatchSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetGeoMatchSetRequestRequestTypeDef

def get_value() -> GetGeoMatchSetRequestRequestTypeDef:
    return {
        "GeoMatchSetId": ...,
    }
```

```python title="Definition"
class GetGeoMatchSetRequestRequestTypeDef(TypedDict):
    GeoMatchSetId: str,
```

## GetIPSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetIPSetRequestRequestTypeDef

def get_value() -> GetIPSetRequestRequestTypeDef:
    return {
        "IPSetId": ...,
    }
```

```python title="Definition"
class GetIPSetRequestRequestTypeDef(TypedDict):
    IPSetId: str,
```

## GetLoggingConfigurationRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetLoggingConfigurationRequestRequestTypeDef

def get_value() -> GetLoggingConfigurationRequestRequestTypeDef:
    return {
        "ResourceArn": ...,
    }
```

```python title="Definition"
class GetLoggingConfigurationRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## GetPermissionPolicyRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetPermissionPolicyRequestRequestTypeDef

def get_value() -> GetPermissionPolicyRequestRequestTypeDef:
    return {
        "ResourceArn": ...,
    }
```

```python title="Definition"
class GetPermissionPolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## GetRateBasedRuleManagedKeysRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetRateBasedRuleManagedKeysRequestRequestTypeDef

def get_value() -> GetRateBasedRuleManagedKeysRequestRequestTypeDef:
    return {
        "RuleId": ...,
    }
```

```python title="Definition"
class GetRateBasedRuleManagedKeysRequestRequestTypeDef(TypedDict):
    RuleId: str,
    NextMarker: NotRequired[str],
```

## GetRateBasedRuleRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetRateBasedRuleRequestRequestTypeDef

def get_value() -> GetRateBasedRuleRequestRequestTypeDef:
    return {
        "RuleId": ...,
    }
```

```python title="Definition"
class GetRateBasedRuleRequestRequestTypeDef(TypedDict):
    RuleId: str,
```

## GetRegexMatchSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetRegexMatchSetRequestRequestTypeDef

def get_value() -> GetRegexMatchSetRequestRequestTypeDef:
    return {
        "RegexMatchSetId": ...,
    }
```

```python title="Definition"
class GetRegexMatchSetRequestRequestTypeDef(TypedDict):
    RegexMatchSetId: str,
```

## GetRegexPatternSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetRegexPatternSetRequestRequestTypeDef

def get_value() -> GetRegexPatternSetRequestRequestTypeDef:
    return {
        "RegexPatternSetId": ...,
    }
```

```python title="Definition"
class GetRegexPatternSetRequestRequestTypeDef(TypedDict):
    RegexPatternSetId: str,
```

## GetRuleGroupRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetRuleGroupRequestRequestTypeDef

def get_value() -> GetRuleGroupRequestRequestTypeDef:
    return {
        "RuleGroupId": ...,
    }
```

```python title="Definition"
class GetRuleGroupRequestRequestTypeDef(TypedDict):
    RuleGroupId: str,
```

## GetRuleRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetRuleRequestRequestTypeDef

def get_value() -> GetRuleRequestRequestTypeDef:
    return {
        "RuleId": ...,
    }
```

```python title="Definition"
class GetRuleRequestRequestTypeDef(TypedDict):
    RuleId: str,
```

## TimeWindowTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import TimeWindowTypeDef

def get_value() -> TimeWindowTypeDef:
    return {
        "StartTime": ...,
        "EndTime": ...,
    }
```

```python title="Definition"
class TimeWindowTypeDef(TypedDict):
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
```

## GetSizeConstraintSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetSizeConstraintSetRequestRequestTypeDef

def get_value() -> GetSizeConstraintSetRequestRequestTypeDef:
    return {
        "SizeConstraintSetId": ...,
    }
```

```python title="Definition"
class GetSizeConstraintSetRequestRequestTypeDef(TypedDict):
    SizeConstraintSetId: str,
```

## GetSqlInjectionMatchSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetSqlInjectionMatchSetRequestRequestTypeDef

def get_value() -> GetSqlInjectionMatchSetRequestRequestTypeDef:
    return {
        "SqlInjectionMatchSetId": ...,
    }
```

```python title="Definition"
class GetSqlInjectionMatchSetRequestRequestTypeDef(TypedDict):
    SqlInjectionMatchSetId: str,
```

## GetWebACLForResourceRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetWebACLForResourceRequestRequestTypeDef

def get_value() -> GetWebACLForResourceRequestRequestTypeDef:
    return {
        "ResourceArn": ...,
    }
```

```python title="Definition"
class GetWebACLForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## WebACLSummaryTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import WebACLSummaryTypeDef

def get_value() -> WebACLSummaryTypeDef:
    return {
        "WebACLId": ...,
        "Name": ...,
    }
```

```python title="Definition"
class WebACLSummaryTypeDef(TypedDict):
    WebACLId: str,
    Name: str,
```

## GetWebACLRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetWebACLRequestRequestTypeDef

def get_value() -> GetWebACLRequestRequestTypeDef:
    return {
        "WebACLId": ...,
    }
```

```python title="Definition"
class GetWebACLRequestRequestTypeDef(TypedDict):
    WebACLId: str,
```

## GetXssMatchSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetXssMatchSetRequestRequestTypeDef

def get_value() -> GetXssMatchSetRequestRequestTypeDef:
    return {
        "XssMatchSetId": ...,
    }
```

```python title="Definition"
class GetXssMatchSetRequestRequestTypeDef(TypedDict):
    XssMatchSetId: str,
```

## HTTPHeaderTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import HTTPHeaderTypeDef

def get_value() -> HTTPHeaderTypeDef:
    return {
        "Name": ...,
    }
```

```python title="Definition"
class HTTPHeaderTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## IPSetDescriptorTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import IPSetDescriptorTypeDef

def get_value() -> IPSetDescriptorTypeDef:
    return {
        "Type": ...,
        "Value": ...,
    }
```

```python title="Definition"
class IPSetDescriptorTypeDef(TypedDict):
    Type: IPSetDescriptorTypeType,  # (1)
    Value: str,
```

1. See [:material-code-brackets: IPSetDescriptorTypeType](./literals.md#ipsetdescriptortypetype) 
## IPSetSummaryTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import IPSetSummaryTypeDef

def get_value() -> IPSetSummaryTypeDef:
    return {
        "IPSetId": ...,
        "Name": ...,
    }
```

```python title="Definition"
class IPSetSummaryTypeDef(TypedDict):
    IPSetId: str,
    Name: str,
```

## ListActivatedRulesInRuleGroupRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListActivatedRulesInRuleGroupRequestRequestTypeDef

def get_value() -> ListActivatedRulesInRuleGroupRequestRequestTypeDef:
    return {
        "RuleGroupId": ...,
    }
```

```python title="Definition"
class ListActivatedRulesInRuleGroupRequestRequestTypeDef(TypedDict):
    RuleGroupId: NotRequired[str],
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## ListByteMatchSetsRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListByteMatchSetsRequestRequestTypeDef

def get_value() -> ListByteMatchSetsRequestRequestTypeDef:
    return {
        "NextMarker": ...,
    }
```

```python title="Definition"
class ListByteMatchSetsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## ListGeoMatchSetsRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListGeoMatchSetsRequestRequestTypeDef

def get_value() -> ListGeoMatchSetsRequestRequestTypeDef:
    return {
        "NextMarker": ...,
    }
```

```python title="Definition"
class ListGeoMatchSetsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## ListIPSetsRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListIPSetsRequestRequestTypeDef

def get_value() -> ListIPSetsRequestRequestTypeDef:
    return {
        "NextMarker": ...,
    }
```

```python title="Definition"
class ListIPSetsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## ListLoggingConfigurationsRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListLoggingConfigurationsRequestRequestTypeDef

def get_value() -> ListLoggingConfigurationsRequestRequestTypeDef:
    return {
        "NextMarker": ...,
    }
```

```python title="Definition"
class ListLoggingConfigurationsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## ListRateBasedRulesRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListRateBasedRulesRequestRequestTypeDef

def get_value() -> ListRateBasedRulesRequestRequestTypeDef:
    return {
        "NextMarker": ...,
    }
```

```python title="Definition"
class ListRateBasedRulesRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## RuleSummaryTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import RuleSummaryTypeDef

def get_value() -> RuleSummaryTypeDef:
    return {
        "RuleId": ...,
        "Name": ...,
    }
```

```python title="Definition"
class RuleSummaryTypeDef(TypedDict):
    RuleId: str,
    Name: str,
```

## ListRegexMatchSetsRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListRegexMatchSetsRequestRequestTypeDef

def get_value() -> ListRegexMatchSetsRequestRequestTypeDef:
    return {
        "NextMarker": ...,
    }
```

```python title="Definition"
class ListRegexMatchSetsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## RegexMatchSetSummaryTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import RegexMatchSetSummaryTypeDef

def get_value() -> RegexMatchSetSummaryTypeDef:
    return {
        "RegexMatchSetId": ...,
        "Name": ...,
    }
```

```python title="Definition"
class RegexMatchSetSummaryTypeDef(TypedDict):
    RegexMatchSetId: str,
    Name: str,
```

## ListRegexPatternSetsRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListRegexPatternSetsRequestRequestTypeDef

def get_value() -> ListRegexPatternSetsRequestRequestTypeDef:
    return {
        "NextMarker": ...,
    }
```

```python title="Definition"
class ListRegexPatternSetsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## RegexPatternSetSummaryTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import RegexPatternSetSummaryTypeDef

def get_value() -> RegexPatternSetSummaryTypeDef:
    return {
        "RegexPatternSetId": ...,
        "Name": ...,
    }
```

```python title="Definition"
class RegexPatternSetSummaryTypeDef(TypedDict):
    RegexPatternSetId: str,
    Name: str,
```

## ListResourcesForWebACLRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListResourcesForWebACLRequestRequestTypeDef

def get_value() -> ListResourcesForWebACLRequestRequestTypeDef:
    return {
        "WebACLId": ...,
    }
```

```python title="Definition"
class ListResourcesForWebACLRequestRequestTypeDef(TypedDict):
    WebACLId: str,
    ResourceType: NotRequired[ResourceTypeType],  # (1)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ListRuleGroupsRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListRuleGroupsRequestRequestTypeDef

def get_value() -> ListRuleGroupsRequestRequestTypeDef:
    return {
        "NextMarker": ...,
    }
```

```python title="Definition"
class ListRuleGroupsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## RuleGroupSummaryTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import RuleGroupSummaryTypeDef

def get_value() -> RuleGroupSummaryTypeDef:
    return {
        "RuleGroupId": ...,
        "Name": ...,
    }
```

```python title="Definition"
class RuleGroupSummaryTypeDef(TypedDict):
    RuleGroupId: str,
    Name: str,
```

## ListRulesRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListRulesRequestRequestTypeDef

def get_value() -> ListRulesRequestRequestTypeDef:
    return {
        "NextMarker": ...,
    }
```

```python title="Definition"
class ListRulesRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## ListSizeConstraintSetsRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListSizeConstraintSetsRequestRequestTypeDef

def get_value() -> ListSizeConstraintSetsRequestRequestTypeDef:
    return {
        "NextMarker": ...,
    }
```

```python title="Definition"
class ListSizeConstraintSetsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## SizeConstraintSetSummaryTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import SizeConstraintSetSummaryTypeDef

def get_value() -> SizeConstraintSetSummaryTypeDef:
    return {
        "SizeConstraintSetId": ...,
        "Name": ...,
    }
```

```python title="Definition"
class SizeConstraintSetSummaryTypeDef(TypedDict):
    SizeConstraintSetId: str,
    Name: str,
```

## ListSqlInjectionMatchSetsRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListSqlInjectionMatchSetsRequestRequestTypeDef

def get_value() -> ListSqlInjectionMatchSetsRequestRequestTypeDef:
    return {
        "NextMarker": ...,
    }
```

```python title="Definition"
class ListSqlInjectionMatchSetsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## SqlInjectionMatchSetSummaryTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import SqlInjectionMatchSetSummaryTypeDef

def get_value() -> SqlInjectionMatchSetSummaryTypeDef:
    return {
        "SqlInjectionMatchSetId": ...,
        "Name": ...,
    }
```

```python title="Definition"
class SqlInjectionMatchSetSummaryTypeDef(TypedDict):
    SqlInjectionMatchSetId: str,
    Name: str,
```

## ListSubscribedRuleGroupsRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListSubscribedRuleGroupsRequestRequestTypeDef

def get_value() -> ListSubscribedRuleGroupsRequestRequestTypeDef:
    return {
        "NextMarker": ...,
    }
```

```python title="Definition"
class ListSubscribedRuleGroupsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## SubscribedRuleGroupSummaryTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import SubscribedRuleGroupSummaryTypeDef

def get_value() -> SubscribedRuleGroupSummaryTypeDef:
    return {
        "RuleGroupId": ...,
        "Name": ...,
        "MetricName": ...,
    }
```

```python title="Definition"
class SubscribedRuleGroupSummaryTypeDef(TypedDict):
    RuleGroupId: str,
    Name: str,
    MetricName: str,
```

## ListTagsForResourceRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListTagsForResourceRequestRequestTypeDef

def get_value() -> ListTagsForResourceRequestRequestTypeDef:
    return {
        "ResourceARN": ...,
    }
```

```python title="Definition"
class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## ListWebACLsRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListWebACLsRequestRequestTypeDef

def get_value() -> ListWebACLsRequestRequestTypeDef:
    return {
        "NextMarker": ...,
    }
```

```python title="Definition"
class ListWebACLsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## ListXssMatchSetsRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListXssMatchSetsRequestRequestTypeDef

def get_value() -> ListXssMatchSetsRequestRequestTypeDef:
    return {
        "NextMarker": ...,
    }
```

```python title="Definition"
class ListXssMatchSetsRequestRequestTypeDef(TypedDict):
    NextMarker: NotRequired[str],
    Limit: NotRequired[int],
```

## XssMatchSetSummaryTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import XssMatchSetSummaryTypeDef

def get_value() -> XssMatchSetSummaryTypeDef:
    return {
        "XssMatchSetId": ...,
        "Name": ...,
    }
```

```python title="Definition"
class XssMatchSetSummaryTypeDef(TypedDict):
    XssMatchSetId: str,
    Name: str,
```

## PredicateTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import PredicateTypeDef

def get_value() -> PredicateTypeDef:
    return {
        "Negated": ...,
        "Type": ...,
        "DataId": ...,
    }
```

```python title="Definition"
class PredicateTypeDef(TypedDict):
    Negated: bool,
    Type: PredicateTypeType,  # (1)
    DataId: str,
```

1. See [:material-code-brackets: PredicateTypeType](./literals.md#predicatetypetype) 
## PutPermissionPolicyRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import PutPermissionPolicyRequestRequestTypeDef

def get_value() -> PutPermissionPolicyRequestRequestTypeDef:
    return {
        "ResourceArn": ...,
        "Policy": ...,
    }
```

```python title="Definition"
class PutPermissionPolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Policy: str,
```

## RegexPatternSetUpdateTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import RegexPatternSetUpdateTypeDef

def get_value() -> RegexPatternSetUpdateTypeDef:
    return {
        "Action": ...,
        "RegexPatternString": ...,
    }
```

```python title="Definition"
class RegexPatternSetUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    RegexPatternString: str,
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
## UntagResourceRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UntagResourceRequestRequestTypeDef

def get_value() -> UntagResourceRequestRequestTypeDef:
    return {
        "ResourceARN": ...,
        "TagKeys": ...,
    }
```

```python title="Definition"
class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## ActivatedRuleTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ActivatedRuleTypeDef

def get_value() -> ActivatedRuleTypeDef:
    return {
        "Priority": ...,
        "RuleId": ...,
    }
```

```python title="Definition"
class ActivatedRuleTypeDef(TypedDict):
    Priority: int,
    RuleId: str,
    Action: NotRequired[WafActionTypeDef],  # (1)
    OverrideAction: NotRequired[WafOverrideActionTypeDef],  # (2)
    Type: NotRequired[WafRuleTypeType],  # (3)
    ExcludedRules: NotRequired[List[ExcludedRuleTypeDef]],  # (4)
```

1. See [:material-code-braces: WafActionTypeDef](./type_defs.md#wafactiontypedef) 
2. See [:material-code-braces: WafOverrideActionTypeDef](./type_defs.md#wafoverrideactiontypedef) 
3. See [:material-code-brackets: WafRuleTypeType](./literals.md#wafruletypetype) 
4. See [:material-code-braces: ExcludedRuleTypeDef](./type_defs.md#excludedruletypedef) 
## ByteMatchTupleTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ByteMatchTupleTypeDef

def get_value() -> ByteMatchTupleTypeDef:
    return {
        "FieldToMatch": ...,
        "TargetString": ...,
        "TextTransformation": ...,
        "PositionalConstraint": ...,
    }
```

```python title="Definition"
class ByteMatchTupleTypeDef(TypedDict):
    FieldToMatch: FieldToMatchTypeDef,  # (1)
    TargetString: bytes,
    TextTransformation: TextTransformationType,  # (2)
    PositionalConstraint: PositionalConstraintType,  # (3)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) 
2. See [:material-code-brackets: TextTransformationType](./literals.md#texttransformationtype) 
3. See [:material-code-brackets: PositionalConstraintType](./literals.md#positionalconstrainttype) 
## LoggingConfigurationTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import LoggingConfigurationTypeDef

def get_value() -> LoggingConfigurationTypeDef:
    return {
        "ResourceArn": ...,
        "LogDestinationConfigs": ...,
    }
```

```python title="Definition"
class LoggingConfigurationTypeDef(TypedDict):
    ResourceArn: str,
    LogDestinationConfigs: List[str],
    RedactedFields: NotRequired[List[FieldToMatchTypeDef]],  # (1)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) 
## RegexMatchTupleTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import RegexMatchTupleTypeDef

def get_value() -> RegexMatchTupleTypeDef:
    return {
        "FieldToMatch": ...,
        "TextTransformation": ...,
        "RegexPatternSetId": ...,
    }
```

```python title="Definition"
class RegexMatchTupleTypeDef(TypedDict):
    FieldToMatch: FieldToMatchTypeDef,  # (1)
    TextTransformation: TextTransformationType,  # (2)
    RegexPatternSetId: str,
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) 
2. See [:material-code-brackets: TextTransformationType](./literals.md#texttransformationtype) 
## SizeConstraintTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import SizeConstraintTypeDef

def get_value() -> SizeConstraintTypeDef:
    return {
        "FieldToMatch": ...,
        "TextTransformation": ...,
        "ComparisonOperator": ...,
        "Size": ...,
    }
```

```python title="Definition"
class SizeConstraintTypeDef(TypedDict):
    FieldToMatch: FieldToMatchTypeDef,  # (1)
    TextTransformation: TextTransformationType,  # (2)
    ComparisonOperator: ComparisonOperatorType,  # (3)
    Size: int,
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) 
2. See [:material-code-brackets: TextTransformationType](./literals.md#texttransformationtype) 
3. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## SqlInjectionMatchTupleTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import SqlInjectionMatchTupleTypeDef

def get_value() -> SqlInjectionMatchTupleTypeDef:
    return {
        "FieldToMatch": ...,
        "TextTransformation": ...,
    }
```

```python title="Definition"
class SqlInjectionMatchTupleTypeDef(TypedDict):
    FieldToMatch: FieldToMatchTypeDef,  # (1)
    TextTransformation: TextTransformationType,  # (2)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) 
2. See [:material-code-brackets: TextTransformationType](./literals.md#texttransformationtype) 
## XssMatchTupleTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import XssMatchTupleTypeDef

def get_value() -> XssMatchTupleTypeDef:
    return {
        "FieldToMatch": ...,
        "TextTransformation": ...,
    }
```

```python title="Definition"
class XssMatchTupleTypeDef(TypedDict):
    FieldToMatch: FieldToMatchTypeDef,  # (1)
    TextTransformation: TextTransformationType,  # (2)
```

1. See [:material-code-braces: FieldToMatchTypeDef](./type_defs.md#fieldtomatchtypedef) 
2. See [:material-code-brackets: TextTransformationType](./literals.md#texttransformationtype) 
## CreateWebACLMigrationStackResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateWebACLMigrationStackResponseTypeDef

def get_value() -> CreateWebACLMigrationStackResponseTypeDef:
    return {
        "S3ObjectUrl": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class CreateWebACLMigrationStackResponseTypeDef(TypedDict):
    S3ObjectUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteByteMatchSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteByteMatchSetResponseTypeDef

def get_value() -> DeleteByteMatchSetResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DeleteByteMatchSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteGeoMatchSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteGeoMatchSetResponseTypeDef

def get_value() -> DeleteGeoMatchSetResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DeleteGeoMatchSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteIPSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteIPSetResponseTypeDef

def get_value() -> DeleteIPSetResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DeleteIPSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRateBasedRuleResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteRateBasedRuleResponseTypeDef

def get_value() -> DeleteRateBasedRuleResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DeleteRateBasedRuleResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRegexMatchSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteRegexMatchSetResponseTypeDef

def get_value() -> DeleteRegexMatchSetResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DeleteRegexMatchSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRegexPatternSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteRegexPatternSetResponseTypeDef

def get_value() -> DeleteRegexPatternSetResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DeleteRegexPatternSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRuleGroupResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteRuleGroupResponseTypeDef

def get_value() -> DeleteRuleGroupResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DeleteRuleGroupResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRuleResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteRuleResponseTypeDef

def get_value() -> DeleteRuleResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DeleteRuleResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSizeConstraintSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteSizeConstraintSetResponseTypeDef

def get_value() -> DeleteSizeConstraintSetResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DeleteSizeConstraintSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSqlInjectionMatchSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteSqlInjectionMatchSetResponseTypeDef

def get_value() -> DeleteSqlInjectionMatchSetResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DeleteSqlInjectionMatchSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteWebACLResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteWebACLResponseTypeDef

def get_value() -> DeleteWebACLResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DeleteWebACLResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteXssMatchSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import DeleteXssMatchSetResponseTypeDef

def get_value() -> DeleteXssMatchSetResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DeleteXssMatchSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetChangeTokenResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetChangeTokenResponseTypeDef

def get_value() -> GetChangeTokenResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetChangeTokenResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetChangeTokenStatusResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetChangeTokenStatusResponseTypeDef

def get_value() -> GetChangeTokenStatusResponseTypeDef:
    return {
        "ChangeTokenStatus": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetChangeTokenStatusResponseTypeDef(TypedDict):
    ChangeTokenStatus: ChangeTokenStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeTokenStatusType](./literals.md#changetokenstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPermissionPolicyResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetPermissionPolicyResponseTypeDef

def get_value() -> GetPermissionPolicyResponseTypeDef:
    return {
        "Policy": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetPermissionPolicyResponseTypeDef(TypedDict):
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRateBasedRuleManagedKeysResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetRateBasedRuleManagedKeysResponseTypeDef

def get_value() -> GetRateBasedRuleManagedKeysResponseTypeDef:
    return {
        "ManagedKeys": ...,
        "NextMarker": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetRateBasedRuleManagedKeysResponseTypeDef(TypedDict):
    ManagedKeys: List[str],
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListByteMatchSetsResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListByteMatchSetsResponseTypeDef

def get_value() -> ListByteMatchSetsResponseTypeDef:
    return {
        "NextMarker": ...,
        "ByteMatchSets": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListByteMatchSetsResponseTypeDef(TypedDict):
    NextMarker: str,
    ByteMatchSets: List[ByteMatchSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ByteMatchSetSummaryTypeDef](./type_defs.md#bytematchsetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourcesForWebACLResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListResourcesForWebACLResponseTypeDef

def get_value() -> ListResourcesForWebACLResponseTypeDef:
    return {
        "ResourceArns": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListResourcesForWebACLResponseTypeDef(TypedDict):
    ResourceArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateByteMatchSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateByteMatchSetResponseTypeDef

def get_value() -> UpdateByteMatchSetResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateByteMatchSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGeoMatchSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateGeoMatchSetResponseTypeDef

def get_value() -> UpdateGeoMatchSetResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateGeoMatchSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIPSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateIPSetResponseTypeDef

def get_value() -> UpdateIPSetResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateIPSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRateBasedRuleResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateRateBasedRuleResponseTypeDef

def get_value() -> UpdateRateBasedRuleResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateRateBasedRuleResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRegexMatchSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateRegexMatchSetResponseTypeDef

def get_value() -> UpdateRegexMatchSetResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateRegexMatchSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRegexPatternSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateRegexPatternSetResponseTypeDef

def get_value() -> UpdateRegexPatternSetResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateRegexPatternSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRuleGroupResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateRuleGroupResponseTypeDef

def get_value() -> UpdateRuleGroupResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateRuleGroupResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRuleResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateRuleResponseTypeDef

def get_value() -> UpdateRuleResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateRuleResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSizeConstraintSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateSizeConstraintSetResponseTypeDef

def get_value() -> UpdateSizeConstraintSetResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateSizeConstraintSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSqlInjectionMatchSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateSqlInjectionMatchSetResponseTypeDef

def get_value() -> UpdateSqlInjectionMatchSetResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateSqlInjectionMatchSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWebACLResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateWebACLResponseTypeDef

def get_value() -> UpdateWebACLResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateWebACLResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateXssMatchSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateXssMatchSetResponseTypeDef

def get_value() -> UpdateXssMatchSetResponseTypeDef:
    return {
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateXssMatchSetResponseTypeDef(TypedDict):
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRateBasedRuleRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateRateBasedRuleRequestRequestTypeDef

def get_value() -> CreateRateBasedRuleRequestRequestTypeDef:
    return {
        "Name": ...,
        "MetricName": ...,
        "RateKey": ...,
        "RateLimit": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class CreateRateBasedRuleRequestRequestTypeDef(TypedDict):
    Name: str,
    MetricName: str,
    RateKey: RateKeyType,  # (1)
    RateLimit: int,
    ChangeToken: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: RateKeyType](./literals.md#ratekeytype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateRuleGroupRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateRuleGroupRequestRequestTypeDef

def get_value() -> CreateRuleGroupRequestRequestTypeDef:
    return {
        "Name": ...,
        "MetricName": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class CreateRuleGroupRequestRequestTypeDef(TypedDict):
    Name: str,
    MetricName: str,
    ChangeToken: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateRuleRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateRuleRequestRequestTypeDef

def get_value() -> CreateRuleRequestRequestTypeDef:
    return {
        "Name": ...,
        "MetricName": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class CreateRuleRequestRequestTypeDef(TypedDict):
    Name: str,
    MetricName: str,
    ChangeToken: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateWebACLRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateWebACLRequestRequestTypeDef

def get_value() -> CreateWebACLRequestRequestTypeDef:
    return {
        "Name": ...,
        "MetricName": ...,
        "DefaultAction": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class CreateWebACLRequestRequestTypeDef(TypedDict):
    Name: str,
    MetricName: str,
    DefaultAction: WafActionTypeDef,  # (1)
    ChangeToken: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: WafActionTypeDef](./type_defs.md#wafactiontypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagInfoForResourceTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import TagInfoForResourceTypeDef

def get_value() -> TagInfoForResourceTypeDef:
    return {
        "ResourceARN": ...,
    }
```

```python title="Definition"
class TagInfoForResourceTypeDef(TypedDict):
    ResourceARN: NotRequired[str],
    TagList: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import TagResourceRequestRequestTypeDef

def get_value() -> TagResourceRequestRequestTypeDef:
    return {
        "ResourceARN": ...,
        "Tags": ...,
    }
```

```python title="Definition"
class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateRegexPatternSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateRegexPatternSetResponseTypeDef

def get_value() -> CreateRegexPatternSetResponseTypeDef:
    return {
        "RegexPatternSet": ...,
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class CreateRegexPatternSetResponseTypeDef(TypedDict):
    RegexPatternSet: RegexPatternSetTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegexPatternSetTypeDef](./type_defs.md#regexpatternsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRegexPatternSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetRegexPatternSetResponseTypeDef

def get_value() -> GetRegexPatternSetResponseTypeDef:
    return {
        "RegexPatternSet": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetRegexPatternSetResponseTypeDef(TypedDict):
    RegexPatternSet: RegexPatternSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegexPatternSetTypeDef](./type_defs.md#regexpatternsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRuleGroupResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateRuleGroupResponseTypeDef

def get_value() -> CreateRuleGroupResponseTypeDef:
    return {
        "RuleGroup": ...,
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class CreateRuleGroupResponseTypeDef(TypedDict):
    RuleGroup: RuleGroupTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleGroupTypeDef](./type_defs.md#rulegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRuleGroupResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetRuleGroupResponseTypeDef

def get_value() -> GetRuleGroupResponseTypeDef:
    return {
        "RuleGroup": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetRuleGroupResponseTypeDef(TypedDict):
    RuleGroup: RuleGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleGroupTypeDef](./type_defs.md#rulegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GeoMatchSetTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GeoMatchSetTypeDef

def get_value() -> GeoMatchSetTypeDef:
    return {
        "GeoMatchSetId": ...,
        "GeoMatchConstraints": ...,
    }
```

```python title="Definition"
class GeoMatchSetTypeDef(TypedDict):
    GeoMatchSetId: str,
    GeoMatchConstraints: List[GeoMatchConstraintTypeDef],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-braces: GeoMatchConstraintTypeDef](./type_defs.md#geomatchconstrainttypedef) 
## GeoMatchSetUpdateTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GeoMatchSetUpdateTypeDef

def get_value() -> GeoMatchSetUpdateTypeDef:
    return {
        "Action": ...,
        "GeoMatchConstraint": ...,
    }
```

```python title="Definition"
class GeoMatchSetUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    GeoMatchConstraint: GeoMatchConstraintTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: GeoMatchConstraintTypeDef](./type_defs.md#geomatchconstrainttypedef) 
## ListGeoMatchSetsResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListGeoMatchSetsResponseTypeDef

def get_value() -> ListGeoMatchSetsResponseTypeDef:
    return {
        "NextMarker": ...,
        "GeoMatchSets": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListGeoMatchSetsResponseTypeDef(TypedDict):
    NextMarker: str,
    GeoMatchSets: List[GeoMatchSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GeoMatchSetSummaryTypeDef](./type_defs.md#geomatchsetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSampledRequestsRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetSampledRequestsRequestRequestTypeDef

def get_value() -> GetSampledRequestsRequestRequestTypeDef:
    return {
        "WebAclId": ...,
        "RuleId": ...,
        "TimeWindow": ...,
        "MaxItems": ...,
    }
```

```python title="Definition"
class GetSampledRequestsRequestRequestTypeDef(TypedDict):
    WebAclId: str,
    RuleId: str,
    TimeWindow: TimeWindowTypeDef,  # (1)
    MaxItems: int,
```

1. See [:material-code-braces: TimeWindowTypeDef](./type_defs.md#timewindowtypedef) 
## GetWebACLForResourceResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetWebACLForResourceResponseTypeDef

def get_value() -> GetWebACLForResourceResponseTypeDef:
    return {
        "WebACLSummary": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetWebACLForResourceResponseTypeDef(TypedDict):
    WebACLSummary: WebACLSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WebACLSummaryTypeDef](./type_defs.md#webaclsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWebACLsResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListWebACLsResponseTypeDef

def get_value() -> ListWebACLsResponseTypeDef:
    return {
        "NextMarker": ...,
        "WebACLs": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListWebACLsResponseTypeDef(TypedDict):
    NextMarker: str,
    WebACLs: List[WebACLSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WebACLSummaryTypeDef](./type_defs.md#webaclsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HTTPRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import HTTPRequestTypeDef

def get_value() -> HTTPRequestTypeDef:
    return {
        "ClientIP": ...,
    }
```

```python title="Definition"
class HTTPRequestTypeDef(TypedDict):
    ClientIP: NotRequired[str],
    Country: NotRequired[str],
    URI: NotRequired[str],
    Method: NotRequired[str],
    HTTPVersion: NotRequired[str],
    Headers: NotRequired[List[HTTPHeaderTypeDef]],  # (1)
```

1. See [:material-code-braces: HTTPHeaderTypeDef](./type_defs.md#httpheadertypedef) 
## IPSetTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import IPSetTypeDef

def get_value() -> IPSetTypeDef:
    return {
        "IPSetId": ...,
        "IPSetDescriptors": ...,
    }
```

```python title="Definition"
class IPSetTypeDef(TypedDict):
    IPSetId: str,
    IPSetDescriptors: List[IPSetDescriptorTypeDef],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-braces: IPSetDescriptorTypeDef](./type_defs.md#ipsetdescriptortypedef) 
## IPSetUpdateTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import IPSetUpdateTypeDef

def get_value() -> IPSetUpdateTypeDef:
    return {
        "Action": ...,
        "IPSetDescriptor": ...,
    }
```

```python title="Definition"
class IPSetUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    IPSetDescriptor: IPSetDescriptorTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: IPSetDescriptorTypeDef](./type_defs.md#ipsetdescriptortypedef) 
## ListIPSetsResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListIPSetsResponseTypeDef

def get_value() -> ListIPSetsResponseTypeDef:
    return {
        "NextMarker": ...,
        "IPSets": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListIPSetsResponseTypeDef(TypedDict):
    NextMarker: str,
    IPSets: List[IPSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IPSetSummaryTypeDef](./type_defs.md#ipsetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRateBasedRulesResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListRateBasedRulesResponseTypeDef

def get_value() -> ListRateBasedRulesResponseTypeDef:
    return {
        "NextMarker": ...,
        "Rules": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListRateBasedRulesResponseTypeDef(TypedDict):
    NextMarker: str,
    Rules: List[RuleSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleSummaryTypeDef](./type_defs.md#rulesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRulesResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListRulesResponseTypeDef

def get_value() -> ListRulesResponseTypeDef:
    return {
        "NextMarker": ...,
        "Rules": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListRulesResponseTypeDef(TypedDict):
    NextMarker: str,
    Rules: List[RuleSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleSummaryTypeDef](./type_defs.md#rulesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRegexMatchSetsResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListRegexMatchSetsResponseTypeDef

def get_value() -> ListRegexMatchSetsResponseTypeDef:
    return {
        "NextMarker": ...,
        "RegexMatchSets": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListRegexMatchSetsResponseTypeDef(TypedDict):
    NextMarker: str,
    RegexMatchSets: List[RegexMatchSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegexMatchSetSummaryTypeDef](./type_defs.md#regexmatchsetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRegexPatternSetsResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListRegexPatternSetsResponseTypeDef

def get_value() -> ListRegexPatternSetsResponseTypeDef:
    return {
        "NextMarker": ...,
        "RegexPatternSets": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListRegexPatternSetsResponseTypeDef(TypedDict):
    NextMarker: str,
    RegexPatternSets: List[RegexPatternSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegexPatternSetSummaryTypeDef](./type_defs.md#regexpatternsetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRuleGroupsResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListRuleGroupsResponseTypeDef

def get_value() -> ListRuleGroupsResponseTypeDef:
    return {
        "NextMarker": ...,
        "RuleGroups": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListRuleGroupsResponseTypeDef(TypedDict):
    NextMarker: str,
    RuleGroups: List[RuleGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleGroupSummaryTypeDef](./type_defs.md#rulegroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSizeConstraintSetsResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListSizeConstraintSetsResponseTypeDef

def get_value() -> ListSizeConstraintSetsResponseTypeDef:
    return {
        "NextMarker": ...,
        "SizeConstraintSets": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListSizeConstraintSetsResponseTypeDef(TypedDict):
    NextMarker: str,
    SizeConstraintSets: List[SizeConstraintSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SizeConstraintSetSummaryTypeDef](./type_defs.md#sizeconstraintsetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSqlInjectionMatchSetsResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListSqlInjectionMatchSetsResponseTypeDef

def get_value() -> ListSqlInjectionMatchSetsResponseTypeDef:
    return {
        "NextMarker": ...,
        "SqlInjectionMatchSets": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListSqlInjectionMatchSetsResponseTypeDef(TypedDict):
    NextMarker: str,
    SqlInjectionMatchSets: List[SqlInjectionMatchSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SqlInjectionMatchSetSummaryTypeDef](./type_defs.md#sqlinjectionmatchsetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSubscribedRuleGroupsResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListSubscribedRuleGroupsResponseTypeDef

def get_value() -> ListSubscribedRuleGroupsResponseTypeDef:
    return {
        "NextMarker": ...,
        "RuleGroups": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListSubscribedRuleGroupsResponseTypeDef(TypedDict):
    NextMarker: str,
    RuleGroups: List[SubscribedRuleGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubscribedRuleGroupSummaryTypeDef](./type_defs.md#subscribedrulegroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListXssMatchSetsResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListXssMatchSetsResponseTypeDef

def get_value() -> ListXssMatchSetsResponseTypeDef:
    return {
        "NextMarker": ...,
        "XssMatchSets": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListXssMatchSetsResponseTypeDef(TypedDict):
    NextMarker: str,
    XssMatchSets: List[XssMatchSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: XssMatchSetSummaryTypeDef](./type_defs.md#xssmatchsetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RateBasedRuleTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import RateBasedRuleTypeDef

def get_value() -> RateBasedRuleTypeDef:
    return {
        "RuleId": ...,
        "MatchPredicates": ...,
        "RateKey": ...,
        "RateLimit": ...,
    }
```

```python title="Definition"
class RateBasedRuleTypeDef(TypedDict):
    RuleId: str,
    MatchPredicates: List[PredicateTypeDef],  # (1)
    RateKey: RateKeyType,  # (2)
    RateLimit: int,
    Name: NotRequired[str],
    MetricName: NotRequired[str],
```

1. See [:material-code-braces: PredicateTypeDef](./type_defs.md#predicatetypedef) 
2. See [:material-code-brackets: RateKeyType](./literals.md#ratekeytype) 
## RuleTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import RuleTypeDef

def get_value() -> RuleTypeDef:
    return {
        "RuleId": ...,
        "Predicates": ...,
    }
```

```python title="Definition"
class RuleTypeDef(TypedDict):
    RuleId: str,
    Predicates: List[PredicateTypeDef],  # (1)
    Name: NotRequired[str],
    MetricName: NotRequired[str],
```

1. See [:material-code-braces: PredicateTypeDef](./type_defs.md#predicatetypedef) 
## RuleUpdateTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import RuleUpdateTypeDef

def get_value() -> RuleUpdateTypeDef:
    return {
        "Action": ...,
        "Predicate": ...,
    }
```

```python title="Definition"
class RuleUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    Predicate: PredicateTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: PredicateTypeDef](./type_defs.md#predicatetypedef) 
## UpdateRegexPatternSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateRegexPatternSetRequestRequestTypeDef

def get_value() -> UpdateRegexPatternSetRequestRequestTypeDef:
    return {
        "RegexPatternSetId": ...,
        "Updates": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class UpdateRegexPatternSetRequestRequestTypeDef(TypedDict):
    RegexPatternSetId: str,
    Updates: Sequence[RegexPatternSetUpdateTypeDef],  # (1)
    ChangeToken: str,
```

1. See [:material-code-braces: RegexPatternSetUpdateTypeDef](./type_defs.md#regexpatternsetupdatetypedef) 
## ListActivatedRulesInRuleGroupResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListActivatedRulesInRuleGroupResponseTypeDef

def get_value() -> ListActivatedRulesInRuleGroupResponseTypeDef:
    return {
        "NextMarker": ...,
        "ActivatedRules": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListActivatedRulesInRuleGroupResponseTypeDef(TypedDict):
    NextMarker: str,
    ActivatedRules: List[ActivatedRuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActivatedRuleTypeDef](./type_defs.md#activatedruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RuleGroupUpdateTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import RuleGroupUpdateTypeDef

def get_value() -> RuleGroupUpdateTypeDef:
    return {
        "Action": ...,
        "ActivatedRule": ...,
    }
```

```python title="Definition"
class RuleGroupUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    ActivatedRule: ActivatedRuleTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: ActivatedRuleTypeDef](./type_defs.md#activatedruletypedef) 
## WebACLTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import WebACLTypeDef

def get_value() -> WebACLTypeDef:
    return {
        "WebACLId": ...,
        "DefaultAction": ...,
        "Rules": ...,
    }
```

```python title="Definition"
class WebACLTypeDef(TypedDict):
    WebACLId: str,
    DefaultAction: WafActionTypeDef,  # (1)
    Rules: List[ActivatedRuleTypeDef],  # (2)
    Name: NotRequired[str],
    MetricName: NotRequired[str],
    WebACLArn: NotRequired[str],
```

1. See [:material-code-braces: WafActionTypeDef](./type_defs.md#wafactiontypedef) 
2. See [:material-code-braces: ActivatedRuleTypeDef](./type_defs.md#activatedruletypedef) 
## WebACLUpdateTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import WebACLUpdateTypeDef

def get_value() -> WebACLUpdateTypeDef:
    return {
        "Action": ...,
        "ActivatedRule": ...,
    }
```

```python title="Definition"
class WebACLUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    ActivatedRule: ActivatedRuleTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: ActivatedRuleTypeDef](./type_defs.md#activatedruletypedef) 
## ByteMatchSetTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ByteMatchSetTypeDef

def get_value() -> ByteMatchSetTypeDef:
    return {
        "ByteMatchSetId": ...,
        "ByteMatchTuples": ...,
    }
```

```python title="Definition"
class ByteMatchSetTypeDef(TypedDict):
    ByteMatchSetId: str,
    ByteMatchTuples: List[ByteMatchTupleTypeDef],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-braces: ByteMatchTupleTypeDef](./type_defs.md#bytematchtupletypedef) 
## ByteMatchSetUpdateTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ByteMatchSetUpdateTypeDef

def get_value() -> ByteMatchSetUpdateTypeDef:
    return {
        "Action": ...,
        "ByteMatchTuple": ...,
    }
```

```python title="Definition"
class ByteMatchSetUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    ByteMatchTuple: ByteMatchTupleTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: ByteMatchTupleTypeDef](./type_defs.md#bytematchtupletypedef) 
## GetLoggingConfigurationResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetLoggingConfigurationResponseTypeDef

def get_value() -> GetLoggingConfigurationResponseTypeDef:
    return {
        "LoggingConfiguration": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetLoggingConfigurationResponseTypeDef(TypedDict):
    LoggingConfiguration: LoggingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLoggingConfigurationsResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListLoggingConfigurationsResponseTypeDef

def get_value() -> ListLoggingConfigurationsResponseTypeDef:
    return {
        "LoggingConfigurations": ...,
        "NextMarker": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListLoggingConfigurationsResponseTypeDef(TypedDict):
    LoggingConfigurations: List[LoggingConfigurationTypeDef],  # (1)
    NextMarker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutLoggingConfigurationRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import PutLoggingConfigurationRequestRequestTypeDef

def get_value() -> PutLoggingConfigurationRequestRequestTypeDef:
    return {
        "LoggingConfiguration": ...,
    }
```

```python title="Definition"
class PutLoggingConfigurationRequestRequestTypeDef(TypedDict):
    LoggingConfiguration: LoggingConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
## PutLoggingConfigurationResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import PutLoggingConfigurationResponseTypeDef

def get_value() -> PutLoggingConfigurationResponseTypeDef:
    return {
        "LoggingConfiguration": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class PutLoggingConfigurationResponseTypeDef(TypedDict):
    LoggingConfiguration: LoggingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegexMatchSetTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import RegexMatchSetTypeDef

def get_value() -> RegexMatchSetTypeDef:
    return {
        "RegexMatchSetId": ...,
    }
```

```python title="Definition"
class RegexMatchSetTypeDef(TypedDict):
    RegexMatchSetId: NotRequired[str],
    Name: NotRequired[str],
    RegexMatchTuples: NotRequired[List[RegexMatchTupleTypeDef]],  # (1)
```

1. See [:material-code-braces: RegexMatchTupleTypeDef](./type_defs.md#regexmatchtupletypedef) 
## RegexMatchSetUpdateTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import RegexMatchSetUpdateTypeDef

def get_value() -> RegexMatchSetUpdateTypeDef:
    return {
        "Action": ...,
        "RegexMatchTuple": ...,
    }
```

```python title="Definition"
class RegexMatchSetUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    RegexMatchTuple: RegexMatchTupleTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: RegexMatchTupleTypeDef](./type_defs.md#regexmatchtupletypedef) 
## SizeConstraintSetTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import SizeConstraintSetTypeDef

def get_value() -> SizeConstraintSetTypeDef:
    return {
        "SizeConstraintSetId": ...,
        "SizeConstraints": ...,
    }
```

```python title="Definition"
class SizeConstraintSetTypeDef(TypedDict):
    SizeConstraintSetId: str,
    SizeConstraints: List[SizeConstraintTypeDef],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-braces: SizeConstraintTypeDef](./type_defs.md#sizeconstrainttypedef) 
## SizeConstraintSetUpdateTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import SizeConstraintSetUpdateTypeDef

def get_value() -> SizeConstraintSetUpdateTypeDef:
    return {
        "Action": ...,
        "SizeConstraint": ...,
    }
```

```python title="Definition"
class SizeConstraintSetUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    SizeConstraint: SizeConstraintTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: SizeConstraintTypeDef](./type_defs.md#sizeconstrainttypedef) 
## SqlInjectionMatchSetTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import SqlInjectionMatchSetTypeDef

def get_value() -> SqlInjectionMatchSetTypeDef:
    return {
        "SqlInjectionMatchSetId": ...,
        "SqlInjectionMatchTuples": ...,
    }
```

```python title="Definition"
class SqlInjectionMatchSetTypeDef(TypedDict):
    SqlInjectionMatchSetId: str,
    SqlInjectionMatchTuples: List[SqlInjectionMatchTupleTypeDef],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-braces: SqlInjectionMatchTupleTypeDef](./type_defs.md#sqlinjectionmatchtupletypedef) 
## SqlInjectionMatchSetUpdateTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import SqlInjectionMatchSetUpdateTypeDef

def get_value() -> SqlInjectionMatchSetUpdateTypeDef:
    return {
        "Action": ...,
        "SqlInjectionMatchTuple": ...,
    }
```

```python title="Definition"
class SqlInjectionMatchSetUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    SqlInjectionMatchTuple: SqlInjectionMatchTupleTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: SqlInjectionMatchTupleTypeDef](./type_defs.md#sqlinjectionmatchtupletypedef) 
## XssMatchSetTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import XssMatchSetTypeDef

def get_value() -> XssMatchSetTypeDef:
    return {
        "XssMatchSetId": ...,
        "XssMatchTuples": ...,
    }
```

```python title="Definition"
class XssMatchSetTypeDef(TypedDict):
    XssMatchSetId: str,
    XssMatchTuples: List[XssMatchTupleTypeDef],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-braces: XssMatchTupleTypeDef](./type_defs.md#xssmatchtupletypedef) 
## XssMatchSetUpdateTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import XssMatchSetUpdateTypeDef

def get_value() -> XssMatchSetUpdateTypeDef:
    return {
        "Action": ...,
        "XssMatchTuple": ...,
    }
```

```python title="Definition"
class XssMatchSetUpdateTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    XssMatchTuple: XssMatchTupleTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: XssMatchTupleTypeDef](./type_defs.md#xssmatchtupletypedef) 
## ListTagsForResourceResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import ListTagsForResourceResponseTypeDef

def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "NextMarker": ...,
        "TagInfoForResource": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListTagsForResourceResponseTypeDef(TypedDict):
    NextMarker: str,
    TagInfoForResource: TagInfoForResourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagInfoForResourceTypeDef](./type_defs.md#taginfoforresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGeoMatchSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateGeoMatchSetResponseTypeDef

def get_value() -> CreateGeoMatchSetResponseTypeDef:
    return {
        "GeoMatchSet": ...,
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class CreateGeoMatchSetResponseTypeDef(TypedDict):
    GeoMatchSet: GeoMatchSetTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GeoMatchSetTypeDef](./type_defs.md#geomatchsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGeoMatchSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetGeoMatchSetResponseTypeDef

def get_value() -> GetGeoMatchSetResponseTypeDef:
    return {
        "GeoMatchSet": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetGeoMatchSetResponseTypeDef(TypedDict):
    GeoMatchSet: GeoMatchSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GeoMatchSetTypeDef](./type_defs.md#geomatchsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGeoMatchSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateGeoMatchSetRequestRequestTypeDef

def get_value() -> UpdateGeoMatchSetRequestRequestTypeDef:
    return {
        "GeoMatchSetId": ...,
        "ChangeToken": ...,
        "Updates": ...,
    }
```

```python title="Definition"
class UpdateGeoMatchSetRequestRequestTypeDef(TypedDict):
    GeoMatchSetId: str,
    ChangeToken: str,
    Updates: Sequence[GeoMatchSetUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: GeoMatchSetUpdateTypeDef](./type_defs.md#geomatchsetupdatetypedef) 
## SampledHTTPRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import SampledHTTPRequestTypeDef

def get_value() -> SampledHTTPRequestTypeDef:
    return {
        "Request": ...,
        "Weight": ...,
    }
```

```python title="Definition"
class SampledHTTPRequestTypeDef(TypedDict):
    Request: HTTPRequestTypeDef,  # (1)
    Weight: int,
    Timestamp: NotRequired[datetime],
    Action: NotRequired[str],
    RuleWithinRuleGroup: NotRequired[str],
```

1. See [:material-code-braces: HTTPRequestTypeDef](./type_defs.md#httprequesttypedef) 
## CreateIPSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateIPSetResponseTypeDef

def get_value() -> CreateIPSetResponseTypeDef:
    return {
        "IPSet": ...,
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class CreateIPSetResponseTypeDef(TypedDict):
    IPSet: IPSetTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IPSetTypeDef](./type_defs.md#ipsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIPSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetIPSetResponseTypeDef

def get_value() -> GetIPSetResponseTypeDef:
    return {
        "IPSet": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetIPSetResponseTypeDef(TypedDict):
    IPSet: IPSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IPSetTypeDef](./type_defs.md#ipsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIPSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateIPSetRequestRequestTypeDef

def get_value() -> UpdateIPSetRequestRequestTypeDef:
    return {
        "IPSetId": ...,
        "ChangeToken": ...,
        "Updates": ...,
    }
```

```python title="Definition"
class UpdateIPSetRequestRequestTypeDef(TypedDict):
    IPSetId: str,
    ChangeToken: str,
    Updates: Sequence[IPSetUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: IPSetUpdateTypeDef](./type_defs.md#ipsetupdatetypedef) 
## CreateRateBasedRuleResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateRateBasedRuleResponseTypeDef

def get_value() -> CreateRateBasedRuleResponseTypeDef:
    return {
        "Rule": ...,
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class CreateRateBasedRuleResponseTypeDef(TypedDict):
    Rule: RateBasedRuleTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RateBasedRuleTypeDef](./type_defs.md#ratebasedruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRateBasedRuleResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetRateBasedRuleResponseTypeDef

def get_value() -> GetRateBasedRuleResponseTypeDef:
    return {
        "Rule": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetRateBasedRuleResponseTypeDef(TypedDict):
    Rule: RateBasedRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RateBasedRuleTypeDef](./type_defs.md#ratebasedruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRuleResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateRuleResponseTypeDef

def get_value() -> CreateRuleResponseTypeDef:
    return {
        "Rule": ...,
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class CreateRuleResponseTypeDef(TypedDict):
    Rule: RuleTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRuleResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetRuleResponseTypeDef

def get_value() -> GetRuleResponseTypeDef:
    return {
        "Rule": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetRuleResponseTypeDef(TypedDict):
    Rule: RuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRateBasedRuleRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateRateBasedRuleRequestRequestTypeDef

def get_value() -> UpdateRateBasedRuleRequestRequestTypeDef:
    return {
        "RuleId": ...,
        "ChangeToken": ...,
        "Updates": ...,
        "RateLimit": ...,
    }
```

```python title="Definition"
class UpdateRateBasedRuleRequestRequestTypeDef(TypedDict):
    RuleId: str,
    ChangeToken: str,
    Updates: Sequence[RuleUpdateTypeDef],  # (1)
    RateLimit: int,
```

1. See [:material-code-braces: RuleUpdateTypeDef](./type_defs.md#ruleupdatetypedef) 
## UpdateRuleRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateRuleRequestRequestTypeDef

def get_value() -> UpdateRuleRequestRequestTypeDef:
    return {
        "RuleId": ...,
        "ChangeToken": ...,
        "Updates": ...,
    }
```

```python title="Definition"
class UpdateRuleRequestRequestTypeDef(TypedDict):
    RuleId: str,
    ChangeToken: str,
    Updates: Sequence[RuleUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: RuleUpdateTypeDef](./type_defs.md#ruleupdatetypedef) 
## UpdateRuleGroupRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateRuleGroupRequestRequestTypeDef

def get_value() -> UpdateRuleGroupRequestRequestTypeDef:
    return {
        "RuleGroupId": ...,
        "Updates": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class UpdateRuleGroupRequestRequestTypeDef(TypedDict):
    RuleGroupId: str,
    Updates: Sequence[RuleGroupUpdateTypeDef],  # (1)
    ChangeToken: str,
```

1. See [:material-code-braces: RuleGroupUpdateTypeDef](./type_defs.md#rulegroupupdatetypedef) 
## CreateWebACLResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateWebACLResponseTypeDef

def get_value() -> CreateWebACLResponseTypeDef:
    return {
        "WebACL": ...,
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class CreateWebACLResponseTypeDef(TypedDict):
    WebACL: WebACLTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WebACLTypeDef](./type_defs.md#webacltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWebACLResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetWebACLResponseTypeDef

def get_value() -> GetWebACLResponseTypeDef:
    return {
        "WebACL": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetWebACLResponseTypeDef(TypedDict):
    WebACL: WebACLTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WebACLTypeDef](./type_defs.md#webacltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWebACLRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateWebACLRequestRequestTypeDef

def get_value() -> UpdateWebACLRequestRequestTypeDef:
    return {
        "WebACLId": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class UpdateWebACLRequestRequestTypeDef(TypedDict):
    WebACLId: str,
    ChangeToken: str,
    Updates: NotRequired[Sequence[WebACLUpdateTypeDef]],  # (1)
    DefaultAction: NotRequired[WafActionTypeDef],  # (2)
```

1. See [:material-code-braces: WebACLUpdateTypeDef](./type_defs.md#webaclupdatetypedef) 
2. See [:material-code-braces: WafActionTypeDef](./type_defs.md#wafactiontypedef) 
## CreateByteMatchSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateByteMatchSetResponseTypeDef

def get_value() -> CreateByteMatchSetResponseTypeDef:
    return {
        "ByteMatchSet": ...,
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class CreateByteMatchSetResponseTypeDef(TypedDict):
    ByteMatchSet: ByteMatchSetTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ByteMatchSetTypeDef](./type_defs.md#bytematchsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetByteMatchSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetByteMatchSetResponseTypeDef

def get_value() -> GetByteMatchSetResponseTypeDef:
    return {
        "ByteMatchSet": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetByteMatchSetResponseTypeDef(TypedDict):
    ByteMatchSet: ByteMatchSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ByteMatchSetTypeDef](./type_defs.md#bytematchsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateByteMatchSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateByteMatchSetRequestRequestTypeDef

def get_value() -> UpdateByteMatchSetRequestRequestTypeDef:
    return {
        "ByteMatchSetId": ...,
        "ChangeToken": ...,
        "Updates": ...,
    }
```

```python title="Definition"
class UpdateByteMatchSetRequestRequestTypeDef(TypedDict):
    ByteMatchSetId: str,
    ChangeToken: str,
    Updates: Sequence[ByteMatchSetUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: ByteMatchSetUpdateTypeDef](./type_defs.md#bytematchsetupdatetypedef) 
## CreateRegexMatchSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateRegexMatchSetResponseTypeDef

def get_value() -> CreateRegexMatchSetResponseTypeDef:
    return {
        "RegexMatchSet": ...,
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class CreateRegexMatchSetResponseTypeDef(TypedDict):
    RegexMatchSet: RegexMatchSetTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegexMatchSetTypeDef](./type_defs.md#regexmatchsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRegexMatchSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetRegexMatchSetResponseTypeDef

def get_value() -> GetRegexMatchSetResponseTypeDef:
    return {
        "RegexMatchSet": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetRegexMatchSetResponseTypeDef(TypedDict):
    RegexMatchSet: RegexMatchSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegexMatchSetTypeDef](./type_defs.md#regexmatchsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRegexMatchSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateRegexMatchSetRequestRequestTypeDef

def get_value() -> UpdateRegexMatchSetRequestRequestTypeDef:
    return {
        "RegexMatchSetId": ...,
        "Updates": ...,
        "ChangeToken": ...,
    }
```

```python title="Definition"
class UpdateRegexMatchSetRequestRequestTypeDef(TypedDict):
    RegexMatchSetId: str,
    Updates: Sequence[RegexMatchSetUpdateTypeDef],  # (1)
    ChangeToken: str,
```

1. See [:material-code-braces: RegexMatchSetUpdateTypeDef](./type_defs.md#regexmatchsetupdatetypedef) 
## CreateSizeConstraintSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateSizeConstraintSetResponseTypeDef

def get_value() -> CreateSizeConstraintSetResponseTypeDef:
    return {
        "SizeConstraintSet": ...,
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class CreateSizeConstraintSetResponseTypeDef(TypedDict):
    SizeConstraintSet: SizeConstraintSetTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SizeConstraintSetTypeDef](./type_defs.md#sizeconstraintsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSizeConstraintSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetSizeConstraintSetResponseTypeDef

def get_value() -> GetSizeConstraintSetResponseTypeDef:
    return {
        "SizeConstraintSet": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetSizeConstraintSetResponseTypeDef(TypedDict):
    SizeConstraintSet: SizeConstraintSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SizeConstraintSetTypeDef](./type_defs.md#sizeconstraintsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSizeConstraintSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateSizeConstraintSetRequestRequestTypeDef

def get_value() -> UpdateSizeConstraintSetRequestRequestTypeDef:
    return {
        "SizeConstraintSetId": ...,
        "ChangeToken": ...,
        "Updates": ...,
    }
```

```python title="Definition"
class UpdateSizeConstraintSetRequestRequestTypeDef(TypedDict):
    SizeConstraintSetId: str,
    ChangeToken: str,
    Updates: Sequence[SizeConstraintSetUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: SizeConstraintSetUpdateTypeDef](./type_defs.md#sizeconstraintsetupdatetypedef) 
## CreateSqlInjectionMatchSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateSqlInjectionMatchSetResponseTypeDef

def get_value() -> CreateSqlInjectionMatchSetResponseTypeDef:
    return {
        "SqlInjectionMatchSet": ...,
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class CreateSqlInjectionMatchSetResponseTypeDef(TypedDict):
    SqlInjectionMatchSet: SqlInjectionMatchSetTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SqlInjectionMatchSetTypeDef](./type_defs.md#sqlinjectionmatchsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSqlInjectionMatchSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetSqlInjectionMatchSetResponseTypeDef

def get_value() -> GetSqlInjectionMatchSetResponseTypeDef:
    return {
        "SqlInjectionMatchSet": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetSqlInjectionMatchSetResponseTypeDef(TypedDict):
    SqlInjectionMatchSet: SqlInjectionMatchSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SqlInjectionMatchSetTypeDef](./type_defs.md#sqlinjectionmatchsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSqlInjectionMatchSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateSqlInjectionMatchSetRequestRequestTypeDef

def get_value() -> UpdateSqlInjectionMatchSetRequestRequestTypeDef:
    return {
        "SqlInjectionMatchSetId": ...,
        "ChangeToken": ...,
        "Updates": ...,
    }
```

```python title="Definition"
class UpdateSqlInjectionMatchSetRequestRequestTypeDef(TypedDict):
    SqlInjectionMatchSetId: str,
    ChangeToken: str,
    Updates: Sequence[SqlInjectionMatchSetUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: SqlInjectionMatchSetUpdateTypeDef](./type_defs.md#sqlinjectionmatchsetupdatetypedef) 
## CreateXssMatchSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import CreateXssMatchSetResponseTypeDef

def get_value() -> CreateXssMatchSetResponseTypeDef:
    return {
        "XssMatchSet": ...,
        "ChangeToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class CreateXssMatchSetResponseTypeDef(TypedDict):
    XssMatchSet: XssMatchSetTypeDef,  # (1)
    ChangeToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: XssMatchSetTypeDef](./type_defs.md#xssmatchsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetXssMatchSetResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetXssMatchSetResponseTypeDef

def get_value() -> GetXssMatchSetResponseTypeDef:
    return {
        "XssMatchSet": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetXssMatchSetResponseTypeDef(TypedDict):
    XssMatchSet: XssMatchSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: XssMatchSetTypeDef](./type_defs.md#xssmatchsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateXssMatchSetRequestRequestTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import UpdateXssMatchSetRequestRequestTypeDef

def get_value() -> UpdateXssMatchSetRequestRequestTypeDef:
    return {
        "XssMatchSetId": ...,
        "ChangeToken": ...,
        "Updates": ...,
    }
```

```python title="Definition"
class UpdateXssMatchSetRequestRequestTypeDef(TypedDict):
    XssMatchSetId: str,
    ChangeToken: str,
    Updates: Sequence[XssMatchSetUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: XssMatchSetUpdateTypeDef](./type_defs.md#xssmatchsetupdatetypedef) 
## GetSampledRequestsResponseTypeDef

```python title="Usage Example"
from types_aiobotocore_waf_regional.type_defs import GetSampledRequestsResponseTypeDef

def get_value() -> GetSampledRequestsResponseTypeDef:
    return {
        "SampledRequests": ...,
        "PopulationSize": ...,
        "TimeWindow": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetSampledRequestsResponseTypeDef(TypedDict):
    SampledRequests: List[SampledHTTPRequestTypeDef],  # (1)
    PopulationSize: int,
    TimeWindow: TimeWindowTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SampledHTTPRequestTypeDef](./type_defs.md#sampledhttprequesttypedef) 
2. See [:material-code-braces: TimeWindowTypeDef](./type_defs.md#timewindowtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
