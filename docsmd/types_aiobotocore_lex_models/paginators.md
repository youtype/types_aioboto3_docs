# Paginators

> [Index](../README.md) > [LexModelBuildingService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [LexModelBuildingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
    type annotations stubs module [types-aiobotocore-lex-models](https://pypi.org/project/types-aiobotocore-lex-models/).

## GetBotAliasesPaginator

Type annotations and code completion for `#!python session.client("lex-models").get_paginator("get_bot_aliases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotAliases)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_lex_models.paginator import GetBotAliasesPaginator

session = Session()

session = get_session()
async with session.client("lex-models") as client:  # (1)
    paginator: GetBotAliasesPaginator = client.get_paginator("get_bot_aliases")  # (2)
    async for item in paginator.paginate(...):
        item: GetBotAliasesResponseTypeDef
        print(item)  # (3)
```

1. client: [LexModelBuildingServiceClient](./client.md)
2. paginator: [GetBotAliasesPaginator](./paginators.md#getbotaliasespaginator)
3. item: [:material-code-braces: GetBotAliasesResponseTypeDef](./type_defs.md#getbotaliasesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetBotAliasesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    botName: str,
    nameContains: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetBotAliasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetBotAliasesResponseTypeDef](./type_defs.md#getbotaliasesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetBotAliasesRequestGetBotAliasesPaginateTypeDef = {  # (1)
    "botName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetBotAliasesRequestGetBotAliasesPaginateTypeDef](./type_defs.md#getbotaliasesrequestgetbotaliasespaginatetypedef) 
## GetBotChannelAssociationsPaginator

Type annotations and code completion for `#!python session.client("lex-models").get_paginator("get_bot_channel_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotChannelAssociations)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_lex_models.paginator import GetBotChannelAssociationsPaginator

session = Session()

session = get_session()
async with session.client("lex-models") as client:  # (1)
    paginator: GetBotChannelAssociationsPaginator = client.get_paginator("get_bot_channel_associations")  # (2)
    async for item in paginator.paginate(...):
        item: GetBotChannelAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [LexModelBuildingServiceClient](./client.md)
2. paginator: [GetBotChannelAssociationsPaginator](./paginators.md#getbotchannelassociationspaginator)
3. item: [:material-code-braces: GetBotChannelAssociationsResponseTypeDef](./type_defs.md#getbotchannelassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetBotChannelAssociationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    botName: str,
    botAlias: str,
    nameContains: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetBotChannelAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetBotChannelAssociationsResponseTypeDef](./type_defs.md#getbotchannelassociationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = {  # (1)
    "botName": ...,
    "botAlias": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef](./type_defs.md#getbotchannelassociationsrequestgetbotchannelassociationspaginatetypedef) 
## GetBotVersionsPaginator

Type annotations and code completion for `#!python session.client("lex-models").get_paginator("get_bot_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotVersions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_lex_models.paginator import GetBotVersionsPaginator

session = Session()

session = get_session()
async with session.client("lex-models") as client:  # (1)
    paginator: GetBotVersionsPaginator = client.get_paginator("get_bot_versions")  # (2)
    async for item in paginator.paginate(...):
        item: GetBotVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [LexModelBuildingServiceClient](./client.md)
2. paginator: [GetBotVersionsPaginator](./paginators.md#getbotversionspaginator)
3. item: [:material-code-braces: GetBotVersionsResponseTypeDef](./type_defs.md#getbotversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetBotVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetBotVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetBotVersionsResponseTypeDef](./type_defs.md#getbotversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetBotVersionsRequestGetBotVersionsPaginateTypeDef = {  # (1)
    "name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetBotVersionsRequestGetBotVersionsPaginateTypeDef](./type_defs.md#getbotversionsrequestgetbotversionspaginatetypedef) 
## GetBotsPaginator

Type annotations and code completion for `#!python session.client("lex-models").get_paginator("get_bots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBots)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_lex_models.paginator import GetBotsPaginator

session = Session()

session = get_session()
async with session.client("lex-models") as client:  # (1)
    paginator: GetBotsPaginator = client.get_paginator("get_bots")  # (2)
    async for item in paginator.paginate(...):
        item: GetBotsResponseTypeDef
        print(item)  # (3)
```

1. client: [LexModelBuildingServiceClient](./client.md)
2. paginator: [GetBotsPaginator](./paginators.md#getbotspaginator)
3. item: [:material-code-braces: GetBotsResponseTypeDef](./type_defs.md#getbotsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetBotsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    nameContains: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetBotsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetBotsResponseTypeDef](./type_defs.md#getbotsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetBotsRequestGetBotsPaginateTypeDef = {  # (1)
    "nameContains": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetBotsRequestGetBotsPaginateTypeDef](./type_defs.md#getbotsrequestgetbotspaginatetypedef) 
## GetBuiltinIntentsPaginator

Type annotations and code completion for `#!python session.client("lex-models").get_paginator("get_builtin_intents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinIntents)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_lex_models.paginator import GetBuiltinIntentsPaginator

session = Session()

session = get_session()
async with session.client("lex-models") as client:  # (1)
    paginator: GetBuiltinIntentsPaginator = client.get_paginator("get_builtin_intents")  # (2)
    async for item in paginator.paginate(...):
        item: GetBuiltinIntentsResponseTypeDef
        print(item)  # (3)
```

1. client: [LexModelBuildingServiceClient](./client.md)
2. paginator: [GetBuiltinIntentsPaginator](./paginators.md#getbuiltinintentspaginator)
3. item: [:material-code-braces: GetBuiltinIntentsResponseTypeDef](./type_defs.md#getbuiltinintentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetBuiltinIntentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    locale: LocaleType = ...,  # (1)
    signatureContains: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetBuiltinIntentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetBuiltinIntentsResponseTypeDef](./type_defs.md#getbuiltinintentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef = {  # (1)
    "locale": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef](./type_defs.md#getbuiltinintentsrequestgetbuiltinintentspaginatetypedef) 
## GetBuiltinSlotTypesPaginator

Type annotations and code completion for `#!python session.client("lex-models").get_paginator("get_builtin_slot_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinSlotTypes)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_lex_models.paginator import GetBuiltinSlotTypesPaginator

session = Session()

session = get_session()
async with session.client("lex-models") as client:  # (1)
    paginator: GetBuiltinSlotTypesPaginator = client.get_paginator("get_builtin_slot_types")  # (2)
    async for item in paginator.paginate(...):
        item: GetBuiltinSlotTypesResponseTypeDef
        print(item)  # (3)
```

1. client: [LexModelBuildingServiceClient](./client.md)
2. paginator: [GetBuiltinSlotTypesPaginator](./paginators.md#getbuiltinslottypespaginator)
3. item: [:material-code-braces: GetBuiltinSlotTypesResponseTypeDef](./type_defs.md#getbuiltinslottypesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetBuiltinSlotTypesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    locale: LocaleType = ...,  # (1)
    signatureContains: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetBuiltinSlotTypesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetBuiltinSlotTypesResponseTypeDef](./type_defs.md#getbuiltinslottypesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef = {  # (1)
    "locale": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef](./type_defs.md#getbuiltinslottypesrequestgetbuiltinslottypespaginatetypedef) 
## GetIntentVersionsPaginator

Type annotations and code completion for `#!python session.client("lex-models").get_paginator("get_intent_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntentVersions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_lex_models.paginator import GetIntentVersionsPaginator

session = Session()

session = get_session()
async with session.client("lex-models") as client:  # (1)
    paginator: GetIntentVersionsPaginator = client.get_paginator("get_intent_versions")  # (2)
    async for item in paginator.paginate(...):
        item: GetIntentVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [LexModelBuildingServiceClient](./client.md)
2. paginator: [GetIntentVersionsPaginator](./paginators.md#getintentversionspaginator)
3. item: [:material-code-braces: GetIntentVersionsResponseTypeDef](./type_defs.md#getintentversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetIntentVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetIntentVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetIntentVersionsResponseTypeDef](./type_defs.md#getintentversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = {  # (1)
    "name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef](./type_defs.md#getintentversionsrequestgetintentversionspaginatetypedef) 
## GetIntentsPaginator

Type annotations and code completion for `#!python session.client("lex-models").get_paginator("get_intents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntents)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_lex_models.paginator import GetIntentsPaginator

session = Session()

session = get_session()
async with session.client("lex-models") as client:  # (1)
    paginator: GetIntentsPaginator = client.get_paginator("get_intents")  # (2)
    async for item in paginator.paginate(...):
        item: GetIntentsResponseTypeDef
        print(item)  # (3)
```

1. client: [LexModelBuildingServiceClient](./client.md)
2. paginator: [GetIntentsPaginator](./paginators.md#getintentspaginator)
3. item: [:material-code-braces: GetIntentsResponseTypeDef](./type_defs.md#getintentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetIntentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    nameContains: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetIntentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetIntentsResponseTypeDef](./type_defs.md#getintentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetIntentsRequestGetIntentsPaginateTypeDef = {  # (1)
    "nameContains": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetIntentsRequestGetIntentsPaginateTypeDef](./type_defs.md#getintentsrequestgetintentspaginatetypedef) 
## GetSlotTypeVersionsPaginator

Type annotations and code completion for `#!python session.client("lex-models").get_paginator("get_slot_type_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypeVersions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_lex_models.paginator import GetSlotTypeVersionsPaginator

session = Session()

session = get_session()
async with session.client("lex-models") as client:  # (1)
    paginator: GetSlotTypeVersionsPaginator = client.get_paginator("get_slot_type_versions")  # (2)
    async for item in paginator.paginate(...):
        item: GetSlotTypeVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [LexModelBuildingServiceClient](./client.md)
2. paginator: [GetSlotTypeVersionsPaginator](./paginators.md#getslottypeversionspaginator)
3. item: [:material-code-braces: GetSlotTypeVersionsResponseTypeDef](./type_defs.md#getslottypeversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetSlotTypeVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetSlotTypeVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetSlotTypeVersionsResponseTypeDef](./type_defs.md#getslottypeversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = {  # (1)
    "name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef](./type_defs.md#getslottypeversionsrequestgetslottypeversionspaginatetypedef) 
## GetSlotTypesPaginator

Type annotations and code completion for `#!python session.client("lex-models").get_paginator("get_slot_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypes)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_lex_models.paginator import GetSlotTypesPaginator

session = Session()

session = get_session()
async with session.client("lex-models") as client:  # (1)
    paginator: GetSlotTypesPaginator = client.get_paginator("get_slot_types")  # (2)
    async for item in paginator.paginate(...):
        item: GetSlotTypesResponseTypeDef
        print(item)  # (3)
```

1. client: [LexModelBuildingServiceClient](./client.md)
2. paginator: [GetSlotTypesPaginator](./paginators.md#getslottypespaginator)
3. item: [:material-code-braces: GetSlotTypesResponseTypeDef](./type_defs.md#getslottypesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetSlotTypesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    nameContains: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetSlotTypesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetSlotTypesResponseTypeDef](./type_defs.md#getslottypesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetSlotTypesRequestGetSlotTypesPaginateTypeDef = {  # (1)
    "nameContains": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetSlotTypesRequestGetSlotTypesPaginateTypeDef](./type_defs.md#getslottypesrequestgetslottypespaginatetypedef) 
