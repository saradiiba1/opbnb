# opBNB - High-performance layer 2 solution

The opBNB network is the Layer 2 scaling solution for the BNB Smart Chain(BSC) powered by [bedrock version](https://community.optimism.io/docs/developers/bedrock/) of Optimism OP Stack.

## Comparison

Besides the [differentiators of bedrock](https://community.optimism.io/docs/developers/bedrock/differences/), opBNB is the solution that we aim to provide the best optimistic rollup solution on the BSC.

| **Parameter**                         | **opBNB value** | **Optimism value** | **Ethereum value (for reference)** |
| ------------------------------------- | --------------- | ------------------ | ---------------------------------- |
| Block gas limit                       | 100,000,000 gas | 30,000,000 gas     | 30,000,000 gas                     |
| Block gas target                      | 50,000,000      | 5,000,000 gas      | 15,000,000 gas                     |
| EIP-1559 elasticity multiplier        | 2               | 6                  | 2                                  |
| EIP-1559 denominator                  | 8               | 50                 | 8                                  |
| Maximum base fee increase (per block) | 12.5%           | 10%                | 12.5%                              |
| Maximum base fee decrease (per block) | 12.5%           | 2%                 | 12.5%                              |
| Block time in seconds                 | 1               | 2                  | 12                                 |

## Documentation

If you want to build on top of opBNB, refer to the [opBNB Doc](https://docs.bnbchain.org/opbnb-docs).

## Community

To get help from other developers, discuss ideas, and stay up-to-date on what's happening, become a part of our community on Discord. Join our [official Discord Channel](https://discord.com/invite/bnbchain).

You can also join the conversation, connect with other projects, and ask questions in our [BNB Chain Forum](https://forum.bnbchain.org/).

## Directory Structure

<pre>
~~ opBNB ~~
├── <a href="./packages">packages</a>
│   └── <a href="./packages/contracts-bedrock">contracts-bedrock</a>: Bedrock smart contracts.
├── <a href="./op-bindings">op-bindings</a>: Go bindings for Bedrock smart contracts.
├── <a href="./op-batcher">op-batcher</a>: L2-Batch Submitter, submits bundles of batches to L1
├── <a href="./op-e2e">op-e2e</a>: End-to-End testing of all bedrock components in Go
├── <a href="./op-node">op-node</a>: rollup consensus-layer client.
├── <a href="./op-proposer">op-proposer</a>: L2-Output Submitter, submits proposals to L1
├── <a href="./ops-bedrock">ops-bedrock</a>: Bedrock devnet work
└── <a href="./specs">specs</a>: Specs of the rollup starting at the Bedrock upgrade
</pre>

## License

All files within this repository are licensed under the [MIT License](https://github.com/bnb-chain/opbnb/blob/master/LICENSE) unless stated otherwise.
