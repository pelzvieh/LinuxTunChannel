# LinuxTunChannel
Open tun device, attach to a network interface (such as tun0) and expose the
network interface to Java programs as Java NIO channels. What you write into
the channel is interpreted as IP packets and sent as such. Traffic routed to
the TUN interface by means of the network configuration of the host will
be read from this channel, each one read operation yielding exactly one
IP packet.
