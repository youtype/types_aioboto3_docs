# IoTTwinMaker module

> [Index](../README.md) > IoTTwinMaker


!!! note ""

    Auto-generated documentation for [IoTTwinMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
    type annotations stubs module [types-aiobotocore-iottwinmaker](https://pypi.org/project/types-aiobotocore-iottwinmaker/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `IoTTwinMaker` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[iottwinmaker]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[iottwinmaker]'


# standalone installation
python -m pip install types-aiobotocore-iottwinmaker
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-iottwinmaker
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IoTTwinMakerClient

Type annotations and code completion for  `#!python session.client("iottwinmaker")` as [IoTTwinMakerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iottwinmaker.client import IoTTwinMakerClient


session = Session()
async with session.client("iottwinmaker") as client:
    client: IoTTwinMakerClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_iottwinmaker.literals import ComponentUpdateTypeType

def get_value() -> ComponentUpdateTypeType:
    return "CREATE"
```

- [ComponentUpdateTypeType](./literals.md#componentupdatetypetype)
- [ErrorCodeType](./literals.md#errorcodetype)
- [InterpolationTypeType](./literals.md#interpolationtypetype)
- [OrderByTimeType](./literals.md#orderbytimetype)
- [ParentEntityUpdateTypeType](./literals.md#parententityupdatetypetype)
- [PropertyUpdateTypeType](./literals.md#propertyupdatetypetype)
- [ScopeType](./literals.md#scopetype)
- [StateType](./literals.md#statetype)
- [TypeType](./literals.md#typetype)
- [IoTTwinMakerServiceName](./literals.md#iottwinmakerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_iottwinmaker.type_defs import ResponseMetadataTypeDef

def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
        "HostId": ...,
        "HTTPStatusCode": ...,
        "HTTPHeaders": ...,
        "RetryAttempts": ...,
    }
```

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [PropertyDefinitionRequestTypeDef](./type_defs.md#propertydefinitionrequesttypedef)
- [CreateSceneRequestRequestTypeDef](./type_defs.md#createscenerequestrequesttypedef)
- [CreateWorkspaceRequestRequestTypeDef](./type_defs.md#createworkspacerequestrequesttypedef)
- [LambdaFunctionTypeDef](./type_defs.md#lambdafunctiontypedef)
- [RelationshipTypeDef](./type_defs.md#relationshiptypedef)
- [RelationshipValueTypeDef](./type_defs.md#relationshipvaluetypedef)
- [DeleteComponentTypeRequestRequestTypeDef](./type_defs.md#deletecomponenttyperequestrequesttypedef)
- [DeleteEntityRequestRequestTypeDef](./type_defs.md#deleteentityrequestrequesttypedef)
- [DeleteSceneRequestRequestTypeDef](./type_defs.md#deletescenerequestrequesttypedef)
- [DeleteWorkspaceRequestRequestTypeDef](./type_defs.md#deleteworkspacerequestrequesttypedef)
- [EntityPropertyReferenceTypeDef](./type_defs.md#entitypropertyreferencetypedef)
- [ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef)
- [GetComponentTypeRequestRequestTypeDef](./type_defs.md#getcomponenttyperequestrequesttypedef)
- [PropertyDefinitionResponseTypeDef](./type_defs.md#propertydefinitionresponsetypedef)
- [GetEntityRequestRequestTypeDef](./type_defs.md#getentityrequestrequesttypedef)
- [InterpolationParametersTypeDef](./type_defs.md#interpolationparameterstypedef)
- [PropertyFilterTypeDef](./type_defs.md#propertyfiltertypedef)
- [GetPropertyValueRequestRequestTypeDef](./type_defs.md#getpropertyvaluerequestrequesttypedef)
- [GetSceneRequestRequestTypeDef](./type_defs.md#getscenerequestrequesttypedef)
- [GetWorkspaceRequestRequestTypeDef](./type_defs.md#getworkspacerequestrequesttypedef)
- [ListComponentTypesFilterTypeDef](./type_defs.md#listcomponenttypesfiltertypedef)
- [ListEntitiesFilterTypeDef](./type_defs.md#listentitiesfiltertypedef)
- [ListScenesRequestRequestTypeDef](./type_defs.md#listscenesrequestrequesttypedef)
- [SceneSummaryTypeDef](./type_defs.md#scenesummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListWorkspacesRequestRequestTypeDef](./type_defs.md#listworkspacesrequestrequesttypedef)
- [WorkspaceSummaryTypeDef](./type_defs.md#workspacesummarytypedef)
- [ParentEntityUpdateRequestTypeDef](./type_defs.md#parententityupdaterequesttypedef)
- [PropertyValueTypeDef](./type_defs.md#propertyvaluetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateSceneRequestRequestTypeDef](./type_defs.md#updatescenerequestrequesttypedef)
- [UpdateWorkspaceRequestRequestTypeDef](./type_defs.md#updateworkspacerequestrequesttypedef)
- [CreateComponentTypeResponseTypeDef](./type_defs.md#createcomponenttyperesponsetypedef)
- [CreateEntityResponseTypeDef](./type_defs.md#createentityresponsetypedef)
- [CreateSceneResponseTypeDef](./type_defs.md#createsceneresponsetypedef)
- [CreateWorkspaceResponseTypeDef](./type_defs.md#createworkspaceresponsetypedef)
- [DeleteComponentTypeResponseTypeDef](./type_defs.md#deletecomponenttyperesponsetypedef)
- [DeleteEntityResponseTypeDef](./type_defs.md#deleteentityresponsetypedef)
- [GetSceneResponseTypeDef](./type_defs.md#getsceneresponsetypedef)
- [GetWorkspaceResponseTypeDef](./type_defs.md#getworkspaceresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdateComponentTypeResponseTypeDef](./type_defs.md#updatecomponenttyperesponsetypedef)
- [UpdateEntityResponseTypeDef](./type_defs.md#updateentityresponsetypedef)
- [UpdateSceneResponseTypeDef](./type_defs.md#updatesceneresponsetypedef)
- [UpdateWorkspaceResponseTypeDef](./type_defs.md#updateworkspaceresponsetypedef)
- [PropertyRequestTypeDef](./type_defs.md#propertyrequesttypedef)
- [DataConnectorTypeDef](./type_defs.md#dataconnectortypedef)
- [DataTypeTypeDef](./type_defs.md#datatypetypedef)
- [DataValueTypeDef](./type_defs.md#datavaluetypedef)
- [PropertyLatestValueTypeDef](./type_defs.md#propertylatestvaluetypedef)
- [StatusTypeDef](./type_defs.md#statustypedef)
- [PropertyResponseTypeDef](./type_defs.md#propertyresponsetypedef)
- [GetPropertyValueHistoryRequestRequestTypeDef](./type_defs.md#getpropertyvaluehistoryrequestrequesttypedef)
- [ListComponentTypesRequestRequestTypeDef](./type_defs.md#listcomponenttypesrequestrequesttypedef)
- [ListEntitiesRequestRequestTypeDef](./type_defs.md#listentitiesrequestrequesttypedef)
- [ListScenesResponseTypeDef](./type_defs.md#listscenesresponsetypedef)
- [ListWorkspacesResponseTypeDef](./type_defs.md#listworkspacesresponsetypedef)
- [PropertyValueEntryTypeDef](./type_defs.md#propertyvalueentrytypedef)
- [PropertyValueHistoryTypeDef](./type_defs.md#propertyvaluehistorytypedef)
- [ComponentRequestTypeDef](./type_defs.md#componentrequesttypedef)
- [ComponentUpdateRequestTypeDef](./type_defs.md#componentupdaterequesttypedef)
- [FunctionRequestTypeDef](./type_defs.md#functionrequesttypedef)
- [FunctionResponseTypeDef](./type_defs.md#functionresponsetypedef)
- [GetPropertyValueResponseTypeDef](./type_defs.md#getpropertyvalueresponsetypedef)
- [ComponentTypeSummaryTypeDef](./type_defs.md#componenttypesummarytypedef)
- [EntitySummaryTypeDef](./type_defs.md#entitysummarytypedef)
- [ComponentResponseTypeDef](./type_defs.md#componentresponsetypedef)
- [BatchPutPropertyErrorTypeDef](./type_defs.md#batchputpropertyerrortypedef)
- [BatchPutPropertyValuesRequestRequestTypeDef](./type_defs.md#batchputpropertyvaluesrequestrequesttypedef)
- [GetPropertyValueHistoryResponseTypeDef](./type_defs.md#getpropertyvaluehistoryresponsetypedef)
- [CreateEntityRequestRequestTypeDef](./type_defs.md#createentityrequestrequesttypedef)
- [UpdateEntityRequestRequestTypeDef](./type_defs.md#updateentityrequestrequesttypedef)
- [CreateComponentTypeRequestRequestTypeDef](./type_defs.md#createcomponenttyperequestrequesttypedef)
- [UpdateComponentTypeRequestRequestTypeDef](./type_defs.md#updatecomponenttyperequestrequesttypedef)
- [GetComponentTypeResponseTypeDef](./type_defs.md#getcomponenttyperesponsetypedef)
- [ListComponentTypesResponseTypeDef](./type_defs.md#listcomponenttypesresponsetypedef)
- [ListEntitiesResponseTypeDef](./type_defs.md#listentitiesresponsetypedef)
- [GetEntityResponseTypeDef](./type_defs.md#getentityresponsetypedef)
- [BatchPutPropertyErrorEntryTypeDef](./type_defs.md#batchputpropertyerrorentrytypedef)
- [BatchPutPropertyValuesResponseTypeDef](./type_defs.md#batchputpropertyvaluesresponsetypedef)

