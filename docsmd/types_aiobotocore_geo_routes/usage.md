# Examples

> [Index](../README.md) > [LocationServiceRoutesV2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LocationServiceRoutesV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-routes.html#locationserviceroutesv2)
    type annotations stubs module [types-aiobotocore-geo-routes](https://pypi.org/project/types-aiobotocore-geo-routes/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[geo-routes]` package installed.

Write your `LocationServiceRoutesV2` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# LocationServiceRoutesV2Client usage example

from aioboto3.session import Session


session = Session()

async with session.client("geo-routes") as client:  # (1)
    result = await client.calculate_isolines()  # (2)
```

1. client: [LocationServiceRoutesV2Client](./client.md)
2. result: [:material-code-braces: CalculateIsolinesResponseTypeDef](./type_defs.md#calculateisolinesresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[geo-routes]`
or a standalone `types_aiobotocore_geo_routes` package, you have to explicitly specify
`client: LocationServiceRoutesV2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# LocationServiceRoutesV2Client usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_geo_routes.client import LocationServiceRoutesV2Client
from types_aiobotocore_geo_routes.type_defs import CalculateIsolinesResponseTypeDef
from types_aiobotocore_geo_routes.type_defs import CalculateIsolinesRequestTypeDef


session = Session()

client: LocationServiceRoutesV2Client
async with session.client("geo-routes") as client:  # (1)
    kwargs: CalculateIsolinesRequestTypeDef = {...}  # (2)
    result: CalculateIsolinesResponseTypeDef = await client.calculate_isolines(**kwargs)  # (3)
```

1. client: [LocationServiceRoutesV2Client](./client.md)
2. kwargs: [:material-code-braces: CalculateIsolinesRequestTypeDef](./type_defs.md#calculateisolinesrequesttypedef)
3. result: [:material-code-braces: CalculateIsolinesResponseTypeDef](./type_defs.md#calculateisolinesresponsetypedef)






