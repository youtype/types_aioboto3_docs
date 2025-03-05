# Examples

> [Index](../README.md) > [IoTJobsDataPlane](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTJobsDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#iotjobsdataplane)
    type annotations stubs module [types-aiobotocore-iot-jobs-data](https://pypi.org/project/types-aiobotocore-iot-jobs-data/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[iot-jobs-data]` package installed.

Write your `IoTJobsDataPlane` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# IoTJobsDataPlaneClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("iot-jobs-data") as client:  # (1)
    result = await client.describe_job_execution()  # (2)
```

1. client: [IoTJobsDataPlaneClient](./client.md)
2. result: [:material-code-braces: DescribeJobExecutionResponseTypeDef](./type_defs.md#describejobexecutionresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[iot-jobs-data]`
or a standalone `types_aiobotocore_iot_jobs_data` package, you have to explicitly specify
`client: IoTJobsDataPlaneClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# IoTJobsDataPlaneClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_iot_jobs_data.client import IoTJobsDataPlaneClient
from types_aiobotocore_iot_jobs_data.type_defs import DescribeJobExecutionResponseTypeDef
from types_aiobotocore_iot_jobs_data.type_defs import DescribeJobExecutionRequestTypeDef


session = Session()

client: IoTJobsDataPlaneClient
async with session.client("iot-jobs-data") as client:  # (1)
    kwargs: DescribeJobExecutionRequestTypeDef = {...}  # (2)
    result: DescribeJobExecutionResponseTypeDef = await client.describe_job_execution(**kwargs)  # (3)
```

1. client: [IoTJobsDataPlaneClient](./client.md)
2. kwargs: [:material-code-braces: DescribeJobExecutionRequestTypeDef](./type_defs.md#describejobexecutionrequesttypedef)
3. result: [:material-code-braces: DescribeJobExecutionResponseTypeDef](./type_defs.md#describejobexecutionresponsetypedef)






