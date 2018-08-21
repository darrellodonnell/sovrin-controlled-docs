## Sovrin Steward Node Criteria

A Steward Node:
1. MUST run as a Validator Node (Observer Nodes will not be introduced until the General
Availability Network).
1. MUST run the current release of the Sovrin Open Source Code as designated by the
Technical Governance Board.
1. MUST upgrade to a new version of the Sovrin Open Source Code within 3 business
days of notification of the new release by the secretary of the Technical Governance
Board.
1. MUST register all Node configuration data required by the Pool Ledger.
1. MUST run a server operating system that receives timely patches from its vendor or
Sovrin Provisional Trust Framework 28 June 2017 Page 26
community.
   1. For Linux, the base OS is less than 2.5 years old.
   1. For Windows, the base OS is less than 4 years old.
1. MUST run on server-class hardware that is less than 4 years old.
1. If a Node is run on a VM, the Steward:
   1. MUST run on a mainstream hypervisor that receives timely patches from its
vendor or community.
   1. SHOULD apply hypervisor patches on a regular basis.
1. MUST run in a machine that is dedicated to the validator, i.e., a single-purpose (physical
or virtual) machine that does not provide services unrelated to Sovrin.
1. MUST have at least one IT-qualified person assigned to administer the node, and at
least one other person that has adequate access and training to administer the box in an
emergency.
1. MUST supply contact info for all administrators to the Sovrin Foundation, whose
accuracy is tested at least quarterly (e.g., by sending an email and/or text that doesn’t
bounce).
1. SHOULD have high-speed (e.g., 100Mbit or gigabit) access to the internet—preferably
with highly available, redundant pipes.
1. SHOULD have at least one dedicated NIC for Sovrin Validator Node consensus traffic,
and a different NIC to process external requests.
1. MUST have a stable, static, world-routable IP address.
1. SHOULD maintain a system backup or snapshot or image such that recovering the
system from failure could be performed in an hour or less.
1. MUST be a single machine, NOT a cluster. (High availability in Sovrin is achieved via the
consensus algorithm; hot-swapped machines in a cluster configuration may actually
make the network less reliable.)
1. SHOULD have 2 or more cores.
1. MUST have at least 8 GB of RAM and an ample amount (e.g., 1-2 TB) of reliable (e.g.,
RAIDed) disk space.
1. MUST run NTP and maintain a system clock that is demonstrably in sync within two
seconds.
1. SHOULD be able to weather modest power brownouts and blackouts (up to 60 minutes).
1. SHOULD run in a locked datacenter with at least one layer of keycard access to provide
an audit trail. (SSAE 16 type II compliance is recommended, but other standards may
also be acceptable.)
1. SHOULD be isolated from internal systems of a Steward (since the Validator Node is
publicly visible and thus an inappropriate candidate for access to privileged internal
networks).
1. SHOULD apply the latest security patches with latency of 1 week or less (24 hours or
less is recommended).
1. MUST run a firewall that:
   1. Disallows public ingress except on ports used by the Validator Node software
(different machines may choose to expose ledger features on different ports, so
no standard port setup is required).
   1. Optionally enables Ssh, Remote Desktop, and similar remote access tools but
constrains ingress for these tools in some way that excludes the public but allows
access for admins.
   3. Locks down egress ports to limit the ability to jump from Steward Node to some
other location.
1. SHOULD allow remote access (including over SSH) only with two-factor authentication.
1. MUST NOT allow access (remote or local) by anyone other than assigned admins.


##FROM PSTF/STF1

For the Provisional Network, a Node operated by a Founding Steward:
1. MUST run as a Validator Node (Observer Nodes will not be introduced until the General
Availability Network).
2. MUST run the current release of the Sovrin Open Source Code as designated by the
Technical Governance Board.
3. MUST upgrade to a new version of the Sovrin Open Source Code within 3 business
days of notification of the new release by the secretary of the Technical Governance
Board.
4. MUST register all Node configuration data required by the Pool Ledger.
5. MUST run a server operating system that receives timely patches from its vendor or
Sovrin Provisional Trust Framework 28 June 2017 Page 26
community.
a. For Linux, the base OS is less than 2.5 years old.
b. For Windows, the base OS is less than 4 years old.
6. MUST run on server-class hardware that is less than 4 years old.
7. If a Node is run on a VM, the Steward:
a. MUST run on a mainstream hypervisor that receives timely patches from its
vendor or community.
b. SHOULD apply hypervisor patches on a regular basis.
8. MUST run in a machine that is dedicated to the validator, i.e., a single-purpose (physical
or virtual) machine that does not provide services unrelated to Sovrin.
9. MUST have at least one IT-qualified person assigned to administer the node, and at
least one other person that has adequate access and training to administer the box in an
emergency.
10. MUST supply contact info for all administrators to the Sovrin Foundation, whose
accuracy is tested at least quarterly (e.g., by sending an email and/or text that doesn’t
bounce).
11. SHOULD have high-speed (e.g., 100Mbit or gigabit) access to the internet—preferably
with highly available, redundant pipes.
12. SHOULD have at least one dedicated NIC for Sovrin Validator Node consensus traffic,
and a different NIC to process external requests.
13. MUST have a stable, static, world-routable IP address.
14. SHOULD maintain a system backup or snapshot or image such that recovering the
system from failure could be performed in an hour or less.
15. MUST be a single machine, NOT a cluster. (High availability in Sovrin is achieved via the
consensus algorithm; hot-swapped machines in a cluster configuration may actually
make the network less reliable.)
16. SHOULD have 2 or more cores.
17. MUST have at least 8 GB of RAM and an ample amount (e.g., 1-2 TB) of reliable (e.g.,
RAIDed) disk space.
18. MUST run NTP and maintain a system clock that is demonstrably in sync within two
seconds.
19. SHOULD be able to weather modest power brownouts and blackouts (up to 60 minutes).
20. SHOULD run in a locked datacenter with at least one layer of keycard access to provide
an audit trail. (SSAE 16 type II compliance is recommended, but other standards may
also be acceptable.)
21. SHOULD be isolated from internal systems of a Steward (since the Validator Node is
publicly visible and thus an inappropriate candidate for access to privileged internal
networks).
22. SHOULD apply the latest security patches with latency of 1 week or less (24 hours or
less is recommended).
1. MUST run a firewall that:
   1. Disallows public ingress except on ports used by the Validator Node software
(different machines may choose to expose ledger features on different ports, so
no standard port setup is required).
   1. Optionally enables Ssh, Remote Desktop, and similar remote access tools but
constrains ingress for these tools in some way that excludes the public but allows
access for admins.
   3. Locks down egress ports to limit the ability to jump from Steward Node to some
other location.
24. SHOULD allow remote access (including over SSH) only with two-factor authentication.
25. MUST NOT allow access (remote or local) by anyone other than assigned admins.