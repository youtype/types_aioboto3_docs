# FSxClient

> [Index](../README.md) > [FSx](./README.md) > FSxClient

!!! note ""

    Auto-generated documentation for [FSx](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#fsx)
    type annotations stubs module [types-aiobotocore-fsx](https://pypi.org/project/types-aiobotocore-fsx/).

## FSxClient

Type annotations and code completion for `#!python session.client("fsx")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# FSxClient usage example

from aioboto3.session import Session
from types_aiobotocore_fsx.client import FSxClient

session = Session()
async with session.client("fsx") as client:
    client: FSxClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("fsx").exceptions` structure.

```python
# FSxClient.exceptions usage example

async with session.client("fsx") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ActiveDirectoryError,
        client.exceptions.BackupBeingCopied,
        client.exceptions.BackupInProgress,
        client.exceptions.BackupNotFound,
        client.exceptions.BackupRestoring,
        client.exceptions.BadRequest,
        client.exceptions.ClientError,
        client.exceptions.DataRepositoryAssociationNotFound,
        client.exceptions.DataRepositoryTaskEnded,
        client.exceptions.DataRepositoryTaskExecuting,
        client.exceptions.DataRepositoryTaskNotFound,
        client.exceptions.FileCacheNotFound,
        client.exceptions.FileSystemNotFound,
        client.exceptions.IncompatibleParameterError,
        client.exceptions.IncompatibleRegionForMultiAZ,
        client.exceptions.InternalServerError,
        client.exceptions.InvalidDataRepositoryType,
        client.exceptions.InvalidDestinationKmsKey,
        client.exceptions.InvalidExportPath,
        client.exceptions.InvalidImportPath,
        client.exceptions.InvalidNetworkSettings,
        client.exceptions.InvalidPerUnitStorageThroughput,
        client.exceptions.InvalidRegion,
        client.exceptions.InvalidSourceKmsKey,
        client.exceptions.MissingFileCacheConfiguration,
        client.exceptions.MissingFileSystemConfiguration,
        client.exceptions.MissingVolumeConfiguration,
        client.exceptions.NotServiceResourceError,
        client.exceptions.ResourceDoesNotSupportTagging,
        client.exceptions.ResourceNotFound,
        client.exceptions.ServiceLimitExceeded,
        client.exceptions.SnapshotNotFound,
        client.exceptions.SourceBackupUnavailable,
        client.exceptions.StorageVirtualMachineNotFound,
        client.exceptions.UnsupportedOperation,
        client.exceptions.VolumeNotFound,
    ) as e:
        print(e)
```

```python
# FSxClient.exceptions type checking example

from types_aiobotocore_fsx.client import Exceptions

def handle_error(exc: Exceptions.ActiveDirectoryError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("fsx").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("fsx").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

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


### associate\_file\_system\_aliases

Use this action to associate one or more Domain Name Server (DNS) aliases with
an existing Amazon FSx for Windows File Server file system.

Type annotations and code completion for `#!python session.client("fsx").associate_file_system_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# associate_file_system_aliases method definition

await def associate_file_system_aliases(
    self,
    *,
    FileSystemId: str,
    Aliases: Sequence[str],
    ClientRequestToken: str = ...,
) -> AssociateFileSystemAliasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateFileSystemAliasesResponseTypeDef](./type_defs.md#associatefilesystemaliasesresponsetypedef) 


```python
# associate_file_system_aliases method usage example with argument unpacking

kwargs: AssociateFileSystemAliasesRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
    "Aliases": ...,
}

parent.associate_file_system_aliases(**kwargs)
```

1. See [:material-code-braces: AssociateFileSystemAliasesRequestRequestTypeDef](./type_defs.md#associatefilesystemaliasesrequestrequesttypedef) 

### cancel\_data\_repository\_task

Cancels an existing Amazon FSx for Lustre data repository task if that task is
in either the <code>PENDING</code> or <code>EXECUTING</code> state.

Type annotations and code completion for `#!python session.client("fsx").cancel_data_repository_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# cancel_data_repository_task method definition

await def cancel_data_repository_task(
    self,
    *,
    TaskId: str,
) -> CancelDataRepositoryTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelDataRepositoryTaskResponseTypeDef](./type_defs.md#canceldatarepositorytaskresponsetypedef) 


```python
# cancel_data_repository_task method usage example with argument unpacking

kwargs: CancelDataRepositoryTaskRequestRequestTypeDef = {  # (1)
    "TaskId": ...,
}

parent.cancel_data_repository_task(**kwargs)
```

1. See [:material-code-braces: CancelDataRepositoryTaskRequestRequestTypeDef](./type_defs.md#canceldatarepositorytaskrequestrequesttypedef) 

### copy\_backup

Copies an existing backup within the same Amazon Web Services account to
another Amazon Web Services Region (cross-Region copy) or within the same
Amazon Web Services Region (in-Region copy).

Type annotations and code completion for `#!python session.client("fsx").copy_backup` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# copy_backup method definition

await def copy_backup(
    self,
    *,
    SourceBackupId: str,
    ClientRequestToken: str = ...,
    SourceRegion: str = ...,
    KmsKeyId: str = ...,
    CopyTags: bool = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CopyBackupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CopyBackupResponseTypeDef](./type_defs.md#copybackupresponsetypedef) 


```python
# copy_backup method usage example with argument unpacking

kwargs: CopyBackupRequestRequestTypeDef = {  # (1)
    "SourceBackupId": ...,
}

parent.copy_backup(**kwargs)
```

1. See [:material-code-braces: CopyBackupRequestRequestTypeDef](./type_defs.md#copybackuprequestrequesttypedef) 

### copy\_snapshot\_and\_update\_volume

Updates an existing volume by using a snapshot from another Amazon FSx for
OpenZFS file system.

Type annotations and code completion for `#!python session.client("fsx").copy_snapshot_and_update_volume` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# copy_snapshot_and_update_volume method definition

await def copy_snapshot_and_update_volume(
    self,
    *,
    VolumeId: str,
    SourceSnapshotARN: str,
    ClientRequestToken: str = ...,
    CopyStrategy: OpenZFSCopyStrategyType = ...,  # (1)
    Options: Sequence[UpdateOpenZFSVolumeOptionType] = ...,  # (2)
) -> CopySnapshotAndUpdateVolumeResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: OpenZFSCopyStrategyType](./literals.md#openzfscopystrategytype) 
2. See [:material-code-brackets: UpdateOpenZFSVolumeOptionType](./literals.md#updateopenzfsvolumeoptiontype) 
3. See [:material-code-braces: CopySnapshotAndUpdateVolumeResponseTypeDef](./type_defs.md#copysnapshotandupdatevolumeresponsetypedef) 


```python
# copy_snapshot_and_update_volume method usage example with argument unpacking

kwargs: CopySnapshotAndUpdateVolumeRequestRequestTypeDef = {  # (1)
    "VolumeId": ...,
    "SourceSnapshotARN": ...,
}

parent.copy_snapshot_and_update_volume(**kwargs)
```

1. See [:material-code-braces: CopySnapshotAndUpdateVolumeRequestRequestTypeDef](./type_defs.md#copysnapshotandupdatevolumerequestrequesttypedef) 

### create\_backup

Creates a backup of an existing Amazon FSx for Windows File Server file system,
Amazon FSx for Lustre file system, Amazon FSx for NetApp ONTAP volume, or
Amazon FSx for OpenZFS file system.

Type annotations and code completion for `#!python session.client("fsx").create_backup` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# create_backup method definition

await def create_backup(
    self,
    *,
    FileSystemId: str = ...,
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    VolumeId: str = ...,
) -> CreateBackupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateBackupResponseTypeDef](./type_defs.md#createbackupresponsetypedef) 


```python
# create_backup method usage example with argument unpacking

kwargs: CreateBackupRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
}

parent.create_backup(**kwargs)
```

1. See [:material-code-braces: CreateBackupRequestRequestTypeDef](./type_defs.md#createbackuprequestrequesttypedef) 

### create\_data\_repository\_association

Creates an Amazon FSx for Lustre data repository association (DRA).

Type annotations and code completion for `#!python session.client("fsx").create_data_repository_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# create_data_repository_association method definition

await def create_data_repository_association(
    self,
    *,
    FileSystemId: str,
    DataRepositoryPath: str,
    FileSystemPath: str = ...,
    BatchImportMetaDataOnCreate: bool = ...,
    ImportedFileChunkSize: int = ...,
    S3: S3DataRepositoryConfigurationTypeDef = ...,  # (1)
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateDataRepositoryAssociationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: S3DataRepositoryConfigurationTypeDef](./type_defs.md#s3datarepositoryconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateDataRepositoryAssociationResponseTypeDef](./type_defs.md#createdatarepositoryassociationresponsetypedef) 


```python
# create_data_repository_association method usage example with argument unpacking

kwargs: CreateDataRepositoryAssociationRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
    "DataRepositoryPath": ...,
}

parent.create_data_repository_association(**kwargs)
```

1. See [:material-code-braces: CreateDataRepositoryAssociationRequestRequestTypeDef](./type_defs.md#createdatarepositoryassociationrequestrequesttypedef) 

### create\_data\_repository\_task

Creates an Amazon FSx for Lustre data repository task.

Type annotations and code completion for `#!python session.client("fsx").create_data_repository_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# create_data_repository_task method definition

await def create_data_repository_task(
    self,
    *,
    Type: DataRepositoryTaskTypeType,  # (1)
    FileSystemId: str,
    Report: CompletionReportTypeDef,  # (2)
    Paths: Sequence[str] = ...,
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    CapacityToRelease: int = ...,
    ReleaseConfiguration: ReleaseConfigurationTypeDef = ...,  # (4)
) -> CreateDataRepositoryTaskResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: DataRepositoryTaskTypeType](./literals.md#datarepositorytasktypetype) 
2. See [:material-code-braces: CompletionReportTypeDef](./type_defs.md#completionreporttypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: ReleaseConfigurationTypeDef](./type_defs.md#releaseconfigurationtypedef) 
5. See [:material-code-braces: CreateDataRepositoryTaskResponseTypeDef](./type_defs.md#createdatarepositorytaskresponsetypedef) 


```python
# create_data_repository_task method usage example with argument unpacking

kwargs: CreateDataRepositoryTaskRequestRequestTypeDef = {  # (1)
    "Type": ...,
    "FileSystemId": ...,
    "Report": ...,
}

parent.create_data_repository_task(**kwargs)
```

1. See [:material-code-braces: CreateDataRepositoryTaskRequestRequestTypeDef](./type_defs.md#createdatarepositorytaskrequestrequesttypedef) 

### create\_file\_cache

Creates a new Amazon File Cache resource.

Type annotations and code completion for `#!python session.client("fsx").create_file_cache` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# create_file_cache method definition

await def create_file_cache(
    self,
    *,
    FileCacheType: FileCacheTypeType,  # (1)
    FileCacheTypeVersion: str,
    StorageCapacity: int,
    SubnetIds: Sequence[str],
    ClientRequestToken: str = ...,
    SecurityGroupIds: Sequence[str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    CopyTagsToDataRepositoryAssociations: bool = ...,
    KmsKeyId: str = ...,
    LustreConfiguration: CreateFileCacheLustreConfigurationTypeDef = ...,  # (3)
    DataRepositoryAssociations: Sequence[FileCacheDataRepositoryAssociationTypeDef] = ...,  # (4)
) -> CreateFileCacheResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: FileCacheTypeType](./literals.md#filecachetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateFileCacheLustreConfigurationTypeDef](./type_defs.md#createfilecachelustreconfigurationtypedef) 
4. See [:material-code-braces: FileCacheDataRepositoryAssociationTypeDef](./type_defs.md#filecachedatarepositoryassociationtypedef) 
5. See [:material-code-braces: CreateFileCacheResponseTypeDef](./type_defs.md#createfilecacheresponsetypedef) 


```python
# create_file_cache method usage example with argument unpacking

kwargs: CreateFileCacheRequestRequestTypeDef = {  # (1)
    "FileCacheType": ...,
    "FileCacheTypeVersion": ...,
    "StorageCapacity": ...,
    "SubnetIds": ...,
}

parent.create_file_cache(**kwargs)
```

1. See [:material-code-braces: CreateFileCacheRequestRequestTypeDef](./type_defs.md#createfilecacherequestrequesttypedef) 

### create\_file\_system

Creates a new, empty Amazon FSx file system.

Type annotations and code completion for `#!python session.client("fsx").create_file_system` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# create_file_system method definition

await def create_file_system(
    self,
    *,
    FileSystemType: FileSystemTypeType,  # (1)
    SubnetIds: Sequence[str],
    ClientRequestToken: str = ...,
    StorageCapacity: int = ...,
    StorageType: StorageTypeType = ...,  # (2)
    SecurityGroupIds: Sequence[str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    KmsKeyId: str = ...,
    WindowsConfiguration: CreateFileSystemWindowsConfigurationTypeDef = ...,  # (4)
    LustreConfiguration: CreateFileSystemLustreConfigurationTypeDef = ...,  # (5)
    OntapConfiguration: CreateFileSystemOntapConfigurationTypeDef = ...,  # (6)
    FileSystemTypeVersion: str = ...,
    OpenZFSConfiguration: CreateFileSystemOpenZFSConfigurationTypeDef = ...,  # (7)
) -> CreateFileSystemResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-brackets: FileSystemTypeType](./literals.md#filesystemtypetype) 
2. See [:material-code-brackets: StorageTypeType](./literals.md#storagetypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateFileSystemWindowsConfigurationTypeDef](./type_defs.md#createfilesystemwindowsconfigurationtypedef) 
5. See [:material-code-braces: CreateFileSystemLustreConfigurationTypeDef](./type_defs.md#createfilesystemlustreconfigurationtypedef) 
6. See [:material-code-braces: CreateFileSystemOntapConfigurationTypeDef](./type_defs.md#createfilesystemontapconfigurationtypedef) 
7. See [:material-code-braces: CreateFileSystemOpenZFSConfigurationTypeDef](./type_defs.md#createfilesystemopenzfsconfigurationtypedef) 
8. See [:material-code-braces: CreateFileSystemResponseTypeDef](./type_defs.md#createfilesystemresponsetypedef) 


```python
# create_file_system method usage example with argument unpacking

kwargs: CreateFileSystemRequestRequestTypeDef = {  # (1)
    "FileSystemType": ...,
    "SubnetIds": ...,
}

parent.create_file_system(**kwargs)
```

1. See [:material-code-braces: CreateFileSystemRequestRequestTypeDef](./type_defs.md#createfilesystemrequestrequesttypedef) 

### create\_file\_system\_from\_backup

Creates a new Amazon FSx for Lustre, Amazon FSx for Windows File Server, or
Amazon FSx for OpenZFS file system from an existing Amazon FSx backup.

Type annotations and code completion for `#!python session.client("fsx").create_file_system_from_backup` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# create_file_system_from_backup method definition

await def create_file_system_from_backup(
    self,
    *,
    BackupId: str,
    SubnetIds: Sequence[str],
    ClientRequestToken: str = ...,
    SecurityGroupIds: Sequence[str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    WindowsConfiguration: CreateFileSystemWindowsConfigurationTypeDef = ...,  # (2)
    LustreConfiguration: CreateFileSystemLustreConfigurationTypeDef = ...,  # (3)
    StorageType: StorageTypeType = ...,  # (4)
    KmsKeyId: str = ...,
    FileSystemTypeVersion: str = ...,
    OpenZFSConfiguration: CreateFileSystemOpenZFSConfigurationTypeDef = ...,  # (5)
    StorageCapacity: int = ...,
) -> CreateFileSystemFromBackupResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateFileSystemWindowsConfigurationTypeDef](./type_defs.md#createfilesystemwindowsconfigurationtypedef) 
3. See [:material-code-braces: CreateFileSystemLustreConfigurationTypeDef](./type_defs.md#createfilesystemlustreconfigurationtypedef) 
4. See [:material-code-brackets: StorageTypeType](./literals.md#storagetypetype) 
5. See [:material-code-braces: CreateFileSystemOpenZFSConfigurationTypeDef](./type_defs.md#createfilesystemopenzfsconfigurationtypedef) 
6. See [:material-code-braces: CreateFileSystemFromBackupResponseTypeDef](./type_defs.md#createfilesystemfrombackupresponsetypedef) 


```python
# create_file_system_from_backup method usage example with argument unpacking

kwargs: CreateFileSystemFromBackupRequestRequestTypeDef = {  # (1)
    "BackupId": ...,
    "SubnetIds": ...,
}

parent.create_file_system_from_backup(**kwargs)
```

1. See [:material-code-braces: CreateFileSystemFromBackupRequestRequestTypeDef](./type_defs.md#createfilesystemfrombackuprequestrequesttypedef) 

### create\_snapshot

Creates a snapshot of an existing Amazon FSx for OpenZFS volume.

Type annotations and code completion for `#!python session.client("fsx").create_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# create_snapshot method definition

await def create_snapshot(
    self,
    *,
    Name: str,
    VolumeId: str,
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateSnapshotResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateSnapshotResponseTypeDef](./type_defs.md#createsnapshotresponsetypedef) 


```python
# create_snapshot method usage example with argument unpacking

kwargs: CreateSnapshotRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "VolumeId": ...,
}

parent.create_snapshot(**kwargs)
```

1. See [:material-code-braces: CreateSnapshotRequestRequestTypeDef](./type_defs.md#createsnapshotrequestrequesttypedef) 

### create\_storage\_virtual\_machine

Creates a storage virtual machine (SVM) for an Amazon FSx for ONTAP file system.

Type annotations and code completion for `#!python session.client("fsx").create_storage_virtual_machine` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# create_storage_virtual_machine method definition

await def create_storage_virtual_machine(
    self,
    *,
    FileSystemId: str,
    Name: str,
    ActiveDirectoryConfiguration: CreateSvmActiveDirectoryConfigurationTypeDef = ...,  # (1)
    ClientRequestToken: str = ...,
    SvmAdminPassword: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    RootVolumeSecurityStyle: StorageVirtualMachineRootVolumeSecurityStyleType = ...,  # (3)
) -> CreateStorageVirtualMachineResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: CreateSvmActiveDirectoryConfigurationTypeDef](./type_defs.md#createsvmactivedirectoryconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: StorageVirtualMachineRootVolumeSecurityStyleType](./literals.md#storagevirtualmachinerootvolumesecuritystyletype) 
4. See [:material-code-braces: CreateStorageVirtualMachineResponseTypeDef](./type_defs.md#createstoragevirtualmachineresponsetypedef) 


```python
# create_storage_virtual_machine method usage example with argument unpacking

kwargs: CreateStorageVirtualMachineRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
    "Name": ...,
}

parent.create_storage_virtual_machine(**kwargs)
```

1. See [:material-code-braces: CreateStorageVirtualMachineRequestRequestTypeDef](./type_defs.md#createstoragevirtualmachinerequestrequesttypedef) 

### create\_volume

Creates an FSx for ONTAP or Amazon FSx for OpenZFS storage volume.

Type annotations and code completion for `#!python session.client("fsx").create_volume` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# create_volume method definition

await def create_volume(
    self,
    *,
    VolumeType: VolumeTypeType,  # (1)
    Name: str,
    ClientRequestToken: str = ...,
    OntapConfiguration: CreateOntapVolumeConfigurationTypeDef = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    OpenZFSConfiguration: CreateOpenZFSVolumeConfigurationTypeDef = ...,  # (4)
) -> CreateVolumeResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: VolumeTypeType](./literals.md#volumetypetype) 
2. See [:material-code-braces: CreateOntapVolumeConfigurationTypeDef](./type_defs.md#createontapvolumeconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateOpenZFSVolumeConfigurationTypeDef](./type_defs.md#createopenzfsvolumeconfigurationtypedef) 
5. See [:material-code-braces: CreateVolumeResponseTypeDef](./type_defs.md#createvolumeresponsetypedef) 


```python
# create_volume method usage example with argument unpacking

kwargs: CreateVolumeRequestRequestTypeDef = {  # (1)
    "VolumeType": ...,
    "Name": ...,
}

parent.create_volume(**kwargs)
```

1. See [:material-code-braces: CreateVolumeRequestRequestTypeDef](./type_defs.md#createvolumerequestrequesttypedef) 

### create\_volume\_from\_backup

Creates a new Amazon FSx for NetApp ONTAP volume from an existing Amazon FSx
volume backup.

Type annotations and code completion for `#!python session.client("fsx").create_volume_from_backup` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# create_volume_from_backup method definition

await def create_volume_from_backup(
    self,
    *,
    BackupId: str,
    Name: str,
    ClientRequestToken: str = ...,
    OntapConfiguration: CreateOntapVolumeConfigurationTypeDef = ...,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateVolumeFromBackupResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: CreateOntapVolumeConfigurationTypeDef](./type_defs.md#createontapvolumeconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateVolumeFromBackupResponseTypeDef](./type_defs.md#createvolumefrombackupresponsetypedef) 


```python
# create_volume_from_backup method usage example with argument unpacking

kwargs: CreateVolumeFromBackupRequestRequestTypeDef = {  # (1)
    "BackupId": ...,
    "Name": ...,
}

parent.create_volume_from_backup(**kwargs)
```

1. See [:material-code-braces: CreateVolumeFromBackupRequestRequestTypeDef](./type_defs.md#createvolumefrombackuprequestrequesttypedef) 

### delete\_backup

Deletes an Amazon FSx backup.

Type annotations and code completion for `#!python session.client("fsx").delete_backup` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# delete_backup method definition

await def delete_backup(
    self,
    *,
    BackupId: str,
    ClientRequestToken: str = ...,
) -> DeleteBackupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteBackupResponseTypeDef](./type_defs.md#deletebackupresponsetypedef) 


```python
# delete_backup method usage example with argument unpacking

kwargs: DeleteBackupRequestRequestTypeDef = {  # (1)
    "BackupId": ...,
}

parent.delete_backup(**kwargs)
```

1. See [:material-code-braces: DeleteBackupRequestRequestTypeDef](./type_defs.md#deletebackuprequestrequesttypedef) 

### delete\_data\_repository\_association

Deletes a data repository association on an Amazon FSx for Lustre file system.

Type annotations and code completion for `#!python session.client("fsx").delete_data_repository_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# delete_data_repository_association method definition

await def delete_data_repository_association(
    self,
    *,
    AssociationId: str,
    ClientRequestToken: str = ...,
    DeleteDataInFileSystem: bool = ...,
) -> DeleteDataRepositoryAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDataRepositoryAssociationResponseTypeDef](./type_defs.md#deletedatarepositoryassociationresponsetypedef) 


```python
# delete_data_repository_association method usage example with argument unpacking

kwargs: DeleteDataRepositoryAssociationRequestRequestTypeDef = {  # (1)
    "AssociationId": ...,
}

parent.delete_data_repository_association(**kwargs)
```

1. See [:material-code-braces: DeleteDataRepositoryAssociationRequestRequestTypeDef](./type_defs.md#deletedatarepositoryassociationrequestrequesttypedef) 

### delete\_file\_cache

Deletes an Amazon File Cache resource.

Type annotations and code completion for `#!python session.client("fsx").delete_file_cache` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# delete_file_cache method definition

await def delete_file_cache(
    self,
    *,
    FileCacheId: str,
    ClientRequestToken: str = ...,
) -> DeleteFileCacheResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteFileCacheResponseTypeDef](./type_defs.md#deletefilecacheresponsetypedef) 


```python
# delete_file_cache method usage example with argument unpacking

kwargs: DeleteFileCacheRequestRequestTypeDef = {  # (1)
    "FileCacheId": ...,
}

parent.delete_file_cache(**kwargs)
```

1. See [:material-code-braces: DeleteFileCacheRequestRequestTypeDef](./type_defs.md#deletefilecacherequestrequesttypedef) 

### delete\_file\_system

Deletes a file system.

Type annotations and code completion for `#!python session.client("fsx").delete_file_system` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# delete_file_system method definition

await def delete_file_system(
    self,
    *,
    FileSystemId: str,
    ClientRequestToken: str = ...,
    WindowsConfiguration: DeleteFileSystemWindowsConfigurationTypeDef = ...,  # (1)
    LustreConfiguration: DeleteFileSystemLustreConfigurationTypeDef = ...,  # (2)
    OpenZFSConfiguration: DeleteFileSystemOpenZFSConfigurationTypeDef = ...,  # (3)
) -> DeleteFileSystemResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DeleteFileSystemWindowsConfigurationTypeDef](./type_defs.md#deletefilesystemwindowsconfigurationtypedef) 
2. See [:material-code-braces: DeleteFileSystemLustreConfigurationTypeDef](./type_defs.md#deletefilesystemlustreconfigurationtypedef) 
3. See [:material-code-braces: DeleteFileSystemOpenZFSConfigurationTypeDef](./type_defs.md#deletefilesystemopenzfsconfigurationtypedef) 
4. See [:material-code-braces: DeleteFileSystemResponseTypeDef](./type_defs.md#deletefilesystemresponsetypedef) 


```python
# delete_file_system method usage example with argument unpacking

kwargs: DeleteFileSystemRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
}

parent.delete_file_system(**kwargs)
```

1. See [:material-code-braces: DeleteFileSystemRequestRequestTypeDef](./type_defs.md#deletefilesystemrequestrequesttypedef) 

### delete\_snapshot

Deletes an Amazon FSx for OpenZFS snapshot.

Type annotations and code completion for `#!python session.client("fsx").delete_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# delete_snapshot method definition

await def delete_snapshot(
    self,
    *,
    SnapshotId: str,
    ClientRequestToken: str = ...,
) -> DeleteSnapshotResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteSnapshotResponseTypeDef](./type_defs.md#deletesnapshotresponsetypedef) 


```python
# delete_snapshot method usage example with argument unpacking

kwargs: DeleteSnapshotRequestRequestTypeDef = {  # (1)
    "SnapshotId": ...,
}

parent.delete_snapshot(**kwargs)
```

1. See [:material-code-braces: DeleteSnapshotRequestRequestTypeDef](./type_defs.md#deletesnapshotrequestrequesttypedef) 

### delete\_storage\_virtual\_machine

Deletes an existing Amazon FSx for ONTAP storage virtual machine (SVM).

Type annotations and code completion for `#!python session.client("fsx").delete_storage_virtual_machine` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# delete_storage_virtual_machine method definition

await def delete_storage_virtual_machine(
    self,
    *,
    StorageVirtualMachineId: str,
    ClientRequestToken: str = ...,
) -> DeleteStorageVirtualMachineResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteStorageVirtualMachineResponseTypeDef](./type_defs.md#deletestoragevirtualmachineresponsetypedef) 


```python
# delete_storage_virtual_machine method usage example with argument unpacking

kwargs: DeleteStorageVirtualMachineRequestRequestTypeDef = {  # (1)
    "StorageVirtualMachineId": ...,
}

parent.delete_storage_virtual_machine(**kwargs)
```

1. See [:material-code-braces: DeleteStorageVirtualMachineRequestRequestTypeDef](./type_defs.md#deletestoragevirtualmachinerequestrequesttypedef) 

### delete\_volume

Deletes an Amazon FSx for NetApp ONTAP or Amazon FSx for OpenZFS volume.

Type annotations and code completion for `#!python session.client("fsx").delete_volume` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# delete_volume method definition

await def delete_volume(
    self,
    *,
    VolumeId: str,
    ClientRequestToken: str = ...,
    OntapConfiguration: DeleteVolumeOntapConfigurationTypeDef = ...,  # (1)
    OpenZFSConfiguration: DeleteVolumeOpenZFSConfigurationTypeDef = ...,  # (2)
) -> DeleteVolumeResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DeleteVolumeOntapConfigurationTypeDef](./type_defs.md#deletevolumeontapconfigurationtypedef) 
2. See [:material-code-braces: DeleteVolumeOpenZFSConfigurationTypeDef](./type_defs.md#deletevolumeopenzfsconfigurationtypedef) 
3. See [:material-code-braces: DeleteVolumeResponseTypeDef](./type_defs.md#deletevolumeresponsetypedef) 


```python
# delete_volume method usage example with argument unpacking

kwargs: DeleteVolumeRequestRequestTypeDef = {  # (1)
    "VolumeId": ...,
}

parent.delete_volume(**kwargs)
```

1. See [:material-code-braces: DeleteVolumeRequestRequestTypeDef](./type_defs.md#deletevolumerequestrequesttypedef) 

### describe\_backups

Returns the description of a specific Amazon FSx backup, if a
<code>BackupIds</code> value is provided for that backup.

Type annotations and code completion for `#!python session.client("fsx").describe_backups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# describe_backups method definition

await def describe_backups(
    self,
    *,
    BackupIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeBackupsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeBackupsResponseTypeDef](./type_defs.md#describebackupsresponsetypedef) 


```python
# describe_backups method usage example with argument unpacking

kwargs: DescribeBackupsRequestRequestTypeDef = {  # (1)
    "BackupIds": ...,
}

parent.describe_backups(**kwargs)
```

1. See [:material-code-braces: DescribeBackupsRequestRequestTypeDef](./type_defs.md#describebackupsrequestrequesttypedef) 

### describe\_data\_repository\_associations

Returns the description of specific Amazon FSx for Lustre or Amazon File Cache
data repository associations, if one or more <code>AssociationIds</code> values
are provided in the request, or if filters are used in the request.

Type annotations and code completion for `#!python session.client("fsx").describe_data_repository_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# describe_data_repository_associations method definition

await def describe_data_repository_associations(
    self,
    *,
    AssociationIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeDataRepositoryAssociationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeDataRepositoryAssociationsResponseTypeDef](./type_defs.md#describedatarepositoryassociationsresponsetypedef) 


```python
# describe_data_repository_associations method usage example with argument unpacking

kwargs: DescribeDataRepositoryAssociationsRequestRequestTypeDef = {  # (1)
    "AssociationIds": ...,
}

parent.describe_data_repository_associations(**kwargs)
```

1. See [:material-code-braces: DescribeDataRepositoryAssociationsRequestRequestTypeDef](./type_defs.md#describedatarepositoryassociationsrequestrequesttypedef) 

### describe\_data\_repository\_tasks

Returns the description of specific Amazon FSx for Lustre or Amazon File Cache
data repository tasks, if one or more <code>TaskIds</code> values are provided
in the request, or if filters are used in the request.

Type annotations and code completion for `#!python session.client("fsx").describe_data_repository_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# describe_data_repository_tasks method definition

await def describe_data_repository_tasks(
    self,
    *,
    TaskIds: Sequence[str] = ...,
    Filters: Sequence[DataRepositoryTaskFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeDataRepositoryTasksResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DataRepositoryTaskFilterTypeDef](./type_defs.md#datarepositorytaskfiltertypedef) 
2. See [:material-code-braces: DescribeDataRepositoryTasksResponseTypeDef](./type_defs.md#describedatarepositorytasksresponsetypedef) 


```python
# describe_data_repository_tasks method usage example with argument unpacking

kwargs: DescribeDataRepositoryTasksRequestRequestTypeDef = {  # (1)
    "TaskIds": ...,
}

parent.describe_data_repository_tasks(**kwargs)
```

1. See [:material-code-braces: DescribeDataRepositoryTasksRequestRequestTypeDef](./type_defs.md#describedatarepositorytasksrequestrequesttypedef) 

### describe\_file\_caches

Returns the description of a specific Amazon File Cache resource, if a
<code>FileCacheIds</code> value is provided for that cache.

Type annotations and code completion for `#!python session.client("fsx").describe_file_caches` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# describe_file_caches method definition

await def describe_file_caches(
    self,
    *,
    FileCacheIds: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeFileCachesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFileCachesResponseTypeDef](./type_defs.md#describefilecachesresponsetypedef) 


```python
# describe_file_caches method usage example with argument unpacking

kwargs: DescribeFileCachesRequestRequestTypeDef = {  # (1)
    "FileCacheIds": ...,
}

parent.describe_file_caches(**kwargs)
```

1. See [:material-code-braces: DescribeFileCachesRequestRequestTypeDef](./type_defs.md#describefilecachesrequestrequesttypedef) 

### describe\_file\_system\_aliases

Returns the DNS aliases that are associated with the specified Amazon FSx for
Windows File Server file system.

Type annotations and code completion for `#!python session.client("fsx").describe_file_system_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# describe_file_system_aliases method definition

await def describe_file_system_aliases(
    self,
    *,
    FileSystemId: str,
    ClientRequestToken: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeFileSystemAliasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFileSystemAliasesResponseTypeDef](./type_defs.md#describefilesystemaliasesresponsetypedef) 


```python
# describe_file_system_aliases method usage example with argument unpacking

kwargs: DescribeFileSystemAliasesRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
}

parent.describe_file_system_aliases(**kwargs)
```

1. See [:material-code-braces: DescribeFileSystemAliasesRequestRequestTypeDef](./type_defs.md#describefilesystemaliasesrequestrequesttypedef) 

### describe\_file\_systems

Returns the description of specific Amazon FSx file systems, if a
<code>FileSystemIds</code> value is provided for that file system.

Type annotations and code completion for `#!python session.client("fsx").describe_file_systems` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# describe_file_systems method definition

await def describe_file_systems(
    self,
    *,
    FileSystemIds: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeFileSystemsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFileSystemsResponseTypeDef](./type_defs.md#describefilesystemsresponsetypedef) 


```python
# describe_file_systems method usage example with argument unpacking

kwargs: DescribeFileSystemsRequestRequestTypeDef = {  # (1)
    "FileSystemIds": ...,
}

parent.describe_file_systems(**kwargs)
```

1. See [:material-code-braces: DescribeFileSystemsRequestRequestTypeDef](./type_defs.md#describefilesystemsrequestrequesttypedef) 

### describe\_shared\_vpc\_configuration

Indicates whether participant accounts in your organization can create Amazon
FSx for NetApp ONTAP Multi-AZ file systems in subnets that are shared by a
virtual private cloud (VPC) owner.

Type annotations and code completion for `#!python session.client("fsx").describe_shared_vpc_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# describe_shared_vpc_configuration method definition

await def describe_shared_vpc_configuration(
    self,
) -> DescribeSharedVpcConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSharedVpcConfigurationResponseTypeDef](./type_defs.md#describesharedvpcconfigurationresponsetypedef) 

### describe\_snapshots

Returns the description of specific Amazon FSx for OpenZFS snapshots, if a
<code>SnapshotIds</code> value is provided.

Type annotations and code completion for `#!python session.client("fsx").describe_snapshots` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# describe_snapshots method definition

await def describe_snapshots(
    self,
    *,
    SnapshotIds: Sequence[str] = ...,
    Filters: Sequence[SnapshotFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
    IncludeShared: bool = ...,
) -> DescribeSnapshotsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SnapshotFilterTypeDef](./type_defs.md#snapshotfiltertypedef) 
2. See [:material-code-braces: DescribeSnapshotsResponseTypeDef](./type_defs.md#describesnapshotsresponsetypedef) 


```python
# describe_snapshots method usage example with argument unpacking

kwargs: DescribeSnapshotsRequestRequestTypeDef = {  # (1)
    "SnapshotIds": ...,
}

parent.describe_snapshots(**kwargs)
```

1. See [:material-code-braces: DescribeSnapshotsRequestRequestTypeDef](./type_defs.md#describesnapshotsrequestrequesttypedef) 

### describe\_storage\_virtual\_machines

Describes one or more Amazon FSx for NetApp ONTAP storage virtual machines
(SVMs).

Type annotations and code completion for `#!python session.client("fsx").describe_storage_virtual_machines` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# describe_storage_virtual_machines method definition

await def describe_storage_virtual_machines(
    self,
    *,
    StorageVirtualMachineIds: Sequence[str] = ...,
    Filters: Sequence[StorageVirtualMachineFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeStorageVirtualMachinesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StorageVirtualMachineFilterTypeDef](./type_defs.md#storagevirtualmachinefiltertypedef) 
2. See [:material-code-braces: DescribeStorageVirtualMachinesResponseTypeDef](./type_defs.md#describestoragevirtualmachinesresponsetypedef) 


```python
# describe_storage_virtual_machines method usage example with argument unpacking

kwargs: DescribeStorageVirtualMachinesRequestRequestTypeDef = {  # (1)
    "StorageVirtualMachineIds": ...,
}

parent.describe_storage_virtual_machines(**kwargs)
```

1. See [:material-code-braces: DescribeStorageVirtualMachinesRequestRequestTypeDef](./type_defs.md#describestoragevirtualmachinesrequestrequesttypedef) 

### describe\_volumes

Describes one or more Amazon FSx for NetApp ONTAP or Amazon FSx for OpenZFS
volumes.

Type annotations and code completion for `#!python session.client("fsx").describe_volumes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# describe_volumes method definition

await def describe_volumes(
    self,
    *,
    VolumeIds: Sequence[str] = ...,
    Filters: Sequence[VolumeFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeVolumesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VolumeFilterTypeDef](./type_defs.md#volumefiltertypedef) 
2. See [:material-code-braces: DescribeVolumesResponseTypeDef](./type_defs.md#describevolumesresponsetypedef) 


```python
# describe_volumes method usage example with argument unpacking

kwargs: DescribeVolumesRequestRequestTypeDef = {  # (1)
    "VolumeIds": ...,
}

parent.describe_volumes(**kwargs)
```

1. See [:material-code-braces: DescribeVolumesRequestRequestTypeDef](./type_defs.md#describevolumesrequestrequesttypedef) 

### disassociate\_file\_system\_aliases

Use this action to disassociate, or remove, one or more Domain Name Service
(DNS) aliases from an Amazon FSx for Windows File Server file system.

Type annotations and code completion for `#!python session.client("fsx").disassociate_file_system_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# disassociate_file_system_aliases method definition

await def disassociate_file_system_aliases(
    self,
    *,
    FileSystemId: str,
    Aliases: Sequence[str],
    ClientRequestToken: str = ...,
) -> DisassociateFileSystemAliasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisassociateFileSystemAliasesResponseTypeDef](./type_defs.md#disassociatefilesystemaliasesresponsetypedef) 


```python
# disassociate_file_system_aliases method usage example with argument unpacking

kwargs: DisassociateFileSystemAliasesRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
    "Aliases": ...,
}

parent.disassociate_file_system_aliases(**kwargs)
```

1. See [:material-code-braces: DisassociateFileSystemAliasesRequestRequestTypeDef](./type_defs.md#disassociatefilesystemaliasesrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists tags for Amazon FSx resources.

Type annotations and code completion for `#!python session.client("fsx").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### release\_file\_system\_nfs\_v3\_locks

Releases the file system lock from an Amazon FSx for OpenZFS file system.

Type annotations and code completion for `#!python session.client("fsx").release_file_system_nfs_v3_locks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# release_file_system_nfs_v3_locks method definition

await def release_file_system_nfs_v3_locks(
    self,
    *,
    FileSystemId: str,
    ClientRequestToken: str = ...,
) -> ReleaseFileSystemNfsV3LocksResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ReleaseFileSystemNfsV3LocksResponseTypeDef](./type_defs.md#releasefilesystemnfsv3locksresponsetypedef) 


```python
# release_file_system_nfs_v3_locks method usage example with argument unpacking

kwargs: ReleaseFileSystemNfsV3LocksRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
}

parent.release_file_system_nfs_v3_locks(**kwargs)
```

1. See [:material-code-braces: ReleaseFileSystemNfsV3LocksRequestRequestTypeDef](./type_defs.md#releasefilesystemnfsv3locksrequestrequesttypedef) 

### restore\_volume\_from\_snapshot

Returns an Amazon FSx for OpenZFS volume to the state saved by the specified
snapshot.

Type annotations and code completion for `#!python session.client("fsx").restore_volume_from_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# restore_volume_from_snapshot method definition

await def restore_volume_from_snapshot(
    self,
    *,
    VolumeId: str,
    SnapshotId: str,
    ClientRequestToken: str = ...,
    Options: Sequence[RestoreOpenZFSVolumeOptionType] = ...,  # (1)
) -> RestoreVolumeFromSnapshotResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RestoreOpenZFSVolumeOptionType](./literals.md#restoreopenzfsvolumeoptiontype) 
2. See [:material-code-braces: RestoreVolumeFromSnapshotResponseTypeDef](./type_defs.md#restorevolumefromsnapshotresponsetypedef) 


```python
# restore_volume_from_snapshot method usage example with argument unpacking

kwargs: RestoreVolumeFromSnapshotRequestRequestTypeDef = {  # (1)
    "VolumeId": ...,
    "SnapshotId": ...,
}

parent.restore_volume_from_snapshot(**kwargs)
```

1. See [:material-code-braces: RestoreVolumeFromSnapshotRequestRequestTypeDef](./type_defs.md#restorevolumefromsnapshotrequestrequesttypedef) 

### start\_misconfigured\_state\_recovery

After performing steps to repair the Active Directory configuration of an FSx
for Windows File Server file system, use this action to initiate the process of
Amazon FSx attempting to reconnect to the file system.

Type annotations and code completion for `#!python session.client("fsx").start_misconfigured_state_recovery` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# start_misconfigured_state_recovery method definition

await def start_misconfigured_state_recovery(
    self,
    *,
    FileSystemId: str,
    ClientRequestToken: str = ...,
) -> StartMisconfiguredStateRecoveryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartMisconfiguredStateRecoveryResponseTypeDef](./type_defs.md#startmisconfiguredstaterecoveryresponsetypedef) 


```python
# start_misconfigured_state_recovery method usage example with argument unpacking

kwargs: StartMisconfiguredStateRecoveryRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
}

parent.start_misconfigured_state_recovery(**kwargs)
```

1. See [:material-code-braces: StartMisconfiguredStateRecoveryRequestRequestTypeDef](./type_defs.md#startmisconfiguredstaterecoveryrequestrequesttypedef) 

### tag\_resource

Tags an Amazon FSx resource.

Type annotations and code completion for `#!python session.client("fsx").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

This action removes a tag from an Amazon FSx resource.

Type annotations and code completion for `#!python session.client("fsx").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_data\_repository\_association

Updates the configuration of an existing data repository association on an
Amazon FSx for Lustre file system.

Type annotations and code completion for `#!python session.client("fsx").update_data_repository_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# update_data_repository_association method definition

await def update_data_repository_association(
    self,
    *,
    AssociationId: str,
    ClientRequestToken: str = ...,
    ImportedFileChunkSize: int = ...,
    S3: S3DataRepositoryConfigurationTypeDef = ...,  # (1)
) -> UpdateDataRepositoryAssociationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: S3DataRepositoryConfigurationTypeDef](./type_defs.md#s3datarepositoryconfigurationtypedef) 
2. See [:material-code-braces: UpdateDataRepositoryAssociationResponseTypeDef](./type_defs.md#updatedatarepositoryassociationresponsetypedef) 


```python
# update_data_repository_association method usage example with argument unpacking

kwargs: UpdateDataRepositoryAssociationRequestRequestTypeDef = {  # (1)
    "AssociationId": ...,
}

parent.update_data_repository_association(**kwargs)
```

1. See [:material-code-braces: UpdateDataRepositoryAssociationRequestRequestTypeDef](./type_defs.md#updatedatarepositoryassociationrequestrequesttypedef) 

### update\_file\_cache

Updates the configuration of an existing Amazon File Cache resource.

Type annotations and code completion for `#!python session.client("fsx").update_file_cache` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# update_file_cache method definition

await def update_file_cache(
    self,
    *,
    FileCacheId: str,
    ClientRequestToken: str = ...,
    LustreConfiguration: UpdateFileCacheLustreConfigurationTypeDef = ...,  # (1)
) -> UpdateFileCacheResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UpdateFileCacheLustreConfigurationTypeDef](./type_defs.md#updatefilecachelustreconfigurationtypedef) 
2. See [:material-code-braces: UpdateFileCacheResponseTypeDef](./type_defs.md#updatefilecacheresponsetypedef) 


```python
# update_file_cache method usage example with argument unpacking

kwargs: UpdateFileCacheRequestRequestTypeDef = {  # (1)
    "FileCacheId": ...,
}

parent.update_file_cache(**kwargs)
```

1. See [:material-code-braces: UpdateFileCacheRequestRequestTypeDef](./type_defs.md#updatefilecacherequestrequesttypedef) 

### update\_file\_system

Use this operation to update the configuration of an existing Amazon FSx file
system.

Type annotations and code completion for `#!python session.client("fsx").update_file_system` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# update_file_system method definition

await def update_file_system(
    self,
    *,
    FileSystemId: str,
    ClientRequestToken: str = ...,
    StorageCapacity: int = ...,
    WindowsConfiguration: UpdateFileSystemWindowsConfigurationTypeDef = ...,  # (1)
    LustreConfiguration: UpdateFileSystemLustreConfigurationTypeDef = ...,  # (2)
    OntapConfiguration: UpdateFileSystemOntapConfigurationTypeDef = ...,  # (3)
    OpenZFSConfiguration: UpdateFileSystemOpenZFSConfigurationTypeDef = ...,  # (4)
    StorageType: StorageTypeType = ...,  # (5)
) -> UpdateFileSystemResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: UpdateFileSystemWindowsConfigurationTypeDef](./type_defs.md#updatefilesystemwindowsconfigurationtypedef) 
2. See [:material-code-braces: UpdateFileSystemLustreConfigurationTypeDef](./type_defs.md#updatefilesystemlustreconfigurationtypedef) 
3. See [:material-code-braces: UpdateFileSystemOntapConfigurationTypeDef](./type_defs.md#updatefilesystemontapconfigurationtypedef) 
4. See [:material-code-braces: UpdateFileSystemOpenZFSConfigurationTypeDef](./type_defs.md#updatefilesystemopenzfsconfigurationtypedef) 
5. See [:material-code-brackets: StorageTypeType](./literals.md#storagetypetype) 
6. See [:material-code-braces: UpdateFileSystemResponseTypeDef](./type_defs.md#updatefilesystemresponsetypedef) 


```python
# update_file_system method usage example with argument unpacking

kwargs: UpdateFileSystemRequestRequestTypeDef = {  # (1)
    "FileSystemId": ...,
}

parent.update_file_system(**kwargs)
```

1. See [:material-code-braces: UpdateFileSystemRequestRequestTypeDef](./type_defs.md#updatefilesystemrequestrequesttypedef) 

### update\_shared\_vpc\_configuration

Configures whether participant accounts in your organization can create Amazon
FSx for NetApp ONTAP Multi-AZ file systems in subnets that are shared by a
virtual private cloud (VPC) owner.

Type annotations and code completion for `#!python session.client("fsx").update_shared_vpc_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# update_shared_vpc_configuration method definition

await def update_shared_vpc_configuration(
    self,
    *,
    EnableFsxRouteTableUpdatesFromParticipantAccounts: str = ...,
    ClientRequestToken: str = ...,
) -> UpdateSharedVpcConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateSharedVpcConfigurationResponseTypeDef](./type_defs.md#updatesharedvpcconfigurationresponsetypedef) 


```python
# update_shared_vpc_configuration method usage example with argument unpacking

kwargs: UpdateSharedVpcConfigurationRequestRequestTypeDef = {  # (1)
    "EnableFsxRouteTableUpdatesFromParticipantAccounts": ...,
}

parent.update_shared_vpc_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateSharedVpcConfigurationRequestRequestTypeDef](./type_defs.md#updatesharedvpcconfigurationrequestrequesttypedef) 

### update\_snapshot

Updates the name of an Amazon FSx for OpenZFS snapshot.

Type annotations and code completion for `#!python session.client("fsx").update_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# update_snapshot method definition

await def update_snapshot(
    self,
    *,
    Name: str,
    SnapshotId: str,
    ClientRequestToken: str = ...,
) -> UpdateSnapshotResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateSnapshotResponseTypeDef](./type_defs.md#updatesnapshotresponsetypedef) 


```python
# update_snapshot method usage example with argument unpacking

kwargs: UpdateSnapshotRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "SnapshotId": ...,
}

parent.update_snapshot(**kwargs)
```

1. See [:material-code-braces: UpdateSnapshotRequestRequestTypeDef](./type_defs.md#updatesnapshotrequestrequesttypedef) 

### update\_storage\_virtual\_machine

Updates an FSx for ONTAP storage virtual machine (SVM).

Type annotations and code completion for `#!python session.client("fsx").update_storage_virtual_machine` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# update_storage_virtual_machine method definition

await def update_storage_virtual_machine(
    self,
    *,
    StorageVirtualMachineId: str,
    ActiveDirectoryConfiguration: UpdateSvmActiveDirectoryConfigurationTypeDef = ...,  # (1)
    ClientRequestToken: str = ...,
    SvmAdminPassword: str = ...,
) -> UpdateStorageVirtualMachineResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UpdateSvmActiveDirectoryConfigurationTypeDef](./type_defs.md#updatesvmactivedirectoryconfigurationtypedef) 
2. See [:material-code-braces: UpdateStorageVirtualMachineResponseTypeDef](./type_defs.md#updatestoragevirtualmachineresponsetypedef) 


```python
# update_storage_virtual_machine method usage example with argument unpacking

kwargs: UpdateStorageVirtualMachineRequestRequestTypeDef = {  # (1)
    "StorageVirtualMachineId": ...,
}

parent.update_storage_virtual_machine(**kwargs)
```

1. See [:material-code-braces: UpdateStorageVirtualMachineRequestRequestTypeDef](./type_defs.md#updatestoragevirtualmachinerequestrequesttypedef) 

### update\_volume

Updates the configuration of an Amazon FSx for NetApp ONTAP or Amazon FSx for
OpenZFS volume.

Type annotations and code completion for `#!python session.client("fsx").update_volume` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# update_volume method definition

await def update_volume(
    self,
    *,
    VolumeId: str,
    ClientRequestToken: str = ...,
    OntapConfiguration: UpdateOntapVolumeConfigurationTypeDef = ...,  # (1)
    Name: str = ...,
    OpenZFSConfiguration: UpdateOpenZFSVolumeConfigurationTypeDef = ...,  # (2)
) -> UpdateVolumeResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: UpdateOntapVolumeConfigurationTypeDef](./type_defs.md#updateontapvolumeconfigurationtypedef) 
2. See [:material-code-braces: UpdateOpenZFSVolumeConfigurationTypeDef](./type_defs.md#updateopenzfsvolumeconfigurationtypedef) 
3. See [:material-code-braces: UpdateVolumeResponseTypeDef](./type_defs.md#updatevolumeresponsetypedef) 


```python
# update_volume method usage example with argument unpacking

kwargs: UpdateVolumeRequestRequestTypeDef = {  # (1)
    "VolumeId": ...,
}

parent.update_volume(**kwargs)
```

1. See [:material-code-braces: UpdateVolumeRequestRequestTypeDef](./type_defs.md#updatevolumerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("fsx").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("fsx").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client)

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

Type annotations and code completion for `#!python session.client("fsx").get_paginator` method with overloads.

- `client.get_paginator("describe_backups")` -> [DescribeBackupsPaginator](./paginators.md#describebackupspaginator)
- `client.get_paginator("describe_file_systems")` -> [DescribeFileSystemsPaginator](./paginators.md#describefilesystemspaginator)
- `client.get_paginator("describe_storage_virtual_machines")` -> [DescribeStorageVirtualMachinesPaginator](./paginators.md#describestoragevirtualmachinespaginator)
- `client.get_paginator("describe_volumes")` -> [DescribeVolumesPaginator](./paginators.md#describevolumespaginator)
- `client.get_paginator("list_tags_for_resource")` -> [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)


