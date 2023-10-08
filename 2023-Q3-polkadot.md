# Proposal: [rpc services](https://stakeworld.io/docs/rpc) for polkadot, including the commons in Q3 2023.

Proponent: 13Jpq4n3PXXaSAbJTMmFD78mXAzs8PzgUUQd5ve8saw7HQS5 (identity: Stakeworld.io)

Requested dot: 1711 

## Description

This is a request for the retroactive funding of maintaining public [rpc services](https://stakeworld.io/docs/rpc) in Q3 2023 for polkadot, including the commons (assethub, bridgehub, collectives), all included in [polkadot.js.org](https://polkadot.js.org/apps/?rpc=wss://dot-rpc.stakeworld.io).

Infrastructure requests are a hot topic on the treasury. Stakeworld is an active participant in the dotsama ecosystem, active as a validator (also in the thousand validator group) as well as running collators, making updates to the wiki, running bootnodes and maintaining robust rpc public endpoints. Especially the rpc endpoints cannot be maintained without adequate funding. 

In the previous 30 days we [served](https://stakeworld.io/docs/rpc#live-stakeworld-rpc-data):
* 117.144.567 Polkadot & common chains rpc requests

Earlier requests can be found [here](https://github.com/stakeworld/stakeworld-treasury#readme).
 
Comparable proposals: [Dwellir RPC service](https://polkadot.polkassembly.io/treasury/289), [Onfinality High Performance Infrastructure](https://polkadot.polkassembly.io/referenda/138)

## Context

### rpc nodes

Stakeworld has been publicly active as a public rpc provider since the end of 2022. We did some [research and stress testing](https://stakeworld.io/docs/rpc), rewrote the [wiki page](https://wiki.polkadot.network/docs/maintain-wss) and in Q2 2023 our polkadot, kusama and westend endpoints including the commons got included in polkadot.js and we expanded our infrastructure to match the higher demand. Since then we have been serving public rpc requests without any outage. 

All the rpc endpoints are included on polkadot.js which generates most of the rpc traffic. After our [rejected](https://polkadot.polkassembly.io/referenda/19) request we scaled down a little and delayed adding ourself to more services like polkassembly and the staking dashboard until it is clear if the polkadot community thinks our service deserves further funding. 

#### Technical

The rpc nodes are hosted on dedicated servers, in different geographical locations, with nodes running in archive mode and rpc requests proxied by ssl enabled nginx instances. Nodes are load balanced by cloudflare services, including automatic failover in case of outages. Usage is monitored and in case of capacity problems extra nodes can be added in a short time.  

All servers are monitored with grafana and alert mechanisms are in place. We keep a [statuspage](https://stakeworld.statuspage.io/). We have had no major outages. 

#### Statistics

Live data can be seen on our [webpage](https://stakeworld.io/docs/rpc#live-stakeworld-rpc-data).

![rpcmonthly](2023-Q3-dot-monthly.png)

## Financial

### Expenses

This request is for 3 months of maintenance in Q3 2023.

Hours are included at a 85 EUR/hour rate.

| Item                                  | Cost                   		|
| ------------                          | -----------------------               |
| **rpc nodes**	 	                |			 		|
| Maintenance                           | 3 months x 6h x 85 EUR = 1530 EUR  	|
| Dedicated nodes polkadot              | 4320 EUR 	                        |
| Dedicated nodes commons               | 720 EUR 	                        |
|                                       |                                       |
| Total                                 | 6570 EUR	 		        |
| Request		                | 6570 EUR * 1.06 = 6964 USD / 4,07 ([EMA7](https://polkadot.subscan.io/tools/charts?type=price)) = 1711 DOT |

