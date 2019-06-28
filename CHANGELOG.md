# ChangeLog

## 2019-6-23

### Added

- Resource: ResourcePriority/ResourceDiskThreshold/ResourceNetworkThreshold

- Operate: OperateGetBatchStop

- Request/Response: ModifyPriority/ModifyDiskThreshold/ModifyNetworkThreshold/StartBatchStopGuest/GetBatchStopGuest

### Changed

- Generate module name base on a specified interface

## 2019-6-3

### Fixed

- Cache truncated payload for parsing JSON message

## 2019-4-17

### Added

- Add service type: ServiceTypeImage (Image Server)

- Register service handler

## 2019-2-28

### Added

- Message/Runnable/Transaction test

- Modify guest name

- Batch creating/deleting guest

- Message::SetID()

- CloneJsonMessage

### Changed

- Refactor runnable

- Enable concurrent session

- Create pip/pid/log base on abs binary path

- Redirect message to incoming channel when the target is self.

### Fixed

- Endpoint test

- Peer Endpoint keep recover after stopped 

## 2018-11-27

### Added

- Resource: ResourceAddressPool/ResourceAddressRange

- Request/Response: QueryAddressPool/GetAddressPool/CreateAddressPool/DeleteAddressPool/ModifyAddressPool/QueryAddressRange/GetAddressRange/AddAddressRange/RemoveAddressRange

- Key: ParamKeyStart/ParamKeyEnd/ParamKeyMask/ParamKeyAllocate/ParamKeyGateway/ParamKeyServer/ParamKeyAssign/ParamKeyInternal/ParamKeyExternal

- Event: AddressPoolChanged

## 2018-10-22

### Added

- Operate: OperateEnable/OperateDisable/OperateMigrate/OperatePurge

- Request/Response: EnableComputePoolCell/DisableComputePoolCell/MigrateInstance/PurgeInstance/AttachInstance/DetachInstance

- Event: InstanceMigratedEvent/InstancePurgedEvent/InstanceAttachedEvent/InstanceDetachedEvent

- Distinguish connection closed by the user or lost

## 2018-9-28

### Added

- Resource: ResourceStoragePool

- Key: ParamKeyAttach

- Request/Response: QueryStoragePool/GetStoragePool/QueryStoragePoolStatus/GetStoragePoolStatus/CreateStoragePool/DeleteStoragePool/ModifyStoragePool

- Event: ComputeCellDisconnectedEvent/ComputeCellAddedEvent/ComputeCellRemovedEvent

### Changed

- Don't recover stub service when stop endpoint

## 2018-8-21

### Added

- Key: ParamKeyPrevious/ParamKeyNext/ParamKeyCurrent/ParamKeyCreate/ParamKeyModify

- Resource: ResourceSnapshot/ResourceMedia

- Operate: OperateAttach/OperateDetach/OperateCommit/OperatePull/OperateRestore

- Request/Response: InsertMedia/EjectMedia/QuerySnapshot/GetSnapshot/CreateSnapshot/DeleteSnapshot/RestoreSnapshot/CommitSnapshot/PullSnapshot

- Event: MediaAttachedEvent/MediaDetachedEvent/SnapshotResumedEvent

## 2018-8-14

### Added

- Key: 	ParamKeyVersion/ ParamKeyAdmin/ ParamKeyModule

## 2018-7-28

### Added

- Resource: ResourceCore/ResourceMemory/ResourceDisk/ResourceAuth

- Operate: OperateResize/OperateShrink

- Request/Response: ModifyCore/ModifyMemory/ModifyAuth/ResizeDisk/ShrinkDisk

- Key: ParamKeyImmediate/ParamKeySystem

## 2018-7-24

### Added

- AddressChangedEvent/ResourceAddress

## [0.1.2] - 2018-7-16

Author: Akumas

### Modified

- send disconnect to remote when stop gracefully

- detect and reconnect stub services when connection lost

- reduce connection check interval
