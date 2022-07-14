# Health module

> [Index](../README.md) > Health


!!! note ""

    Auto-generated documentation for [Health](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
    type annotations stubs module [types-aiobotocore-health](https://pypi.org/project/types-aiobotocore-health/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `Health`.

### From PyPI with pip

Install `types-aioboto3` for `Health` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[health]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[health]'


# standalone installation
python -m pip install types-aiobotocore-health
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-health
```

## Usage

Code samples can be found in [Examples](./usage.md).

## HealthClient

Type annotations and code completion for  `#!python session.client("health")` as [HealthClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_health.client import HealthClient


session = Session()
async with session.client("health") as client:
    client: HealthClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("health").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_health.paginator import DescribeAffectedAccountsForOrganizationPaginator

def get_describe_affected_accounts_for_organization_paginator() -> DescribeAffectedAccountsForOrganizationPaginator:
    return client.get_paginator("describe_affected_accounts_for_organization"))
```

- [DescribeAffectedAccountsForOrganizationPaginator](./paginators.md#describeaffectedaccountsfororganizationpaginator)
- [DescribeAffectedEntitiesPaginator](./paginators.md#describeaffectedentitiespaginator)
- [DescribeAffectedEntitiesForOrganizationPaginator](./paginators.md#describeaffectedentitiesfororganizationpaginator)
- [DescribeEventAggregatesPaginator](./paginators.md#describeeventaggregatespaginator)
- [DescribeEventTypesPaginator](./paginators.md#describeeventtypespaginator)
- [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
- [DescribeEventsForOrganizationPaginator](./paginators.md#describeeventsfororganizationpaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_health.literals import DescribeAffectedAccountsForOrganizationPaginatorName

def get_value() -> DescribeAffectedAccountsForOrganizationPaginatorName:
    return "describe_affected_accounts_for_organization"
```

- [DescribeAffectedAccountsForOrganizationPaginatorName](./literals.md#describeaffectedaccountsfororganizationpaginatorname)
- [DescribeAffectedEntitiesForOrganizationPaginatorName](./literals.md#describeaffectedentitiesfororganizationpaginatorname)
- [DescribeAffectedEntitiesPaginatorName](./literals.md#describeaffectedentitiespaginatorname)
- [DescribeEventAggregatesPaginatorName](./literals.md#describeeventaggregatespaginatorname)
- [DescribeEventTypesPaginatorName](./literals.md#describeeventtypespaginatorname)
- [DescribeEventsForOrganizationPaginatorName](./literals.md#describeeventsfororganizationpaginatorname)
- [DescribeEventsPaginatorName](./literals.md#describeeventspaginatorname)
- [entityStatusCodeType](./literals.md#entitystatuscodetype)
- [eventAggregateFieldType](./literals.md#eventaggregatefieldtype)
- [eventScopeCodeType](./literals.md#eventscopecodetype)
- [eventStatusCodeType](./literals.md#eventstatuscodetype)
- [eventTypeCategoryType](./literals.md#eventtypecategorytype)
- [HealthServiceName](./literals.md#healthservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_health.type_defs import AffectedEntityTypeDef

def get_value() -> AffectedEntityTypeDef:
    return {
        "entityArn": ...,
    }
```

- [AffectedEntityTypeDef](./type_defs.md#affectedentitytypedef)
- [DateTimeRangeTypeDef](./type_defs.md#datetimerangetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeAffectedAccountsForOrganizationRequestRequestTypeDef](./type_defs.md#describeaffectedaccountsfororganizationrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [EventAccountFilterTypeDef](./type_defs.md#eventaccountfiltertypedef)
- [OrganizationAffectedEntitiesErrorItemTypeDef](./type_defs.md#organizationaffectedentitieserroritemtypedef)
- [DescribeEntityAggregatesRequestRequestTypeDef](./type_defs.md#describeentityaggregatesrequestrequesttypedef)
- [EntityAggregateTypeDef](./type_defs.md#entityaggregatetypedef)
- [EventAggregateTypeDef](./type_defs.md#eventaggregatetypedef)
- [OrganizationEventDetailsErrorItemTypeDef](./type_defs.md#organizationeventdetailserroritemtypedef)
- [DescribeEventDetailsRequestRequestTypeDef](./type_defs.md#describeeventdetailsrequestrequesttypedef)
- [EventDetailsErrorItemTypeDef](./type_defs.md#eventdetailserroritemtypedef)
- [EventTypeFilterTypeDef](./type_defs.md#eventtypefiltertypedef)
- [EventTypeTypeDef](./type_defs.md#eventtypetypedef)
- [OrganizationEventTypeDef](./type_defs.md#organizationeventtypedef)
- [EventTypeDef](./type_defs.md#eventtypedef)
- [EventDescriptionTypeDef](./type_defs.md#eventdescriptiontypedef)
- [EntityFilterTypeDef](./type_defs.md#entityfiltertypedef)
- [EventFilterTypeDef](./type_defs.md#eventfiltertypedef)
- [OrganizationEventFilterTypeDef](./type_defs.md#organizationeventfiltertypedef)
- [DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef](./type_defs.md#describeaffectedaccountsfororganizationrequestdescribeaffectedaccountsfororganizationpaginatetypedef)
- [DescribeAffectedAccountsForOrganizationResponseTypeDef](./type_defs.md#describeaffectedaccountsfororganizationresponsetypedef)
- [DescribeAffectedEntitiesResponseTypeDef](./type_defs.md#describeaffectedentitiesresponsetypedef)
- [DescribeHealthServiceStatusForOrganizationResponseTypeDef](./type_defs.md#describehealthservicestatusfororganizationresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef](./type_defs.md#describeaffectedentitiesfororganizationrequestdescribeaffectedentitiesfororganizationpaginatetypedef)
- [DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef](./type_defs.md#describeaffectedentitiesfororganizationrequestrequesttypedef)
- [DescribeEventDetailsForOrganizationRequestRequestTypeDef](./type_defs.md#describeeventdetailsfororganizationrequestrequesttypedef)
- [DescribeAffectedEntitiesForOrganizationResponseTypeDef](./type_defs.md#describeaffectedentitiesfororganizationresponsetypedef)
- [DescribeEntityAggregatesResponseTypeDef](./type_defs.md#describeentityaggregatesresponsetypedef)
- [DescribeEventAggregatesResponseTypeDef](./type_defs.md#describeeventaggregatesresponsetypedef)
- [DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef](./type_defs.md#describeeventtypesrequestdescribeeventtypespaginatetypedef)
- [DescribeEventTypesRequestRequestTypeDef](./type_defs.md#describeeventtypesrequestrequesttypedef)
- [DescribeEventTypesResponseTypeDef](./type_defs.md#describeeventtypesresponsetypedef)
- [DescribeEventsForOrganizationResponseTypeDef](./type_defs.md#describeeventsfororganizationresponsetypedef)
- [DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef)
- [EventDetailsTypeDef](./type_defs.md#eventdetailstypedef)
- [OrganizationEventDetailsTypeDef](./type_defs.md#organizationeventdetailstypedef)
- [DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef](./type_defs.md#describeaffectedentitiesrequestdescribeaffectedentitiespaginatetypedef)
- [DescribeAffectedEntitiesRequestRequestTypeDef](./type_defs.md#describeaffectedentitiesrequestrequesttypedef)
- [DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef](./type_defs.md#describeeventaggregatesrequestdescribeeventaggregatespaginatetypedef)
- [DescribeEventAggregatesRequestRequestTypeDef](./type_defs.md#describeeventaggregatesrequestrequesttypedef)
- [DescribeEventsRequestDescribeEventsPaginateTypeDef](./type_defs.md#describeeventsrequestdescribeeventspaginatetypedef)
- [DescribeEventsRequestRequestTypeDef](./type_defs.md#describeeventsrequestrequesttypedef)
- [DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef](./type_defs.md#describeeventsfororganizationrequestdescribeeventsfororganizationpaginatetypedef)
- [DescribeEventsForOrganizationRequestRequestTypeDef](./type_defs.md#describeeventsfororganizationrequestrequesttypedef)
- [DescribeEventDetailsResponseTypeDef](./type_defs.md#describeeventdetailsresponsetypedef)
- [DescribeEventDetailsForOrganizationResponseTypeDef](./type_defs.md#describeeventdetailsfororganizationresponsetypedef)

