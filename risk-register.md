# Cloud Security Risk Register

This register includes real-world cloud security risks with business impact ratings and mitigation actions. Each entry is written in risk statement format, suitable for executive and technical stakeholders.

| Risk Name               | Likelihood | Impact | Risk Statement                                                                                              | Mitigation Action                          |
|------------------------|------------|--------|--------------------------------------------------------------------------------------------------------------|--------------------------------------------|
| Insecure Storage Blob  | High       | Medium | There is a risk that internal data could be accessed due to misconfigured Blob permissions, resulting in data leakage and compliance violations. | Set container to private; enforce RBAC     |
| Open SSH Access        | High       | High   | There is a risk of unauthorized remote access due to exposed SSH port and weak credentials, leading to potential infrastructure compromise. | Restrict SSH to known IPs; use SSH keys    |
| Misconfigured Firewall | Medium     | High   | There is a risk that attackers could exploit exposed database services due to overly permissive firewall rules, resulting in unauthorized access or data loss. | Harden NSG rules; apply least privilege     |
