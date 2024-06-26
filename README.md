# Arbitrum BOLD Utilities

Implements a few CLI utilities for interacting with Arbitrum BOLD challenges. It contains the following commands:

- `mint-stake-token`: Mints and approves spending of a mock stake token implementation on Ethereum testnets for use in the Arbitrum BOLD challenge protocol
- `bridge-eth`: Bridges ETH to an Arbitrum inbox contract

```
Usage:
  bold-utils bridge-eth [flags]

Flags:
      --wei-to-deposit uint          eth to bridge over, in wei (0.002 ETH)
  -h, --help                         help for bridge-eth
      --inbox-address string         inbox address
      --l1-chain-id string           l1 chain id (sepolia default) (default "11155111")
      --l1-endpoint string           l1 endpoint
      --validator-priv-keys string   comma-separated validator private keys
```

and for minting stake tokens:

```
Usage:
  bold-utils mint-stake-token [flags]

Flags:
      --wei-to-mint uint             eth to mint into tokens, in wei (default 50 WETH)
  -h, --help                         help for mint-stake-token
      --l1-chain-id string           l1 chain id (sepolia default) (default "11155111")
      --l1-endpoint string           l1 endpoint
      --rollup-address string        rollup address
      --stake-token-address string   stake token address
      --validator-priv-keys string   comma-separated validator private keys
```