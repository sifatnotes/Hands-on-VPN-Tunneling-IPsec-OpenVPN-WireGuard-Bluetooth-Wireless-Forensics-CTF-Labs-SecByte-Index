# Hands-on-VPN-Tunneling-IPsec-OpenVPN-WireGuard-Bluetooth-Wireless-Forensics-CTF-Labs-SecByte-Index
A practical collection of cybersecurity CTF labs covering virtual private network (VPN) technologies (IPsec IKE, OpenVPN config drift, WireGuard routing, split-tunneling traffic analysis, authentication deep dives) and wireless/Bluetooth security (BlueEcho forensics, silent peripheral pairing attacks, BLE beacon tracking).
# VPN Tunneling, IPsec, OpenVPN, WireGuard & Bluetooth Wireless Forensics CTF Labs

Welcome to the **VPN Tunneling, IPsec, OpenVPN, WireGuard & Bluetooth Wireless Forensics CTF Lab Collection**. This repository serves as an organized, searchable catalog of practical cybersecurity labs hosted on Learn SecByte.

This collection focuses on network-level cryptographic tunnels, secure remote access architectures, protocol misconfigurations, and short-range wireless threat vectors—spanning **VPN Fundamentals & Tunnel Technologies (Northbridge tunnel, comparative VPN protocol analysis)**, **IPsec, OpenVPN & WireGuard Misconfiguration (IPsec IKE Phase 1/2 failures, OpenVPN client configuration drift, WireGuard routing loops)**, **Split-Tunneling & Authentication Troubleshooting (Remote access split-tunnel breaches, PCAP traffic analysis, multi-factor VPN auth deep dives)**, and **Bluetooth Security, Peripheral Pairing & BLE Forensics (BlueEcho analysis, silent peripheral attacks, BLE beacon geolocation breaches)**.

---

## Lab Collection Index

