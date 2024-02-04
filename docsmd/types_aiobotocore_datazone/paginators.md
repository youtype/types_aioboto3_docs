# Paginators

> [Index](../README.md) > [DataZone](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [DataZone](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
    type annotations stubs module [types-aiobotocore-datazone](https://pypi.org/project/types-aiobotocore-datazone/).

## ListAssetRevisionsPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("list_asset_revisions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListAssetRevisions)

```python
# ListAssetRevisionsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import ListAssetRevisionsPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: ListAssetRevisionsPaginator = client.get_paginator("list_asset_revisions")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssetRevisionsOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [ListAssetRevisionsPaginator](./paginators.md#listassetrevisionspaginator)
3. item: [:material-code-braces: ListAssetRevisionsOutputTypeDef](./type_defs.md#listassetrevisionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListAssetRevisionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAssetRevisionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAssetRevisionsOutputTypeDef](./type_defs.md#listassetrevisionsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssetRevisionsInputListAssetRevisionsPaginateTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssetRevisionsInputListAssetRevisionsPaginateTypeDef](./type_defs.md#listassetrevisionsinputlistassetrevisionspaginatetypedef) 
## ListDataSourceRunActivitiesPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("list_data_source_run_activities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListDataSourceRunActivities)

```python
# ListDataSourceRunActivitiesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import ListDataSourceRunActivitiesPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: ListDataSourceRunActivitiesPaginator = client.get_paginator("list_data_source_run_activities")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataSourceRunActivitiesOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [ListDataSourceRunActivitiesPaginator](./paginators.md#listdatasourcerunactivitiespaginator)
3. item: [:material-code-braces: ListDataSourceRunActivitiesOutputTypeDef](./type_defs.md#listdatasourcerunactivitiesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDataSourceRunActivitiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainIdentifier: str,
    identifier: str,
    status: DataAssetActivityStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDataSourceRunActivitiesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DataAssetActivityStatusType](./literals.md#dataassetactivitystatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDataSourceRunActivitiesOutputTypeDef](./type_defs.md#listdatasourcerunactivitiesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDataSourceRunActivitiesInputListDataSourceRunActivitiesPaginateTypeDef = {  # (1)
    "domainIdentifier": ...,
    "identifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataSourceRunActivitiesInputListDataSourceRunActivitiesPaginateTypeDef](./type_defs.md#listdatasourcerunactivitiesinputlistdatasourcerunactivitiespaginatetypedef) 
## ListDataSourceRunsPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("list_data_source_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListDataSourceRuns)

```python
# ListDataSourceRunsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import ListDataSourceRunsPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: ListDataSourceRunsPaginator = client.get_paginator("list_data_source_runs")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataSourceRunsOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [ListDataSourceRunsPaginator](./paginators.md#listdatasourcerunspaginator)
3. item: [:material-code-braces: ListDataSourceRunsOutputTypeDef](./type_defs.md#listdatasourcerunsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDataSourceRunsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    dataSourceIdentifier: str,
    domainIdentifier: str,
    status: DataSourceRunStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDataSourceRunsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DataSourceRunStatusType](./literals.md#datasourcerunstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDataSourceRunsOutputTypeDef](./type_defs.md#listdatasourcerunsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDataSourceRunsInputListDataSourceRunsPaginateTypeDef = {  # (1)
    "dataSourceIdentifier": ...,
    "domainIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataSourceRunsInputListDataSourceRunsPaginateTypeDef](./type_defs.md#listdatasourcerunsinputlistdatasourcerunspaginatetypedef) 
## ListDataSourcesPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("list_data_sources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListDataSources)

```python
# ListDataSourcesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import ListDataSourcesPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: ListDataSourcesPaginator = client.get_paginator("list_data_sources")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataSourcesOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [ListDataSourcesPaginator](./paginators.md#listdatasourcespaginator)
3. item: [:material-code-braces: ListDataSourcesOutputTypeDef](./type_defs.md#listdatasourcesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDataSourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainIdentifier: str,
    projectIdentifier: str,
    environmentIdentifier: str = ...,
    name: str = ...,
    status: DataSourceStatusType = ...,  # (1)
    type: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDataSourcesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDataSourcesOutputTypeDef](./type_defs.md#listdatasourcesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDataSourcesInputListDataSourcesPaginateTypeDef = {  # (1)
    "domainIdentifier": ...,
    "projectIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataSourcesInputListDataSourcesPaginateTypeDef](./type_defs.md#listdatasourcesinputlistdatasourcespaginatetypedef) 
## ListDomainsPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("list_domains")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListDomains)

```python
# ListDomainsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import ListDomainsPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: ListDomainsPaginator = client.get_paginator("list_domains")  # (2)
    async for item in paginator.paginate(...):
        item: ListDomainsOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [ListDomainsPaginator](./paginators.md#listdomainspaginator)
3. item: [:material-code-braces: ListDomainsOutputTypeDef](./type_defs.md#listdomainsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDomainsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    status: DomainStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDomainsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDomainsOutputTypeDef](./type_defs.md#listdomainsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDomainsInputListDomainsPaginateTypeDef = {  # (1)
    "status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDomainsInputListDomainsPaginateTypeDef](./type_defs.md#listdomainsinputlistdomainspaginatetypedef) 
## ListEnvironmentBlueprintConfigurationsPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("list_environment_blueprint_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListEnvironmentBlueprintConfigurations)

```python
# ListEnvironmentBlueprintConfigurationsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import ListEnvironmentBlueprintConfigurationsPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: ListEnvironmentBlueprintConfigurationsPaginator = client.get_paginator("list_environment_blueprint_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnvironmentBlueprintConfigurationsOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [ListEnvironmentBlueprintConfigurationsPaginator](./paginators.md#listenvironmentblueprintconfigurationspaginator)
3. item: [:material-code-braces: ListEnvironmentBlueprintConfigurationsOutputTypeDef](./type_defs.md#listenvironmentblueprintconfigurationsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListEnvironmentBlueprintConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEnvironmentBlueprintConfigurationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEnvironmentBlueprintConfigurationsOutputTypeDef](./type_defs.md#listenvironmentblueprintconfigurationsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEnvironmentBlueprintConfigurationsInputListEnvironmentBlueprintConfigurationsPaginateTypeDef = {  # (1)
    "domainIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentBlueprintConfigurationsInputListEnvironmentBlueprintConfigurationsPaginateTypeDef](./type_defs.md#listenvironmentblueprintconfigurationsinputlistenvironmentblueprintconfigurationspaginatetypedef) 
## ListEnvironmentBlueprintsPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("list_environment_blueprints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListEnvironmentBlueprints)

```python
# ListEnvironmentBlueprintsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import ListEnvironmentBlueprintsPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: ListEnvironmentBlueprintsPaginator = client.get_paginator("list_environment_blueprints")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnvironmentBlueprintsOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [ListEnvironmentBlueprintsPaginator](./paginators.md#listenvironmentblueprintspaginator)
3. item: [:material-code-braces: ListEnvironmentBlueprintsOutputTypeDef](./type_defs.md#listenvironmentblueprintsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListEnvironmentBlueprintsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainIdentifier: str,
    managed: bool = ...,
    name: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEnvironmentBlueprintsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEnvironmentBlueprintsOutputTypeDef](./type_defs.md#listenvironmentblueprintsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEnvironmentBlueprintsInputListEnvironmentBlueprintsPaginateTypeDef = {  # (1)
    "domainIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentBlueprintsInputListEnvironmentBlueprintsPaginateTypeDef](./type_defs.md#listenvironmentblueprintsinputlistenvironmentblueprintspaginatetypedef) 
## ListEnvironmentProfilesPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("list_environment_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListEnvironmentProfiles)

```python
# ListEnvironmentProfilesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import ListEnvironmentProfilesPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: ListEnvironmentProfilesPaginator = client.get_paginator("list_environment_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnvironmentProfilesOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [ListEnvironmentProfilesPaginator](./paginators.md#listenvironmentprofilespaginator)
3. item: [:material-code-braces: ListEnvironmentProfilesOutputTypeDef](./type_defs.md#listenvironmentprofilesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListEnvironmentProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainIdentifier: str,
    awsAccountId: str = ...,
    awsAccountRegion: str = ...,
    environmentBlueprintIdentifier: str = ...,
    name: str = ...,
    projectIdentifier: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEnvironmentProfilesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEnvironmentProfilesOutputTypeDef](./type_defs.md#listenvironmentprofilesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEnvironmentProfilesInputListEnvironmentProfilesPaginateTypeDef = {  # (1)
    "domainIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentProfilesInputListEnvironmentProfilesPaginateTypeDef](./type_defs.md#listenvironmentprofilesinputlistenvironmentprofilespaginatetypedef) 
## ListEnvironmentsPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("list_environments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListEnvironments)

```python
# ListEnvironmentsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import ListEnvironmentsPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnvironmentsOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
3. item: [:material-code-braces: ListEnvironmentsOutputTypeDef](./type_defs.md#listenvironmentsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListEnvironmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainIdentifier: str,
    projectIdentifier: str,
    awsAccountId: str = ...,
    awsAccountRegion: str = ...,
    environmentBlueprintIdentifier: str = ...,
    environmentProfileIdentifier: str = ...,
    name: str = ...,
    provider: str = ...,
    status: EnvironmentStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListEnvironmentsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListEnvironmentsOutputTypeDef](./type_defs.md#listenvironmentsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEnvironmentsInputListEnvironmentsPaginateTypeDef = {  # (1)
    "domainIdentifier": ...,
    "projectIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentsInputListEnvironmentsPaginateTypeDef](./type_defs.md#listenvironmentsinputlistenvironmentspaginatetypedef) 
## ListNotificationsPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("list_notifications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListNotifications)

```python
# ListNotificationsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import ListNotificationsPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: ListNotificationsPaginator = client.get_paginator("list_notifications")  # (2)
    async for item in paginator.paginate(...):
        item: ListNotificationsOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [ListNotificationsPaginator](./paginators.md#listnotificationspaginator)
3. item: [:material-code-braces: ListNotificationsOutputTypeDef](./type_defs.md#listnotificationsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListNotificationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainIdentifier: str,
    type: NotificationTypeType,  # (1)
    afterTimestamp: Union[datetime, str] = ...,
    beforeTimestamp: Union[datetime, str] = ...,
    subjects: Sequence[str] = ...,
    taskStatus: TaskStatusType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListNotificationsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
2. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListNotificationsOutputTypeDef](./type_defs.md#listnotificationsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListNotificationsInputListNotificationsPaginateTypeDef = {  # (1)
    "domainIdentifier": ...,
    "type": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNotificationsInputListNotificationsPaginateTypeDef](./type_defs.md#listnotificationsinputlistnotificationspaginatetypedef) 
## ListProjectMembershipsPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("list_project_memberships")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListProjectMemberships)

```python
# ListProjectMembershipsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import ListProjectMembershipsPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: ListProjectMembershipsPaginator = client.get_paginator("list_project_memberships")  # (2)
    async for item in paginator.paginate(...):
        item: ListProjectMembershipsOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [ListProjectMembershipsPaginator](./paginators.md#listprojectmembershipspaginator)
3. item: [:material-code-braces: ListProjectMembershipsOutputTypeDef](./type_defs.md#listprojectmembershipsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListProjectMembershipsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainIdentifier: str,
    projectIdentifier: str,
    sortBy: SortFieldProjectType = ...,  # (1)
    sortOrder: SortOrderType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListProjectMembershipsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SortFieldProjectType](./literals.md#sortfieldprojecttype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListProjectMembershipsOutputTypeDef](./type_defs.md#listprojectmembershipsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProjectMembershipsInputListProjectMembershipsPaginateTypeDef = {  # (1)
    "domainIdentifier": ...,
    "projectIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProjectMembershipsInputListProjectMembershipsPaginateTypeDef](./type_defs.md#listprojectmembershipsinputlistprojectmembershipspaginatetypedef) 
## ListProjectsPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("list_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListProjects)

```python
# ListProjectsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import ListProjectsPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")  # (2)
    async for item in paginator.paginate(...):
        item: ListProjectsOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [ListProjectsPaginator](./paginators.md#listprojectspaginator)
3. item: [:material-code-braces: ListProjectsOutputTypeDef](./type_defs.md#listprojectsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListProjectsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainIdentifier: str,
    groupIdentifier: str = ...,
    name: str = ...,
    userIdentifier: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListProjectsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProjectsOutputTypeDef](./type_defs.md#listprojectsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProjectsInputListProjectsPaginateTypeDef = {  # (1)
    "domainIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProjectsInputListProjectsPaginateTypeDef](./type_defs.md#listprojectsinputlistprojectspaginatetypedef) 
## ListSubscriptionGrantsPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("list_subscription_grants")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListSubscriptionGrants)

```python
# ListSubscriptionGrantsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import ListSubscriptionGrantsPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: ListSubscriptionGrantsPaginator = client.get_paginator("list_subscription_grants")  # (2)
    async for item in paginator.paginate(...):
        item: ListSubscriptionGrantsOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [ListSubscriptionGrantsPaginator](./paginators.md#listsubscriptiongrantspaginator)
3. item: [:material-code-braces: ListSubscriptionGrantsOutputTypeDef](./type_defs.md#listsubscriptiongrantsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSubscriptionGrantsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainIdentifier: str,
    environmentId: str = ...,
    sortBy: SortKeyType = ...,  # (1)
    sortOrder: SortOrderType = ...,  # (2)
    subscribedListingId: str = ...,
    subscriptionId: str = ...,
    subscriptionTargetId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListSubscriptionGrantsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SortKeyType](./literals.md#sortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListSubscriptionGrantsOutputTypeDef](./type_defs.md#listsubscriptiongrantsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSubscriptionGrantsInputListSubscriptionGrantsPaginateTypeDef = {  # (1)
    "domainIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSubscriptionGrantsInputListSubscriptionGrantsPaginateTypeDef](./type_defs.md#listsubscriptiongrantsinputlistsubscriptiongrantspaginatetypedef) 
## ListSubscriptionRequestsPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("list_subscription_requests")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListSubscriptionRequests)

```python
# ListSubscriptionRequestsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import ListSubscriptionRequestsPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: ListSubscriptionRequestsPaginator = client.get_paginator("list_subscription_requests")  # (2)
    async for item in paginator.paginate(...):
        item: ListSubscriptionRequestsOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [ListSubscriptionRequestsPaginator](./paginators.md#listsubscriptionrequestspaginator)
3. item: [:material-code-braces: ListSubscriptionRequestsOutputTypeDef](./type_defs.md#listsubscriptionrequestsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSubscriptionRequestsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainIdentifier: str,
    approverProjectId: str = ...,
    owningProjectId: str = ...,
    sortBy: SortKeyType = ...,  # (1)
    sortOrder: SortOrderType = ...,  # (2)
    status: SubscriptionRequestStatusType = ...,  # (3)
    subscribedListingId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AsyncIterator[ListSubscriptionRequestsOutputTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: SortKeyType](./literals.md#sortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: SubscriptionRequestStatusType](./literals.md#subscriptionrequeststatustype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListSubscriptionRequestsOutputTypeDef](./type_defs.md#listsubscriptionrequestsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSubscriptionRequestsInputListSubscriptionRequestsPaginateTypeDef = {  # (1)
    "domainIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSubscriptionRequestsInputListSubscriptionRequestsPaginateTypeDef](./type_defs.md#listsubscriptionrequestsinputlistsubscriptionrequestspaginatetypedef) 
## ListSubscriptionTargetsPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("list_subscription_targets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListSubscriptionTargets)

```python
# ListSubscriptionTargetsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import ListSubscriptionTargetsPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: ListSubscriptionTargetsPaginator = client.get_paginator("list_subscription_targets")  # (2)
    async for item in paginator.paginate(...):
        item: ListSubscriptionTargetsOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [ListSubscriptionTargetsPaginator](./paginators.md#listsubscriptiontargetspaginator)
3. item: [:material-code-braces: ListSubscriptionTargetsOutputTypeDef](./type_defs.md#listsubscriptiontargetsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSubscriptionTargetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainIdentifier: str,
    environmentIdentifier: str,
    sortBy: SortKeyType = ...,  # (1)
    sortOrder: SortOrderType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListSubscriptionTargetsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SortKeyType](./literals.md#sortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListSubscriptionTargetsOutputTypeDef](./type_defs.md#listsubscriptiontargetsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSubscriptionTargetsInputListSubscriptionTargetsPaginateTypeDef = {  # (1)
    "domainIdentifier": ...,
    "environmentIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSubscriptionTargetsInputListSubscriptionTargetsPaginateTypeDef](./type_defs.md#listsubscriptiontargetsinputlistsubscriptiontargetspaginatetypedef) 
## ListSubscriptionsPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("list_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListSubscriptions)

```python
# ListSubscriptionsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import ListSubscriptionsPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: ListSubscriptionsPaginator = client.get_paginator("list_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSubscriptionsOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [ListSubscriptionsPaginator](./paginators.md#listsubscriptionspaginator)
3. item: [:material-code-braces: ListSubscriptionsOutputTypeDef](./type_defs.md#listsubscriptionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSubscriptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainIdentifier: str,
    approverProjectId: str = ...,
    owningProjectId: str = ...,
    sortBy: SortKeyType = ...,  # (1)
    sortOrder: SortOrderType = ...,  # (2)
    status: SubscriptionStatusType = ...,  # (3)
    subscribedListingId: str = ...,
    subscriptionRequestIdentifier: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AsyncIterator[ListSubscriptionsOutputTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: SortKeyType](./literals.md#sortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: SubscriptionStatusType](./literals.md#subscriptionstatustype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListSubscriptionsOutputTypeDef](./type_defs.md#listsubscriptionsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSubscriptionsInputListSubscriptionsPaginateTypeDef = {  # (1)
    "domainIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSubscriptionsInputListSubscriptionsPaginateTypeDef](./type_defs.md#listsubscriptionsinputlistsubscriptionspaginatetypedef) 
## SearchPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("search")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.Search)

```python
# SearchPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import SearchPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: SearchPaginator = client.get_paginator("search")  # (2)
    async for item in paginator.paginate(...):
        item: SearchOutputPaginatorTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [SearchPaginator](./paginators.md#searchpaginator)
3. item: [:material-code-braces: SearchOutputPaginatorTypeDef](./type_defs.md#searchoutputpaginatortypedef) 


### paginate

Type annotations and code completion for `#!python SearchPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainIdentifier: str,
    searchScope: InventorySearchScopeType,  # (1)
    additionalAttributes: Sequence[SearchOutputAdditionalAttributeType] = ...,  # (2)
    filters: FilterClauseTypeDef = ...,  # (3)
    owningProjectIdentifier: str = ...,
    searchIn: Sequence[SearchInItemTypeDef] = ...,  # (4)
    searchText: str = ...,
    sort: SearchSortTypeDef = ...,  # (5)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (6)
) -> AsyncIterator[SearchOutputPaginatorTypeDef]:  # (7)
    ...
```

1. See [:material-code-brackets: InventorySearchScopeType](./literals.md#inventorysearchscopetype) 
2. See [:material-code-brackets: SearchOutputAdditionalAttributeType](./literals.md#searchoutputadditionalattributetype) 
3. See [:material-code-braces: FilterClauseTypeDef](./type_defs.md#filterclausetypedef) 
4. See [:material-code-braces: SearchInItemTypeDef](./type_defs.md#searchinitemtypedef) 
5. See [:material-code-braces: SearchSortTypeDef](./type_defs.md#searchsorttypedef) 
6. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
7. See [:material-code-braces: SearchOutputPaginatorTypeDef](./type_defs.md#searchoutputpaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchInputSearchPaginateTypeDef = {  # (1)
    "domainIdentifier": ...,
    "searchScope": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchInputSearchPaginateTypeDef](./type_defs.md#searchinputsearchpaginatetypedef) 
## SearchGroupProfilesPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("search_group_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.SearchGroupProfiles)

```python
# SearchGroupProfilesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import SearchGroupProfilesPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: SearchGroupProfilesPaginator = client.get_paginator("search_group_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: SearchGroupProfilesOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [SearchGroupProfilesPaginator](./paginators.md#searchgroupprofilespaginator)
3. item: [:material-code-braces: SearchGroupProfilesOutputTypeDef](./type_defs.md#searchgroupprofilesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python SearchGroupProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainIdentifier: str,
    groupType: GroupSearchTypeType,  # (1)
    searchText: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[SearchGroupProfilesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: GroupSearchTypeType](./literals.md#groupsearchtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SearchGroupProfilesOutputTypeDef](./type_defs.md#searchgroupprofilesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchGroupProfilesInputSearchGroupProfilesPaginateTypeDef = {  # (1)
    "domainIdentifier": ...,
    "groupType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchGroupProfilesInputSearchGroupProfilesPaginateTypeDef](./type_defs.md#searchgroupprofilesinputsearchgroupprofilespaginatetypedef) 
## SearchListingsPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("search_listings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.SearchListings)

```python
# SearchListingsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import SearchListingsPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: SearchListingsPaginator = client.get_paginator("search_listings")  # (2)
    async for item in paginator.paginate(...):
        item: SearchListingsOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [SearchListingsPaginator](./paginators.md#searchlistingspaginator)
3. item: [:material-code-braces: SearchListingsOutputTypeDef](./type_defs.md#searchlistingsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python SearchListingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainIdentifier: str,
    additionalAttributes: Sequence[SearchOutputAdditionalAttributeType] = ...,  # (1)
    filters: FilterClauseTypeDef = ...,  # (2)
    searchIn: Sequence[SearchInItemTypeDef] = ...,  # (3)
    searchText: str = ...,
    sort: SearchSortTypeDef = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> AsyncIterator[SearchListingsOutputTypeDef]:  # (6)
    ...
```

1. See [:material-code-brackets: SearchOutputAdditionalAttributeType](./literals.md#searchoutputadditionalattributetype) 
2. See [:material-code-braces: FilterClauseTypeDef](./type_defs.md#filterclausetypedef) 
3. See [:material-code-braces: SearchInItemTypeDef](./type_defs.md#searchinitemtypedef) 
4. See [:material-code-braces: SearchSortTypeDef](./type_defs.md#searchsorttypedef) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
6. See [:material-code-braces: SearchListingsOutputTypeDef](./type_defs.md#searchlistingsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchListingsInputSearchListingsPaginateTypeDef = {  # (1)
    "domainIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchListingsInputSearchListingsPaginateTypeDef](./type_defs.md#searchlistingsinputsearchlistingspaginatetypedef) 
## SearchTypesPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("search_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.SearchTypes)

```python
# SearchTypesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import SearchTypesPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: SearchTypesPaginator = client.get_paginator("search_types")  # (2)
    async for item in paginator.paginate(...):
        item: SearchTypesOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [SearchTypesPaginator](./paginators.md#searchtypespaginator)
3. item: [:material-code-braces: SearchTypesOutputTypeDef](./type_defs.md#searchtypesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python SearchTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainIdentifier: str,
    managed: bool,
    searchScope: TypesSearchScopeType,  # (1)
    filters: FilterClauseTypeDef = ...,  # (2)
    searchIn: Sequence[SearchInItemTypeDef] = ...,  # (3)
    searchText: str = ...,
    sort: SearchSortTypeDef = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> AsyncIterator[SearchTypesOutputTypeDef]:  # (6)
    ...
```

1. See [:material-code-brackets: TypesSearchScopeType](./literals.md#typessearchscopetype) 
2. See [:material-code-braces: FilterClauseTypeDef](./type_defs.md#filterclausetypedef) 
3. See [:material-code-braces: SearchInItemTypeDef](./type_defs.md#searchinitemtypedef) 
4. See [:material-code-braces: SearchSortTypeDef](./type_defs.md#searchsorttypedef) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
6. See [:material-code-braces: SearchTypesOutputTypeDef](./type_defs.md#searchtypesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchTypesInputSearchTypesPaginateTypeDef = {  # (1)
    "domainIdentifier": ...,
    "managed": ...,
    "searchScope": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchTypesInputSearchTypesPaginateTypeDef](./type_defs.md#searchtypesinputsearchtypespaginatetypedef) 
## SearchUserProfilesPaginator

Type annotations and code completion for `#!python session.client("datazone").get_paginator("search_user_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.SearchUserProfiles)

```python
# SearchUserProfilesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datazone.paginator import SearchUserProfilesPaginator

session = Session()

session = get_session()
async with session.client("datazone") as client:  # (1)
    paginator: SearchUserProfilesPaginator = client.get_paginator("search_user_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: SearchUserProfilesOutputTypeDef
        print(item)  # (3)
```

1. client: [DataZoneClient](./client.md)
2. paginator: [SearchUserProfilesPaginator](./paginators.md#searchuserprofilespaginator)
3. item: [:material-code-braces: SearchUserProfilesOutputTypeDef](./type_defs.md#searchuserprofilesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python SearchUserProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainIdentifier: str,
    userType: UserSearchTypeType,  # (1)
    searchText: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[SearchUserProfilesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: UserSearchTypeType](./literals.md#usersearchtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SearchUserProfilesOutputTypeDef](./type_defs.md#searchuserprofilesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchUserProfilesInputSearchUserProfilesPaginateTypeDef = {  # (1)
    "domainIdentifier": ...,
    "userType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchUserProfilesInputSearchUserProfilesPaginateTypeDef](./type_defs.md#searchuserprofilesinputsearchuserprofilespaginatetypedef) 
