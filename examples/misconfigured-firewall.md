# Misconfigured Firewall Rule

### Issue
An Azure Network Security Group (NSG) is configured to allow inbound access from any IP (0.0.0.0/0) to port 1433, which is used by Microsoft SQL Server.

### Business Impact
- Increases attack surface for brute-force and exploit attempts on database services
- Risk of data exfiltration or corruption if credentials are compromised
- Could trigger compliance violations if sensitive or regulated data is exposed

### Risk Assessment
- **Likelihood:** Medium  
- **Impact:** High

### Risk Statement
There is a risk that attackers could exploit exposed database services due to overly permissive firewall rules, leading to unauthorized access to sensitive data and potential regulatory breaches.
