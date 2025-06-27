# Task 4: Windows Firewall Configuration and Testing

## 🎯 Objective
Configure a basic firewall rule to block specific network traffic and verify its effect.

## 🛠 Tool Used
- Windows Defender Firewall

## 🔧 Steps Performed

### 1. Firewall Rule Creation
- Created a custom **inbound rule**.
- Blocked **Port 23** (used by Telnet) to demonstrate securing an insecure service.

### 2. Telnet Client Setup
- Enabled **Telnet Client** via Windows Features.

### 3. Rule Testing
- Used Command Prompt to initiate a Telnet connection.
- Connection was blocked — confirming the firewall rule is active.

### 4. Firewall Rule Behavior
- Rules can be based on:
  - **Port** (e.g., 23, 80)
  - **Protocol** (TCP/UDP)
  - **Direction** (Inbound/Outbound)
  - **Application/Service**
  - **Network Type** (Domain/Private/Public)
- Rule evaluation:
  - If a matching **allow** rule is found → traffic allowed.
  - If a matching **block** rule is found first → traffic denied.
  - If no rule matches → default policy applies.

## ✅ Conclusion
Firewall successfully blocked Telnet traffic on port 23. This confirms that properly configured rules can protect systems from unauthorized access.
