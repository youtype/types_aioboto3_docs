# ManagedBlockchainQueryClient

> [Index](../README.md) > [ManagedBlockchainQuery](./README.md) > ManagedBlockchainQueryClient

!!! note ""

    Auto-generated documentation for [ManagedBlockchainQuery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#managedblockchainquery)
    type annotations stubs module [types-aiobotocore-managedblockchain-query](https://pypi.org/project/types-aiobotocore-managedblockchain-query/).

## ManagedBlockchainQueryClient

Type annotations and code completion for `#!python session.client("managedblockchain-query")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client)

```python
# ManagedBlockchainQueryClient usage example

from aioboto3.session import Session
from types_aiobotocore_managedblockchain_query.client import ManagedBlockchainQueryClient

session = Session()
async with session.client("managedblockchain-query") as client:
    client: ManagedBlockchainQueryClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("managedblockchain-query").exceptions` structure.

```python
# ManagedBlockchainQueryClient.exceptions usage example

async with session.client("managedblockchain-query") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# ManagedBlockchainQueryClient.exceptions type checking example

from types_aiobotocore_managedblockchain_query.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("managedblockchain-query").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("managedblockchain-query").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client)

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


### batch\_get\_token\_balance

Gets the token balance for a batch of tokens by using the
<code>BatchGetTokenBalance</code> action for every token in the request.

Type annotations and code completion for `#!python session.client("managedblockchain-query").batch_get_token_balance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client)

```python
# batch_get_token_balance method definition

await def batch_get_token_balance(
    self,
    *,
    getTokenBalanceInputs: Sequence[BatchGetTokenBalanceInputItemTypeDef] = ...,  # (1)
) -> BatchGetTokenBalanceOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BatchGetTokenBalanceInputItemTypeDef](./type_defs.md#batchgettokenbalanceinputitemtypedef) 
2. See [:material-code-braces: BatchGetTokenBalanceOutputTypeDef](./type_defs.md#batchgettokenbalanceoutputtypedef) 


```python
# batch_get_token_balance method usage example with argument unpacking

kwargs: BatchGetTokenBalanceInputRequestTypeDef = {  # (1)
    "getTokenBalanceInputs": ...,
}

parent.batch_get_token_balance(**kwargs)
```

1. See [:material-code-braces: BatchGetTokenBalanceInputRequestTypeDef](./type_defs.md#batchgettokenbalanceinputrequesttypedef) 

### get\_asset\_contract

Gets the information about a specific contract deployed on the blockchain.

Type annotations and code completion for `#!python session.client("managedblockchain-query").get_asset_contract` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client)

```python
# get_asset_contract method definition

await def get_asset_contract(
    self,
    *,
    contractIdentifier: ContractIdentifierTypeDef,  # (1)
) -> GetAssetContractOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ContractIdentifierTypeDef](./type_defs.md#contractidentifiertypedef) 
2. See [:material-code-braces: GetAssetContractOutputTypeDef](./type_defs.md#getassetcontractoutputtypedef) 


```python
# get_asset_contract method usage example with argument unpacking

kwargs: GetAssetContractInputRequestTypeDef = {  # (1)
    "contractIdentifier": ...,
}

parent.get_asset_contract(**kwargs)
```

1. See [:material-code-braces: GetAssetContractInputRequestTypeDef](./type_defs.md#getassetcontractinputrequesttypedef) 

### get\_token\_balance

Gets the balance of a specific token, including native tokens, for a given
address (wallet or contract) on the blockchain.

Type annotations and code completion for `#!python session.client("managedblockchain-query").get_token_balance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client)

```python
# get_token_balance method definition

await def get_token_balance(
    self,
    *,
    tokenIdentifier: TokenIdentifierTypeDef,  # (1)
    ownerIdentifier: OwnerIdentifierTypeDef,  # (2)
    atBlockchainInstant: BlockchainInstantTypeDef = ...,  # (3)
) -> GetTokenBalanceOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: TokenIdentifierTypeDef](./type_defs.md#tokenidentifiertypedef) 
2. See [:material-code-braces: OwnerIdentifierTypeDef](./type_defs.md#owneridentifiertypedef) 
3. See [:material-code-braces: BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef) 
4. See [:material-code-braces: GetTokenBalanceOutputTypeDef](./type_defs.md#gettokenbalanceoutputtypedef) 


```python
# get_token_balance method usage example with argument unpacking

kwargs: GetTokenBalanceInputRequestTypeDef = {  # (1)
    "tokenIdentifier": ...,
    "ownerIdentifier": ...,
}

parent.get_token_balance(**kwargs)
```

1. See [:material-code-braces: GetTokenBalanceInputRequestTypeDef](./type_defs.md#gettokenbalanceinputrequesttypedef) 

### get\_transaction

Gets the details of a transaction.

Type annotations and code completion for `#!python session.client("managedblockchain-query").get_transaction` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client)

```python
# get_transaction method definition

await def get_transaction(
    self,
    *,
    network: QueryNetworkType,  # (1)
    transactionHash: str = ...,
    transactionId: str = ...,
) -> GetTransactionOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
2. See [:material-code-braces: GetTransactionOutputTypeDef](./type_defs.md#gettransactionoutputtypedef) 


```python
# get_transaction method usage example with argument unpacking

kwargs: GetTransactionInputRequestTypeDef = {  # (1)
    "network": ...,
}

parent.get_transaction(**kwargs)
```

1. See [:material-code-braces: GetTransactionInputRequestTypeDef](./type_defs.md#gettransactioninputrequesttypedef) 

### list\_asset\_contracts

Lists all the contracts for a given contract type deployed by an address
(either a contract address or a wallet address).

Type annotations and code completion for `#!python session.client("managedblockchain-query").list_asset_contracts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client)

```python
# list_asset_contracts method definition

await def list_asset_contracts(
    self,
    *,
    contractFilter: ContractFilterTypeDef,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAssetContractsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ContractFilterTypeDef](./type_defs.md#contractfiltertypedef) 
2. See [:material-code-braces: ListAssetContractsOutputTypeDef](./type_defs.md#listassetcontractsoutputtypedef) 


```python
# list_asset_contracts method usage example with argument unpacking

kwargs: ListAssetContractsInputRequestTypeDef = {  # (1)
    "contractFilter": ...,
}

parent.list_asset_contracts(**kwargs)
```

1. See [:material-code-braces: ListAssetContractsInputRequestTypeDef](./type_defs.md#listassetcontractsinputrequesttypedef) 

### list\_filtered\_transaction\_events

Lists all the transaction events for an address on the blockchain.

Type annotations and code completion for `#!python session.client("managedblockchain-query").list_filtered_transaction_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client)

```python
# list_filtered_transaction_events method definition

await def list_filtered_transaction_events(
    self,
    *,
    network: str,
    addressIdentifierFilter: AddressIdentifierFilterTypeDef,  # (1)
    timeFilter: TimeFilterTypeDef = ...,  # (2)
    voutFilter: VoutFilterTypeDef = ...,  # (3)
    confirmationStatusFilter: ConfirmationStatusFilterTypeDef = ...,  # (4)
    sort: ListFilteredTransactionEventsSortTypeDef = ...,  # (5)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListFilteredTransactionEventsOutputTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: AddressIdentifierFilterTypeDef](./type_defs.md#addressidentifierfiltertypedef) 
2. See [:material-code-braces: TimeFilterTypeDef](./type_defs.md#timefiltertypedef) 
3. See [:material-code-braces: VoutFilterTypeDef](./type_defs.md#voutfiltertypedef) 
4. See [:material-code-braces: ConfirmationStatusFilterTypeDef](./type_defs.md#confirmationstatusfiltertypedef) 
5. See [:material-code-braces: ListFilteredTransactionEventsSortTypeDef](./type_defs.md#listfilteredtransactioneventssorttypedef) 
6. See [:material-code-braces: ListFilteredTransactionEventsOutputTypeDef](./type_defs.md#listfilteredtransactioneventsoutputtypedef) 


```python
# list_filtered_transaction_events method usage example with argument unpacking

kwargs: ListFilteredTransactionEventsInputRequestTypeDef = {  # (1)
    "network": ...,
    "addressIdentifierFilter": ...,
}

parent.list_filtered_transaction_events(**kwargs)
```

1. See [:material-code-braces: ListFilteredTransactionEventsInputRequestTypeDef](./type_defs.md#listfilteredtransactioneventsinputrequesttypedef) 

### list\_token\_balances

This action returns the following for a given blockchain network:.

Type annotations and code completion for `#!python session.client("managedblockchain-query").list_token_balances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client)

```python
# list_token_balances method definition

await def list_token_balances(
    self,
    *,
    tokenFilter: TokenFilterTypeDef,  # (1)
    ownerFilter: OwnerFilterTypeDef = ...,  # (2)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTokenBalancesOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TokenFilterTypeDef](./type_defs.md#tokenfiltertypedef) 
2. See [:material-code-braces: OwnerFilterTypeDef](./type_defs.md#ownerfiltertypedef) 
3. See [:material-code-braces: ListTokenBalancesOutputTypeDef](./type_defs.md#listtokenbalancesoutputtypedef) 


```python
# list_token_balances method usage example with argument unpacking

kwargs: ListTokenBalancesInputRequestTypeDef = {  # (1)
    "tokenFilter": ...,
}

parent.list_token_balances(**kwargs)
```

1. See [:material-code-braces: ListTokenBalancesInputRequestTypeDef](./type_defs.md#listtokenbalancesinputrequesttypedef) 

### list\_transaction\_events

Lists all the transaction events for a transaction.

Type annotations and code completion for `#!python session.client("managedblockchain-query").list_transaction_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client)

```python
# list_transaction_events method definition

await def list_transaction_events(
    self,
    *,
    network: QueryNetworkType,  # (1)
    transactionHash: str = ...,
    transactionId: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTransactionEventsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
2. See [:material-code-braces: ListTransactionEventsOutputTypeDef](./type_defs.md#listtransactioneventsoutputtypedef) 


```python
# list_transaction_events method usage example with argument unpacking

kwargs: ListTransactionEventsInputRequestTypeDef = {  # (1)
    "network": ...,
}

parent.list_transaction_events(**kwargs)
```

1. See [:material-code-braces: ListTransactionEventsInputRequestTypeDef](./type_defs.md#listtransactioneventsinputrequesttypedef) 

### list\_transactions

Lists all the transaction events for a transaction.

Type annotations and code completion for `#!python session.client("managedblockchain-query").list_transactions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client)

```python
# list_transactions method definition

await def list_transactions(
    self,
    *,
    address: str,
    network: QueryNetworkType,  # (1)
    fromBlockchainInstant: BlockchainInstantTypeDef = ...,  # (2)
    toBlockchainInstant: BlockchainInstantTypeDef = ...,  # (2)
    sort: ListTransactionsSortTypeDef = ...,  # (4)
    nextToken: str = ...,
    maxResults: int = ...,
    confirmationStatusFilter: ConfirmationStatusFilterTypeDef = ...,  # (5)
) -> ListTransactionsOutputTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
2. See [:material-code-braces: BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef) 
3. See [:material-code-braces: BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef) 
4. See [:material-code-braces: ListTransactionsSortTypeDef](./type_defs.md#listtransactionssorttypedef) 
5. See [:material-code-braces: ConfirmationStatusFilterTypeDef](./type_defs.md#confirmationstatusfiltertypedef) 
6. See [:material-code-braces: ListTransactionsOutputTypeDef](./type_defs.md#listtransactionsoutputtypedef) 


```python
# list_transactions method usage example with argument unpacking

kwargs: ListTransactionsInputRequestTypeDef = {  # (1)
    "address": ...,
    "network": ...,
}

parent.list_transactions(**kwargs)
```

1. See [:material-code-braces: ListTransactionsInputRequestTypeDef](./type_defs.md#listtransactionsinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("managedblockchain-query").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("managedblockchain-query").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client)

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

Type annotations and code completion for `#!python session.client("managedblockchain-query").get_paginator` method with overloads.

- `client.get_paginator("list_asset_contracts")` -> [ListAssetContractsPaginator](./paginators.md#listassetcontractspaginator)
- `client.get_paginator("list_filtered_transaction_events")` -> [ListFilteredTransactionEventsPaginator](./paginators.md#listfilteredtransactioneventspaginator)
- `client.get_paginator("list_token_balances")` -> [ListTokenBalancesPaginator](./paginators.md#listtokenbalancespaginator)
- `client.get_paginator("list_transaction_events")` -> [ListTransactionEventsPaginator](./paginators.md#listtransactioneventspaginator)
- `client.get_paginator("list_transactions")` -> [ListTransactionsPaginator](./paginators.md#listtransactionspaginator)


