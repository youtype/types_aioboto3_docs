# LocationServiceMapsV2 module

> [Index](../README.md) > LocationServiceMapsV2


!!! note ""

    Auto-generated documentation for [LocationServiceMapsV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-maps.html#locationservicemapsv2)
    type annotations stubs module [types-aiobotocore-geo-maps](https://pypi.org/project/types-aiobotocore-geo-maps/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `LocationServiceMapsV2` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `LocationServiceMapsV2` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[geo-maps]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[geo-maps]'

# standalone installation
python -m pip install types-aiobotocore-geo-maps
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-geo-maps
```

## Usage

Code samples can be found in [Examples](./usage.md).

## LocationServiceMapsV2Client

Type annotations and code completion for  `#!python session.client("geo-maps")` as [LocationServiceMapsV2Client](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-maps.html#LocationServiceMapsV2.Client)

```python
# LocationServiceMapsV2Client usage example

from aioboto3.session import Session

from types_aiobotocore_geo_maps.client import LocationServiceMapsV2Client


session = Session()
async with session.client("geo-maps") as client:
    client: LocationServiceMapsV2Client
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ColorSchemeType usage example

from types_aiobotocore_geo_maps.literals import ColorSchemeType

def get_value() -> ColorSchemeType:
    return "Dark"
```

- [ColorSchemeType](./literals.md#colorschemetype)
- [MapStyleType](./literals.md#mapstyletype)
- [ScaleBarUnitType](./literals.md#scalebarunittype)
- [StaticMapStyleType](./literals.md#staticmapstyletype)
- [VariantType](./literals.md#varianttype)
- [LocationServiceMapsV2ServiceName](./literals.md#locationservicemapsv2servicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [GetGlyphsRequestRequestTypeDef](./type_defs.md#getglyphsrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetSpritesRequestRequestTypeDef](./type_defs.md#getspritesrequestrequesttypedef)
- [GetStaticMapRequestRequestTypeDef](./type_defs.md#getstaticmaprequestrequesttypedef)
- [GetStyleDescriptorRequestRequestTypeDef](./type_defs.md#getstyledescriptorrequestrequesttypedef)
- [GetTileRequestRequestTypeDef](./type_defs.md#gettilerequestrequesttypedef)
- [GetGlyphsResponseTypeDef](./type_defs.md#getglyphsresponsetypedef)
- [GetSpritesResponseTypeDef](./type_defs.md#getspritesresponsetypedef)
- [GetStaticMapResponseTypeDef](./type_defs.md#getstaticmapresponsetypedef)
- [GetStyleDescriptorResponseTypeDef](./type_defs.md#getstyledescriptorresponsetypedef)
- [GetTileResponseTypeDef](./type_defs.md#gettileresponsetypedef)