### 1. VPN Fundamentals & Comparative Tunnel Architecture
* **VPN Fundamentals: The Tunnel at Northbridge**  
  *Lab Link:* [https://learn.secbyte.org/ctf/vpn-fundamentals-the-tunnel-at-northbridge](https://learn.secbyte.org/ctf/vpn-fundamentals-the-tunnel-at-northbridge)  
  *Focus:* Core principles of Virtual Private Networks (VPNs), establishing encrypted site-to-site communication paths, dissecting outer IP headers vs. inner payload encapsulation, and validating tunnel interface state.

* **Tunnel Vision: VPN Technologies Under the Microscope**  
  *Lab Link:* [https://learn.secbyte.org/ctf/tunnel-vision-vpn-technologies-under-the-microscope](https://learn.secbyte.org/ctf/tunnel-vision-vpn-technologies-under-the-microscope)  
  *Focus:* Comparative technical evaluation of tunneling protocols (IPsec, OpenVPN/TLS, WireGuard, SSTP, L2TP/IPsec), evaluating speed/overhead tradeoffs, and auditing cipher suite security.

### 2. IPsec, OpenVPN & WireGuard Protocol Security
* **IPsec Essentials: The Broken Tunnel**  
  *Lab Link:* [https://learn.secbyte.org/ctf/ipsec-essentials-the-broken-tunnel](https://learn.secbyte.org/ctf/ipsec-essentials-the-broken-tunnel)  
  *Focus:* Diagnosing IPsec IKEv1/IKEv2 negotiation failures, troubleshooting Security Association (SA) proposal mismatches, auditing Diffie-Hellman group selections, and fixing broken ESP payloads.

* **OpenVPN Config Drift**  
  *Lab Link:* [https://learn.secbyte.org/ctf/openvpn-config-drift](https://learn.secbyte.org/ctf/openvpn-config-drift)  
  *Focus:* Auditing client `.ovpn` configuration profiles for security drift, identifying missing TLS-Auth/TLS-Crypt HMAC signatures, preventing unsafe cipher downgrades, and verifying CA certificate chains.

* **WireGuard Deployment: Misrouted VPN**  
  *Lab Link:* [https://learn.secbyte.org/ctf/wireguard-deployment-misrouted-vpn](https://learn.secbyte.org/ctf/wireguard-deployment-misrouted-vpn)  
  *Focus:* Debugging modern WireGuard kernel module deployments, fixing `AllowedIPs` routing rule misconfigurations, isolating peer public key mismatches, and repairing broken handshake exchanges.

### 3. Split-Tunneling, Traffic Analysis & Gateway Authentication
* **Remote Access VPN Split-Tunnel Incident**  
  *Lab Link:* [https://learn.secbyte.org/ctf/remote-access-vpn-split-tunnel-incident](https://learn.secbyte.org/ctf/remote-access-vpn-split-tunnel-incident)  
  *Focus:* Triaging remote worker split-tunneling breaches, identifying insecure split-route declarations that bypass corporate inspection engines, and mitigating split-tunnel exfiltration paths.

<Image src="image_agent_tag_9147652919240266844" alt="Diagram showing corporate VPN split-tunneling routing paths for remote users" caption="Corporate VPN Split-Tunneling Architecture & Routing Paths" />

---

* **VPN Traffic Analysis: Split-Tunnel Incident**  
  *Lab Link:* [https://learn.secbyte.org/ctf/vpn-traffic-analysis-split-tunnel-incident](https://learn.secbyte.org/ctf/vpn-traffic-analysis-split-tunnel-incident)  
  *Focus:* Analyzing PCAP packet captures to detect cleartext DNS leakage, unencrypted HTTP traffic bypassing active VPN interfaces, and mapping routing table leak paths.

* **Broken Tunnel: VPN Authentication Deep Dive**  
  *Lab Link:* [https://learn.secbyte.org/ctf/broken-tunnel-vpn-authentication-deep-dive](https://learn.secbyte.org/ctf/broken-tunnel-vpn-authentication-deep-dive)  
  *Focus:* Deep dive into VPN gateway authentication mechanisms (RADIUS, LDAP, SAML/IdP integration), auditing pre-shared key (PSK) leaks, and fixing RADIUS secret drift.

* **Tunnel Logic: Site-to-Site VPN Incident Response**  
  *Lab Link:* [https://learn.secbyte.org/ctf/tunnel-logic-site-to-site-vpn-incident-response](https://learn.secbyte.org/ctf/tunnel-logic-site-to-site-vpn-incident-response)  
  *Focus:* Investigating Phase 1 / Phase 2 IPsec IKE negotiations, triaging pre-shared key (PSK) compromise incidents, analyzing site-to-site tunnel traffic captures, and restoring encrypted site links.

### 4. Wireless Security, Bluetooth Exploitation & BLE Forensics
* **BlueEcho: Bluetooth Forensics and Exploitation**  
  *Lab Link:* [https://learn.secbyte.org/ctf/blueecho-bluetooth-forensics-and-exploitation](https://learn.secbyte.org/ctf/blueecho-bluetooth-forensics-and-exploitation)  
  *Focus:* Capturing and analyzing Bluetooth Classic (BR/EDR) and Low Energy (BLE) HCI traffic logs (`btsnoop_hci.log`), discovering PIN cracking vulnerabilities, and auditing L2CAP/ATT protocols.

<Image src="image_agent_tag_9147652919240267527" alt="Bluetooth Host, HCI, and Controller architecture diagram" caption="Bluetooth Subsystem Stack & Host Controller Interface (HCI) Architecture" />

---

* **Silent Pairing: Wireless Peripheral Attacks**  
  *Lab Link:* [https://learn.secbyte.org/ctf/silent-pairing-wireless-peripheral-attacks](https://learn.secbyte.org/ctf/silent-pairing-wireless-peripheral-attacks)  
  *Focus:* Analyzing unauthorized silent Bluetooth pairing routines, exploiting Just Works authentication flaws, capturing keystrokes from wireless Human Interface Devices (HID), and securing peripheral connections.

* **Bluetooth Beacon Breach**  
  *Lab Link:* [https://learn.secbyte.org/ctf/bluetooth-beacon-breach](https://learn.secbyte.org/ctf/bluetooth-beacon-breach)  
  *Focus:* Investigating malicious Bluetooth Low Energy (BLE) beacon deployments, analyzing Eddystone/iBeacon frame telemetry, detecting proximity tracking attacks, and locating rogue physical transmitters.

---

## Learning Path

### Path A: VPN Tunneling & Encryption Specialist
1. **VPN & Protocol Fundamentals:** Start with [VPN Fundamentals: The Tunnel at Northbridge](https://learn.secbyte.org/ctf/vpn-fundamentals-the-tunnel-at-northbridge) and [Tunnel Vision](https://learn.secbyte.org/ctf/tunnel-vision-vpn-technologies-under-the-microscope).
2. **IPsec, OpenVPN & WireGuard:** Master gateway protocols in [IPsec Essentials](https://learn.secbyte.org/ctf/ipsec-essentials-the-broken-tunnel), [OpenVPN Config Drift](https://learn.secbyte.org/ctf/openvpn-config-drift), and [WireGuard Deployment](https://learn.secbyte.org/ctf/wireguard-deployment-misrouted-vpn).

### Path B: Remote Access, Split-Tunnel & Authentication Analyst
1. **Traffic & Routing Triage:** Analyze split-tunnel leaks via [Remote Access VPN Split-Tunnel Incident](https://learn.secbyte.org/ctf/remote-access-vpn-split-tunnel-incident) and [VPN Traffic Analysis](https://learn.secbyte.org/ctf/vpn-traffic-analysis-split-tunnel-incident).
2. **Auth & Site-to-Site Response:** Debug enterprise auth in [Broken Tunnel: VPN Authentication Deep Dive](https://learn.secbyte.org/ctf/broken-tunnel-vpn-authentication-deep-dive) and [Tunnel Logic: Site-to-Site VPN Incident Response](https://learn.secbyte.org/ctf/tunnel-logic-site-to-site-vpn-incident-response).

### Path C: Wireless Security & Bluetooth Forensic Investigator
1. **HCI Traffic & Exploitation:** Analyze Bluetooth logs in [BlueEcho: Bluetooth Forensics and Exploitation](https://learn.secbyte.org/ctf/blueecho-bluetooth-forensics-and-exploitation).
2. **Peripheral & Beacon Defense:** Triage short-range wireless threats in [Silent Pairing: Wireless Peripheral Attacks](https://learn.secbyte.org/ctf/silent-pairing-wireless-peripheral-attacks) and [Bluetooth Beacon Breach](https://learn.secbyte.org/ctf/bluetooth-beacon-breach).

---

## How to Use the Labs

1. Select a practice scenario from the **Lab Collection Index**.
2. Click the corresponding direct link to launch the exercise environment hosted on Learn SecByte.
3. Review scenario directives, Wireshark packet captures (`.pcap`/`.pcapng`), OpenVPN `.ovpn` configuration profiles, or `btsnoop_hci.log` packet dumps.
4. Resolve IPsec IKE SA mismatches, repair WireGuard `AllowedIPs` routing, detect cleartext DNS leaks in split-tunnel PCAPs, or extract paired Bluetooth link keys from HCI logs to capture flags.

---

## Target Audience

* **Network Security Engineers & VPN Administrators:** Deploy and troubleshoot IPsec, OpenVPN, and WireGuard tunnels, fix client configuration drift, and audit gateway authentication backends.
* **SOC Analysts & Network Forensic Examiners:** Parse packet captures (`.pcap`) for split-tunnel DNS leaks, analyze IPsec IKE handshakes, and investigate unauthorized network routing paths.
* **Wireless Security Researchers & Mobile Forensic Analysts:** Inspect Bluetooth HCI trace logs (`btsnoop`), analyze BLE advertisement packets, audit Bluetooth pairing methods, and track rogue BLE beacons.
* **Cybersecurity Students:** Acquire practical skills in VPN protocols, cryptographic tunneling, packet analysis with Wireshark, and short-range wireless security.

---

## Disclaimer

All lab links provided in this repository direct to official training environments hosted on Learn SecByte. All materials and exercises are provided strictly for educational purposes, defensive skill building, and authorized security research. Unauthorized scanning, packet interception, or RF probing against external systems is strictly prohibited.
