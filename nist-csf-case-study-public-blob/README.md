# NIST CSF Case Study – Public Azure Blob Container

This case study maps a common cloud misconfiguration — a public Azure Blob Storage container — to the five functions of the NIST Cybersecurity Framework (CSF). It shows how a security team would handle the issue across the Identify, Protect, Detect, Respond, and Recover lifecycle.

---

## 🔍 Identify

**Objective:** Know what you have and what’s at risk

- Asset: Azure Blob Storage container holding internal customer data
- Risk: Public access could lead to data breach or regulatory violations
- Gap: No tagging or inventory to track exposure

---

## 🔐 Protect

**Objective:** Apply controls to prevent threats

- Set container access to `Private`
- Enforce RBAC for read/write permissions
- Apply Azure Policy to deny creation of publicly accessible blobs
- Implement secure-by-default Terraform templates

---

## 🔎 Detect

**Objective:** Identify when something goes wrong

- Enable Microsoft Defender for Cloud or Azure Security Center
- Alert on anonymous blob access in logs
- Run scheduled scans (e.g., with Trivy or `az storage` CLI)

---

## 🛠️ Respond

**Objective:** React quickly and contain the threat

- Auto-remove public access using Azure Functions or logic apps
- Notify stakeholders and document the issue
- Investigate blob access logs to check for unauthorized downloads

---

## 🔄 Recover

**Objective:** Restore operations and improve for the future

- Enable blob versioning and soft delete to recover overwritten data
- Update the risk register with this incident
- Add Terraform guardrails, CI/CD checks, or OPA policies to prevent recurrence

---

## ✅ Outcome

By using the NIST CSF, we ensured the risk of public blob exposure was:
- Identified quickly
- Mitigated with policy
- Detectable with alerts
- Handled with an automated response
- Prevented in future deployments

---

## 🔗 Related

- [Microsoft Defender for Cloud](https://learn.microsoft.com/en-us/azure/defender-for-cloud/)
- [NIST CSF Reference](https://www.nist.gov/cyberframework)
- [Azure Blob Storage Access Levels](https://learn.microsoft.com/en-us/azure/storage/blobs/anonymous-read-access-configure)

