# ImportExportClient

> [Index](../README.md) > [ImportExport](./README.md) > ImportExportClient

!!! note ""

    Auto-generated documentation for [ImportExport](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#importexport)
    type annotations stubs module [types-aiobotocore-importexport](https://pypi.org/project/types-aiobotocore-importexport/).

## ImportExportClient

Type annotations and code completion for `#!python session.client("importexport")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client)

```python
# ImportExportClient usage example

from aioboto3.session import Session
from types_aiobotocore_importexport.client import ImportExportClient

session = Session()
async with session.client("importexport") as client:
    client: ImportExportClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("importexport").exceptions` structure.

```python
# ImportExportClient.exceptions usage example

async with session.client("importexport") as client:
    try:
        do_something(client)
    except (
            client.exceptions.BucketPermissionException,
        client.exceptions.CanceledJobIdException,
        client.exceptions.ClientError,
        client.exceptions.CreateJobQuotaExceededException,
        client.exceptions.ExpiredJobIdException,
        client.exceptions.InvalidAccessKeyIdException,
        client.exceptions.InvalidAddressException,
        client.exceptions.InvalidCustomsException,
        client.exceptions.InvalidFileSystemException,
        client.exceptions.InvalidJobIdException,
        client.exceptions.InvalidManifestFieldException,
        client.exceptions.InvalidParameterException,
        client.exceptions.InvalidVersionException,
        client.exceptions.MalformedManifestException,
        client.exceptions.MissingCustomsException,
        client.exceptions.MissingManifestFieldException,
        client.exceptions.MissingParameterException,
        client.exceptions.MultipleRegionsException,
        client.exceptions.NoSuchBucketException,
        client.exceptions.UnableToCancelJobIdException,
        client.exceptions.UnableToUpdateJobIdException,
    ) as e:
        print(e)
```

```python
# ImportExportClient.exceptions type checking example

from types_aiobotocore_importexport.client import Exceptions

def handle_error(exc: Exceptions.BucketPermissionException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("importexport").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("importexport").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client)

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


### cancel\_job

This operation cancels a specified job.

Type annotations and code completion for `#!python session.client("importexport").cancel_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client)

```python
# cancel_job method definition

await def cancel_job(
    self,
    *,
    JobId: str,
    APIVersion: str = ...,
) -> CancelJobOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelJobOutputTypeDef](./type_defs.md#canceljoboutputtypedef)


```python
# cancel_job method usage example with argument unpacking

kwargs: CancelJobInputTypeDef = {  # (1)
    "JobId": ...,
}

parent.cancel_job(**kwargs)
```

1. See [:material-code-braces: CancelJobInputTypeDef](./type_defs.md#canceljobinputtypedef)

### create\_job

This operation initiates the process of scheduling an upload or download of
your data.

Type annotations and code completion for `#!python session.client("importexport").create_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client)

```python
# create_job method definition

await def create_job(
    self,
    *,
    JobType: JobTypeType,  # (1)
    Manifest: str,
    ValidateOnly: bool,
    ManifestAddendum: str = ...,
    APIVersion: str = ...,
) -> CreateJobOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype)
2. See [:material-code-braces: CreateJobOutputTypeDef](./type_defs.md#createjoboutputtypedef)


```python
# create_job method usage example with argument unpacking

kwargs: CreateJobInputTypeDef = {  # (1)
    "JobType": ...,
    "Manifest": ...,
    "ValidateOnly": ...,
}

parent.create_job(**kwargs)
```

1. See [:material-code-braces: CreateJobInputTypeDef](./type_defs.md#createjobinputtypedef)

### get\_shipping\_label

This operation generates a pre-paid UPS shipping label that you will use to
ship your device to AWS for processing.

Type annotations and code completion for `#!python session.client("importexport").get_shipping_label` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client)

```python
# get_shipping_label method definition

await def get_shipping_label(
    self,
    *,
    jobIds: Sequence[str],
    name: str = ...,
    company: str = ...,
    phoneNumber: str = ...,
    country: str = ...,
    stateOrProvince: str = ...,
    city: str = ...,
    postalCode: str = ...,
    street1: str = ...,
    street2: str = ...,
    street3: str = ...,
    APIVersion: str = ...,
) -> GetShippingLabelOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetShippingLabelOutputTypeDef](./type_defs.md#getshippinglabeloutputtypedef)


```python
# get_shipping_label method usage example with argument unpacking

kwargs: GetShippingLabelInputTypeDef = {  # (1)
    "jobIds": ...,
}

parent.get_shipping_label(**kwargs)
```

1. See [:material-code-braces: GetShippingLabelInputTypeDef](./type_defs.md#getshippinglabelinputtypedef)

### get\_status

This operation returns information about a job, including where the job is in
the processing pipeline, the status of the results, and the signature value
associated with the job.

Type annotations and code completion for `#!python session.client("importexport").get_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client)

```python
# get_status method definition

await def get_status(
    self,
    *,
    JobId: str,
    APIVersion: str = ...,
) -> GetStatusOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStatusOutputTypeDef](./type_defs.md#getstatusoutputtypedef)


```python
# get_status method usage example with argument unpacking

kwargs: GetStatusInputTypeDef = {  # (1)
    "JobId": ...,
}

parent.get_status(**kwargs)
```

1. See [:material-code-braces: GetStatusInputTypeDef](./type_defs.md#getstatusinputtypedef)

### list\_jobs

This operation returns the jobs associated with the requester.

Type annotations and code completion for `#!python session.client("importexport").list_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client)

```python
# list_jobs method definition

await def list_jobs(
    self,
    *,
    MaxJobs: int = ...,
    Marker: str = ...,
    APIVersion: str = ...,
) -> ListJobsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListJobsOutputTypeDef](./type_defs.md#listjobsoutputtypedef)


```python
# list_jobs method usage example with argument unpacking

kwargs: ListJobsInputTypeDef = {  # (1)
    "MaxJobs": ...,
}

parent.list_jobs(**kwargs)
```

1. See [:material-code-braces: ListJobsInputTypeDef](./type_defs.md#listjobsinputtypedef)

### update\_job

You use this operation to change the parameters specified in the original
manifest file by supplying a new manifest file.

Type annotations and code completion for `#!python session.client("importexport").update_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client)

```python
# update_job method definition

await def update_job(
    self,
    *,
    JobId: str,
    Manifest: str,
    JobType: JobTypeType,  # (1)
    ValidateOnly: bool,
    APIVersion: str = ...,
) -> UpdateJobOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype)
2. See [:material-code-braces: UpdateJobOutputTypeDef](./type_defs.md#updatejoboutputtypedef)


```python
# update_job method usage example with argument unpacking

kwargs: UpdateJobInputTypeDef = {  # (1)
    "JobId": ...,
    "Manifest": ...,
    "JobType": ...,
    "ValidateOnly": ...,
}

parent.update_job(**kwargs)
```

1. See [:material-code-braces: UpdateJobInputTypeDef](./type_defs.md#updatejobinputtypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("importexport").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("importexport").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Client)

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




### get_paginator

Type annotations and code completion for `#!python session.client("importexport").get_paginator` method with overloads.

- `client.get_paginator("list_jobs")` -> [ListJobsPaginator](./paginators.md#listjobspaginator)



