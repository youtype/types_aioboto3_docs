# Examples

> [Index](../README.md) > [DataAutomationforBedrock](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DataAutomationforBedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation.html#dataautomationforbedrock)
    type annotations stubs module [types-aiobotocore-bedrock-data-automation](https://pypi.org/project/types-aiobotocore-bedrock-data-automation/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[bedrock-data-automation]` package installed.

Write your `DataAutomationforBedrock` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# DataAutomationforBedrockClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("bedrock-data-automation") as client:  # (1)
    result = await client.create_blueprint()  # (2)
```

1. client: [DataAutomationforBedrockClient](./client.md)
2. result: [:material-code-braces: CreateBlueprintResponseTypeDef](./type_defs.md#createblueprintresponsetypedef)



#### Paginator usage example

```python
# ListBlueprintsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("bedrock-data-automation") as client:  # (1)
    paginator = client.get_paginator("list_blueprints")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DataAutomationforBedrockClient](./client.md)
2. paginator: [ListBlueprintsPaginator](./paginators.md#listblueprintspaginator)
3. item: [:material-code-braces: ListBlueprintsResponseTypeDef](./type_defs.md#listblueprintsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[bedrock-data-automation]`
or a standalone `types_aiobotocore_bedrock_data_automation` package, you have to explicitly specify
`client: DataAutomationforBedrockClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# DataAutomationforBedrockClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_bedrock_data_automation.client import DataAutomationforBedrockClient
from types_aiobotocore_bedrock_data_automation.type_defs import CreateBlueprintResponseTypeDef
from types_aiobotocore_bedrock_data_automation.type_defs import CreateBlueprintRequestTypeDef


session = Session()

client: DataAutomationforBedrockClient
async with session.client("bedrock-data-automation") as client:  # (1)
    kwargs: CreateBlueprintRequestTypeDef = {...}  # (2)
    result: CreateBlueprintResponseTypeDef = await client.create_blueprint(**kwargs)  # (3)
```

1. client: [DataAutomationforBedrockClient](./client.md)
2. kwargs: [:material-code-braces: CreateBlueprintRequestTypeDef](./type_defs.md#createblueprintrequesttypedef)
3. result: [:material-code-braces: CreateBlueprintResponseTypeDef](./type_defs.md#createblueprintresponsetypedef)



#### Paginator usage example

```python
# ListBlueprintsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_bedrock_data_automation.client import DataAutomationforBedrockClient
from types_aiobotocore_bedrock_data_automation.paginator import ListBlueprintsPaginator
from types_aiobotocore_bedrock_data_automation.type_defs import ListBlueprintsResponseTypeDef


session = Session()

client: DataAutomationforBedrockClient
async with session.client("bedrock-data-automation") as client:  # (1)
    paginator: ListBlueprintsPaginator = client.get_paginator("list_blueprints")  # (2)
    async for item in paginator.paginate(...):
        item: ListBlueprintsResponseTypeDef
        print(item)  # (3)
```

1. client: [DataAutomationforBedrockClient](./client.md)
2. paginator: [ListBlueprintsPaginator](./paginators.md#listblueprintspaginator)
3. item: [:material-code-braces: ListBlueprintsResponseTypeDef](./type_defs.md#listblueprintsresponsetypedef)




