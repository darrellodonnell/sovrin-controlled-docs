# Trust by Design Policies
```
Last Revised: 22AUG2018
Prior Versions (link):

```
## Network Governance
>This section pertains to the polices associated with the participants and stakeholders that deal with the operation of the network.

1. The Sovrin Foundation is the Trust Framework Authority (TFA) for the Sovrin Network and as such is the governing agent responsible for upholding the Sovrin Trust Framework.

1. The TFA is responsible for establishing an operating budget that is compliant with non-profit regulations and adequate enough to maintain the sustainability of the Sovin Network.  

1. There are four major requirements for the Sovrin Network to meet the needs of a self-sovereign identity network:

   1. Governance: how the network can be trusted by all stakeholders.
   1. Performance: how the network can provide self-sovereign identity at Internet scale.
   1. Accessibility: how the network can ensure that identity is available to all.
   1. Privacy: how the network can meet the strongest privacy standards in the world.

1. The Sovrin Network will leverage a DLT that allows for the establishment and operation of a public global utility that is sufficient to meet the needs of our four major requirements.

## Infrastructure Participation
1. As an implementation of a public-permissioned global ledger comprised of ```nodes```, network addressable processing units, the governing agent of the Sovrin Network will define the processes associated with participation qualification and active state selection for each node. Specifically, policies need to be established for:

   1. the qualification criteria for determining which entities can be invited to operate nodes in the network
   1. Algorithm selection criteria that will determine which set of nodes are active at anyone time in the network.

1. Invitation qualification criteria MUST take into consideration:

   1. Stewards can run more than one read--permissioned nodes ("observers") so that the pool of ready and available nodes is large enough to handle public access at global scale
   1. The pool of active write-permissioned nodes ("validators") need not be large since consensus protocols can only scale to an optimal threshold, a limited number
   1. The state of a Steward's nodes at any one time (ready, active-observers, active-validator) should have no bearing on the entity's participation in then network
   1. Participation as a Steward must require evidence of the entity's ability to sustain the costs (*shoulder the burden*) of supporting a public-permissioned ledger.
   1. Stewards must be able to remain in compliance with the four basic requirements of the network: governance, scalability, accessibility, and privacy.
   1. The *credibility* of a candidate since the quality and trustworthiness of the Sovrin Network starts with the a user's confidence in who is running it.

1. It is the responsibility of the TFA that approved Stewards are provided explicit options for the data center geographic locations at time of approval and those options MUST be refreshed if not acted upon in a specific timeframe.

1. In the spirit of decentralization and in accordance with our open governance requirements:

   1. the operation of a validator node must not be bound to or influenced by reward or financial gain of any kind;
   1. the review criteria for validator nodes to be in the inactive-and-ready pool must ensure that an entity's operation of a validator node must not in anyway place the entity in an economic or power in-balance position with respect to the general users of the public network;  
   1. a pool of qualified and approved validator nodes will be intermittently and systematically parsed for selection to be part of the active pool.

1. The selection process for validator nodes in the active pool needs to balance between *system diversity* and *performance* based on a standard that is implemented and maintained by the governing entity of the permissioned network. This selection process can be implemented using a scoring algorithm (which is used at network run-time). The algorithm  SHOULD consider the facets of datacenter diversity such as IT staff access, geography, legal, and political jurisdiction as independent factors but these factors must be balanced with historical performance history of a validator node.

1. Any and all facets associated with *system diversity* criteria should be pertain to and be focused on maximize diversity of hosting locations, environments, networks, and systems in order to optimize availability and security.

1. Any and all facets associated with *performance* criteria be pertain to and be focused on both functional and operational elements. Attention should be placed on recorded computational (functional) metrics for a node as well as the track record for the responsiveness of infrastructure and human support (operational) systems. For example, transaction speeds and DDoS attach history needs to be balanced alongside fire-drill grades and upgrade responsiveness.

## Token Relevance
A cryptocurrency is *not* necessary to meet the four major requirements for the Sovrin Network.

The Sovrin Network does require a non-profit governing agency, a TFA, which must establish sustainable funding to cover its operating budget.

Such sustainable funding can be achieve using a variety of business models. If the TFA decides to leverage a cryptocurrency token as the funding source, such a token MUST not detract from the four major requirements for the Sovrin Network.

A Sovrin Token:

1. SHOULD adhere to the legal parameters of a "utility token" so that it is not misconstrued as a "security token"
1. COULD be used by the TFA as a:

   1. Deterrent for spam attacks against the public network
   1. Source of revenue for the TFA in accordance with the sustainable mission of the non-profit organization

1. COULD be used by network users (Issuers, Holders, Verifier) as a convenience utility for the exchange of value in association with the exchange of identity between peers at the edges of the network
1. MUST NOT be used by the TFA as a reward, gift or some form of payment for services rendered
