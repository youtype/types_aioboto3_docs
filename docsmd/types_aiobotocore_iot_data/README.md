# IoTDataPlane module

> [Index](../README.md) > IoTDataPlane


!!! note ""

    Auto-generated documentation for [IoTDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#iotdataplane)
    type annotations stubs module [types-aiobotocore-iot-data](https://pypi.org/project/types-aiobotocore-iot-data/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==14.1.0' mypy-boto3-builder`
1. Select `aioboto3` AWS SDK.
1. Add `IoTDataPlane` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `IoTDataPlane` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[iot-data]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[iot-data]'

# standalone installation
python -m pip install types-aiobotocore-iot-data
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-iot-data
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IoTDataPlaneClient

Type annotations and code completion for  `#!python session.client("iot-data")` as [IoTDataPlaneClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client)

```python
# IoTDataPlaneClient usage example

from aioboto3.session import Session

from types_aiobotocore_iot_data.client import IoTDataPlaneClient


session = Session()
async with session.client("iot-data") as client:
    client: IoTDataPlaneClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("iot-data").get_paginator("...")`.

```python
# ListRetainedMessagesPaginator usage example

from types_aiobotocore_iot_data.paginator import ListRetainedMessagesPaginator

def get_list_retained_messages_paginator() -> ListRetainedMessagesPaginator:
    return client.get_paginator("list_retained_messages"))
```

- [ListRetainedMessagesPaginator](./paginators.md#listretainedmessagespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ListRetainedMessagesPaginatorName usage example

from types_aiobotocore_iot_data.literals import ListRetainedMessagesPaginatorName

def get_value() -> ListRetainedMessagesPaginatorName:
    return "list_retained_messages"
```

- [ListRetainedMessagesPaginatorName](./literals.md#listretainedmessagespaginatorname)
- [PayloadFormatIndicatorType](./literals.md#payloadformatindicatortype)
- [IoTDataPlaneServiceName](./literals.md#iotdataplaneservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BlobTypeDef](./type_defs.md#blobtypedef)
- [DeleteThingShadowRequestTypeDef](./type_defs.md#deletethingshadowrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetRetainedMessageRequestTypeDef](./type_defs.md#getretainedmessagerequesttypedef)
- [GetThingShadowRequestTypeDef](./type_defs.md#getthingshadowrequesttypedef)
- [ListNamedShadowsForThingRequestTypeDef](./type_defs.md#listnamedshadowsforthingrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListRetainedMessagesRequestTypeDef](./type_defs.md#listretainedmessagesrequesttypedef)
- [RetainedMessageSummaryTypeDef](./type_defs.md#retainedmessagesummarytypedef)
- [PublishRequestTypeDef](./type_defs.md#publishrequesttypedef)
- [UpdateThingShadowRequestTypeDef](./type_defs.md#updatethingshadowrequesttypedef)
- [DeleteThingShadowResponseTypeDef](./type_defs.md#deletethingshadowresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetRetainedMessageResponseTypeDef](./type_defs.md#getretainedmessageresponsetypedef)
- [GetThingShadowResponseTypeDef](./type_defs.md#getthingshadowresponsetypedef)
- [ListNamedShadowsForThingResponseTypeDef](./type_defs.md#listnamedshadowsforthingresponsetypedef)
- [UpdateThingShadowResponseTypeDef](./type_defs.md#updatethingshadowresponsetypedef)
- [ListRetainedMessagesRequestPaginateTypeDef](./type_defs.md#listretainedmessagesrequestpaginatetypedef)
- [ListRetainedMessagesResponseTypeDef](./type_defs.md#listretainedmessagesresponsetypedef)

