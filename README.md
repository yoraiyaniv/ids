
## Problem Statement: 

**Home networks are blind to subtle intrusions.**

Consumer grade routers rarely log more than DHCP leases and basic firewall drops, leaving owners unaware when a laptop starts port scanning the LAN, a smart‑TV joins a botnet, or a guest device bypasses the firewall and sends sensitive data over DNS tunnelling.

**Goal**  
Build a _lightweight, always‑on Intrusion‑Detection System (IDS)_
that passively sniffs all LAN traffic, transforms Zeek flow logs
into streaming events, and flags statistically anomalous behavior
within **\< 5 s end‑to‑alert** on .

**Success Metrics**  
* ≥ 90 % true‑positive rate on CIC‑IDS 2018 port‑scan subset  
* ≤ 3 % false‑positive rate on 48 h of real home traffic  
* CPU \< 50 % and RAM \< 1 GB on the Pi during peak load

**Attacks Focus**
Port‑scans, SSH brute‑force, basic DNS tunnelling.