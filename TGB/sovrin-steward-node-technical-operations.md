![logo](../images/banner.png)

# Node Selection Process
```
Last Revised: 28JUN2017 (PSTF)
Prior Versions (link):

```

# EARLY DOCUMENT - NEEDS STRONG INPUT & EDITING

## POLICIES:

1. In the spirit of decentralization and in accordance with our open governance requirements: 
   1. the operation of a validator node must not be bound to or influenced by reward or financial gain of any kind; 
   2. the review criteria for validator nodes to be in the inactive-and-ready pool must ensure that an entity's operation of a validator node must not in anyway place the entity in an economic or power in-balance position with respect to the general users of the public network; 
   3. a pool of qualified and approved validator nodes will be intermittently and systematically parsed for selection to be part of the active pool. 

## Purpose
Establish a transparent and fair process for the collecting and scoring of data. The results of which will be used by an algorithm for deciding which nodes will participate in consensus, based on which ones are likely to add the least risk of network downtime.

## Algorithm
Based on an the [RBFT: Redundant Byzantine Fault Tolerance](https://pakupaku.me/plaublin/rbft/5000a297.pdf) paper published at the 2013 IEEE Conference on Distributed Computing Systems, the Sovrin's Steward Selection Algorithm was captured as a reference implementation in [Sovrin Improvement Proposal (SIP 5001)](https://github.com/sovrin-foundation/sovrin-sip/blob/master/text/5001-steward-selection-algorithm/README.md).

This algorithm will be implemented using manual analysis as the STF2 goes into effect. Eventually, we imagine establishing software tools and processes to make the selection process automatic.

## Data
The selection algorithm requires real data to drive the selection process. The data needs to be harvested and analyzed.

### Collection
Initially, diversity and performance metrics will be manually gathered by Sovrin Foundation staff. It is the intent of the Sovrin Foundation to formalize both automated push and pull data collection techniques for Validator and Observer nodes as part of STFv3.

The Technical Governance Board in collaboration with the Steward Community will:

* establish the facets and associated data models for the monitoring of a node;
* define and implement the infrastructure necessary to collect this data and subsequently publishing it to a public and transparent ```performance``` ledger .

### Scoring

Our selection algorithm operates on scored data. Currently, this scoring process is performed using manual human assessments over the data that is available.

The Technical Governance Board in collaboration with the Steward Community will:

* establish processes for how often the data is analyzed
* establish procedures to determine which tools are used and how often to produce the scores
* review analysis and coordinate adjustments as required to data facets and scoring models

## Selection
Our selection algorithm is intermittently executed using a pool of available nodes and the ```performance``` ledger as inputs to select the nodes that will comprise the active set.

The frequency of this selection process is currently monthly. Eventually, this should be a very frequent and automated process with selection refreshes as often as every hour.
