# Insecure Storage Blob

### Issue
An Azure Blob Storage container containing internal documents is publicly accessible due to misconfigured access level (`Container` instead of `Private`).

### Business Impact
- Confidential business or technical documentation could be downloaded by unauthorized users
- Loss of intellectual property
- Potential non-compliance with data privacy policies or external regulations (e.g., GDPR)

### Risk Assessment
- **Likelihood:** High  
- **Impact:** Medium

### Risk Statement
There is a risk that internal data could be accessed or downloaded by external parties due to misconfigured Azure Blob Storage permissions, resulting in data leakage and compliance violations.
