![logo](../images/banner.png)
# Sovrin Steward Node Criteria
```
Last Revised: 28JUN2017 (PSTF)
Prior Versions (link):

```

# TODO

* change wording to be more self-declaratory.
*

# Policies

A Steward Node:

1. MUST meet or exceed the General Requirements
1. MUST run a server with the most recent compatible version of the Ubuntu operating system as specified by the Hyperledger Indy Node requirements.
1. MUST have 8 or more cores.
1. MUST have at least 32 GB of RAM
1. MUST have at least 1 TB, with ability to grow to 2 TB, of reliable (e.g., RAIDed) disk space.
1. MUST have a high-speed connection to the internet of at least 100 Mbps with highly available, redundant pipes.
1. MUST be implemented by exactly ONE system process answering at exactly ONE pair of network addresses (client ip/port, validator ip/port), using exactly ONE set of credentials that are responding to Sovrin/Indy protocol traffic at any one time whereby the system process adheres to a minimal fail-over recovery delay period specified by the Sovrin Foundation (or 30 secs if not specified).

# General Requirements

`TODO: make self-declaratory (is that a word?) - confirm with Ryan`

A Steward Node:
1. (makes no sense - code flips this) MUST run as a Validator Node or Observer Node.
2. MUST run the current release of the Sovrin Open Source Code as designated by the Technical Governance Board.
3. MUST upgrade to a new version of the Sovrin Open Source Code within 3 business days of notification of the new release by the secretary of the Technical Governance Board.
4. MUST register all Node configuration data required by the Pool Ledger.
5. MUST run on server-class hardware that is less than 4 years old.
6. If a Node is run on a VM, the Steward:
7. MUST run on a mainstream hypervisor that receives timely patches from its vendor or community.
8. SHOULD apply hypervisor patches on a regular basis.
9. MUST run in a machine that is dedicated to the validator, i.e., a single-purpose (physical or virtual) machine that does not provide services unrelated to Sovrin.
10. MUST have at least one IT-qualified person assigned to administer the node, and at least one other person that has adequate access and training to administer the box in an emergency.
11. MUST supply contact info for all administrators to the Sovrin Foundation, whose accuracy is tested at least quarterly (e.g., by sending an email and/or text that doesn’t bounce).
12. SHOULD have at least one dedicated NIC for Sovrin Validator Node consensus traffic, and a different NIC to process external requests.
13. MUST have a stable, static, world-routable IP address.
14. SHOULD maintain a system backup or snapshot or image such that recovering the system from failure could be performed in an hour or less.
15. MUST run NTP and maintain a system clock that is demonstrably in sync within two seconds.
16. SHOULD be able to weather modest power brownouts and blackouts (up to 60 minutes).
17. SHOULD run in a locked datacenter with at least one layer of keycard access to provide an audit trail. (SSAE 16 type II compliance is recommended, but other standards may also be acceptable.)
18. SHOULD be isolated from internal systems of a Steward (since the Validator Node is publicly visible and thus an inappropriate candidate for access to privileged internal networks).
19. SHOULD apply the latest security patches with latency of 1 week or less (24 hours or less is recommended).
20. MUST run a firewall that:
    1. Disallows public ingress except on ports used by the Validator Node software (different machines may choose to expose ledger features on different ports, so no standard port setup is required).
    2. Optionally enables Ssh, Remote Desktop, and similar remote access tools but constrains ingress for these tools in some way that excludes the public but allows access for admins.
    3. Locks down egress ports to limit the ability to jump from Steward Node to some other location.
21. SHOULD allow remote access (including over SSH) only with two-factor authentication.
22. MUST NOT allow access (remote or local) by anyone other than assigned admins.



# REFERENCED BY

The following key documents rely on this file:

* Sovrin Steward Agreement V2
* Sovrin Trust Framework V2
