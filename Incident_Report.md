# Incident Report – Suspicious Login Activity

## Incident Type
Potential Brute Force Attack

## Severity
Medium

## Affected User
jdoe

## Source IP
198.51.100.77

## Summary
Five failed login attempts were observed for the user "jdoe" from the same source IP address. A successful login was then recorded shortly afterwards.

## Analysis
The repeated failed login attempts followed by a successful login may indicate a brute-force or password-guessing attempt.

Because the successful login occurred after several failed attempts from the same source IP, the account should be investigated for possible compromise.

## MITRE ATT&CK
**T1110 – Brute Force**

The repeated authentication attempts are consistent with possible brute-force or password-guessing activity.

## Potential Impact
If the successful login was unauthorized, the user account may have been compromised. This could allow an attacker to access resources using valid user credentials.

## Recommended Response
- Verify whether the successful login was legitimate
- Contact the affected user
- Reset the user's password if compromise is suspected
- Verify that MFA is enabled
- Review additional authentication activity
- Check for suspicious activity after the successful login
- Block the source IP if it is confirmed to be malicious

## Conclusion
The activity should be investigated further because a successful login occurred shortly after multiple failed login attempts from the same source IP address.