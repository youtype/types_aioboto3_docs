# Type definitions

> [Index](../README.md) > [ManagedBlockchainQuery](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ManagedBlockchainQuery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
    type annotations stubs module [types-aiobotocore-managedblockchain-query](https://pypi.org/project/types-aiobotocore-managedblockchain-query/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## ContractIdentifierTypeDef

```python
# ContractIdentifierTypeDef definition

class ContractIdentifierTypeDef(TypedDict):
    network: QueryNetworkType,  # (1)
    contractAddress: str,
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
## OwnerIdentifierTypeDef

```python
# OwnerIdentifierTypeDef definition

class OwnerIdentifierTypeDef(TypedDict):
    address: str,
```

## TokenIdentifierTypeDef

```python
# TokenIdentifierTypeDef definition

class TokenIdentifierTypeDef(TypedDict):
    network: QueryNetworkType,  # (1)
    contractAddress: NotRequired[str],
    tokenId: NotRequired[str],
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## BlockchainInstantPaginatorTypeDef

```python
# BlockchainInstantPaginatorTypeDef definition

class BlockchainInstantPaginatorTypeDef(TypedDict):
    time: NotRequired[datetime],
```

## ConfirmationStatusFilterTypeDef

```python
# ConfirmationStatusFilterTypeDef definition

class ConfirmationStatusFilterTypeDef(TypedDict):
    include: Sequence[ConfirmationStatusType],  # (1)
```

1. See [:material-code-brackets: ConfirmationStatusType](./literals.md#confirmationstatustype) 
## ContractFilterTypeDef

```python
# ContractFilterTypeDef definition

class ContractFilterTypeDef(TypedDict):
    network: QueryNetworkType,  # (1)
    tokenStandard: QueryTokenStandardType,  # (2)
    deployerAddress: str,
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
2. See [:material-code-brackets: QueryTokenStandardType](./literals.md#querytokenstandardtype) 
## ContractMetadataTypeDef

```python
# ContractMetadataTypeDef definition

class ContractMetadataTypeDef(TypedDict):
    name: NotRequired[str],
    symbol: NotRequired[str],
    decimals: NotRequired[int],
```

## GetTransactionInputRequestTypeDef

```python
# GetTransactionInputRequestTypeDef definition

class GetTransactionInputRequestTypeDef(TypedDict):
    transactionHash: str,
    network: QueryNetworkType,  # (1)
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
## TransactionTypeDef

```python
# TransactionTypeDef definition

class TransactionTypeDef(TypedDict):
    network: QueryNetworkType,  # (1)
    transactionHash: str,
    transactionTimestamp: datetime,
    transactionIndex: int,
    numberOfTransactions: int,
    to: str,
    blockHash: NotRequired[str],
    blockNumber: NotRequired[str],
    from: NotRequired[str],
    contractAddress: NotRequired[str],
    gasUsed: NotRequired[str],
    cumulativeGasUsed: NotRequired[str],
    effectiveGasPrice: NotRequired[str],
    signatureV: NotRequired[int],
    signatureR: NotRequired[str],
    signatureS: NotRequired[str],
    transactionFee: NotRequired[str],
    transactionId: NotRequired[str],
    confirmationStatus: NotRequired[ConfirmationStatusType],  # (2)
    executionStatus: NotRequired[ExecutionStatusType],  # (3)
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
2. See [:material-code-brackets: ConfirmationStatusType](./literals.md#confirmationstatustype) 
3. See [:material-code-brackets: ExecutionStatusType](./literals.md#executionstatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## OwnerFilterTypeDef

```python
# OwnerFilterTypeDef definition

class OwnerFilterTypeDef(TypedDict):
    address: str,
```

## TokenFilterTypeDef

```python
# TokenFilterTypeDef definition

class TokenFilterTypeDef(TypedDict):
    network: QueryNetworkType,  # (1)
    contractAddress: NotRequired[str],
    tokenId: NotRequired[str],
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
## ListTransactionEventsInputRequestTypeDef

```python
# ListTransactionEventsInputRequestTypeDef definition

class ListTransactionEventsInputRequestTypeDef(TypedDict):
    transactionHash: str,
    network: QueryNetworkType,  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
## TransactionEventTypeDef

```python
# TransactionEventTypeDef definition

class TransactionEventTypeDef(TypedDict):
    network: QueryNetworkType,  # (1)
    transactionHash: str,
    eventType: QueryTransactionEventTypeType,  # (2)
    from: NotRequired[str],
    to: NotRequired[str],
    value: NotRequired[str],
    contractAddress: NotRequired[str],
    tokenId: NotRequired[str],
    transactionId: NotRequired[str],
    voutIndex: NotRequired[int],
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
2. See [:material-code-brackets: QueryTransactionEventTypeType](./literals.md#querytransactioneventtypetype) 
## ListTransactionsSortTypeDef

```python
# ListTransactionsSortTypeDef definition

class ListTransactionsSortTypeDef(TypedDict):
    sortBy: NotRequired[ListTransactionsSortByType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: ListTransactionsSortByType](./literals.md#listtransactionssortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## TransactionOutputItemTypeDef

```python
# TransactionOutputItemTypeDef definition

class TransactionOutputItemTypeDef(TypedDict):
    transactionHash: str,
    network: QueryNetworkType,  # (1)
    transactionTimestamp: datetime,
    confirmationStatus: NotRequired[ConfirmationStatusType],  # (2)
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
2. See [:material-code-brackets: ConfirmationStatusType](./literals.md#confirmationstatustype) 
## AssetContractTypeDef

```python
# AssetContractTypeDef definition

class AssetContractTypeDef(TypedDict):
    contractIdentifier: ContractIdentifierTypeDef,  # (1)
    tokenStandard: QueryTokenStandardType,  # (2)
    deployerAddress: str,
```

1. See [:material-code-braces: ContractIdentifierTypeDef](./type_defs.md#contractidentifiertypedef) 
2. See [:material-code-brackets: QueryTokenStandardType](./literals.md#querytokenstandardtype) 
## GetAssetContractInputRequestTypeDef

```python
# GetAssetContractInputRequestTypeDef definition

class GetAssetContractInputRequestTypeDef(TypedDict):
    contractIdentifier: ContractIdentifierTypeDef,  # (1)
```

1. See [:material-code-braces: ContractIdentifierTypeDef](./type_defs.md#contractidentifiertypedef) 
## TokenBalancePaginatorTypeDef

```python
# TokenBalancePaginatorTypeDef definition

class TokenBalancePaginatorTypeDef(TypedDict):
    balance: str,
    atBlockchainInstant: BlockchainInstantPaginatorTypeDef,  # (3)
    ownerIdentifier: NotRequired[OwnerIdentifierTypeDef],  # (1)
    tokenIdentifier: NotRequired[TokenIdentifierTypeDef],  # (2)
    lastUpdatedTime: NotRequired[BlockchainInstantPaginatorTypeDef],  # (3)
```

1. See [:material-code-braces: OwnerIdentifierTypeDef](./type_defs.md#owneridentifiertypedef) 
2. See [:material-code-braces: TokenIdentifierTypeDef](./type_defs.md#tokenidentifiertypedef) 
3. See [:material-code-braces: BlockchainInstantPaginatorTypeDef](./type_defs.md#blockchaininstantpaginatortypedef) 
4. See [:material-code-braces: BlockchainInstantPaginatorTypeDef](./type_defs.md#blockchaininstantpaginatortypedef) 
## BlockchainInstantTypeDef

```python
# BlockchainInstantTypeDef definition

class BlockchainInstantTypeDef(TypedDict):
    time: NotRequired[Union[datetime, str]],
```

## ListAssetContractsInputRequestTypeDef

```python
# ListAssetContractsInputRequestTypeDef definition

class ListAssetContractsInputRequestTypeDef(TypedDict):
    contractFilter: ContractFilterTypeDef,  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: ContractFilterTypeDef](./type_defs.md#contractfiltertypedef) 
## GetAssetContractOutputTypeDef

```python
# GetAssetContractOutputTypeDef definition

class GetAssetContractOutputTypeDef(TypedDict):
    contractIdentifier: ContractIdentifierTypeDef,  # (1)
    tokenStandard: QueryTokenStandardType,  # (2)
    deployerAddress: str,
    metadata: ContractMetadataTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ContractIdentifierTypeDef](./type_defs.md#contractidentifiertypedef) 
2. See [:material-code-brackets: QueryTokenStandardType](./literals.md#querytokenstandardtype) 
3. See [:material-code-braces: ContractMetadataTypeDef](./type_defs.md#contractmetadatatypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTransactionOutputTypeDef

```python
# GetTransactionOutputTypeDef definition

class GetTransactionOutputTypeDef(TypedDict):
    transaction: TransactionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TransactionTypeDef](./type_defs.md#transactiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssetContractsInputListAssetContractsPaginateTypeDef

```python
# ListAssetContractsInputListAssetContractsPaginateTypeDef definition

class ListAssetContractsInputListAssetContractsPaginateTypeDef(TypedDict):
    contractFilter: ContractFilterTypeDef,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ContractFilterTypeDef](./type_defs.md#contractfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTransactionEventsInputListTransactionEventsPaginateTypeDef

```python
# ListTransactionEventsInputListTransactionEventsPaginateTypeDef definition

class ListTransactionEventsInputListTransactionEventsPaginateTypeDef(TypedDict):
    transactionHash: str,
    network: QueryNetworkType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTokenBalancesInputListTokenBalancesPaginateTypeDef

```python
# ListTokenBalancesInputListTokenBalancesPaginateTypeDef definition

class ListTokenBalancesInputListTokenBalancesPaginateTypeDef(TypedDict):
    tokenFilter: TokenFilterTypeDef,  # (1)
    ownerFilter: NotRequired[OwnerFilterTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: TokenFilterTypeDef](./type_defs.md#tokenfiltertypedef) 
2. See [:material-code-braces: OwnerFilterTypeDef](./type_defs.md#ownerfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTokenBalancesInputRequestTypeDef

```python
# ListTokenBalancesInputRequestTypeDef definition

class ListTokenBalancesInputRequestTypeDef(TypedDict):
    tokenFilter: TokenFilterTypeDef,  # (1)
    ownerFilter: NotRequired[OwnerFilterTypeDef],  # (2)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: TokenFilterTypeDef](./type_defs.md#tokenfiltertypedef) 
2. See [:material-code-braces: OwnerFilterTypeDef](./type_defs.md#ownerfiltertypedef) 
## ListTransactionEventsOutputTypeDef

```python
# ListTransactionEventsOutputTypeDef definition

class ListTransactionEventsOutputTypeDef(TypedDict):
    events: List[TransactionEventTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TransactionEventTypeDef](./type_defs.md#transactioneventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTransactionsInputListTransactionsPaginateTypeDef

```python
# ListTransactionsInputListTransactionsPaginateTypeDef definition

class ListTransactionsInputListTransactionsPaginateTypeDef(TypedDict):
    address: str,
    network: QueryNetworkType,  # (1)
    fromBlockchainInstant: NotRequired[BlockchainInstantPaginatorTypeDef],  # (2)
    toBlockchainInstant: NotRequired[BlockchainInstantPaginatorTypeDef],  # (2)
    sort: NotRequired[ListTransactionsSortTypeDef],  # (4)
    confirmationStatusFilter: NotRequired[ConfirmationStatusFilterTypeDef],  # (5)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (6)
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
2. See [:material-code-braces: BlockchainInstantPaginatorTypeDef](./type_defs.md#blockchaininstantpaginatortypedef) 
3. See [:material-code-braces: BlockchainInstantPaginatorTypeDef](./type_defs.md#blockchaininstantpaginatortypedef) 
4. See [:material-code-braces: ListTransactionsSortTypeDef](./type_defs.md#listtransactionssorttypedef) 
5. See [:material-code-braces: ConfirmationStatusFilterTypeDef](./type_defs.md#confirmationstatusfiltertypedef) 
6. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTransactionsOutputTypeDef

```python
# ListTransactionsOutputTypeDef definition

class ListTransactionsOutputTypeDef(TypedDict):
    transactions: List[TransactionOutputItemTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TransactionOutputItemTypeDef](./type_defs.md#transactionoutputitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssetContractsOutputTypeDef

```python
# ListAssetContractsOutputTypeDef definition

class ListAssetContractsOutputTypeDef(TypedDict):
    contracts: List[AssetContractTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetContractTypeDef](./type_defs.md#assetcontracttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTokenBalancesOutputPaginatorTypeDef

```python
# ListTokenBalancesOutputPaginatorTypeDef definition

class ListTokenBalancesOutputPaginatorTypeDef(TypedDict):
    tokenBalances: List[TokenBalancePaginatorTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TokenBalancePaginatorTypeDef](./type_defs.md#tokenbalancepaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetTokenBalanceErrorItemTypeDef

```python
# BatchGetTokenBalanceErrorItemTypeDef definition

class BatchGetTokenBalanceErrorItemTypeDef(TypedDict):
    errorCode: str,
    errorMessage: str,
    errorType: ErrorTypeType,  # (4)
    tokenIdentifier: NotRequired[TokenIdentifierTypeDef],  # (1)
    ownerIdentifier: NotRequired[OwnerIdentifierTypeDef],  # (2)
    atBlockchainInstant: NotRequired[BlockchainInstantTypeDef],  # (3)
```

1. See [:material-code-braces: TokenIdentifierTypeDef](./type_defs.md#tokenidentifiertypedef) 
2. See [:material-code-braces: OwnerIdentifierTypeDef](./type_defs.md#owneridentifiertypedef) 
3. See [:material-code-braces: BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef) 
4. See [:material-code-brackets: ErrorTypeType](./literals.md#errortypetype) 
## BatchGetTokenBalanceInputItemTypeDef

```python
# BatchGetTokenBalanceInputItemTypeDef definition

class BatchGetTokenBalanceInputItemTypeDef(TypedDict):
    tokenIdentifier: TokenIdentifierTypeDef,  # (1)
    ownerIdentifier: OwnerIdentifierTypeDef,  # (2)
    atBlockchainInstant: NotRequired[BlockchainInstantTypeDef],  # (3)
```

1. See [:material-code-braces: TokenIdentifierTypeDef](./type_defs.md#tokenidentifiertypedef) 
2. See [:material-code-braces: OwnerIdentifierTypeDef](./type_defs.md#owneridentifiertypedef) 
3. See [:material-code-braces: BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef) 
## BatchGetTokenBalanceOutputItemTypeDef

```python
# BatchGetTokenBalanceOutputItemTypeDef definition

class BatchGetTokenBalanceOutputItemTypeDef(TypedDict):
    balance: str,
    atBlockchainInstant: BlockchainInstantTypeDef,  # (3)
    ownerIdentifier: NotRequired[OwnerIdentifierTypeDef],  # (1)
    tokenIdentifier: NotRequired[TokenIdentifierTypeDef],  # (2)
    lastUpdatedTime: NotRequired[BlockchainInstantTypeDef],  # (3)
```

1. See [:material-code-braces: OwnerIdentifierTypeDef](./type_defs.md#owneridentifiertypedef) 
2. See [:material-code-braces: TokenIdentifierTypeDef](./type_defs.md#tokenidentifiertypedef) 
3. See [:material-code-braces: BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef) 
4. See [:material-code-braces: BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef) 
## GetTokenBalanceInputRequestTypeDef

```python
# GetTokenBalanceInputRequestTypeDef definition

class GetTokenBalanceInputRequestTypeDef(TypedDict):
    tokenIdentifier: TokenIdentifierTypeDef,  # (1)
    ownerIdentifier: OwnerIdentifierTypeDef,  # (2)
    atBlockchainInstant: NotRequired[BlockchainInstantTypeDef],  # (3)
```

1. See [:material-code-braces: TokenIdentifierTypeDef](./type_defs.md#tokenidentifiertypedef) 
2. See [:material-code-braces: OwnerIdentifierTypeDef](./type_defs.md#owneridentifiertypedef) 
3. See [:material-code-braces: BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef) 
## GetTokenBalanceOutputTypeDef

```python
# GetTokenBalanceOutputTypeDef definition

class GetTokenBalanceOutputTypeDef(TypedDict):
    ownerIdentifier: OwnerIdentifierTypeDef,  # (1)
    tokenIdentifier: TokenIdentifierTypeDef,  # (2)
    balance: str,
    atBlockchainInstant: BlockchainInstantTypeDef,  # (3)
    lastUpdatedTime: BlockchainInstantTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: OwnerIdentifierTypeDef](./type_defs.md#owneridentifiertypedef) 
2. See [:material-code-braces: TokenIdentifierTypeDef](./type_defs.md#tokenidentifiertypedef) 
3. See [:material-code-braces: BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef) 
4. See [:material-code-braces: BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTransactionsInputRequestTypeDef

```python
# ListTransactionsInputRequestTypeDef definition

class ListTransactionsInputRequestTypeDef(TypedDict):
    address: str,
    network: QueryNetworkType,  # (1)
    fromBlockchainInstant: NotRequired[BlockchainInstantTypeDef],  # (2)
    toBlockchainInstant: NotRequired[BlockchainInstantTypeDef],  # (2)
    sort: NotRequired[ListTransactionsSortTypeDef],  # (4)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    confirmationStatusFilter: NotRequired[ConfirmationStatusFilterTypeDef],  # (5)
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
2. See [:material-code-braces: BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef) 
3. See [:material-code-braces: BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef) 
4. See [:material-code-braces: ListTransactionsSortTypeDef](./type_defs.md#listtransactionssorttypedef) 
5. See [:material-code-braces: ConfirmationStatusFilterTypeDef](./type_defs.md#confirmationstatusfiltertypedef) 
## TokenBalanceTypeDef

```python
# TokenBalanceTypeDef definition

class TokenBalanceTypeDef(TypedDict):
    balance: str,
    atBlockchainInstant: BlockchainInstantTypeDef,  # (3)
    ownerIdentifier: NotRequired[OwnerIdentifierTypeDef],  # (1)
    tokenIdentifier: NotRequired[TokenIdentifierTypeDef],  # (2)
    lastUpdatedTime: NotRequired[BlockchainInstantTypeDef],  # (3)
```

1. See [:material-code-braces: OwnerIdentifierTypeDef](./type_defs.md#owneridentifiertypedef) 
2. See [:material-code-braces: TokenIdentifierTypeDef](./type_defs.md#tokenidentifiertypedef) 
3. See [:material-code-braces: BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef) 
4. See [:material-code-braces: BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef) 
## BatchGetTokenBalanceInputRequestTypeDef

```python
# BatchGetTokenBalanceInputRequestTypeDef definition

class BatchGetTokenBalanceInputRequestTypeDef(TypedDict):
    getTokenBalanceInputs: NotRequired[Sequence[BatchGetTokenBalanceInputItemTypeDef]],  # (1)
```

1. See [:material-code-braces: BatchGetTokenBalanceInputItemTypeDef](./type_defs.md#batchgettokenbalanceinputitemtypedef) 
## BatchGetTokenBalanceOutputTypeDef

```python
# BatchGetTokenBalanceOutputTypeDef definition

class BatchGetTokenBalanceOutputTypeDef(TypedDict):
    tokenBalances: List[BatchGetTokenBalanceOutputItemTypeDef],  # (1)
    errors: List[BatchGetTokenBalanceErrorItemTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchGetTokenBalanceOutputItemTypeDef](./type_defs.md#batchgettokenbalanceoutputitemtypedef) 
2. See [:material-code-braces: BatchGetTokenBalanceErrorItemTypeDef](./type_defs.md#batchgettokenbalanceerroritemtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTokenBalancesOutputTypeDef

```python
# ListTokenBalancesOutputTypeDef definition

class ListTokenBalancesOutputTypeDef(TypedDict):
    tokenBalances: List[TokenBalanceTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TokenBalanceTypeDef](./type_defs.md#tokenbalancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
