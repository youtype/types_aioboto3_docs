# MigrationHubStrategyRecommendationsClient

> [Index](../README.md) > [MigrationHubStrategyRecommendations](./README.md) > MigrationHubStrategyRecommendationsClient

!!! note ""

    Auto-generated documentation for [MigrationHubStrategyRecommendations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#migrationhubstrategyrecommendations)
    type annotations stubs module [types-aiobotocore-migrationhubstrategy](https://pypi.org/project/types-aiobotocore-migrationhubstrategy/).

## MigrationHubStrategyRecommendationsClient

Type annotations and code completion for `#!python session.client("migrationhubstrategy")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# MigrationHubStrategyRecommendationsClient usage example

from aioboto3.session import Session
from types_aiobotocore_migrationhubstrategy.client import MigrationHubStrategyRecommendationsClient

session = Session()
async with session.client("migrationhubstrategy") as client:
    client: MigrationHubStrategyRecommendationsClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("migrationhubstrategy").exceptions` structure.

```python
# MigrationHubStrategyRecommendationsClient.exceptions usage example

async with session.client("migrationhubstrategy") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.DependencyException,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceLinkedRoleLockClientException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# MigrationHubStrategyRecommendationsClient.exceptions type checking example

from types_aiobotocore_migrationhubstrategy.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("migrationhubstrategy").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("migrationhubstrategy").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

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


### get\_application\_component\_details

Retrieves details about an application component.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").get_application_component_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# get_application_component_details method definition

await def get_application_component_details(
    self,
    *,
    applicationComponentId: str,
) -> GetApplicationComponentDetailsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetApplicationComponentDetailsResponseTypeDef](./type_defs.md#getapplicationcomponentdetailsresponsetypedef) 


```python
# get_application_component_details method usage example with argument unpacking

kwargs: GetApplicationComponentDetailsRequestRequestTypeDef = {  # (1)
    "applicationComponentId": ...,
}

parent.get_application_component_details(**kwargs)
```

1. See [:material-code-braces: GetApplicationComponentDetailsRequestRequestTypeDef](./type_defs.md#getapplicationcomponentdetailsrequestrequesttypedef) 

### get\_application\_component\_strategies

Retrieves a list of all the recommended strategies and tools for an application
component running on a server.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").get_application_component_strategies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# get_application_component_strategies method definition

await def get_application_component_strategies(
    self,
    *,
    applicationComponentId: str,
) -> GetApplicationComponentStrategiesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetApplicationComponentStrategiesResponseTypeDef](./type_defs.md#getapplicationcomponentstrategiesresponsetypedef) 


```python
# get_application_component_strategies method usage example with argument unpacking

kwargs: GetApplicationComponentStrategiesRequestRequestTypeDef = {  # (1)
    "applicationComponentId": ...,
}

parent.get_application_component_strategies(**kwargs)
```

1. See [:material-code-braces: GetApplicationComponentStrategiesRequestRequestTypeDef](./type_defs.md#getapplicationcomponentstrategiesrequestrequesttypedef) 

### get\_assessment

Retrieves the status of an on-going assessment.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").get_assessment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# get_assessment method definition

await def get_assessment(
    self,
    *,
    id: str,
) -> GetAssessmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAssessmentResponseTypeDef](./type_defs.md#getassessmentresponsetypedef) 


```python
# get_assessment method usage example with argument unpacking

kwargs: GetAssessmentRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_assessment(**kwargs)
```

1. See [:material-code-braces: GetAssessmentRequestRequestTypeDef](./type_defs.md#getassessmentrequestrequesttypedef) 

### get\_import\_file\_task

Retrieves the details about a specific import task.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").get_import_file_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# get_import_file_task method definition

await def get_import_file_task(
    self,
    *,
    id: str,
) -> GetImportFileTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetImportFileTaskResponseTypeDef](./type_defs.md#getimportfiletaskresponsetypedef) 


```python
# get_import_file_task method usage example with argument unpacking

kwargs: GetImportFileTaskRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_import_file_task(**kwargs)
```

1. See [:material-code-braces: GetImportFileTaskRequestRequestTypeDef](./type_defs.md#getimportfiletaskrequestrequesttypedef) 

### get\_latest\_assessment\_id

Retrieve the latest ID of a specific assessment task.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").get_latest_assessment_id` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# get_latest_assessment_id method definition

await def get_latest_assessment_id(
    self,
) -> GetLatestAssessmentIdResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLatestAssessmentIdResponseTypeDef](./type_defs.md#getlatestassessmentidresponsetypedef) 

### get\_portfolio\_preferences

Retrieves your migration and modernization preferences.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").get_portfolio_preferences` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# get_portfolio_preferences method definition

await def get_portfolio_preferences(
    self,
) -> GetPortfolioPreferencesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPortfolioPreferencesResponseTypeDef](./type_defs.md#getportfoliopreferencesresponsetypedef) 

### get\_portfolio\_summary

Retrieves overall summary including the number of servers to rehost and the
overall number of anti-patterns.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").get_portfolio_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# get_portfolio_summary method definition

await def get_portfolio_summary(
    self,
) -> GetPortfolioSummaryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPortfolioSummaryResponseTypeDef](./type_defs.md#getportfoliosummaryresponsetypedef) 

### get\_recommendation\_report\_details

Retrieves detailed information about the specified recommendation report.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").get_recommendation_report_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# get_recommendation_report_details method definition

await def get_recommendation_report_details(
    self,
    *,
    id: str,
) -> GetRecommendationReportDetailsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRecommendationReportDetailsResponseTypeDef](./type_defs.md#getrecommendationreportdetailsresponsetypedef) 


```python
# get_recommendation_report_details method usage example with argument unpacking

kwargs: GetRecommendationReportDetailsRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_recommendation_report_details(**kwargs)
```

1. See [:material-code-braces: GetRecommendationReportDetailsRequestRequestTypeDef](./type_defs.md#getrecommendationreportdetailsrequestrequesttypedef) 

### get\_server\_details

Retrieves detailed information about a specified server.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").get_server_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# get_server_details method definition

await def get_server_details(
    self,
    *,
    serverId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> GetServerDetailsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServerDetailsResponseTypeDef](./type_defs.md#getserverdetailsresponsetypedef) 


```python
# get_server_details method usage example with argument unpacking

kwargs: GetServerDetailsRequestRequestTypeDef = {  # (1)
    "serverId": ...,
}

parent.get_server_details(**kwargs)
```

1. See [:material-code-braces: GetServerDetailsRequestRequestTypeDef](./type_defs.md#getserverdetailsrequestrequesttypedef) 

### get\_server\_strategies

Retrieves recommended strategies and tools for the specified server.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").get_server_strategies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# get_server_strategies method definition

await def get_server_strategies(
    self,
    *,
    serverId: str,
) -> GetServerStrategiesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServerStrategiesResponseTypeDef](./type_defs.md#getserverstrategiesresponsetypedef) 


```python
# get_server_strategies method usage example with argument unpacking

kwargs: GetServerStrategiesRequestRequestTypeDef = {  # (1)
    "serverId": ...,
}

parent.get_server_strategies(**kwargs)
```

1. See [:material-code-braces: GetServerStrategiesRequestRequestTypeDef](./type_defs.md#getserverstrategiesrequestrequesttypedef) 

### list\_analyzable\_servers

Retrieves a list of all the servers fetched from customer vCenter using
Strategy Recommendation Collector.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").list_analyzable_servers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# list_analyzable_servers method definition

await def list_analyzable_servers(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    sort: SortOrderType = ...,  # (1)
) -> ListAnalyzableServersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-braces: ListAnalyzableServersResponseTypeDef](./type_defs.md#listanalyzableserversresponsetypedef) 


```python
# list_analyzable_servers method usage example with argument unpacking

kwargs: ListAnalyzableServersRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_analyzable_servers(**kwargs)
```

1. See [:material-code-braces: ListAnalyzableServersRequestRequestTypeDef](./type_defs.md#listanalyzableserversrequestrequesttypedef) 

### list\_application\_components

Retrieves a list of all the application components (processes).

Type annotations and code completion for `#!python session.client("migrationhubstrategy").list_application_components` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# list_application_components method definition

await def list_application_components(
    self,
    *,
    applicationComponentCriteria: ApplicationComponentCriteriaType = ...,  # (1)
    filterValue: str = ...,
    groupIdFilter: Sequence[GroupTypeDef] = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
    sort: SortOrderType = ...,  # (3)
) -> ListApplicationComponentsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ApplicationComponentCriteriaType](./literals.md#applicationcomponentcriteriatype) 
2. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListApplicationComponentsResponseTypeDef](./type_defs.md#listapplicationcomponentsresponsetypedef) 


```python
# list_application_components method usage example with argument unpacking

kwargs: ListApplicationComponentsRequestRequestTypeDef = {  # (1)
    "applicationComponentCriteria": ...,
}

parent.list_application_components(**kwargs)
```

1. See [:material-code-braces: ListApplicationComponentsRequestRequestTypeDef](./type_defs.md#listapplicationcomponentsrequestrequesttypedef) 

### list\_collectors

Retrieves a list of all the installed collectors.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").list_collectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# list_collectors method definition

await def list_collectors(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListCollectorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCollectorsResponseTypeDef](./type_defs.md#listcollectorsresponsetypedef) 


```python
# list_collectors method usage example with argument unpacking

kwargs: ListCollectorsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_collectors(**kwargs)
```

1. See [:material-code-braces: ListCollectorsRequestRequestTypeDef](./type_defs.md#listcollectorsrequestrequesttypedef) 

### list\_import\_file\_task

Retrieves a list of all the imports performed.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").list_import_file_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# list_import_file_task method definition

await def list_import_file_task(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListImportFileTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListImportFileTaskResponseTypeDef](./type_defs.md#listimportfiletaskresponsetypedef) 


```python
# list_import_file_task method usage example with argument unpacking

kwargs: ListImportFileTaskRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_import_file_task(**kwargs)
```

1. See [:material-code-braces: ListImportFileTaskRequestRequestTypeDef](./type_defs.md#listimportfiletaskrequestrequesttypedef) 

### list\_servers

Returns a list of all the servers.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").list_servers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# list_servers method definition

await def list_servers(
    self,
    *,
    filterValue: str = ...,
    groupIdFilter: Sequence[GroupTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
    serverCriteria: ServerCriteriaType = ...,  # (2)
    sort: SortOrderType = ...,  # (3)
) -> ListServersResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-brackets: ServerCriteriaType](./literals.md#servercriteriatype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListServersResponseTypeDef](./type_defs.md#listserversresponsetypedef) 


```python
# list_servers method usage example with argument unpacking

kwargs: ListServersRequestRequestTypeDef = {  # (1)
    "filterValue": ...,
}

parent.list_servers(**kwargs)
```

1. See [:material-code-braces: ListServersRequestRequestTypeDef](./type_defs.md#listserversrequestrequesttypedef) 

### put\_portfolio\_preferences

Saves the specified migration and modernization preferences.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").put_portfolio_preferences` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# put_portfolio_preferences method definition

await def put_portfolio_preferences(
    self,
    *,
    applicationMode: ApplicationModeType = ...,  # (1)
    applicationPreferences: ApplicationPreferencesTypeDef = ...,  # (2)
    databasePreferences: DatabasePreferencesTypeDef = ...,  # (3)
    prioritizeBusinessGoals: PrioritizeBusinessGoalsTypeDef = ...,  # (4)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ApplicationModeType](./literals.md#applicationmodetype) 
2. See [:material-code-braces: ApplicationPreferencesTypeDef](./type_defs.md#applicationpreferencestypedef) 
3. See [:material-code-braces: DatabasePreferencesTypeDef](./type_defs.md#databasepreferencestypedef) 
4. See [:material-code-braces: PrioritizeBusinessGoalsTypeDef](./type_defs.md#prioritizebusinessgoalstypedef) 


```python
# put_portfolio_preferences method usage example with argument unpacking

kwargs: PutPortfolioPreferencesRequestRequestTypeDef = {  # (1)
    "applicationMode": ...,
}

parent.put_portfolio_preferences(**kwargs)
```

1. See [:material-code-braces: PutPortfolioPreferencesRequestRequestTypeDef](./type_defs.md#putportfoliopreferencesrequestrequesttypedef) 

### start\_assessment

Starts the assessment of an on-premises environment.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").start_assessment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# start_assessment method definition

await def start_assessment(
    self,
    *,
    assessmentDataSourceType: AssessmentDataSourceTypeType = ...,  # (1)
    assessmentTargets: Sequence[AssessmentTargetUnionTypeDef] = ...,  # (2)
    s3bucketForAnalysisData: str = ...,
    s3bucketForReportData: str = ...,
) -> StartAssessmentResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AssessmentDataSourceTypeType](./literals.md#assessmentdatasourcetypetype) 
2. See [:material-code-braces: AssessmentTargetTypeDef](./type_defs.md#assessmenttargettypedef) [:material-code-braces: AssessmentTargetOutputTypeDef](./type_defs.md#assessmenttargetoutputtypedef) 
3. See [:material-code-braces: StartAssessmentResponseTypeDef](./type_defs.md#startassessmentresponsetypedef) 


```python
# start_assessment method usage example with argument unpacking

kwargs: StartAssessmentRequestRequestTypeDef = {  # (1)
    "assessmentDataSourceType": ...,
}

parent.start_assessment(**kwargs)
```

1. See [:material-code-braces: StartAssessmentRequestRequestTypeDef](./type_defs.md#startassessmentrequestrequesttypedef) 

### start\_import\_file\_task

Starts a file import.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").start_import_file_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# start_import_file_task method definition

await def start_import_file_task(
    self,
    *,
    S3Bucket: str,
    name: str,
    s3key: str,
    dataSourceType: DataSourceTypeType = ...,  # (1)
    groupId: Sequence[GroupTypeDef] = ...,  # (2)
    s3bucketForReportData: str = ...,
) -> StartImportFileTaskResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
2. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
3. See [:material-code-braces: StartImportFileTaskResponseTypeDef](./type_defs.md#startimportfiletaskresponsetypedef) 


```python
# start_import_file_task method usage example with argument unpacking

kwargs: StartImportFileTaskRequestRequestTypeDef = {  # (1)
    "S3Bucket": ...,
    "name": ...,
    "s3key": ...,
}

parent.start_import_file_task(**kwargs)
```

1. See [:material-code-braces: StartImportFileTaskRequestRequestTypeDef](./type_defs.md#startimportfiletaskrequestrequesttypedef) 

### start\_recommendation\_report\_generation

Starts generating a recommendation report.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").start_recommendation_report_generation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# start_recommendation_report_generation method definition

await def start_recommendation_report_generation(
    self,
    *,
    groupIdFilter: Sequence[GroupTypeDef] = ...,  # (1)
    outputFormat: OutputFormatType = ...,  # (2)
) -> StartRecommendationReportGenerationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
3. See [:material-code-braces: StartRecommendationReportGenerationResponseTypeDef](./type_defs.md#startrecommendationreportgenerationresponsetypedef) 


```python
# start_recommendation_report_generation method usage example with argument unpacking

kwargs: StartRecommendationReportGenerationRequestRequestTypeDef = {  # (1)
    "groupIdFilter": ...,
}

parent.start_recommendation_report_generation(**kwargs)
```

1. See [:material-code-braces: StartRecommendationReportGenerationRequestRequestTypeDef](./type_defs.md#startrecommendationreportgenerationrequestrequesttypedef) 

### stop\_assessment

Stops the assessment of an on-premises environment.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").stop_assessment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# stop_assessment method definition

await def stop_assessment(
    self,
    *,
    assessmentId: str,
) -> dict[str, Any]:
    ...
```



```python
# stop_assessment method usage example with argument unpacking

kwargs: StopAssessmentRequestRequestTypeDef = {  # (1)
    "assessmentId": ...,
}

parent.stop_assessment(**kwargs)
```

1. See [:material-code-braces: StopAssessmentRequestRequestTypeDef](./type_defs.md#stopassessmentrequestrequesttypedef) 

### update\_application\_component\_config

Updates the configuration of an application component.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").update_application_component_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# update_application_component_config method definition

await def update_application_component_config(
    self,
    *,
    applicationComponentId: str,
    appType: AppTypeType = ...,  # (1)
    configureOnly: bool = ...,
    inclusionStatus: InclusionStatusType = ...,  # (2)
    secretsManagerKey: str = ...,
    sourceCodeList: Sequence[SourceCodeTypeDef] = ...,  # (3)
    strategyOption: StrategyOptionTypeDef = ...,  # (4)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: AppTypeType](./literals.md#apptypetype) 
2. See [:material-code-brackets: InclusionStatusType](./literals.md#inclusionstatustype) 
3. See [:material-code-braces: SourceCodeTypeDef](./type_defs.md#sourcecodetypedef) 
4. See [:material-code-braces: StrategyOptionTypeDef](./type_defs.md#strategyoptiontypedef) 


```python
# update_application_component_config method usage example with argument unpacking

kwargs: UpdateApplicationComponentConfigRequestRequestTypeDef = {  # (1)
    "applicationComponentId": ...,
}

parent.update_application_component_config(**kwargs)
```

1. See [:material-code-braces: UpdateApplicationComponentConfigRequestRequestTypeDef](./type_defs.md#updateapplicationcomponentconfigrequestrequesttypedef) 

### update\_server\_config

Updates the configuration of the specified server.

Type annotations and code completion for `#!python session.client("migrationhubstrategy").update_server_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# update_server_config method definition

await def update_server_config(
    self,
    *,
    serverId: str,
    strategyOption: StrategyOptionTypeDef = ...,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: StrategyOptionTypeDef](./type_defs.md#strategyoptiontypedef) 


```python
# update_server_config method usage example with argument unpacking

kwargs: UpdateServerConfigRequestRequestTypeDef = {  # (1)
    "serverId": ...,
}

parent.update_server_config(**kwargs)
```

1. See [:material-code-braces: UpdateServerConfigRequestRequestTypeDef](./type_defs.md#updateserverconfigrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("migrationhubstrategy").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("migrationhubstrategy").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("migrationhubstrategy").get_paginator` method with overloads.

- `client.get_paginator("get_server_details")` -> [GetServerDetailsPaginator](./paginators.md#getserverdetailspaginator)
- `client.get_paginator("list_analyzable_servers")` -> [ListAnalyzableServersPaginator](./paginators.md#listanalyzableserverspaginator)
- `client.get_paginator("list_application_components")` -> [ListApplicationComponentsPaginator](./paginators.md#listapplicationcomponentspaginator)
- `client.get_paginator("list_collectors")` -> [ListCollectorsPaginator](./paginators.md#listcollectorspaginator)
- `client.get_paginator("list_import_file_task")` -> [ListImportFileTaskPaginator](./paginators.md#listimportfiletaskpaginator)
- `client.get_paginator("list_servers")` -> [ListServersPaginator](./paginators.md#listserverspaginator)


