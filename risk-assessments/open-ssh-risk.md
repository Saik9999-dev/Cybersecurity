# Risk Assessment – Open SSH Port on Azure VM

- **Asset**: Azure Virtual Machine (Ubuntu)
- **Threat**: External attacker attempting brute-force access
- **Vulnerability**: Port 22 open to 0.0.0.0/0 (the internet)
- **Likelihood**: High
- **Impact**: High (could lead to privilege escalation or ransomware)

## Risk Score: Critical

### Recommended Treatment
- **Mitigate**: Restrict SSH access to known IPs using NSG
- **Mitigate**: Enforce SSH key-based authentication, disable password login
- **Monitor**: Enable Azure Defender alerts for SSH brute force
