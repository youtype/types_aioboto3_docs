# InspectorscanClient

> [Index](../README.md) > [Inspectorscan](./README.md) > InspectorscanClient

!!! note ""

    Auto-generated documentation for [Inspectorscan](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan.html#inspectorscan)
    type annotations stubs module [types-aiobotocore-inspector-scan](https://pypi.org/project/types-aiobotocore-inspector-scan/).

## InspectorscanClient

Type annotations and code completion for `#!python session.client("inspector-scan")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan.html#Inspectorscan.Client)

```python
# InspectorscanClient usage example

from aioboto3.session import Session
from types_aiobotocore_inspector_scan.client import InspectorscanClient

session = Session()
async with session.client("inspector-scan") as client:
    client: InspectorscanClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("inspector-scan").exceptions` structure.

```python
# InspectorscanClient.exceptions usage example

async with session.client("inspector-scan") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.InternalServerException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# InspectorscanClient.exceptions type checking example

from types_aiobotocore_inspector_scan.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("inspector-scan").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan.html#Inspectorscan.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("inspector-scan").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan.html#Inspectorscan.Client)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### scan\_sbom

Scans a provided CycloneDX 1.5 SBOM and reports on any vulnerabilities
discovered in that SBOM.

Type annotations and code completion for `#!python session.client("inspector-scan").scan_sbom` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan.html#Inspectorscan.Client)

```python
# scan_sbom method definition

await def scan_sbom(
    self,
    *,
    sbom: Mapping[str, Any],
    outputFormat: OutputFormatType = ...,  # (1)
) -> ScanSbomResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype)
2. See [:material-code-braces: ScanSbomResponseTypeDef](./type_defs.md#scansbomresponsetypedef)


```python
# scan_sbom method usage example with argument unpacking

kwargs: ScanSbomRequestTypeDef = {  # (1)
    "sbom": ...,
}

parent.scan_sbom(**kwargs)
```

1. See [:material-code-braces: ScanSbomRequestTypeDef](./type_defs.md#scansbomrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("inspector-scan").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan.html#Inspectorscan.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("inspector-scan").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan.html#Inspectorscan.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```





