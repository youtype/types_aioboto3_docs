# Examples

> [Index](../README.md) > [LocationServiceMapsV2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LocationServiceMapsV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-maps.html#locationservicemapsv2)
    type annotations stubs module [types-aiobotocore-geo-maps](https://pypi.org/project/types-aiobotocore-geo-maps/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[geo-maps]` package installed.

Write your `LocationServiceMapsV2` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# LocationServiceMapsV2Client usage example

from aioboto3.session import Session


session = Session()

async with session.client("geo-maps") as client:  # (1)
    result = await client.get_glyphs()  # (2)
```

1. client: [LocationServiceMapsV2Client](./client.md)
2. result: [:material-code-braces: GetGlyphsResponseTypeDef](./type_defs.md#getglyphsresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[geo-maps]`
or a standalone `types_aiobotocore_geo_maps` package, you have to explicitly specify
`client: LocationServiceMapsV2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# LocationServiceMapsV2Client usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_geo_maps.client import LocationServiceMapsV2Client
from types_aiobotocore_geo_maps.type_defs import GetGlyphsResponseTypeDef
from types_aiobotocore_geo_maps.type_defs import GetGlyphsRequestTypeDef


session = Session()

client: LocationServiceMapsV2Client
async with session.client("geo-maps") as client:  # (1)
    kwargs: GetGlyphsRequestTypeDef = {...}  # (2)
    result: GetGlyphsResponseTypeDef = await client.get_glyphs(**kwargs)  # (3)
```

1. client: [LocationServiceMapsV2Client](./client.md)
2. kwargs: [:material-code-braces: GetGlyphsRequestTypeDef](./type_defs.md#getglyphsrequesttypedef)
3. result: [:material-code-braces: GetGlyphsResponseTypeDef](./type_defs.md#getglyphsresponsetypedef)






