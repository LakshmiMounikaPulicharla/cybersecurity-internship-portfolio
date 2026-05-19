# Task 11: Phishing Attack Simulation & Detection

## Objective
The goal of this task is to understand how phishing attacks work, how users are tricked, and how such attacks can be detected and prevented. This experiment was performed in a controlled lab environment using GoPhish.

## Tools Used
- GoPhish
- Ubuntu (Attacker System)
- Windows VirtualBox (Victim System)
- Gmail SMTP
- VirtualBox

## Lab Setup
| System | Purpose |
|--------|---------|
| Ubuntu | Hosts the GoPhish server |
| Windows VM | Acts as the victim |

## Steps Followed

1. Studied how phishing and social engineering attacks work.
2. Created a fake email template with a suspicious IT warning.
3. Designed a fake login landing page.
4. Configured SMTP using Gmail.
5. Added a test victim email.
6. Launched a phishing campaign.
7. Clicked the phishing link from the Windows VM.
8. Observed tracking results in the GoPhish dashboard.

## Results
The GoPhish dashboard showed that:
- The phishing email was opened.
- The malicious link was clicked.
This proves how easily users can be tricked by social engineering attacks.

## Red Flags Observed
- Urgent language
- Fake IT identity
- Suspicious links
- No official domain

## Prevention
- Awareness training
- Avoid clicking unknown links
- Verify senders
- Enable MFA
- Use spam filters

## Conclusion
This experiment helped me understand the real impact of phishing attacks and the importance of user awareness in cybersecurity.
