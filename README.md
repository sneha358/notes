# notes
## ICMP
The ICMP Echo and Echo Reply messages are sent and received by the ping command. In fact, when people say that they sent a ping packet, they really mean that they sent an ICMP Echo Request. These two messages are very much self-explanatory. The Echo Request simply means that the host to which it is addressed should reply to the packet. The Echo Reply is the ICMP message type that should be used in the reply. The Request includes some data, which can be specified by the ping command; whatever data is sent in the Echo Request is sent back in the Echo Reply.

The Internet Control Message Protocol (ICMP) is a supporting protocol in the Internet protocol suite. It is used by network devices, including routers, to send error messages and operational information indicating success or failure when communicating with another IP address, for example, an error is indicated when a requested service is not available or that a host or router could not be reached.[2] ICMP differs from transport protocols such as TCP and UDP in that it is not typically used to exchange data between systems, nor is it regularly employed by end-user network applications (with the exception of some diagnostic tools like ping and traceroute).

For example, every device (such as an intermediate router) forwarding an IP datagram first decrements the time to live (TTL) field in the IP header by one. If the resulting TTL is 0, the packet is discarded and an ICMP time exceeded in transit message is sent to the datagram's source address.

Many commonly used network utilities are based on ICMP messages. The traceroute command can be implemented by transmitting IP datagrams with specially set IP TTL header fields, and looking for ICMP time exceeded in transit and Destination unreachable messages generated in response. The related ping utility is implemented using the ICMP echo request and echo reply messages.

## CLI
1. An argument is a single part of a command line, delimited by blanks.
1. An option is a particular type of argument (or a part of an argument) that can modify the behavior of the command line.
1. A parameter is a particular type of argument that provides additional information to a single option or command.
