---
title: Network/wifi
---
# Wired Equivalent Privacy

WEP uses the [Rivest Cipher 4](crypto.org::*RC4) algorithm for packet
encryption and the 32-bit version of the Cyclic Rendundancy Check to
verify packet integrity.

## Fluhrer, Mantin, Shamir Attack

The FMS attack exploits WEP\'s use of weak initialization vectors (only
24 bits) with RC4.

### Passive Initialization Vector Capture

If a target network has enough traffic, an attacker can passively sniff
packets until identical IV\'s are captured.

### Packet Injection

Packet injection can be used to generate more traffic in a WEP network,
generating more IV\'s to capture.

## Fake Authentication

# Wi-Fi Protected Access 1

# Wi-Fi Protected Access 2

## KRACK

## Four-Way Handshake Capture

The authentication handshake of WPA2 contains the passkey salted with
the access point\'s ESSID and hashed with
PBKDF2-HMAC-[SHA](crypto.org::*SHA)1. This hash can be bruteforced.

### Passively

If clients often connect to the target network, or reconnect after the
network starts, an attacker may be able to capture all four parts of the
handshake.

### Deauthentication

If the authentication handshakes cannot be captured passively, an
attacker can perform a deauthentication attack until all four parts of
the handshake are captured.

## Pairwise Master Key Identifier Capture

# Wi-Fi Protected Access 3

## Dragonfly

# Bluetooth

## KNOB

# Jargon

EAPOL:: Extensible Authentication Protocol over LAN LAN:: Local Area
Network WPA:: Wireless Protected Access PSK:: Preshared Key PMKID::
Pairwise Master Key Identifier WPS:: Wi-Fi Protected Setup WEP:: Wired
Equivalent Privacy KRACK:: Key Reinstallation Attack FRAG::
Fragmentation and Aggregation Attacks FMS:: Fluhrer, Mantin,Shamir PTW::
Pyshkin, Tews, Weinmann
