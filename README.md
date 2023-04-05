## Observations from create.tsx file

A transaction is submitted to rpc endpoint along with the required params object like accounts, fee etc. rpc endpoint submits the transaction in case of break. The way we handle transactions in lesson4-helloworld code is straight forward. We first establish a connection to one of the Solana clusters and create a payer account with some airdropped funds to cover for TX cost and then we check if our program is deployed and finally call the program and log the results.

Accounts in break project is also more advanced with support for parallelization and batch size config. Accounts gets supplied to create file via useAccountsState React context.
