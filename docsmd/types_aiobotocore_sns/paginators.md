# Paginators

> [Index](../README.md) > [SNS](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SNS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
    type annotations stubs module [types-aiobotocore-sns](https://pypi.org/project/types-aiobotocore-sns/).

## ListEndpointsByPlatformApplicationPaginator

Type annotations and code completion for `#!python session.client("sns").get_paginator("list_endpoints_by_platform_application")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListEndpointsByPlatformApplication)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sns.paginator import ListEndpointsByPlatformApplicationPaginator

session = Session()

session = get_session()
async with session.client("sns") as client:  # (1)
    paginator: ListEndpointsByPlatformApplicationPaginator = client.get_paginator("list_endpoints_by_platform_application")  # (2)
    async for item in paginator.paginate(...):
        item: ListEndpointsByPlatformApplicationResponseTypeDef
        print(item)  # (3)
```

1. client: [SNSClient](./client.md)
2. paginator: [ListEndpointsByPlatformApplicationPaginator](./paginators.md#listendpointsbyplatformapplicationpaginator)
3. item: [:material-code-braces: ListEndpointsByPlatformApplicationResponseTypeDef](./type_defs.md#listendpointsbyplatformapplicationresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEndpointsByPlatformApplicationPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PlatformApplicationArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEndpointsByPlatformApplicationResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEndpointsByPlatformApplicationResponseTypeDef](./type_defs.md#listendpointsbyplatformapplicationresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef = {  # (1)
    "PlatformApplicationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef](./type_defs.md#listendpointsbyplatformapplicationinputlistendpointsbyplatformapplicationpaginatetypedef) 
## ListOriginationNumbersPaginator

Type annotations and code completion for `#!python session.client("sns").get_paginator("list_origination_numbers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListOriginationNumbers)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sns.paginator import ListOriginationNumbersPaginator

session = Session()

session = get_session()
async with session.client("sns") as client:  # (1)
    paginator: ListOriginationNumbersPaginator = client.get_paginator("list_origination_numbers")  # (2)
    async for item in paginator.paginate(...):
        item: ListOriginationNumbersResultTypeDef
        print(item)  # (3)
```

1. client: [SNSClient](./client.md)
2. paginator: [ListOriginationNumbersPaginator](./paginators.md#listoriginationnumberspaginator)
3. item: [:material-code-braces: ListOriginationNumbersResultTypeDef](./type_defs.md#listoriginationnumbersresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListOriginationNumbersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListOriginationNumbersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOriginationNumbersResultTypeDef](./type_defs.md#listoriginationnumbersresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef](./type_defs.md#listoriginationnumbersrequestlistoriginationnumberspaginatetypedef) 
## ListPhoneNumbersOptedOutPaginator

Type annotations and code completion for `#!python session.client("sns").get_paginator("list_phone_numbers_opted_out")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListPhoneNumbersOptedOut)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sns.paginator import ListPhoneNumbersOptedOutPaginator

session = Session()

session = get_session()
async with session.client("sns") as client:  # (1)
    paginator: ListPhoneNumbersOptedOutPaginator = client.get_paginator("list_phone_numbers_opted_out")  # (2)
    async for item in paginator.paginate(...):
        item: ListPhoneNumbersOptedOutResponseTypeDef
        print(item)  # (3)
```

1. client: [SNSClient](./client.md)
2. paginator: [ListPhoneNumbersOptedOutPaginator](./paginators.md#listphonenumbersoptedoutpaginator)
3. item: [:material-code-braces: ListPhoneNumbersOptedOutResponseTypeDef](./type_defs.md#listphonenumbersoptedoutresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPhoneNumbersOptedOutPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPhoneNumbersOptedOutResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPhoneNumbersOptedOutResponseTypeDef](./type_defs.md#listphonenumbersoptedoutresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef](./type_defs.md#listphonenumbersoptedoutinputlistphonenumbersoptedoutpaginatetypedef) 
## ListPlatformApplicationsPaginator

Type annotations and code completion for `#!python session.client("sns").get_paginator("list_platform_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListPlatformApplications)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sns.paginator import ListPlatformApplicationsPaginator

session = Session()

session = get_session()
async with session.client("sns") as client:  # (1)
    paginator: ListPlatformApplicationsPaginator = client.get_paginator("list_platform_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListPlatformApplicationsResponseTypeDef
        print(item)  # (3)
```

1. client: [SNSClient](./client.md)
2. paginator: [ListPlatformApplicationsPaginator](./paginators.md#listplatformapplicationspaginator)
3. item: [:material-code-braces: ListPlatformApplicationsResponseTypeDef](./type_defs.md#listplatformapplicationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPlatformApplicationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPlatformApplicationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPlatformApplicationsResponseTypeDef](./type_defs.md#listplatformapplicationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef](./type_defs.md#listplatformapplicationsinputlistplatformapplicationspaginatetypedef) 
## ListSMSSandboxPhoneNumbersPaginator

Type annotations and code completion for `#!python session.client("sns").get_paginator("list_sms_sandbox_phone_numbers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSMSSandboxPhoneNumbers)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sns.paginator import ListSMSSandboxPhoneNumbersPaginator

session = Session()

session = get_session()
async with session.client("sns") as client:  # (1)
    paginator: ListSMSSandboxPhoneNumbersPaginator = client.get_paginator("list_sms_sandbox_phone_numbers")  # (2)
    async for item in paginator.paginate(...):
        item: ListSMSSandboxPhoneNumbersResultTypeDef
        print(item)  # (3)
```

1. client: [SNSClient](./client.md)
2. paginator: [ListSMSSandboxPhoneNumbersPaginator](./paginators.md#listsmssandboxphonenumberspaginator)
3. item: [:material-code-braces: ListSMSSandboxPhoneNumbersResultTypeDef](./type_defs.md#listsmssandboxphonenumbersresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListSMSSandboxPhoneNumbersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSMSSandboxPhoneNumbersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSMSSandboxPhoneNumbersResultTypeDef](./type_defs.md#listsmssandboxphonenumbersresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef](./type_defs.md#listsmssandboxphonenumbersinputlistsmssandboxphonenumberspaginatetypedef) 
## ListSubscriptionsPaginator

Type annotations and code completion for `#!python session.client("sns").get_paginator("list_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSubscriptions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sns.paginator import ListSubscriptionsPaginator

session = Session()

session = get_session()
async with session.client("sns") as client:  # (1)
    paginator: ListSubscriptionsPaginator = client.get_paginator("list_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSubscriptionsResponseTypeDef
        print(item)  # (3)
```

1. client: [SNSClient](./client.md)
2. paginator: [ListSubscriptionsPaginator](./paginators.md#listsubscriptionspaginator)
3. item: [:material-code-braces: ListSubscriptionsResponseTypeDef](./type_defs.md#listsubscriptionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSubscriptionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSubscriptionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSubscriptionsResponseTypeDef](./type_defs.md#listsubscriptionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSubscriptionsInputListSubscriptionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSubscriptionsInputListSubscriptionsPaginateTypeDef](./type_defs.md#listsubscriptionsinputlistsubscriptionspaginatetypedef) 
## ListSubscriptionsByTopicPaginator

Type annotations and code completion for `#!python session.client("sns").get_paginator("list_subscriptions_by_topic")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSubscriptionsByTopic)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sns.paginator import ListSubscriptionsByTopicPaginator

session = Session()

session = get_session()
async with session.client("sns") as client:  # (1)
    paginator: ListSubscriptionsByTopicPaginator = client.get_paginator("list_subscriptions_by_topic")  # (2)
    async for item in paginator.paginate(...):
        item: ListSubscriptionsByTopicResponseTypeDef
        print(item)  # (3)
```

1. client: [SNSClient](./client.md)
2. paginator: [ListSubscriptionsByTopicPaginator](./paginators.md#listsubscriptionsbytopicpaginator)
3. item: [:material-code-braces: ListSubscriptionsByTopicResponseTypeDef](./type_defs.md#listsubscriptionsbytopicresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSubscriptionsByTopicPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TopicArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSubscriptionsByTopicResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSubscriptionsByTopicResponseTypeDef](./type_defs.md#listsubscriptionsbytopicresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef = {  # (1)
    "TopicArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef](./type_defs.md#listsubscriptionsbytopicinputlistsubscriptionsbytopicpaginatetypedef) 
## ListTopicsPaginator

Type annotations and code completion for `#!python session.client("sns").get_paginator("list_topics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListTopics)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sns.paginator import ListTopicsPaginator

session = Session()

session = get_session()
async with session.client("sns") as client:  # (1)
    paginator: ListTopicsPaginator = client.get_paginator("list_topics")  # (2)
    async for item in paginator.paginate(...):
        item: ListTopicsResponseTypeDef
        print(item)  # (3)
```

1. client: [SNSClient](./client.md)
2. paginator: [ListTopicsPaginator](./paginators.md#listtopicspaginator)
3. item: [:material-code-braces: ListTopicsResponseTypeDef](./type_defs.md#listtopicsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTopicsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTopicsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTopicsResponseTypeDef](./type_defs.md#listtopicsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTopicsInputListTopicsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTopicsInputListTopicsPaginateTypeDef](./type_defs.md#listtopicsinputlisttopicspaginatetypedef) 
