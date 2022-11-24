# Proposal: STAKEWORLD RPC nodes setup and maintenance Q4 2022

Proponent: Et9M3rrA7H2kHQEGRXHxufcp9HTEmFirMWtKHvjoJ85r1C9 (identity: STAKEWORLD)

Date: 24.11.2022

Requested KSM: 58 KSM 

## Description
This request is for funding first setup and maintenace of stakeworld RPC services for kusama and polkadot. We are proposing it as a tip just like the [snapshot service](/Q3-setup-maintenance.md) which was also submitted as a tip (as adviced by the council).

## Context/problem/solution

### RPC nodes
RPC nodes are an essential part of the kusama/polkadot ecosystem since they give the possibility to interact with the chain. STAKEWORLD has been running 2 (pruned) public RPC servers ([dot.rpc.stakeworld.nl](http://dot.rpc.stakeworld.nl/) and [ksm.rpc.stakeworld.nl](http://ksm.rpc.stakeworld.nl/)) for a while now which were originally deployed for internal use and according to the logs also have found their way to some public use. We created a [pull request](https://github.com/polkadot-js/apps/pull/8227) for inclusion in the polkadot.js app but after reviewing earlier pulls, commits and remarks concluded that a full node was required so started setting up two full archive RPC nodes. 

## Technical
The RPC services are hosted on a dedicated server, with unlimited traffic and a 1 Gbit network link and run in archive mode (`--state-pruning archive --blocks-pruning archive`). System and logs are monitored for errors, network problems and other issues. At this moment a pruned rpc service can quickly be deployed as backup in the case of failure of the main rpc. If the funding allows we will setup more full nodes to create better fault tolerance and load balancing. 

## Publicity
There was some exposure through the kusama and polkadot validator pages on element but the main focus is to include it on the polkadot.js website, getting selected from there and thus strengthening the dotsama ecosystem.

## Financial

### Expenses
This request is for setting up and deploying the service and 2 months of hosting (Q4).

Hours are included at a 80 EUR/hour rate.

| Item                  | Cost                   |
| ------------          | -----------------------|
| Setup and testing     | 6 h x 80 EUR = 480 EUR  |
| Maintenance           | 2 months x 4 h x 80 EUR = 640 EUR  |
| Hosting		| 2 months x 140 EUR = 280 EUR |
| TOTAL                 | EUR 1400 / 0.9602 -> USD 1458 [/25.23 (=EMA7)](https://kusama.subscan.io/tools/charts?type=price) = 58 KSM |
| REQUEST		| 58 KSM |

For simplicity treasury requests for our services will only be done on kusama.
