# Threat Actor Mapping to Cloud Security Risks

This document maps common cloud misconfigurations to relevant threat actors, their tactics, and motivations.

| Threat Actor        | Cloud Misconfiguration           | Tactics / Tools                     | Motivation      | Risk Example |
|---------------------|----------------------------------|-------------------------------------|------------------|--------------|
| Cybercriminals      | Public Blob or S3 Bucket         | Internet scanning, S3Scanner        | Financial gain   | Data theft / ransomware |
| Insider (Disgruntled Employee) | Over-permissioned IAM roles | Legitimate access, privilege misuse | Revenge or negligence | Data exfiltration |
| Script Kiddies      | Open SSH Ports                   | Shodan, metasploit, brute-forcers   | Mischief or fame | Unauthorized access |
| Nation-State Actor  | Exposed DevOps tooling           | Zero-day exploits, supply chain attacks | Espionage       | Compromise CI/CD pipelines |
| Hacktivists         | Insecure APIs                    | Public exploits, DDoS tools         | Political cause  | Service disruption |
