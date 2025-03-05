# PersonalizeEvents module

> [Index](../README.md) > PersonalizeEvents


!!! note ""

    Auto-generated documentation for [PersonalizeEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#personalizeevents)
    type annotations stubs module [types-aiobotocore-personalize-events](https://pypi.org/project/types-aiobotocore-personalize-events/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==14.1.0' mypy-boto3-builder`
1. Select `aioboto3` AWS SDK.
1. Add `PersonalizeEvents` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `PersonalizeEvents` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[personalize-events]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[personalize-events]'

# standalone installation
python -m pip install types-aiobotocore-personalize-events
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-personalize-events
```

## Usage

Code samples can be found in [Examples](./usage.md).

## PersonalizeEventsClient

Type annotations and code completion for  `#!python session.client("personalize-events")` as [PersonalizeEventsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client)

```python
# PersonalizeEventsClient usage example

from aioboto3.session import Session

from types_aiobotocore_personalize_events.client import PersonalizeEventsClient


session = Session()
async with session.client("personalize-events") as client:
    client: PersonalizeEventsClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# PersonalizeEventsServiceName usage example

from types_aiobotocore_personalize_events.literals import PersonalizeEventsServiceName

def get_value() -> PersonalizeEventsServiceName:
    return "personalize-events"
```

- [PersonalizeEventsServiceName](./literals.md#personalizeeventsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ActionTypeDef](./type_defs.md#actiontypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [MetricAttributionTypeDef](./type_defs.md#metricattributiontypedef)
- [ItemTypeDef](./type_defs.md#itemtypedef)
- [UserTypeDef](./type_defs.md#usertypedef)
- [ActionInteractionTypeDef](./type_defs.md#actioninteractiontypedef)
- [PutActionsRequestTypeDef](./type_defs.md#putactionsrequesttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [EventTypeDef](./type_defs.md#eventtypedef)
- [PutItemsRequestTypeDef](./type_defs.md#putitemsrequesttypedef)
- [PutUsersRequestTypeDef](./type_defs.md#putusersrequesttypedef)
- [PutActionInteractionsRequestTypeDef](./type_defs.md#putactioninteractionsrequesttypedef)
- [PutEventsRequestTypeDef](./type_defs.md#puteventsrequesttypedef)

