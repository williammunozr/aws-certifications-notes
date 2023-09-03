# AWS PrivateLink

`AWS PrivateLink` establishes secure connectivity between VPCs and AWS services, preventing exposure of traffic to the internet.

`PrivateLink` essentially provides access to the resources hosted in other VPC or other AWS accounts within the same subnet as the requester.
This eliminates the need to use any NAT gateway, IGW, public IP address, or VPN. Therefore, it provides better control over your services, which are reachable via a client VPC.
