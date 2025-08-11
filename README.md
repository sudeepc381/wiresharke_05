# Task 5 – Capture and Analyze Network Traffic Using Wireshark

## Objective
Capture live network traffic using Wireshark, identify different protocols, and analyze packet details to gain practical experience in network monitoring and troubleshooting.

## Tools Used
- Wireshark (Free Network Protocol Analyzer)
- Operating System: Windows 10

## Steps Performed
1. Installed Wireshark from the official website.
2. Selected the active network interface (Ethernet 2) and started live capture.
3. Generated traffic by browsing websites and performing ping commands.
4. Applied protocol filter "tcp" to view only TCP packets.
5. Observed TCP handshake, acknowledgment (ACK), and push (PSH) packets.
6. Identified additional UDP traffic from the capture.
7. Stopped capture and reviewed packet details in the packet details pane.
8. Saved capture as `.pcap` for submission.

## Analysis from Capture
From the filtered view in the screenshot:
- **TCP Traffic** observed between IPv6 addresses, showing:
  - ACK packets confirming successful data receipt.
  - PSH, ACK packet indicating data push along with acknowledgment.
  - Consistent sequence and acknowledgment number increments.
- **UDP Traffic** observed with consistent packet lengths (~1077 bytes) between the same IPv6 hosts.

## Protocols Identified
1. **TCP** – Reliable transport protocol with acknowledgments and sequence numbers.
2. **UDP** – Connectionless protocol, no handshake, faster delivery.
3. **IPv6** – Internet Protocol version 6 used as the underlying network protocol.

## Findings Summary
Protocol | Description | Example Usage | Observations
-------- | ----------- | ------------- | ------------
TCP      | Reliable, connection-oriented | Web traffic, file transfers | ACK, PSH packets, sequence control
UDP      | Fast, connectionless | Streaming, DNS | Constant packet sizes, no retransmissions
IPv6     | Next-gen internet protocol | Modern networks | Source/destination addresses in IPv6 format

## Outcomes
- Learned to filter and analyze TCP/UDP packets in Wireshark.
- Understood how to interpret sequence and acknowledgment numbers.
- Gained practical experience with IPv6 packet structure and data fields.

## Deliverables
- Screenshot (wireshake.png) of packet capture with filter applied.
- Packet Capture File (.pcap) for verification.
- README.md summarizing findings.
