# 2. Endpoint Security
Section 2 of the Paranoid Digital Security Standard sets forth standard device and endpoint security controls required for a device to be considered a "secure device".

## 2.1 BIOS/UEFI Requirements

### 2.1.1 BIOS/UEFI Access
Access to BIOS and UEIF features MUST be locked with a password. Access to boot menus and the ability for a user to select an alternate boot source MUST be locked with a password.

### 2.1.2 Secure Boot, Boot Verification, Rooting, and Jailbreaking
ANY device used to access ANY account or data MUST be configured to use manufacturer recommended security features. Specifically, they MUST:
  * Have "Secure Boot" enabled.
  * Have "Driver Signature Verification" enabled.

They MUST NOT:
  * Be "rooted", "jailbroken", or in any other way allow the user or applications to modify the operating system beyond what is permitted by the manufacturer.

### 2.1.3 UEFI Mode
  * Where possible, devices MUST be set to use UEFI, as opposed to BIOS.


## 2.2 CPU and System Settings

### 2.2.1 Intel Software Guard Extensions (SGX)
Intel Software Guard Extensions (SGX) MUST be disabled in BIOS, and SGX drivers MUST be removed from the operating system.[1]

### 2.2.2 Intel Management Engine Interface (IMEI)
Where possible, Intel Management Engine Interface (IMEI) MUST be disabled in BIOS, and IMEI-related drivers MUST be removed from the operating system. ANY IMEI-related devices MUST be disabled in the operating system.


## 2.3 Disk Encryption

### 2.3.1 Where Required

### 2.3.2 Cipher Strength

### 2.3.3 Encryption Key Safeguards


## 2.4 Separation of Privilege

### 2.4.1 Standard Accounts

### 2.4.2 Administrative Accounts


## 2.5 Firewall Requirements

### 2.5.1 Inbound Firewall

### 2.5.2 Outbound Firewall


## 2.6 Anti-Malware Requirements

### 2.6.1 Real-time scanning

### 2.6.2 Scheduled Scanning

### 2.6.3 Ransomware Protection

### 2.6.4 Self Defense and Tamper Protection


## 2.7 System and Application Updates

### 2.7.1 Auto-Update

### 2.7.2 Update Scanning


## 2.8 Miscellaneous Security Measures

### 2.8.1 USB Access Control

--

[1]: Intel Software Guard Extensions (SGX) enclaves are not widely used in modern desktop operating systems and applications. There have been numerous flaws discovered which undermine their effectiveness, and any future flaws are not likely to be addressed, and it may not even be possible to address them via a microcode update in the first place. Additionally, there has been research that hints at the possibility of malware residing in SGX enclaves which would be invisible to the operating system and anti-virus products.
