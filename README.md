# DHCP-Computer-Network-Project

This repository contains the code for a DHCP server implementation as part of a Computer Networks project. The server supports basic DHCP functionality such as IP address allocation, lease management, and configuration provisioning.

## Project Description

This project implements a DHCP server using Python. It supports the following features:

*   **IP Address Allocation:** Dynamically assigns IP addresses from a predefined pool.
*   **Lease Management:** Manages IP address leases, including lease renewal and expiration.
*   **Configuration Provisioning:** Provides clients with necessary network configuration parameters such as subnet mask, gateway, and DNS server addresses.
*   **Configuration File:** The project can load configuration from a JSON file to specify the address pool, subnet, lease time, reservation list, and blocked devices.
*   **Dynamic Reloading of Configuration:** The configuration file is monitored for changes and is reloaded when any changes are observed.
*   **Multithreading:** Multiple threads are used to perform IP cleanups on a regular interval.

## Project Structure

The repository is organized as follows:

*   `Phase 2/`: Contains the code for phase 2 of the project, which focuses on basic client-server communication.
*   `Phase 3/`: Contains the code for phase 3 of the project, which includes DHCP server implementation with enhanced features.
*   `dhcp_packet.py`: Defines the `DHCPPacket` class for creating and decoding DHCP packets.
*   `dhcp_packet_handler.py`: Script for handling DHCP packets.
*   `client.py`: Client implementation for testing DHCP server.
*   `server.py`: Primary DHCP server implementation.
*   `configs.json`: Configuration file for DHCP server settings.

## Requirements

*   Python 3.x
*   Libraries: `socket`, `binascii`, `threading`, `json`, `ipaddress`, `datetime`, `time`

## How to Run the DHCP Server

1.  Clone the repository to your local machine.
2.  Install the required libraries.
3.  Configure the server using `configs.json`.
4.  Run the server using: `python Phase 3/DHCP_server.py`.
5.  Run the client using: `python client.py`.

## Acknowledgements

*   This project was inspired by the need for a clear and concise DHCP server implementation for educational purposes.

## Team members
*   Saifeldin Haitham
*   Mohamed Ehab Badr
*   Omar Baher Hussein
*   Saifeldin Mohamed Yousry
