# WAFV2Client

> [Index](../README.md) > [WAFV2](./README.md) > WAFV2Client

!!! note ""

    Auto-generated documentation for [WAFV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#wafv2)
    type annotations stubs module [types-aiobotocore-wafv2](https://pypi.org/project/types-aiobotocore-wafv2/).

## WAFV2Client

Type annotations and code completion for `#!python session.client("wafv2")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# WAFV2Client usage example

from aioboto3.session import Session
from types_aiobotocore_wafv2.client import WAFV2Client

session = Session()
async with session.client("wafv2") as client:
    client: WAFV2Client
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("wafv2").exceptions` structure.

```python
# WAFV2Client.exceptions usage example

async with session.client("wafv2") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.WAFAssociatedItemException,
        client.exceptions.WAFConfigurationWarningException,
        client.exceptions.WAFDuplicateItemException,
        client.exceptions.WAFExpiredManagedRuleGroupVersionException,
        client.exceptions.WAFInternalErrorException,
        client.exceptions.WAFInvalidOperationException,
        client.exceptions.WAFInvalidParameterException,
        client.exceptions.WAFInvalidPermissionPolicyException,
        client.exceptions.WAFInvalidResourceException,
        client.exceptions.WAFLimitsExceededException,
        client.exceptions.WAFLogDestinationPermissionIssueException,
        client.exceptions.WAFNonexistentItemException,
        client.exceptions.WAFOptimisticLockException,
        client.exceptions.WAFServiceLinkedRoleErrorException,
        client.exceptions.WAFSubscriptionNotFoundException,
        client.exceptions.WAFTagOperationException,
        client.exceptions.WAFTagOperationInternalErrorException,
        client.exceptions.WAFUnavailableEntityException,
        client.exceptions.WAFUnsupportedAggregateKeyTypeException,
    ) as e:
        print(e)
```

```python
# WAFV2Client.exceptions type checking example

from types_aiobotocore_wafv2.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("wafv2").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("wafv2").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### associate\_web\_acl

Associates a web ACL with a regional application resource, to protect the
resource.

Type annotations and code completion for `#!python session.client("wafv2").associate_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# associate_web_acl method definition

await def associate_web_acl(
    self,
    *,
    WebACLArn: str,
    ResourceArn: str,
) -> dict[str, Any]:
    ...
```



```python
# associate_web_acl method usage example with argument unpacking

kwargs: AssociateWebACLRequestRequestTypeDef = {  # (1)
    "WebACLArn": ...,
    "ResourceArn": ...,
}

parent.associate_web_acl(**kwargs)
```

1. See [:material-code-braces: AssociateWebACLRequestRequestTypeDef](./type_defs.md#associatewebaclrequestrequesttypedef) 

### check\_capacity

Returns the web ACL capacity unit (WCU) requirements for a specified scope and
set of rules.

Type annotations and code completion for `#!python session.client("wafv2").check_capacity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# check_capacity method definition

await def check_capacity(
    self,
    *,
    Scope: ScopeType,  # (1)
    Rules: Sequence[RuleUnionTypeDef],  # (2)
) -> CheckCapacityResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
3. See [:material-code-braces: CheckCapacityResponseTypeDef](./type_defs.md#checkcapacityresponsetypedef) 


```python
# check_capacity method usage example with argument unpacking

kwargs: CheckCapacityRequestRequestTypeDef = {  # (1)
    "Scope": ...,
    "Rules": ...,
}

parent.check_capacity(**kwargs)
```

1. See [:material-code-braces: CheckCapacityRequestRequestTypeDef](./type_defs.md#checkcapacityrequestrequesttypedef) 

### create\_api\_key

Creates an API key that contains a set of token domains.

Type annotations and code completion for `#!python session.client("wafv2").create_api_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# create_api_key method definition

await def create_api_key(
    self,
    *,
    Scope: ScopeType,  # (1)
    TokenDomains: Sequence[str],
) -> CreateAPIKeyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: CreateAPIKeyResponseTypeDef](./type_defs.md#createapikeyresponsetypedef) 


```python
# create_api_key method usage example with argument unpacking

kwargs: CreateAPIKeyRequestRequestTypeDef = {  # (1)
    "Scope": ...,
    "TokenDomains": ...,
}

parent.create_api_key(**kwargs)
```

1. See [:material-code-braces: CreateAPIKeyRequestRequestTypeDef](./type_defs.md#createapikeyrequestrequesttypedef) 

### create\_ip\_set

Creates an <a>IPSet</a>, which you use to identify web requests that originate
from specific IP addresses or ranges of IP addresses.

Type annotations and code completion for `#!python session.client("wafv2").create_ip_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# create_ip_set method definition

await def create_ip_set(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    IPAddressVersion: IPAddressVersionType,  # (2)
    Addresses: Sequence[str],
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateIPSetResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-brackets: IPAddressVersionType](./literals.md#ipaddressversiontype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateIPSetResponseTypeDef](./type_defs.md#createipsetresponsetypedef) 


```python
# create_ip_set method usage example with argument unpacking

kwargs: CreateIPSetRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "IPAddressVersion": ...,
    "Addresses": ...,
}

parent.create_ip_set(**kwargs)
```

1. See [:material-code-braces: CreateIPSetRequestRequestTypeDef](./type_defs.md#createipsetrequestrequesttypedef) 

### create\_regex\_pattern\_set

Creates a <a>RegexPatternSet</a>, which you reference in a
<a>RegexPatternSetReferenceStatement</a>, to have WAF inspect a web request
component for the specified patterns.

Type annotations and code completion for `#!python session.client("wafv2").create_regex_pattern_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# create_regex_pattern_set method definition

await def create_regex_pattern_set(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    RegularExpressionList: Sequence[RegexTypeDef],  # (2)
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateRegexPatternSetResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: RegexTypeDef](./type_defs.md#regextypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateRegexPatternSetResponseTypeDef](./type_defs.md#createregexpatternsetresponsetypedef) 


```python
# create_regex_pattern_set method usage example with argument unpacking

kwargs: CreateRegexPatternSetRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "RegularExpressionList": ...,
}

parent.create_regex_pattern_set(**kwargs)
```

1. See [:material-code-braces: CreateRegexPatternSetRequestRequestTypeDef](./type_defs.md#createregexpatternsetrequestrequesttypedef) 

### create\_rule\_group

Creates a <a>RuleGroup</a> per the specifications provided.

Type annotations and code completion for `#!python session.client("wafv2").create_rule_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# create_rule_group method definition

await def create_rule_group(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Capacity: int,
    VisibilityConfig: VisibilityConfigTypeDef,  # (2)
    Description: str = ...,
    Rules: Sequence[RuleTypeDef] = ...,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
    CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,  # (5)
) -> CreateRuleGroupResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
3. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CustomResponseBodyTypeDef](./type_defs.md#customresponsebodytypedef) 
6. See [:material-code-braces: CreateRuleGroupResponseTypeDef](./type_defs.md#createrulegroupresponsetypedef) 


```python
# create_rule_group method usage example with argument unpacking

kwargs: CreateRuleGroupRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Capacity": ...,
    "VisibilityConfig": ...,
}

parent.create_rule_group(**kwargs)
```

1. See [:material-code-braces: CreateRuleGroupRequestRequestTypeDef](./type_defs.md#createrulegrouprequestrequesttypedef) 

### create\_web\_acl

Creates a <a>WebACL</a> per the specifications provided.

Type annotations and code completion for `#!python session.client("wafv2").create_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# create_web_acl method definition

await def create_web_acl(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    DefaultAction: DefaultActionTypeDef,  # (2)
    VisibilityConfig: VisibilityConfigTypeDef,  # (3)
    Description: str = ...,
    Rules: Sequence[RuleTypeDef] = ...,  # (4)
    Tags: Sequence[TagTypeDef] = ...,  # (5)
    CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,  # (6)
    CaptchaConfig: CaptchaConfigTypeDef = ...,  # (7)
    ChallengeConfig: ChallengeConfigTypeDef = ...,  # (8)
    TokenDomains: Sequence[str] = ...,
    AssociationConfig: AssociationConfigTypeDef = ...,  # (9)
) -> CreateWebACLResponseTypeDef:  # (10)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: DefaultActionTypeDef](./type_defs.md#defaultactiontypedef) 
3. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
4. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: CustomResponseBodyTypeDef](./type_defs.md#customresponsebodytypedef) 
7. See [:material-code-braces: CaptchaConfigTypeDef](./type_defs.md#captchaconfigtypedef) 
8. See [:material-code-braces: ChallengeConfigTypeDef](./type_defs.md#challengeconfigtypedef) 
9. See [:material-code-braces: AssociationConfigTypeDef](./type_defs.md#associationconfigtypedef) 
10. See [:material-code-braces: CreateWebACLResponseTypeDef](./type_defs.md#createwebaclresponsetypedef) 


```python
# create_web_acl method usage example with argument unpacking

kwargs: CreateWebACLRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "DefaultAction": ...,
    "VisibilityConfig": ...,
}

parent.create_web_acl(**kwargs)
```

1. See [:material-code-braces: CreateWebACLRequestRequestTypeDef](./type_defs.md#createwebaclrequestrequesttypedef) 

### delete\_api\_key

Deletes the specified API key.

Type annotations and code completion for `#!python session.client("wafv2").delete_api_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# delete_api_key method definition

await def delete_api_key(
    self,
    *,
    Scope: ScopeType,  # (1)
    APIKey: str,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 


```python
# delete_api_key method usage example with argument unpacking

kwargs: DeleteAPIKeyRequestRequestTypeDef = {  # (1)
    "Scope": ...,
    "APIKey": ...,
}

parent.delete_api_key(**kwargs)
```

1. See [:material-code-braces: DeleteAPIKeyRequestRequestTypeDef](./type_defs.md#deleteapikeyrequestrequesttypedef) 

### delete\_firewall\_manager\_rule\_groups

Deletes all rule groups that are managed by Firewall Manager from the specified
<a>WebACL</a>.

Type annotations and code completion for `#!python session.client("wafv2").delete_firewall_manager_rule_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# delete_firewall_manager_rule_groups method definition

await def delete_firewall_manager_rule_groups(
    self,
    *,
    WebACLArn: str,
    WebACLLockToken: str,
) -> DeleteFirewallManagerRuleGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteFirewallManagerRuleGroupsResponseTypeDef](./type_defs.md#deletefirewallmanagerrulegroupsresponsetypedef) 


```python
# delete_firewall_manager_rule_groups method usage example with argument unpacking

kwargs: DeleteFirewallManagerRuleGroupsRequestRequestTypeDef = {  # (1)
    "WebACLArn": ...,
    "WebACLLockToken": ...,
}

parent.delete_firewall_manager_rule_groups(**kwargs)
```

1. See [:material-code-braces: DeleteFirewallManagerRuleGroupsRequestRequestTypeDef](./type_defs.md#deletefirewallmanagerrulegroupsrequestrequesttypedef) 

### delete\_ip\_set

Deletes the specified <a>IPSet</a>.

Type annotations and code completion for `#!python session.client("wafv2").delete_ip_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# delete_ip_set method definition

await def delete_ip_set(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    LockToken: str,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 


```python
# delete_ip_set method usage example with argument unpacking

kwargs: DeleteIPSetRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
    "LockToken": ...,
}

parent.delete_ip_set(**kwargs)
```

1. See [:material-code-braces: DeleteIPSetRequestRequestTypeDef](./type_defs.md#deleteipsetrequestrequesttypedef) 

### delete\_logging\_configuration

Deletes the <a>LoggingConfiguration</a> from the specified web ACL.

Type annotations and code completion for `#!python session.client("wafv2").delete_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# delete_logging_configuration method definition

await def delete_logging_configuration(
    self,
    *,
    ResourceArn: str,
    LogType: LogTypeType = ...,  # (1)
    LogScope: LogScopeType = ...,  # (2)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
2. See [:material-code-brackets: LogScopeType](./literals.md#logscopetype) 


```python
# delete_logging_configuration method usage example with argument unpacking

kwargs: DeleteLoggingConfigurationRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.delete_logging_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteLoggingConfigurationRequestRequestTypeDef](./type_defs.md#deleteloggingconfigurationrequestrequesttypedef) 

### delete\_permission\_policy

Permanently deletes an IAM policy from the specified rule group.

Type annotations and code completion for `#!python session.client("wafv2").delete_permission_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# delete_permission_policy method definition

await def delete_permission_policy(
    self,
    *,
    ResourceArn: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_permission_policy method usage example with argument unpacking

kwargs: DeletePermissionPolicyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.delete_permission_policy(**kwargs)
```

1. See [:material-code-braces: DeletePermissionPolicyRequestRequestTypeDef](./type_defs.md#deletepermissionpolicyrequestrequesttypedef) 

### delete\_regex\_pattern\_set

Deletes the specified <a>RegexPatternSet</a>.

Type annotations and code completion for `#!python session.client("wafv2").delete_regex_pattern_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# delete_regex_pattern_set method definition

await def delete_regex_pattern_set(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    LockToken: str,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 


```python
# delete_regex_pattern_set method usage example with argument unpacking

kwargs: DeleteRegexPatternSetRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
    "LockToken": ...,
}

parent.delete_regex_pattern_set(**kwargs)
```

1. See [:material-code-braces: DeleteRegexPatternSetRequestRequestTypeDef](./type_defs.md#deleteregexpatternsetrequestrequesttypedef) 

### delete\_rule\_group

Deletes the specified <a>RuleGroup</a>.

Type annotations and code completion for `#!python session.client("wafv2").delete_rule_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# delete_rule_group method definition

await def delete_rule_group(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    LockToken: str,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 


```python
# delete_rule_group method usage example with argument unpacking

kwargs: DeleteRuleGroupRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
    "LockToken": ...,
}

parent.delete_rule_group(**kwargs)
```

1. See [:material-code-braces: DeleteRuleGroupRequestRequestTypeDef](./type_defs.md#deleterulegrouprequestrequesttypedef) 

### delete\_web\_acl

Deletes the specified <a>WebACL</a>.

Type annotations and code completion for `#!python session.client("wafv2").delete_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# delete_web_acl method definition

await def delete_web_acl(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    LockToken: str,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 


```python
# delete_web_acl method usage example with argument unpacking

kwargs: DeleteWebACLRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
    "LockToken": ...,
}

parent.delete_web_acl(**kwargs)
```

1. See [:material-code-braces: DeleteWebACLRequestRequestTypeDef](./type_defs.md#deletewebaclrequestrequesttypedef) 

### describe\_all\_managed\_products

Provides high-level information for the Amazon Web Services Managed Rules rule
groups and Amazon Web Services Marketplace managed rule groups.

Type annotations and code completion for `#!python session.client("wafv2").describe_all_managed_products` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# describe_all_managed_products method definition

await def describe_all_managed_products(
    self,
    *,
    Scope: ScopeType,  # (1)
) -> DescribeAllManagedProductsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: DescribeAllManagedProductsResponseTypeDef](./type_defs.md#describeallmanagedproductsresponsetypedef) 


```python
# describe_all_managed_products method usage example with argument unpacking

kwargs: DescribeAllManagedProductsRequestRequestTypeDef = {  # (1)
    "Scope": ...,
}

parent.describe_all_managed_products(**kwargs)
```

1. See [:material-code-braces: DescribeAllManagedProductsRequestRequestTypeDef](./type_defs.md#describeallmanagedproductsrequestrequesttypedef) 

### describe\_managed\_products\_by\_vendor

Provides high-level information for the managed rule groups owned by a specific
vendor.

Type annotations and code completion for `#!python session.client("wafv2").describe_managed_products_by_vendor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# describe_managed_products_by_vendor method definition

await def describe_managed_products_by_vendor(
    self,
    *,
    VendorName: str,
    Scope: ScopeType,  # (1)
) -> DescribeManagedProductsByVendorResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: DescribeManagedProductsByVendorResponseTypeDef](./type_defs.md#describemanagedproductsbyvendorresponsetypedef) 


```python
# describe_managed_products_by_vendor method usage example with argument unpacking

kwargs: DescribeManagedProductsByVendorRequestRequestTypeDef = {  # (1)
    "VendorName": ...,
    "Scope": ...,
}

parent.describe_managed_products_by_vendor(**kwargs)
```

1. See [:material-code-braces: DescribeManagedProductsByVendorRequestRequestTypeDef](./type_defs.md#describemanagedproductsbyvendorrequestrequesttypedef) 

### describe\_managed\_rule\_group

Provides high-level information for a managed rule group, including
descriptions of the rules.

Type annotations and code completion for `#!python session.client("wafv2").describe_managed_rule_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# describe_managed_rule_group method definition

await def describe_managed_rule_group(
    self,
    *,
    VendorName: str,
    Name: str,
    Scope: ScopeType,  # (1)
    VersionName: str = ...,
) -> DescribeManagedRuleGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: DescribeManagedRuleGroupResponseTypeDef](./type_defs.md#describemanagedrulegroupresponsetypedef) 


```python
# describe_managed_rule_group method usage example with argument unpacking

kwargs: DescribeManagedRuleGroupRequestRequestTypeDef = {  # (1)
    "VendorName": ...,
    "Name": ...,
    "Scope": ...,
}

parent.describe_managed_rule_group(**kwargs)
```

1. See [:material-code-braces: DescribeManagedRuleGroupRequestRequestTypeDef](./type_defs.md#describemanagedrulegrouprequestrequesttypedef) 

### disassociate\_web\_acl

Disassociates the specified regional application resource from any existing web
ACL association.

Type annotations and code completion for `#!python session.client("wafv2").disassociate_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# disassociate_web_acl method definition

await def disassociate_web_acl(
    self,
    *,
    ResourceArn: str,
) -> dict[str, Any]:
    ...
```



```python
# disassociate_web_acl method usage example with argument unpacking

kwargs: DisassociateWebACLRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.disassociate_web_acl(**kwargs)
```

1. See [:material-code-braces: DisassociateWebACLRequestRequestTypeDef](./type_defs.md#disassociatewebaclrequestrequesttypedef) 

### generate\_mobile\_sdk\_release\_url

Generates a presigned download URL for the specified release of the mobile SDK.

Type annotations and code completion for `#!python session.client("wafv2").generate_mobile_sdk_release_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# generate_mobile_sdk_release_url method definition

await def generate_mobile_sdk_release_url(
    self,
    *,
    Platform: PlatformType,  # (1)
    ReleaseVersion: str,
) -> GenerateMobileSdkReleaseUrlResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
2. See [:material-code-braces: GenerateMobileSdkReleaseUrlResponseTypeDef](./type_defs.md#generatemobilesdkreleaseurlresponsetypedef) 


```python
# generate_mobile_sdk_release_url method usage example with argument unpacking

kwargs: GenerateMobileSdkReleaseUrlRequestRequestTypeDef = {  # (1)
    "Platform": ...,
    "ReleaseVersion": ...,
}

parent.generate_mobile_sdk_release_url(**kwargs)
```

1. See [:material-code-braces: GenerateMobileSdkReleaseUrlRequestRequestTypeDef](./type_defs.md#generatemobilesdkreleaseurlrequestrequesttypedef) 

### get\_decrypted\_api\_key

Returns your API key in decrypted form.

Type annotations and code completion for `#!python session.client("wafv2").get_decrypted_api_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# get_decrypted_api_key method definition

await def get_decrypted_api_key(
    self,
    *,
    Scope: ScopeType,  # (1)
    APIKey: str,
) -> GetDecryptedAPIKeyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: GetDecryptedAPIKeyResponseTypeDef](./type_defs.md#getdecryptedapikeyresponsetypedef) 


```python
# get_decrypted_api_key method usage example with argument unpacking

kwargs: GetDecryptedAPIKeyRequestRequestTypeDef = {  # (1)
    "Scope": ...,
    "APIKey": ...,
}

parent.get_decrypted_api_key(**kwargs)
```

1. See [:material-code-braces: GetDecryptedAPIKeyRequestRequestTypeDef](./type_defs.md#getdecryptedapikeyrequestrequesttypedef) 

### get\_ip\_set

Retrieves the specified <a>IPSet</a>.

Type annotations and code completion for `#!python session.client("wafv2").get_ip_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# get_ip_set method definition

await def get_ip_set(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
) -> GetIPSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: GetIPSetResponseTypeDef](./type_defs.md#getipsetresponsetypedef) 


```python
# get_ip_set method usage example with argument unpacking

kwargs: GetIPSetRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
}

parent.get_ip_set(**kwargs)
```

1. See [:material-code-braces: GetIPSetRequestRequestTypeDef](./type_defs.md#getipsetrequestrequesttypedef) 

### get\_logging\_configuration

Returns the <a>LoggingConfiguration</a> for the specified web ACL.

Type annotations and code completion for `#!python session.client("wafv2").get_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# get_logging_configuration method definition

await def get_logging_configuration(
    self,
    *,
    ResourceArn: str,
    LogType: LogTypeType = ...,  # (1)
    LogScope: LogScopeType = ...,  # (2)
) -> GetLoggingConfigurationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
2. See [:material-code-brackets: LogScopeType](./literals.md#logscopetype) 
3. See [:material-code-braces: GetLoggingConfigurationResponseTypeDef](./type_defs.md#getloggingconfigurationresponsetypedef) 


```python
# get_logging_configuration method usage example with argument unpacking

kwargs: GetLoggingConfigurationRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_logging_configuration(**kwargs)
```

1. See [:material-code-braces: GetLoggingConfigurationRequestRequestTypeDef](./type_defs.md#getloggingconfigurationrequestrequesttypedef) 

### get\_managed\_rule\_set

Retrieves the specified managed rule set.

Type annotations and code completion for `#!python session.client("wafv2").get_managed_rule_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# get_managed_rule_set method definition

await def get_managed_rule_set(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
) -> GetManagedRuleSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: GetManagedRuleSetResponseTypeDef](./type_defs.md#getmanagedrulesetresponsetypedef) 


```python
# get_managed_rule_set method usage example with argument unpacking

kwargs: GetManagedRuleSetRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
}

parent.get_managed_rule_set(**kwargs)
```

1. See [:material-code-braces: GetManagedRuleSetRequestRequestTypeDef](./type_defs.md#getmanagedrulesetrequestrequesttypedef) 

### get\_mobile\_sdk\_release

Retrieves information for the specified mobile SDK release, including release
notes and tags.

Type annotations and code completion for `#!python session.client("wafv2").get_mobile_sdk_release` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# get_mobile_sdk_release method definition

await def get_mobile_sdk_release(
    self,
    *,
    Platform: PlatformType,  # (1)
    ReleaseVersion: str,
) -> GetMobileSdkReleaseResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
2. See [:material-code-braces: GetMobileSdkReleaseResponseTypeDef](./type_defs.md#getmobilesdkreleaseresponsetypedef) 


```python
# get_mobile_sdk_release method usage example with argument unpacking

kwargs: GetMobileSdkReleaseRequestRequestTypeDef = {  # (1)
    "Platform": ...,
    "ReleaseVersion": ...,
}

parent.get_mobile_sdk_release(**kwargs)
```

1. See [:material-code-braces: GetMobileSdkReleaseRequestRequestTypeDef](./type_defs.md#getmobilesdkreleaserequestrequesttypedef) 

### get\_permission\_policy

Returns the IAM policy that is attached to the specified rule group.

Type annotations and code completion for `#!python session.client("wafv2").get_permission_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# get_permission_policy method definition

await def get_permission_policy(
    self,
    *,
    ResourceArn: str,
) -> GetPermissionPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPermissionPolicyResponseTypeDef](./type_defs.md#getpermissionpolicyresponsetypedef) 


```python
# get_permission_policy method usage example with argument unpacking

kwargs: GetPermissionPolicyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_permission_policy(**kwargs)
```

1. See [:material-code-braces: GetPermissionPolicyRequestRequestTypeDef](./type_defs.md#getpermissionpolicyrequestrequesttypedef) 

### get\_rate\_based\_statement\_managed\_keys

Retrieves the IP addresses that are currently blocked by a rate-based rule
instance.

Type annotations and code completion for `#!python session.client("wafv2").get_rate_based_statement_managed_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# get_rate_based_statement_managed_keys method definition

await def get_rate_based_statement_managed_keys(
    self,
    *,
    Scope: ScopeType,  # (1)
    WebACLName: str,
    WebACLId: str,
    RuleName: str,
    RuleGroupRuleName: str = ...,
) -> GetRateBasedStatementManagedKeysResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: GetRateBasedStatementManagedKeysResponseTypeDef](./type_defs.md#getratebasedstatementmanagedkeysresponsetypedef) 


```python
# get_rate_based_statement_managed_keys method usage example with argument unpacking

kwargs: GetRateBasedStatementManagedKeysRequestRequestTypeDef = {  # (1)
    "Scope": ...,
    "WebACLName": ...,
    "WebACLId": ...,
    "RuleName": ...,
}

parent.get_rate_based_statement_managed_keys(**kwargs)
```

1. See [:material-code-braces: GetRateBasedStatementManagedKeysRequestRequestTypeDef](./type_defs.md#getratebasedstatementmanagedkeysrequestrequesttypedef) 

### get\_regex\_pattern\_set

Retrieves the specified <a>RegexPatternSet</a>.

Type annotations and code completion for `#!python session.client("wafv2").get_regex_pattern_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# get_regex_pattern_set method definition

await def get_regex_pattern_set(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
) -> GetRegexPatternSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: GetRegexPatternSetResponseTypeDef](./type_defs.md#getregexpatternsetresponsetypedef) 


```python
# get_regex_pattern_set method usage example with argument unpacking

kwargs: GetRegexPatternSetRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
}

parent.get_regex_pattern_set(**kwargs)
```

1. See [:material-code-braces: GetRegexPatternSetRequestRequestTypeDef](./type_defs.md#getregexpatternsetrequestrequesttypedef) 

### get\_rule\_group

Retrieves the specified <a>RuleGroup</a>.

Type annotations and code completion for `#!python session.client("wafv2").get_rule_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# get_rule_group method definition

await def get_rule_group(
    self,
    *,
    Name: str = ...,
    Scope: ScopeType = ...,  # (1)
    Id: str = ...,
    ARN: str = ...,
) -> GetRuleGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: GetRuleGroupResponseTypeDef](./type_defs.md#getrulegroupresponsetypedef) 


```python
# get_rule_group method usage example with argument unpacking

kwargs: GetRuleGroupRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_rule_group(**kwargs)
```

1. See [:material-code-braces: GetRuleGroupRequestRequestTypeDef](./type_defs.md#getrulegrouprequestrequesttypedef) 

### get\_sampled\_requests

Gets detailed information about a specified number of requests--a sample--that
WAF randomly selects from among the first 5,000 requests that your Amazon Web
Services resource received during a time range that you choose.

Type annotations and code completion for `#!python session.client("wafv2").get_sampled_requests` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# get_sampled_requests method definition

await def get_sampled_requests(
    self,
    *,
    WebAclArn: str,
    RuleMetricName: str,
    Scope: ScopeType,  # (1)
    TimeWindow: TimeWindowTypeDef,  # (2)
    MaxItems: int,
) -> GetSampledRequestsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: TimeWindowTypeDef](./type_defs.md#timewindowtypedef) 
3. See [:material-code-braces: GetSampledRequestsResponseTypeDef](./type_defs.md#getsampledrequestsresponsetypedef) 


```python
# get_sampled_requests method usage example with argument unpacking

kwargs: GetSampledRequestsRequestRequestTypeDef = {  # (1)
    "WebAclArn": ...,
    "RuleMetricName": ...,
    "Scope": ...,
    "TimeWindow": ...,
    "MaxItems": ...,
}

parent.get_sampled_requests(**kwargs)
```

1. See [:material-code-braces: GetSampledRequestsRequestRequestTypeDef](./type_defs.md#getsampledrequestsrequestrequesttypedef) 

### get\_web\_acl

Retrieves the specified <a>WebACL</a>.

Type annotations and code completion for `#!python session.client("wafv2").get_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# get_web_acl method definition

await def get_web_acl(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
) -> GetWebACLResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: GetWebACLResponseTypeDef](./type_defs.md#getwebaclresponsetypedef) 


```python
# get_web_acl method usage example with argument unpacking

kwargs: GetWebACLRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
}

parent.get_web_acl(**kwargs)
```

1. See [:material-code-braces: GetWebACLRequestRequestTypeDef](./type_defs.md#getwebaclrequestrequesttypedef) 

### get\_web\_acl\_for\_resource

Retrieves the <a>WebACL</a> for the specified resource.

Type annotations and code completion for `#!python session.client("wafv2").get_web_acl_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# get_web_acl_for_resource method definition

await def get_web_acl_for_resource(
    self,
    *,
    ResourceArn: str,
) -> GetWebACLForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWebACLForResourceResponseTypeDef](./type_defs.md#getwebaclforresourceresponsetypedef) 


```python
# get_web_acl_for_resource method usage example with argument unpacking

kwargs: GetWebACLForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_web_acl_for_resource(**kwargs)
```

1. See [:material-code-braces: GetWebACLForResourceRequestRequestTypeDef](./type_defs.md#getwebaclforresourcerequestrequesttypedef) 

### list\_api\_keys

Retrieves a list of the API keys that you've defined for the specified scope.

Type annotations and code completion for `#!python session.client("wafv2").list_api_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# list_api_keys method definition

await def list_api_keys(
    self,
    *,
    Scope: ScopeType,  # (1)
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListAPIKeysResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: ListAPIKeysResponseTypeDef](./type_defs.md#listapikeysresponsetypedef) 


```python
# list_api_keys method usage example with argument unpacking

kwargs: ListAPIKeysRequestRequestTypeDef = {  # (1)
    "Scope": ...,
}

parent.list_api_keys(**kwargs)
```

1. See [:material-code-braces: ListAPIKeysRequestRequestTypeDef](./type_defs.md#listapikeysrequestrequesttypedef) 

### list\_available\_managed\_rule\_group\_versions

Returns a list of the available versions for the specified managed rule group.

Type annotations and code completion for `#!python session.client("wafv2").list_available_managed_rule_group_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# list_available_managed_rule_group_versions method definition

await def list_available_managed_rule_group_versions(
    self,
    *,
    VendorName: str,
    Name: str,
    Scope: ScopeType,  # (1)
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListAvailableManagedRuleGroupVersionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: ListAvailableManagedRuleGroupVersionsResponseTypeDef](./type_defs.md#listavailablemanagedrulegroupversionsresponsetypedef) 


```python
# list_available_managed_rule_group_versions method usage example with argument unpacking

kwargs: ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef = {  # (1)
    "VendorName": ...,
    "Name": ...,
    "Scope": ...,
}

parent.list_available_managed_rule_group_versions(**kwargs)
```

1. See [:material-code-braces: ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef](./type_defs.md#listavailablemanagedrulegroupversionsrequestrequesttypedef) 

### list\_available\_managed\_rule\_groups

Retrieves an array of managed rule groups that are available for you to use.

Type annotations and code completion for `#!python session.client("wafv2").list_available_managed_rule_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# list_available_managed_rule_groups method definition

await def list_available_managed_rule_groups(
    self,
    *,
    Scope: ScopeType,  # (1)
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListAvailableManagedRuleGroupsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: ListAvailableManagedRuleGroupsResponseTypeDef](./type_defs.md#listavailablemanagedrulegroupsresponsetypedef) 


```python
# list_available_managed_rule_groups method usage example with argument unpacking

kwargs: ListAvailableManagedRuleGroupsRequestRequestTypeDef = {  # (1)
    "Scope": ...,
}

parent.list_available_managed_rule_groups(**kwargs)
```

1. See [:material-code-braces: ListAvailableManagedRuleGroupsRequestRequestTypeDef](./type_defs.md#listavailablemanagedrulegroupsrequestrequesttypedef) 

### list\_ip\_sets

Retrieves an array of <a>IPSetSummary</a> objects for the IP sets that you
manage.

Type annotations and code completion for `#!python session.client("wafv2").list_ip_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# list_ip_sets method definition

await def list_ip_sets(
    self,
    *,
    Scope: ScopeType,  # (1)
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListIPSetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: ListIPSetsResponseTypeDef](./type_defs.md#listipsetsresponsetypedef) 


```python
# list_ip_sets method usage example with argument unpacking

kwargs: ListIPSetsRequestRequestTypeDef = {  # (1)
    "Scope": ...,
}

parent.list_ip_sets(**kwargs)
```

1. See [:material-code-braces: ListIPSetsRequestRequestTypeDef](./type_defs.md#listipsetsrequestrequesttypedef) 

### list\_logging\_configurations

Retrieves an array of your <a>LoggingConfiguration</a> objects.

Type annotations and code completion for `#!python session.client("wafv2").list_logging_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# list_logging_configurations method definition

await def list_logging_configurations(
    self,
    *,
    Scope: ScopeType,  # (1)
    NextMarker: str = ...,
    Limit: int = ...,
    LogScope: LogScopeType = ...,  # (2)
) -> ListLoggingConfigurationsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-brackets: LogScopeType](./literals.md#logscopetype) 
3. See [:material-code-braces: ListLoggingConfigurationsResponseTypeDef](./type_defs.md#listloggingconfigurationsresponsetypedef) 


```python
# list_logging_configurations method usage example with argument unpacking

kwargs: ListLoggingConfigurationsRequestRequestTypeDef = {  # (1)
    "Scope": ...,
}

parent.list_logging_configurations(**kwargs)
```

1. See [:material-code-braces: ListLoggingConfigurationsRequestRequestTypeDef](./type_defs.md#listloggingconfigurationsrequestrequesttypedef) 

### list\_managed\_rule\_sets

Retrieves the managed rule sets that you own.

Type annotations and code completion for `#!python session.client("wafv2").list_managed_rule_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# list_managed_rule_sets method definition

await def list_managed_rule_sets(
    self,
    *,
    Scope: ScopeType,  # (1)
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListManagedRuleSetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: ListManagedRuleSetsResponseTypeDef](./type_defs.md#listmanagedrulesetsresponsetypedef) 


```python
# list_managed_rule_sets method usage example with argument unpacking

kwargs: ListManagedRuleSetsRequestRequestTypeDef = {  # (1)
    "Scope": ...,
}

parent.list_managed_rule_sets(**kwargs)
```

1. See [:material-code-braces: ListManagedRuleSetsRequestRequestTypeDef](./type_defs.md#listmanagedrulesetsrequestrequesttypedef) 

### list\_mobile\_sdk\_releases

Retrieves a list of the available releases for the mobile SDK and the specified
device platform.

Type annotations and code completion for `#!python session.client("wafv2").list_mobile_sdk_releases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# list_mobile_sdk_releases method definition

await def list_mobile_sdk_releases(
    self,
    *,
    Platform: PlatformType,  # (1)
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListMobileSdkReleasesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
2. See [:material-code-braces: ListMobileSdkReleasesResponseTypeDef](./type_defs.md#listmobilesdkreleasesresponsetypedef) 


```python
# list_mobile_sdk_releases method usage example with argument unpacking

kwargs: ListMobileSdkReleasesRequestRequestTypeDef = {  # (1)
    "Platform": ...,
}

parent.list_mobile_sdk_releases(**kwargs)
```

1. See [:material-code-braces: ListMobileSdkReleasesRequestRequestTypeDef](./type_defs.md#listmobilesdkreleasesrequestrequesttypedef) 

### list\_regex\_pattern\_sets

Retrieves an array of <a>RegexPatternSetSummary</a> objects for the regex
pattern sets that you manage.

Type annotations and code completion for `#!python session.client("wafv2").list_regex_pattern_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# list_regex_pattern_sets method definition

await def list_regex_pattern_sets(
    self,
    *,
    Scope: ScopeType,  # (1)
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListRegexPatternSetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: ListRegexPatternSetsResponseTypeDef](./type_defs.md#listregexpatternsetsresponsetypedef) 


```python
# list_regex_pattern_sets method usage example with argument unpacking

kwargs: ListRegexPatternSetsRequestRequestTypeDef = {  # (1)
    "Scope": ...,
}

parent.list_regex_pattern_sets(**kwargs)
```

1. See [:material-code-braces: ListRegexPatternSetsRequestRequestTypeDef](./type_defs.md#listregexpatternsetsrequestrequesttypedef) 

### list\_resources\_for\_web\_acl

Retrieves an array of the Amazon Resource Names (ARNs) for the regional
resources that are associated with the specified web ACL.

Type annotations and code completion for `#!python session.client("wafv2").list_resources_for_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# list_resources_for_web_acl method definition

await def list_resources_for_web_acl(
    self,
    *,
    WebACLArn: str,
    ResourceType: ResourceTypeType = ...,  # (1)
) -> ListResourcesForWebACLResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ListResourcesForWebACLResponseTypeDef](./type_defs.md#listresourcesforwebaclresponsetypedef) 


```python
# list_resources_for_web_acl method usage example with argument unpacking

kwargs: ListResourcesForWebACLRequestRequestTypeDef = {  # (1)
    "WebACLArn": ...,
}

parent.list_resources_for_web_acl(**kwargs)
```

1. See [:material-code-braces: ListResourcesForWebACLRequestRequestTypeDef](./type_defs.md#listresourcesforwebaclrequestrequesttypedef) 

### list\_rule\_groups

Retrieves an array of <a>RuleGroupSummary</a> objects for the rule groups that
you manage.

Type annotations and code completion for `#!python session.client("wafv2").list_rule_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# list_rule_groups method definition

await def list_rule_groups(
    self,
    *,
    Scope: ScopeType,  # (1)
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListRuleGroupsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: ListRuleGroupsResponseTypeDef](./type_defs.md#listrulegroupsresponsetypedef) 


```python
# list_rule_groups method usage example with argument unpacking

kwargs: ListRuleGroupsRequestRequestTypeDef = {  # (1)
    "Scope": ...,
}

parent.list_rule_groups(**kwargs)
```

1. See [:material-code-braces: ListRuleGroupsRequestRequestTypeDef](./type_defs.md#listrulegroupsrequestrequesttypedef) 

### list\_tags\_for\_resource

Retrieves the <a>TagInfoForResource</a> for the specified resource.

Type annotations and code completion for `#!python session.client("wafv2").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_web\_acls

Retrieves an array of <a>WebACLSummary</a> objects for the web ACLs that you
manage.

Type annotations and code completion for `#!python session.client("wafv2").list_web_acls` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# list_web_acls method definition

await def list_web_acls(
    self,
    *,
    Scope: ScopeType,  # (1)
    NextMarker: str = ...,
    Limit: int = ...,
) -> ListWebACLsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: ListWebACLsResponseTypeDef](./type_defs.md#listwebaclsresponsetypedef) 


```python
# list_web_acls method usage example with argument unpacking

kwargs: ListWebACLsRequestRequestTypeDef = {  # (1)
    "Scope": ...,
}

parent.list_web_acls(**kwargs)
```

1. See [:material-code-braces: ListWebACLsRequestRequestTypeDef](./type_defs.md#listwebaclsrequestrequesttypedef) 

### put\_logging\_configuration

Enables the specified <a>LoggingConfiguration</a>, to start logging from a web
ACL, according to the configuration provided.

Type annotations and code completion for `#!python session.client("wafv2").put_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# put_logging_configuration method definition

await def put_logging_configuration(
    self,
    *,
    LoggingConfiguration: LoggingConfigurationTypeDef,  # (1)
) -> PutLoggingConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
2. See [:material-code-braces: PutLoggingConfigurationResponseTypeDef](./type_defs.md#putloggingconfigurationresponsetypedef) 


```python
# put_logging_configuration method usage example with argument unpacking

kwargs: PutLoggingConfigurationRequestRequestTypeDef = {  # (1)
    "LoggingConfiguration": ...,
}

parent.put_logging_configuration(**kwargs)
```

1. See [:material-code-braces: PutLoggingConfigurationRequestRequestTypeDef](./type_defs.md#putloggingconfigurationrequestrequesttypedef) 

### put\_managed\_rule\_set\_versions

Defines the versions of your managed rule set that you are offering to the
customers.

Type annotations and code completion for `#!python session.client("wafv2").put_managed_rule_set_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# put_managed_rule_set_versions method definition

await def put_managed_rule_set_versions(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    LockToken: str,
    RecommendedVersion: str = ...,
    VersionsToPublish: Mapping[str, VersionToPublishTypeDef] = ...,  # (2)
) -> PutManagedRuleSetVersionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: VersionToPublishTypeDef](./type_defs.md#versiontopublishtypedef) 
3. See [:material-code-braces: PutManagedRuleSetVersionsResponseTypeDef](./type_defs.md#putmanagedrulesetversionsresponsetypedef) 


```python
# put_managed_rule_set_versions method usage example with argument unpacking

kwargs: PutManagedRuleSetVersionsRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
    "LockToken": ...,
}

parent.put_managed_rule_set_versions(**kwargs)
```

1. See [:material-code-braces: PutManagedRuleSetVersionsRequestRequestTypeDef](./type_defs.md#putmanagedrulesetversionsrequestrequesttypedef) 

### put\_permission\_policy

Use this to share a rule group with other accounts.

Type annotations and code completion for `#!python session.client("wafv2").put_permission_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# put_permission_policy method definition

await def put_permission_policy(
    self,
    *,
    ResourceArn: str,
    Policy: str,
) -> dict[str, Any]:
    ...
```



```python
# put_permission_policy method usage example with argument unpacking

kwargs: PutPermissionPolicyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Policy": ...,
}

parent.put_permission_policy(**kwargs)
```

1. See [:material-code-braces: PutPermissionPolicyRequestRequestTypeDef](./type_defs.md#putpermissionpolicyrequestrequesttypedef) 

### tag\_resource

Associates tags with the specified Amazon Web Services resource.

Type annotations and code completion for `#!python session.client("wafv2").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Disassociates tags from an Amazon Web Services resource.

Type annotations and code completion for `#!python session.client("wafv2").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_ip\_set

Updates the specified <a>IPSet</a>.

Type annotations and code completion for `#!python session.client("wafv2").update_ip_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# update_ip_set method definition

await def update_ip_set(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    Addresses: Sequence[str],
    LockToken: str,
    Description: str = ...,
) -> UpdateIPSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: UpdateIPSetResponseTypeDef](./type_defs.md#updateipsetresponsetypedef) 


```python
# update_ip_set method usage example with argument unpacking

kwargs: UpdateIPSetRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
    "Addresses": ...,
    "LockToken": ...,
}

parent.update_ip_set(**kwargs)
```

1. See [:material-code-braces: UpdateIPSetRequestRequestTypeDef](./type_defs.md#updateipsetrequestrequesttypedef) 

### update\_managed\_rule\_set\_version\_expiry\_date

Updates the expiration information for your managed rule set.

Type annotations and code completion for `#!python session.client("wafv2").update_managed_rule_set_version_expiry_date` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# update_managed_rule_set_version_expiry_date method definition

await def update_managed_rule_set_version_expiry_date(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    LockToken: str,
    VersionToExpire: str,
    ExpiryTimestamp: TimestampTypeDef,
) -> UpdateManagedRuleSetVersionExpiryDateResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: UpdateManagedRuleSetVersionExpiryDateResponseTypeDef](./type_defs.md#updatemanagedrulesetversionexpirydateresponsetypedef) 


```python
# update_managed_rule_set_version_expiry_date method usage example with argument unpacking

kwargs: UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
    "LockToken": ...,
    "VersionToExpire": ...,
    "ExpiryTimestamp": ...,
}

parent.update_managed_rule_set_version_expiry_date(**kwargs)
```

1. See [:material-code-braces: UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef](./type_defs.md#updatemanagedrulesetversionexpirydaterequestrequesttypedef) 

### update\_regex\_pattern\_set

Updates the specified <a>RegexPatternSet</a>.

Type annotations and code completion for `#!python session.client("wafv2").update_regex_pattern_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# update_regex_pattern_set method definition

await def update_regex_pattern_set(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    RegularExpressionList: Sequence[RegexTypeDef],  # (2)
    LockToken: str,
    Description: str = ...,
) -> UpdateRegexPatternSetResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: RegexTypeDef](./type_defs.md#regextypedef) 
3. See [:material-code-braces: UpdateRegexPatternSetResponseTypeDef](./type_defs.md#updateregexpatternsetresponsetypedef) 


```python
# update_regex_pattern_set method usage example with argument unpacking

kwargs: UpdateRegexPatternSetRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
    "RegularExpressionList": ...,
    "LockToken": ...,
}

parent.update_regex_pattern_set(**kwargs)
```

1. See [:material-code-braces: UpdateRegexPatternSetRequestRequestTypeDef](./type_defs.md#updateregexpatternsetrequestrequesttypedef) 

### update\_rule\_group

Updates the specified <a>RuleGroup</a>.

Type annotations and code completion for `#!python session.client("wafv2").update_rule_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# update_rule_group method definition

await def update_rule_group(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    VisibilityConfig: VisibilityConfigTypeDef,  # (2)
    LockToken: str,
    Description: str = ...,
    Rules: Sequence[RuleTypeDef] = ...,  # (3)
    CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,  # (4)
) -> UpdateRuleGroupResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
3. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
4. See [:material-code-braces: CustomResponseBodyTypeDef](./type_defs.md#customresponsebodytypedef) 
5. See [:material-code-braces: UpdateRuleGroupResponseTypeDef](./type_defs.md#updaterulegroupresponsetypedef) 


```python
# update_rule_group method usage example with argument unpacking

kwargs: UpdateRuleGroupRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
    "VisibilityConfig": ...,
    "LockToken": ...,
}

parent.update_rule_group(**kwargs)
```

1. See [:material-code-braces: UpdateRuleGroupRequestRequestTypeDef](./type_defs.md#updaterulegrouprequestrequesttypedef) 

### update\_web\_acl

Updates the specified <a>WebACL</a>.

Type annotations and code completion for `#!python session.client("wafv2").update_web_acl` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# update_web_acl method definition

await def update_web_acl(
    self,
    *,
    Name: str,
    Scope: ScopeType,  # (1)
    Id: str,
    DefaultAction: DefaultActionTypeDef,  # (2)
    VisibilityConfig: VisibilityConfigTypeDef,  # (3)
    LockToken: str,
    Description: str = ...,
    Rules: Sequence[RuleTypeDef] = ...,  # (4)
    CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,  # (5)
    CaptchaConfig: CaptchaConfigTypeDef = ...,  # (6)
    ChallengeConfig: ChallengeConfigTypeDef = ...,  # (7)
    TokenDomains: Sequence[str] = ...,
    AssociationConfig: AssociationConfigTypeDef = ...,  # (8)
) -> UpdateWebACLResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
2. See [:material-code-braces: DefaultActionTypeDef](./type_defs.md#defaultactiontypedef) 
3. See [:material-code-braces: VisibilityConfigTypeDef](./type_defs.md#visibilityconfigtypedef) 
4. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
5. See [:material-code-braces: CustomResponseBodyTypeDef](./type_defs.md#customresponsebodytypedef) 
6. See [:material-code-braces: CaptchaConfigTypeDef](./type_defs.md#captchaconfigtypedef) 
7. See [:material-code-braces: ChallengeConfigTypeDef](./type_defs.md#challengeconfigtypedef) 
8. See [:material-code-braces: AssociationConfigTypeDef](./type_defs.md#associationconfigtypedef) 
9. See [:material-code-braces: UpdateWebACLResponseTypeDef](./type_defs.md#updatewebaclresponsetypedef) 


```python
# update_web_acl method usage example with argument unpacking

kwargs: UpdateWebACLRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Id": ...,
    "DefaultAction": ...,
    "VisibilityConfig": ...,
    "LockToken": ...,
}

parent.update_web_acl(**kwargs)
```

1. See [:material-code-braces: UpdateWebACLRequestRequestTypeDef](./type_defs.md#updatewebaclrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("wafv2").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("wafv2").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




