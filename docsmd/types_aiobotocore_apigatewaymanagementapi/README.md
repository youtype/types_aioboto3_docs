# ApiGatewayManagementApi module

> [Index](../README.md) > ApiGatewayManagementApi


!!! note ""

    Auto-generated documentation for [ApiGatewayManagementApi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#apigatewaymanagementapi)
    type annotations stubs module [types-aiobotocore-apigatewaymanagementapi](https://pypi.org/project/types-aiobotocore-apigatewaymanagementapi/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `ApiGatewayManagementApi` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `ApiGatewayManagementApi` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[apigatewaymanagementapi]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[apigatewaymanagementapi]'

# standalone installation
python -m pip install types-aiobotocore-apigatewaymanagementapi
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-apigatewaymanagementapi
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ApiGatewayManagementApiClient

Type annotations and code completion for  `#!python session.client("apigatewaymanagementapi")` as [ApiGatewayManagementApiClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client)

```python
# ApiGatewayManagementApiClient usage example

from aioboto3.session import Session

from types_aiobotocore_apigatewaymanagementapi.client import ApiGatewayManagementApiClient


session = Session()
async with session.client("apigatewaymanagementapi") as client:
    client: ApiGatewayManagementApiClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ApiGatewayManagementApiServiceName usage example

from types_aiobotocore_apigatewaymanagementapi.literals import ApiGatewayManagementApiServiceName

def get_value() -> ApiGatewayManagementApiServiceName:
    return "apigatewaymanagementapi"
```

- [ApiGatewayManagementApiServiceName](./literals.md#apigatewaymanagementapiservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BlobTypeDef](./type_defs.md#blobtypedef)
- [DeleteConnectionRequestRequestTypeDef](./type_defs.md#deleteconnectionrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetConnectionRequestRequestTypeDef](./type_defs.md#getconnectionrequestrequesttypedef)
- [IdentityTypeDef](./type_defs.md#identitytypedef)
- [PostToConnectionRequestRequestTypeDef](./type_defs.md#posttoconnectionrequestrequesttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetConnectionResponseTypeDef](./type_defs.md#getconnectionresponsetypedef)
