# Investigation: Brute Force Leading to Lateral Movement via PowerShell

## Summary
A brute force attack against a privileged account succeeded, leading to 
malicious PowerShell execution and spread to two additional hosts.

## Timeline
- 09:03 - 22 failed login attempts on account jsmith from 91.219.212.7
- 09:06:52 - Successful login from same IP
- 09:09 - Encoded PowerShell execution observed
- 09:10 - Same execution replicated on 2 additional finance hosts

## Analysis (ATT&CK Mapping)
- Brute Force (T1110)
- Suspicious PowerShell Execution (T1059.001)
- Lateral Movement (T1021)

## Recommendation
Immediate lockout of jsmith and isolation of affected hosts.
