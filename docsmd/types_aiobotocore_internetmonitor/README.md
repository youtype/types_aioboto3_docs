# CloudWatchInternetMonitor module

> [Index](../README.md) > CloudWatchInternetMonitor


!!! note ""

    Auto-generated documentation for [CloudWatchInternetMonitor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#cloudwatchinternetmonitor)
    type annotations stubs module [types-aiobotocore-internetmonitor](https://pypi.org/project/types-aiobotocore-internetmonitor/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `CloudWatchInternetMonitor` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `CloudWatchInternetMonitor` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[internetmonitor]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[internetmonitor]'

# standalone installation
python -m pip install types-aiobotocore-internetmonitor
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-internetmonitor
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CloudWatchInternetMonitorClient

Type annotations and code completion for  `#!python session.client("internetmonitor")` as [CloudWatchInternetMonitorClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# CloudWatchInternetMonitorClient usage example

from aioboto3.session import Session

from types_aiobotocore_internetmonitor.client import CloudWatchInternetMonitorClient


session = Session()
async with session.client("internetmonitor") as client:
    client: CloudWatchInternetMonitorClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("internetmonitor").get_paginator("...")`.

```python
# ListHealthEventsPaginator usage example

from types_aiobotocore_internetmonitor.paginator import ListHealthEventsPaginator

def get_list_health_events_paginator() -> ListHealthEventsPaginator:
    return client.get_paginator("list_health_events"))
```

- [ListHealthEventsPaginator](./paginators.md#listhealtheventspaginator)
- [ListInternetEventsPaginator](./paginators.md#listinterneteventspaginator)
- [ListMonitorsPaginator](./paginators.md#listmonitorspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# HealthEventImpactTypeType usage example

from types_aiobotocore_internetmonitor.literals import HealthEventImpactTypeType

def get_value() -> HealthEventImpactTypeType:
    return "AVAILABILITY"
```

- [HealthEventImpactTypeType](./literals.md#healtheventimpacttypetype)
- [HealthEventStatusType](./literals.md#healtheventstatustype)
- [InternetEventStatusType](./literals.md#interneteventstatustype)
- [InternetEventTypeType](./literals.md#interneteventtypetype)
- [ListHealthEventsPaginatorName](./literals.md#listhealtheventspaginatorname)
- [ListInternetEventsPaginatorName](./literals.md#listinterneteventspaginatorname)
- [ListMonitorsPaginatorName](./literals.md#listmonitorspaginatorname)
- [LocalHealthEventsConfigStatusType](./literals.md#localhealtheventsconfigstatustype)
- [LogDeliveryStatusType](./literals.md#logdeliverystatustype)
- [MonitorConfigStateType](./literals.md#monitorconfigstatetype)
- [MonitorProcessingStatusCodeType](./literals.md#monitorprocessingstatuscodetype)
- [OperatorType](./literals.md#operatortype)
- [QueryStatusType](./literals.md#querystatustype)
- [QueryTypeType](./literals.md#querytypetype)
- [TriangulationEventTypeType](./literals.md#triangulationeventtypetype)
- [CloudWatchInternetMonitorServiceName](./literals.md#cloudwatchinternetmonitorservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AvailabilityMeasurementTypeDef](./type_defs.md#availabilitymeasurementtypedef)
- [ClientLocationTypeDef](./type_defs.md#clientlocationtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteMonitorInputRequestTypeDef](./type_defs.md#deletemonitorinputrequesttypedef)
- [FilterParameterTypeDef](./type_defs.md#filterparametertypedef)
- [GetHealthEventInputRequestTypeDef](./type_defs.md#gethealtheventinputrequesttypedef)
- [GetInternetEventInputRequestTypeDef](./type_defs.md#getinterneteventinputrequesttypedef)
- [GetMonitorInputRequestTypeDef](./type_defs.md#getmonitorinputrequesttypedef)
- [GetQueryResultsInputRequestTypeDef](./type_defs.md#getqueryresultsinputrequesttypedef)
- [QueryFieldTypeDef](./type_defs.md#queryfieldtypedef)
- [GetQueryStatusInputRequestTypeDef](./type_defs.md#getquerystatusinputrequesttypedef)
- [LocalHealthEventsConfigTypeDef](./type_defs.md#localhealtheventsconfigtypedef)
- [S3ConfigTypeDef](./type_defs.md#s3configtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ListMonitorsInputRequestTypeDef](./type_defs.md#listmonitorsinputrequesttypedef)
- [MonitorTypeDef](./type_defs.md#monitortypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [NetworkTypeDef](./type_defs.md#networktypedef)
- [RoundTripTimeTypeDef](./type_defs.md#roundtriptimetypedef)
- [StopQueryInputRequestTypeDef](./type_defs.md#stopqueryinputrequesttypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [InternetEventSummaryTypeDef](./type_defs.md#interneteventsummarytypedef)
- [CreateMonitorOutputTypeDef](./type_defs.md#createmonitoroutputtypedef)
- [GetInternetEventOutputTypeDef](./type_defs.md#getinterneteventoutputtypedef)
- [GetQueryStatusOutputTypeDef](./type_defs.md#getquerystatusoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [StartQueryOutputTypeDef](./type_defs.md#startqueryoutputtypedef)
- [UpdateMonitorOutputTypeDef](./type_defs.md#updatemonitoroutputtypedef)
- [GetQueryResultsOutputTypeDef](./type_defs.md#getqueryresultsoutputtypedef)
- [HealthEventsConfigTypeDef](./type_defs.md#healtheventsconfigtypedef)
- [InternetMeasurementsLogDeliveryTypeDef](./type_defs.md#internetmeasurementslogdeliverytypedef)
- [ListMonitorsInputPaginateTypeDef](./type_defs.md#listmonitorsinputpaginatetypedef)
- [ListHealthEventsInputPaginateTypeDef](./type_defs.md#listhealtheventsinputpaginatetypedef)
- [ListHealthEventsInputRequestTypeDef](./type_defs.md#listhealtheventsinputrequesttypedef)
- [ListInternetEventsInputPaginateTypeDef](./type_defs.md#listinterneteventsinputpaginatetypedef)
- [ListInternetEventsInputRequestTypeDef](./type_defs.md#listinterneteventsinputrequesttypedef)
- [StartQueryInputRequestTypeDef](./type_defs.md#startqueryinputrequesttypedef)
- [ListMonitorsOutputTypeDef](./type_defs.md#listmonitorsoutputtypedef)
- [NetworkImpairmentTypeDef](./type_defs.md#networkimpairmenttypedef)
- [PerformanceMeasurementTypeDef](./type_defs.md#performancemeasurementtypedef)
- [ListInternetEventsOutputTypeDef](./type_defs.md#listinterneteventsoutputtypedef)
- [CreateMonitorInputRequestTypeDef](./type_defs.md#createmonitorinputrequesttypedef)
- [GetMonitorOutputTypeDef](./type_defs.md#getmonitoroutputtypedef)
- [UpdateMonitorInputRequestTypeDef](./type_defs.md#updatemonitorinputrequesttypedef)
- [InternetHealthTypeDef](./type_defs.md#internethealthtypedef)
- [ImpactedLocationTypeDef](./type_defs.md#impactedlocationtypedef)
- [GetHealthEventOutputTypeDef](./type_defs.md#gethealtheventoutputtypedef)
- [HealthEventTypeDef](./type_defs.md#healtheventtypedef)
- [ListHealthEventsOutputTypeDef](./type_defs.md#listhealtheventsoutputtypedef)
