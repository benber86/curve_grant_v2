# Funding for Analytics Team


## Index

- [Sentence summary](#sentence-summary)
- [Proposal details](#proposal-details)
  - [Expansion and improvement of Curve Monitor](#expansion-and-improvement-of-curve-monitor)
  - [Further development of Curve's Python backend](#further-development-of-curves-python-backend-curve-prices)
  - [Ad-hoc analytics](#ad-hoc-analytics)
  - [Maintenance of existing services and infrastructure](#maintenance-of-existing-services-and-infrastructure)
- [Achievements to date](#achievements-to-date)
  - [Curve Monitor](#curve-monitor)
  - [Backend services](#backend-services)
  - [Other tasks](#other-tasks)
- [Budget](#budget)
  - [Team](#team)
  - [Infrastructure & operational costs](#infrastructure--operational-costs)
- [Payment](#payment-)



## Sentence summary

We apply for a **$835,000 grant** to fund an analytics team of **4 engineers** for **two years**  to continue working on the curvemonitor platform, infrastructure for curve.fi's backend, platform monitoring bots on social media and reports on topics ranging from MEV to crvUSD borrower behavior.

## Proposal details

The analytics team currently consists of three developers. Funded last year by the grant council to work on curvemonitor.com, the scope of our work has grown with Curve and expanded to other areas (cf. [Achievements to date](#achievements-to-date) section below). 

The present proposal is to continue funding the current team and hire another contributor for two years (cf. [Team](#team) section below for details on work arrangement details), with the possibility of an early clawback (cf. [Payment](#payment-) section) by the DAO. The longer timeframe is to provide developers with an assurance of stability for what is an otherwise very precarious employment position (no health insurance or benefits, no formal contract, no guarantees of grant renewals, volatility of token used for salary payment).

The total costs are **$820,200 for payroll** for the four developers and **$14,800 for infrastructure expenses** and overhead, adding up to a **total of $800,000**. Unused funds will be returned to the DAO at the end of the grant period.

The team will be working on the following tasks:

### Expansion and improvement of Curve Monitor
- Improve the range and accuracy of analytics currently offered on the platform: MEV analysis, DAO stats, chain-specific dashboards, in-depth pool analytics
- Offer interactive applets: impermanent loss simulator, simulation and visualization of the effect of parameter changes, soft-liquidation loss simulations
- Develop the platform into a "command center" by offering users more options to interact directly with Curve contracts on the front-end and additional tooling
- Eventually make Curve Monitor a full-fledged alternative front-end for Curve. As recent [discussions around MiCA regulations in the EU](https://twitter.com/BillHughesDC/status/1717697038819942586) have shown, only having a single front-end represents a non negligible regulatory risk for the DAO. 


### Further development of Curve's Python backend (`curve-prices`)
- Indexing of DAO contracts and DAO-related API endpoints
- Expansion of side-chain indexing to new or currently unsupported chains
- Development of a separate API for advanced analytics using the `curve-prices` database


### Ad-hoc analytics
- In addition to the data and charts offered on [curvemonitor.com](https://www.curvemonitor.com) the team also works directly with the core Curve team and other ecosystem partners to produce targeted reports on specific, punctual issues. These include, for instance, the study of arbitrageur or user behavior to better parametrize Curve's products. 


### Maintenance of existing services and infrastructure
- Telegram bots: the analytics team currently maintains a number of telegram bots and their associated channels to give users and the Curve team real time monitoring of Curve products via social media.
- Subgraphs: while currently being replaced by the new Python backend, subgraphs are still used as a data source by a number of third-parties and require regular maintenance and updates to keep up with Curve's new products.


## Achievements to date

During the past year, the team has worked to provide data indexing, live monitoring and analytics dashboard for crvUSD as quickly as possible after the product was released. We operated a complete redesign of the Curve Monitor website and expanded the available dashboards to better serve the needs of the DAO and the Core team. 

We spent a significant amount of effort on the new Python backend for Curve that will allow us to progressively phase out our current reliance on subgraphs and give us more flexibility in indexing. We also made significant process on the analysis of MEV activity on Curve to accurately spot sandwiches, atomic arbitrage transaction and CEX-DEX arbitrages. 

### Curve Monitor:
- Hiring of a designer and front-end work to implement the new design from the figma specifications 
- [crvUSD dashboards](https://curvemonitor.com/#/platform/crvusd)
- Making the Curve Monitor front-end fully mobile friendly
- [DAO page](https://curvemonitor.com/#/dao/proposals) listing fully decoded proposals, with the ability to vote directly from the site
- A first version of an [MEV dashboard](https://curvemonitor.com/#/pool/mev) 
- A ["couch cushion" dashboard](https://curvemonitor.com/#/platform/revenue/cushions) facilitating the tracking of undistributed accrued fees accross all chains

### Backend services:
- Development and maintenance of Telegram monitoring bots for Curve pools and crvUSD user activity, MEV activity and gas usage. The Telegram bots proved [instrumental in mitigating an attack of Conic Finance](https://twitter.com/curvefinance/status/1682495649302958080) in 2023 by reporting the suspicious transactions in real time.
- Continuous contributions to the development of Curve's new Python backend, `curve-prices`. The new backend replaces the subgraph for the indexing of on-chain activity on Curve pools and crvUSD and offers REST endpoints and websocket channels which now provide the Curve front-end with essential platform statistics. 
- Development and maintenance of a crvUSD subgraph also used by third parties such as [Chaos Labs's crvUSD risk monitoring platform](https://community.chaoslabs.xyz/crv-usd/risk/overview), the Curve research team, Xenophon Labs, etc.
- Development of an EVM transaction parsing module to detect atomic arbitrage trades and CEX-DEX trades
- Maintenance of the existing pool subgraphs to track new pool types

### Other tasks
- Compiling of custom datasets and charts for the Curve core team, research team and third-party analysts
- Liaison with Curve front end team for the integration of the `curve-prices` backend, curvemonitor-specific endpoints and the reproduction of curve monitor features on the curve.fi frontend.
- Moderation of the Telegram bot channels


## Budget


### Team

The team will consist of the three current members of the analytics team, and an additional team member to be recruited within six months of the grant's commencement. Current streams/grants to team members will be revoked upon approval of this proposal and any left-over funds returned to the DAO.

| Team member    | Responsibilities                                                                                                                                                           | Schedule                                                     | Salary                                                                     |
|----------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------|----------------------------------------------------------------------------|
| Alunara        | Full-stack engineer, DevOps                                                                                                                                                | Full time                                                    | $212,000 for 2 years ($104k first year, $108k 2nd year)                    |
| benny          | Back-end engineer (`curve-prices` and analytics API), subgraphs, ad-hoc analytics reports, management and liaison with other teams within the DAO & integrating protocols | Part-time (80%) for the first year, full time for the second | $191,200 for 2 years ($83,200 1st year, $108k 2nd year)                    |
| Philipp        | Back-end engineer, MEV analytics, ad-hoc analytics reports, telegram bots                                                                                                 | Full time                                                    | $212,000 for 2 years ($104k first year, $108k 2nd year)                    |
| New hire (TBD) | Back-end engineer (analytics API), ad-hoc analytics reports                                                                                                               | Full time                                                    | $160,000 for 2 years ($52k after recruitment mid-1st year, $108k 2nd year) |

Salary payment will thus total **$775,200** over two years.

In addition to the salaries, team members will receive a 1000 CRV / month risk bonus (cf. [Payment](#payment) below) of an approximate value of **$45,000** (as of Jan. 8 2024)

### Infrastructure & operational costs

Total projected cost of **$14,800 for 2 years**, unused funds will be returned to the DAO at the end of the grant period.

**Cloud computing (AWS/Digital Ocean) Costs:**

_Total: $3,960 for 2 years_

| Usage                                   | Instance specs                             | Cost                            |
|-----------------------------------------|--------------------------------------------|---------------------------------|
| MEV analytics and telegram bots backend | t2.large, 500GB SSD                        | $73.65/m or $1767.6 for 2 years |
| Analytics API backend                   | t2.medium                                  | $16.86/m or $404.6 for 2 years  |
| Fixed IPs for backend services          | Elastic IP (free until 02/24)              | $7/m or $168 for 2 years        |
| DB backup storage                       | S3 Infrequent access + Data transfer costs | $34.26/m or $411.2 for 2 years  |
| Frontend hosting                        | Basic DO Droplet, 8GB RAM, 4 vCPUs         | $50/m or $1200 for 2 years      |


**RPC and data providers costs:**

_Total: $9,200 for 2 years_

| Provider        | Description                                                                                                                                                                                                                       | Cost                        |
|-----------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------|
| Flipside crypto | SQL-queryable database similar to Dune. Used to pull data for contracts that are not part of Curve and not indexed on our side. (Free tier + on-the-go payment for queries in excess of free tier as Pro subscription is $1.2k/m) | $100/m or $2400 for 2 years |
| Alchemy         | For node access with full archive and parity traces, used for backend services and MEV analysis                                                                                                                                   | $199/m or $4800 for 2 years |
| Dappnode        | Hardware node used for faster local querying for MEV analytics and as backup source if Alchemy is unavailable                                                                                                                     | $2000 one time cost         |



**Additional services and operational costs:**

_Total: $1,640 for 2 years_

| Provider       | Description                                                       | Cost                      |
|----------------|-------------------------------------------------------------------|---------------------------|
| Keepersecurity | Secure password/secret sharing between team members               | $10/m or $240 for 2 years |
| Cloudflare     | DNS, CDN, DDos protection                                         | $20/m or $480 for 2 years |
| Gas tokens     | Used to pay for transactions on Ethereum mainnet and other chains | $920 for 2 years          |



## Payment 

We ask for a payment of $835,000 streamed over 2 years with the possibility of clawback at any time by the DAO.
The payment can be vested through a [vesting proxy contract](https://github.com/WormholeOracle/Curve-Vest) developed for this purpose in collaboration with the risk and research teams. 

As the payment is in CRV, which price may fluctuate greatly over the 2 year duration of the grant, we request that the grant be priced at a value of $0.40 per CRV, or 2 million CRV to account for potential future price depreciation.
The streamed amount will be converted to a USD stablecoin each month to pay for salaries and operational expenses. 
Any surplus left over will be set aside as a buffer to top up payments on months during which the value of CRV is below $0.40, unless there is already enough in the buffer to cover the next 6 months of expenses. At the end of the grant period, all remaining USD stable holdings will be transferred back to the DAO.

As the method proposed above still leaves significant downside risk for the team, we further request a monthly risk premium of 1000 CRV tokens to be paid out monthly to each active team member.

The total amount of CRV requested is thus as follows:
- $790,000 (payroll + expenses) at $0.4/CRV = 1975000 CRV
- Monthly bonuses to members: 1000 * (24 * 3 + 18) = 90000

**Total CRV tokens: 2,065,000**