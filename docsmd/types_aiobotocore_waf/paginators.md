# Paginators

> [Index](../README.md) > [WAF](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [WAF](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
    type annotations stubs module [types-aiobotocore-waf](https://pypi.org/project/types-aiobotocore-waf/).

## GetRateBasedRuleManagedKeysPaginator

Type annotations and code completion for `#!python session.client("waf").get_paginator("get_rate_based_rule_managed_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.GetRateBasedRuleManagedKeys)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_waf.paginator import GetRateBasedRuleManagedKeysPaginator

session = Session()

session = get_session()
async with session.client("waf") as client:  # (1)
    paginator: GetRateBasedRuleManagedKeysPaginator = client.get_paginator("get_rate_based_rule_managed_keys")  # (2)
    async for item in paginator.paginate(...):
        item: GetRateBasedRuleManagedKeysResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [GetRateBasedRuleManagedKeysPaginator](./paginators.md#getratebasedrulemanagedkeyspaginator)
3. item: [:material-code-braces: GetRateBasedRuleManagedKeysResponseTypeDef](./type_defs.md#getratebasedrulemanagedkeysresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetRateBasedRuleManagedKeysPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    RuleId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetRateBasedRuleManagedKeysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetRateBasedRuleManagedKeysResponseTypeDef](./type_defs.md#getratebasedrulemanagedkeysresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef = {  # (1)
    "RuleId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef](./type_defs.md#getratebasedrulemanagedkeysrequestgetratebasedrulemanagedkeyspaginatetypedef) 
## ListActivatedRulesInRuleGroupPaginator

Type annotations and code completion for `#!python session.client("waf").get_paginator("list_activated_rules_in_rule_group")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListActivatedRulesInRuleGroup)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_waf.paginator import ListActivatedRulesInRuleGroupPaginator

session = Session()

session = get_session()
async with session.client("waf") as client:  # (1)
    paginator: ListActivatedRulesInRuleGroupPaginator = client.get_paginator("list_activated_rules_in_rule_group")  # (2)
    async for item in paginator.paginate(...):
        item: ListActivatedRulesInRuleGroupResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListActivatedRulesInRuleGroupPaginator](./paginators.md#listactivatedrulesinrulegrouppaginator)
3. item: [:material-code-braces: ListActivatedRulesInRuleGroupResponseTypeDef](./type_defs.md#listactivatedrulesinrulegroupresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListActivatedRulesInRuleGroupPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    RuleGroupId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListActivatedRulesInRuleGroupResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListActivatedRulesInRuleGroupResponseTypeDef](./type_defs.md#listactivatedrulesinrulegroupresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef = {  # (1)
    "RuleGroupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef](./type_defs.md#listactivatedrulesinrulegrouprequestlistactivatedrulesinrulegrouppaginatetypedef) 
## ListByteMatchSetsPaginator

Type annotations and code completion for `#!python session.client("waf").get_paginator("list_byte_match_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListByteMatchSets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_waf.paginator import ListByteMatchSetsPaginator

session = Session()

session = get_session()
async with session.client("waf") as client:  # (1)
    paginator: ListByteMatchSetsPaginator = client.get_paginator("list_byte_match_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListByteMatchSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListByteMatchSetsPaginator](./paginators.md#listbytematchsetspaginator)
3. item: [:material-code-braces: ListByteMatchSetsResponseTypeDef](./type_defs.md#listbytematchsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListByteMatchSetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListByteMatchSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListByteMatchSetsResponseTypeDef](./type_defs.md#listbytematchsetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef](./type_defs.md#listbytematchsetsrequestlistbytematchsetspaginatetypedef) 
## ListGeoMatchSetsPaginator

Type annotations and code completion for `#!python session.client("waf").get_paginator("list_geo_match_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListGeoMatchSets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_waf.paginator import ListGeoMatchSetsPaginator

session = Session()

session = get_session()
async with session.client("waf") as client:  # (1)
    paginator: ListGeoMatchSetsPaginator = client.get_paginator("list_geo_match_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListGeoMatchSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListGeoMatchSetsPaginator](./paginators.md#listgeomatchsetspaginator)
3. item: [:material-code-braces: ListGeoMatchSetsResponseTypeDef](./type_defs.md#listgeomatchsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGeoMatchSetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGeoMatchSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGeoMatchSetsResponseTypeDef](./type_defs.md#listgeomatchsetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef](./type_defs.md#listgeomatchsetsrequestlistgeomatchsetspaginatetypedef) 
## ListIPSetsPaginator

Type annotations and code completion for `#!python session.client("waf").get_paginator("list_ip_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListIPSets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_waf.paginator import ListIPSetsPaginator

session = Session()

session = get_session()
async with session.client("waf") as client:  # (1)
    paginator: ListIPSetsPaginator = client.get_paginator("list_ip_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListIPSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListIPSetsPaginator](./paginators.md#listipsetspaginator)
3. item: [:material-code-braces: ListIPSetsResponseTypeDef](./type_defs.md#listipsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListIPSetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListIPSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIPSetsResponseTypeDef](./type_defs.md#listipsetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListIPSetsRequestListIPSetsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIPSetsRequestListIPSetsPaginateTypeDef](./type_defs.md#listipsetsrequestlistipsetspaginatetypedef) 
## ListLoggingConfigurationsPaginator

Type annotations and code completion for `#!python session.client("waf").get_paginator("list_logging_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListLoggingConfigurations)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_waf.paginator import ListLoggingConfigurationsPaginator

session = Session()

session = get_session()
async with session.client("waf") as client:  # (1)
    paginator: ListLoggingConfigurationsPaginator = client.get_paginator("list_logging_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListLoggingConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListLoggingConfigurationsPaginator](./paginators.md#listloggingconfigurationspaginator)
3. item: [:material-code-braces: ListLoggingConfigurationsResponseTypeDef](./type_defs.md#listloggingconfigurationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLoggingConfigurationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListLoggingConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLoggingConfigurationsResponseTypeDef](./type_defs.md#listloggingconfigurationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef](./type_defs.md#listloggingconfigurationsrequestlistloggingconfigurationspaginatetypedef) 
## ListRateBasedRulesPaginator

Type annotations and code completion for `#!python session.client("waf").get_paginator("list_rate_based_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRateBasedRules)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_waf.paginator import ListRateBasedRulesPaginator

session = Session()

session = get_session()
async with session.client("waf") as client:  # (1)
    paginator: ListRateBasedRulesPaginator = client.get_paginator("list_rate_based_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListRateBasedRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListRateBasedRulesPaginator](./paginators.md#listratebasedrulespaginator)
3. item: [:material-code-braces: ListRateBasedRulesResponseTypeDef](./type_defs.md#listratebasedrulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRateBasedRulesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRateBasedRulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRateBasedRulesResponseTypeDef](./type_defs.md#listratebasedrulesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef](./type_defs.md#listratebasedrulesrequestlistratebasedrulespaginatetypedef) 
## ListRegexMatchSetsPaginator

Type annotations and code completion for `#!python session.client("waf").get_paginator("list_regex_match_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRegexMatchSets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_waf.paginator import ListRegexMatchSetsPaginator

session = Session()

session = get_session()
async with session.client("waf") as client:  # (1)
    paginator: ListRegexMatchSetsPaginator = client.get_paginator("list_regex_match_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListRegexMatchSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListRegexMatchSetsPaginator](./paginators.md#listregexmatchsetspaginator)
3. item: [:material-code-braces: ListRegexMatchSetsResponseTypeDef](./type_defs.md#listregexmatchsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRegexMatchSetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRegexMatchSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRegexMatchSetsResponseTypeDef](./type_defs.md#listregexmatchsetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef](./type_defs.md#listregexmatchsetsrequestlistregexmatchsetspaginatetypedef) 
## ListRegexPatternSetsPaginator

Type annotations and code completion for `#!python session.client("waf").get_paginator("list_regex_pattern_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRegexPatternSets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_waf.paginator import ListRegexPatternSetsPaginator

session = Session()

session = get_session()
async with session.client("waf") as client:  # (1)
    paginator: ListRegexPatternSetsPaginator = client.get_paginator("list_regex_pattern_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListRegexPatternSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListRegexPatternSetsPaginator](./paginators.md#listregexpatternsetspaginator)
3. item: [:material-code-braces: ListRegexPatternSetsResponseTypeDef](./type_defs.md#listregexpatternsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRegexPatternSetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRegexPatternSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRegexPatternSetsResponseTypeDef](./type_defs.md#listregexpatternsetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef](./type_defs.md#listregexpatternsetsrequestlistregexpatternsetspaginatetypedef) 
## ListRuleGroupsPaginator

Type annotations and code completion for `#!python session.client("waf").get_paginator("list_rule_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRuleGroups)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_waf.paginator import ListRuleGroupsPaginator

session = Session()

session = get_session()
async with session.client("waf") as client:  # (1)
    paginator: ListRuleGroupsPaginator = client.get_paginator("list_rule_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListRuleGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListRuleGroupsPaginator](./paginators.md#listrulegroupspaginator)
3. item: [:material-code-braces: ListRuleGroupsResponseTypeDef](./type_defs.md#listrulegroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRuleGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRuleGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRuleGroupsResponseTypeDef](./type_defs.md#listrulegroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRuleGroupsRequestListRuleGroupsPaginateTypeDef](./type_defs.md#listrulegroupsrequestlistrulegroupspaginatetypedef) 
## ListRulesPaginator

Type annotations and code completion for `#!python session.client("waf").get_paginator("list_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRules)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_waf.paginator import ListRulesPaginator

session = Session()

session = get_session()
async with session.client("waf") as client:  # (1)
    paginator: ListRulesPaginator = client.get_paginator("list_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListRulesPaginator](./paginators.md#listrulespaginator)
3. item: [:material-code-braces: ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRulesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRulesRequestListRulesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRulesRequestListRulesPaginateTypeDef](./type_defs.md#listrulesrequestlistrulespaginatetypedef) 
## ListSizeConstraintSetsPaginator

Type annotations and code completion for `#!python session.client("waf").get_paginator("list_size_constraint_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSizeConstraintSets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_waf.paginator import ListSizeConstraintSetsPaginator

session = Session()

session = get_session()
async with session.client("waf") as client:  # (1)
    paginator: ListSizeConstraintSetsPaginator = client.get_paginator("list_size_constraint_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListSizeConstraintSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListSizeConstraintSetsPaginator](./paginators.md#listsizeconstraintsetspaginator)
3. item: [:material-code-braces: ListSizeConstraintSetsResponseTypeDef](./type_defs.md#listsizeconstraintsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSizeConstraintSetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSizeConstraintSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSizeConstraintSetsResponseTypeDef](./type_defs.md#listsizeconstraintsetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef](./type_defs.md#listsizeconstraintsetsrequestlistsizeconstraintsetspaginatetypedef) 
## ListSqlInjectionMatchSetsPaginator

Type annotations and code completion for `#!python session.client("waf").get_paginator("list_sql_injection_match_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSqlInjectionMatchSets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_waf.paginator import ListSqlInjectionMatchSetsPaginator

session = Session()

session = get_session()
async with session.client("waf") as client:  # (1)
    paginator: ListSqlInjectionMatchSetsPaginator = client.get_paginator("list_sql_injection_match_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListSqlInjectionMatchSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListSqlInjectionMatchSetsPaginator](./paginators.md#listsqlinjectionmatchsetspaginator)
3. item: [:material-code-braces: ListSqlInjectionMatchSetsResponseTypeDef](./type_defs.md#listsqlinjectionmatchsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSqlInjectionMatchSetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSqlInjectionMatchSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSqlInjectionMatchSetsResponseTypeDef](./type_defs.md#listsqlinjectionmatchsetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef](./type_defs.md#listsqlinjectionmatchsetsrequestlistsqlinjectionmatchsetspaginatetypedef) 
## ListSubscribedRuleGroupsPaginator

Type annotations and code completion for `#!python session.client("waf").get_paginator("list_subscribed_rule_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSubscribedRuleGroups)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_waf.paginator import ListSubscribedRuleGroupsPaginator

session = Session()

session = get_session()
async with session.client("waf") as client:  # (1)
    paginator: ListSubscribedRuleGroupsPaginator = client.get_paginator("list_subscribed_rule_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListSubscribedRuleGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListSubscribedRuleGroupsPaginator](./paginators.md#listsubscribedrulegroupspaginator)
3. item: [:material-code-braces: ListSubscribedRuleGroupsResponseTypeDef](./type_defs.md#listsubscribedrulegroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSubscribedRuleGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSubscribedRuleGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSubscribedRuleGroupsResponseTypeDef](./type_defs.md#listsubscribedrulegroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef](./type_defs.md#listsubscribedrulegroupsrequestlistsubscribedrulegroupspaginatetypedef) 
## ListWebACLsPaginator

Type annotations and code completion for `#!python session.client("waf").get_paginator("list_web_acls")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListWebACLs)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_waf.paginator import ListWebACLsPaginator

session = Session()

session = get_session()
async with session.client("waf") as client:  # (1)
    paginator: ListWebACLsPaginator = client.get_paginator("list_web_acls")  # (2)
    async for item in paginator.paginate(...):
        item: ListWebACLsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListWebACLsPaginator](./paginators.md#listwebaclspaginator)
3. item: [:material-code-braces: ListWebACLsResponseTypeDef](./type_defs.md#listwebaclsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWebACLsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListWebACLsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWebACLsResponseTypeDef](./type_defs.md#listwebaclsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListWebACLsRequestListWebACLsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWebACLsRequestListWebACLsPaginateTypeDef](./type_defs.md#listwebaclsrequestlistwebaclspaginatetypedef) 
## ListXssMatchSetsPaginator

Type annotations and code completion for `#!python session.client("waf").get_paginator("list_xss_match_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListXssMatchSets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_waf.paginator import ListXssMatchSetsPaginator

session = Session()

session = get_session()
async with session.client("waf") as client:  # (1)
    paginator: ListXssMatchSetsPaginator = client.get_paginator("list_xss_match_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListXssMatchSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [ListXssMatchSetsPaginator](./paginators.md#listxssmatchsetspaginator)
3. item: [:material-code-braces: ListXssMatchSetsResponseTypeDef](./type_defs.md#listxssmatchsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListXssMatchSetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListXssMatchSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListXssMatchSetsResponseTypeDef](./type_defs.md#listxssmatchsetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef](./type_defs.md#listxssmatchsetsrequestlistxssmatchsetspaginatetypedef) 
