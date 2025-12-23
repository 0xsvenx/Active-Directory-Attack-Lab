## Initial Enumeration
Performed network scan using Nmap to identify live hosts and open services.
Discovered SMB and LDAP services indicating Active Directory environment.

## SMB Enumeration
Used CrackMapExec to enumerate users and validate credentials.
Identified weak password policy allowing password spraying.

## Credential Access
Exploited Kerberoasting vulnerability to extract service account hashes.
Cracked hash offline and obtained valid domain credentials.

## Privilege Escalation
Used BloodHound to identify misconfigured delegation.
Exploited privilege escalation path to gain elevated access.

## Lateral Movement
Authenticated to domain controller using Impacket tools.
Dumped credentials using Mimikatz.

## Domain Compromise
Successfully obtained Domain Admin privileges.

## Remediation
- Enforce strong password policy
- Disable Kerberoasting vulnerable accounts
- Restrict delegation permissions
- Monitor lateral movement activity
