# Snowball module

> [Index](../README.md) > Snowball


!!! note ""

    Auto-generated documentation for [Snowball](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#snowball)
    type annotations stubs module [types-aiobotocore-snowball](https://pypi.org/project/types-aiobotocore-snowball/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `Snowball` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `Snowball` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[snowball]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[snowball]'

# standalone installation
python -m pip install types-aiobotocore-snowball
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-snowball
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SnowballClient

Type annotations and code completion for  `#!python session.client("snowball")` as [SnowballClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client)

```python
# SnowballClient usage example

from aioboto3.session import Session

from types_aiobotocore_snowball.client import SnowballClient


session = Session()
async with session.client("snowball") as client:
    client: SnowballClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("snowball").get_paginator("...")`.

```python
# DescribeAddressesPaginator usage example

from types_aiobotocore_snowball.paginator import DescribeAddressesPaginator

def get_describe_addresses_paginator() -> DescribeAddressesPaginator:
    return client.get_paginator("describe_addresses"))
```

- [DescribeAddressesPaginator](./paginators.md#describeaddressespaginator)
- [ListClusterJobsPaginator](./paginators.md#listclusterjobspaginator)
- [ListClustersPaginator](./paginators.md#listclusterspaginator)
- [ListCompatibleImagesPaginator](./paginators.md#listcompatibleimagespaginator)
- [ListJobsPaginator](./paginators.md#listjobspaginator)
- [ListLongTermPricingPaginator](./paginators.md#listlongtermpricingpaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AddressTypeType usage example

from types_aiobotocore_snowball.literals import AddressTypeType

def get_value() -> AddressTypeType:
    return "AWS_SHIP"
```

- [AddressTypeType](./literals.md#addresstypetype)
- [ClusterStateType](./literals.md#clusterstatetype)
- [DescribeAddressesPaginatorName](./literals.md#describeaddressespaginatorname)
- [DeviceServiceNameType](./literals.md#deviceservicenametype)
- [ImpactLevelType](./literals.md#impactleveltype)
- [JobStateType](./literals.md#jobstatetype)
- [JobTypeType](./literals.md#jobtypetype)
- [ListClusterJobsPaginatorName](./literals.md#listclusterjobspaginatorname)
- [ListClustersPaginatorName](./literals.md#listclusterspaginatorname)
- [ListCompatibleImagesPaginatorName](./literals.md#listcompatibleimagespaginatorname)
- [ListJobsPaginatorName](./literals.md#listjobspaginatorname)
- [ListLongTermPricingPaginatorName](./literals.md#listlongtermpricingpaginatorname)
- [LongTermPricingTypeType](./literals.md#longtermpricingtypetype)
- [RemoteManagementType](./literals.md#remotemanagementtype)
- [ServiceNameType](./literals.md#servicenametype)
- [ShipmentStateType](./literals.md#shipmentstatetype)
- [ShippingLabelStatusType](./literals.md#shippinglabelstatustype)
- [ShippingOptionType](./literals.md#shippingoptiontype)
- [SnowballCapacityType](./literals.md#snowballcapacitytype)
- [SnowballTypeType](./literals.md#snowballtypetype)
- [StorageUnitType](./literals.md#storageunittype)
- [TransferOptionType](./literals.md#transferoptiontype)
- [SnowballServiceName](./literals.md#snowballservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AddressTypeDef](./type_defs.md#addresstypedef)
- [CancelClusterRequestRequestTypeDef](./type_defs.md#cancelclusterrequestrequesttypedef)
- [CancelJobRequestRequestTypeDef](./type_defs.md#canceljobrequestrequesttypedef)
- [ClusterListEntryTypeDef](./type_defs.md#clusterlistentrytypedef)
- [NotificationOutputTypeDef](./type_defs.md#notificationoutputtypedef)
- [CompatibleImageTypeDef](./type_defs.md#compatibleimagetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [NotificationTypeDef](./type_defs.md#notificationtypedef)
- [JobListEntryTypeDef](./type_defs.md#joblistentrytypedef)
- [CreateLongTermPricingRequestRequestTypeDef](./type_defs.md#createlongtermpricingrequestrequesttypedef)
- [CreateReturnShippingLabelRequestRequestTypeDef](./type_defs.md#createreturnshippinglabelrequestrequesttypedef)
- [DataTransferTypeDef](./type_defs.md#datatransfertypedef)
- [ServiceVersionTypeDef](./type_defs.md#serviceversiontypedef)
- [DescribeAddressRequestRequestTypeDef](./type_defs.md#describeaddressrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeAddressesRequestRequestTypeDef](./type_defs.md#describeaddressesrequestrequesttypedef)
- [DescribeClusterRequestRequestTypeDef](./type_defs.md#describeclusterrequestrequesttypedef)
- [DescribeJobRequestRequestTypeDef](./type_defs.md#describejobrequestrequesttypedef)
- [DescribeReturnShippingLabelRequestRequestTypeDef](./type_defs.md#describereturnshippinglabelrequestrequesttypedef)
- [EKSOnDeviceServiceConfigurationTypeDef](./type_defs.md#eksondeviceserviceconfigurationtypedef)
- [Ec2AmiResourceTypeDef](./type_defs.md#ec2amiresourcetypedef)
- [EventTriggerDefinitionTypeDef](./type_defs.md#eventtriggerdefinitiontypedef)
- [GetJobManifestRequestRequestTypeDef](./type_defs.md#getjobmanifestrequestrequesttypedef)
- [GetJobUnlockCodeRequestRequestTypeDef](./type_defs.md#getjobunlockcoderequestrequesttypedef)
- [GetSoftwareUpdatesRequestRequestTypeDef](./type_defs.md#getsoftwareupdatesrequestrequesttypedef)
- [INDTaxDocumentsTypeDef](./type_defs.md#indtaxdocumentstypedef)
- [JobLogsTypeDef](./type_defs.md#joblogstypedef)
- [PickupDetailsOutputTypeDef](./type_defs.md#pickupdetailsoutputtypedef)
- [KeyRangeTypeDef](./type_defs.md#keyrangetypedef)
- [ListClusterJobsRequestRequestTypeDef](./type_defs.md#listclusterjobsrequestrequesttypedef)
- [ListClustersRequestRequestTypeDef](./type_defs.md#listclustersrequestrequesttypedef)
- [ListCompatibleImagesRequestRequestTypeDef](./type_defs.md#listcompatibleimagesrequestrequesttypedef)
- [ListJobsRequestRequestTypeDef](./type_defs.md#listjobsrequestrequesttypedef)
- [ListLongTermPricingRequestRequestTypeDef](./type_defs.md#listlongtermpricingrequestrequesttypedef)
- [LongTermPricingListEntryTypeDef](./type_defs.md#longtermpricinglistentrytypedef)
- [ListPickupLocationsRequestRequestTypeDef](./type_defs.md#listpickuplocationsrequestrequesttypedef)
- [NFSOnDeviceServiceConfigurationTypeDef](./type_defs.md#nfsondeviceserviceconfigurationtypedef)
- [S3OnDeviceServiceConfigurationTypeDef](./type_defs.md#s3ondeviceserviceconfigurationtypedef)
- [TGWOnDeviceServiceConfigurationTypeDef](./type_defs.md#tgwondeviceserviceconfigurationtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [TargetOnDeviceServiceTypeDef](./type_defs.md#targetondeviceservicetypedef)
- [ShipmentTypeDef](./type_defs.md#shipmenttypedef)
- [WirelessConnectionTypeDef](./type_defs.md#wirelessconnectiontypedef)
- [UpdateJobShipmentStateRequestRequestTypeDef](./type_defs.md#updatejobshipmentstaterequestrequesttypedef)
- [UpdateLongTermPricingRequestRequestTypeDef](./type_defs.md#updatelongtermpricingrequestrequesttypedef)
- [CreateAddressRequestRequestTypeDef](./type_defs.md#createaddressrequestrequesttypedef)
- [CreateAddressResultTypeDef](./type_defs.md#createaddressresulttypedef)
- [CreateJobResultTypeDef](./type_defs.md#createjobresulttypedef)
- [CreateLongTermPricingResultTypeDef](./type_defs.md#createlongtermpricingresulttypedef)
- [CreateReturnShippingLabelResultTypeDef](./type_defs.md#createreturnshippinglabelresulttypedef)
- [DescribeAddressResultTypeDef](./type_defs.md#describeaddressresulttypedef)
- [DescribeAddressesResultTypeDef](./type_defs.md#describeaddressesresulttypedef)
- [DescribeReturnShippingLabelResultTypeDef](./type_defs.md#describereturnshippinglabelresulttypedef)
- [GetJobManifestResultTypeDef](./type_defs.md#getjobmanifestresulttypedef)
- [GetJobUnlockCodeResultTypeDef](./type_defs.md#getjobunlockcoderesulttypedef)
- [GetSnowballUsageResultTypeDef](./type_defs.md#getsnowballusageresulttypedef)
- [GetSoftwareUpdatesResultTypeDef](./type_defs.md#getsoftwareupdatesresulttypedef)
- [ListClustersResultTypeDef](./type_defs.md#listclustersresulttypedef)
- [ListCompatibleImagesResultTypeDef](./type_defs.md#listcompatibleimagesresulttypedef)
- [ListPickupLocationsResultTypeDef](./type_defs.md#listpickuplocationsresulttypedef)
- [CreateClusterResultTypeDef](./type_defs.md#createclusterresulttypedef)
- [ListClusterJobsResultTypeDef](./type_defs.md#listclusterjobsresulttypedef)
- [ListJobsResultTypeDef](./type_defs.md#listjobsresulttypedef)
- [DependentServiceTypeDef](./type_defs.md#dependentservicetypedef)
- [DescribeAddressesRequestPaginateTypeDef](./type_defs.md#describeaddressesrequestpaginatetypedef)
- [ListClusterJobsRequestPaginateTypeDef](./type_defs.md#listclusterjobsrequestpaginatetypedef)
- [ListClustersRequestPaginateTypeDef](./type_defs.md#listclustersrequestpaginatetypedef)
- [ListCompatibleImagesRequestPaginateTypeDef](./type_defs.md#listcompatibleimagesrequestpaginatetypedef)
- [ListJobsRequestPaginateTypeDef](./type_defs.md#listjobsrequestpaginatetypedef)
- [ListLongTermPricingRequestPaginateTypeDef](./type_defs.md#listlongtermpricingrequestpaginatetypedef)
- [LambdaResourceOutputTypeDef](./type_defs.md#lambdaresourceoutputtypedef)
- [LambdaResourceTypeDef](./type_defs.md#lambdaresourcetypedef)
- [TaxDocumentsTypeDef](./type_defs.md#taxdocumentstypedef)
- [ListLongTermPricingResultTypeDef](./type_defs.md#listlongtermpricingresulttypedef)
- [OnDeviceServiceConfigurationTypeDef](./type_defs.md#ondeviceserviceconfigurationtypedef)
- [PickupDetailsTypeDef](./type_defs.md#pickupdetailstypedef)
- [S3ResourceOutputTypeDef](./type_defs.md#s3resourceoutputtypedef)
- [S3ResourceTypeDef](./type_defs.md#s3resourcetypedef)
- [ShippingDetailsTypeDef](./type_defs.md#shippingdetailstypedef)
- [SnowconeDeviceConfigurationTypeDef](./type_defs.md#snowconedeviceconfigurationtypedef)
- [ListServiceVersionsRequestRequestTypeDef](./type_defs.md#listserviceversionsrequestrequesttypedef)
- [ListServiceVersionsResultTypeDef](./type_defs.md#listserviceversionsresulttypedef)
- [LambdaResourceUnionTypeDef](./type_defs.md#lambdaresourceuniontypedef)
- [JobResourceOutputTypeDef](./type_defs.md#jobresourceoutputtypedef)
- [S3ResourceUnionTypeDef](./type_defs.md#s3resourceuniontypedef)
- [DeviceConfigurationTypeDef](./type_defs.md#deviceconfigurationtypedef)
- [ClusterMetadataTypeDef](./type_defs.md#clustermetadatatypedef)
- [JobResourceTypeDef](./type_defs.md#jobresourcetypedef)
- [JobMetadataTypeDef](./type_defs.md#jobmetadatatypedef)
- [DescribeClusterResultTypeDef](./type_defs.md#describeclusterresulttypedef)
- [CreateClusterRequestRequestTypeDef](./type_defs.md#createclusterrequestrequesttypedef)
- [CreateJobRequestRequestTypeDef](./type_defs.md#createjobrequestrequesttypedef)
- [UpdateClusterRequestRequestTypeDef](./type_defs.md#updateclusterrequestrequesttypedef)
- [UpdateJobRequestRequestTypeDef](./type_defs.md#updatejobrequestrequesttypedef)
- [DescribeJobResultTypeDef](./type_defs.md#describejobresulttypedef)
