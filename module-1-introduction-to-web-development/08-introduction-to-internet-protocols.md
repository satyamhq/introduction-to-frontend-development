# Introduction to Internet Protocols

## Introduction

Email is a common method of communication today, but before it existed, people relied on the postal system to send messages.  
Interestingly, there is a strong parallel between how the postal system works and how computers send and receive data across the internet.

At the core of this communication system are **Internet Protocols**, which make it possible for data to travel reliably between computers.

---

## What Are Internet Protocols?

When computers communicate over the internet, they rely on a set of rules known as **Internet Protocols**.

In simple terms:
- Computers are the destinations that send and receive data
- Networks act as the routes the data travels through
- Internet Protocols define how the data is addressed, sent, and delivered

---

## IP Addresses

An **IP address** works much like a home address in the postal system.  
It uniquely identifies a computer on a network so data can be delivered to the correct destination.

Every device connected to a network is assigned an IP address.

### IPv4

- Uses four numbers called octets
- Octets are separated by dots
- Example: `192.0.2.235`

### IPv6

- Uses eight groups of hexadecimal values
- Groups are separated by colons
- Designed to support a much larger number of devices

IPv4 and IPv6 are currently the two most widely used versions of the Internet Protocol.

---

## IP Packets and Datagrams

Data sent across the internet is broken into small units called **IP packets**, also known as **datagrams**.

Each IP packet contains:
- **Header**: includes source IP address, destination IP address, and delivery information
- **Payload**: contains the actual data being sent

Just like a letter includes both the sender’s and recipient’s address, IP packets include both source and destination addresses.

---

## What Can Go Wrong During Transmission?

Similar to the postal system, problems can occur when sending data across a network.

IP packets may:
- Arrive out of order
- Become corrupted during transmission
- Be dropped or lost entirely

To handle these issues, additional protocols are used inside the payload of IP packets.

---

## TCP and UDP

Two of the most common transport protocols are **TCP** and **UDP**.

### Transmission Control Protocol (TCP)

TCP:
- Ensures data arrives in the correct order
- Detects and retransmits lost packets
- Prevents corrupted data from being delivered

Because of these checks, TCP introduces a small delay.  
It is commonly used for:
- Text data
- Images
- Files that must arrive correctly

---

### User Datagram Protocol (UDP)

UDP:
- Fixes corrupted packets
- Does not guarantee order
- Does not guarantee delivery

UDP is faster than TCP and is used for data that can tolerate some loss, such as:
- Voice calls
- Live video streaming
- Online gaming

---

## How Internet Protocols Work Together

Internet communication relies on layers of protocols working together:
- IP handles addressing and routing
- TCP or UDP manages data delivery
- Additional protocols may exist inside payloads

This layered approach ensures efficient and reliable data transmission.

---

## Conclusion

In summary:
- Internet Protocols define how data travels across the internet
- IP addresses uniquely identify devices on a network
- Data is sent using IP packets
- TCP and UDP manage how packets are delivered
- These protocols work together to ensure communication is reliable and efficient

Understanding Internet Protocols is essential for understanding how the internet functions behind the scenes.
