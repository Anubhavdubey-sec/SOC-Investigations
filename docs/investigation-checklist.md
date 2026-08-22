# SOC Investigation Checklist

Use this checklist when conducting a security investigation.

---

## 1. Alert Triage

- [ ] What triggered the alert?
- [ ] When did the activity occur?
- [ ] Which user is involved?
- [ ] Which host or system is involved?
- [ ] What source IP is involved?
- [ ] What destination is involved?
- [ ] Is the activity expected?

---

## 2. Initial Assessment

- [ ] Define the investigation problem.
- [ ] Record the initial hypothesis.
- [ ] Identify available data sources.
- [ ] Determine whether additional evidence is required.

---

## 3. Evidence Collection

- [ ] Authentication logs
- [ ] Windows Event Logs
- [ ] Sysmon
- [ ] Process execution
- [ ] PowerShell logs
- [ ] DNS logs
- [ ] Firewall logs
- [ ] Proxy logs
- [ ] Web server logs
- [ ] Email headers
- [ ] PCAP
- [ ] Endpoint telemetry
- [ ] SIEM alerts

---

## 4. Investigation

- [ ] Analyze relevant events.
- [ ] Search for related activity.
- [ ] Correlate multiple data sources.
- [ ] Identify unusual behavior.
- [ ] Test the initial hypothesis.
- [ ] Update the hypothesis when evidence changes.

---

## 5. Timeline

- [ ] Identify the first relevant event.
- [ ] Identify the sequence of events.
- [ ] Identify the most important event.
- [ ] Identify activity immediately before the incident.
- [ ] Identify activity immediately after the incident.

---

## 6. IOC Extraction

- [ ] IP addresses
- [ ] Domains
- [ ] URLs
- [ ] File hashes
- [ ] File names
- [ ] Email addresses
- [ ] User agents
- [ ] Processes
- [ ] Registry paths
- [ ] Other relevant indicators

---

## 7. Threat Intelligence

- [ ] Investigate suspicious IPs.
- [ ] Investigate suspicious domains.
- [ ] Investigate URLs.
- [ ] Investigate file hashes.
- [ ] Compare indicators with known malicious infrastructure.
- [ ] Record intelligence sources.
- [ ] Avoid relying on a single reputation source.

---

## 8. MITRE ATT&CK

- [ ] Identify attacker behavior.
- [ ] Map relevant tactics.
- [ ] Map techniques.
- [ ] Map sub-techniques where appropriate.
- [ ] Document evidence supporting each mapping.
- [ ] Assign mapping confidence.

---

## 9. Scope

- [ ] Identify affected users.
- [ ] Identify affected endpoints.
- [ ] Identify affected servers.
- [ ] Search for related indicators.
- [ ] Search for additional compromised accounts.
- [ ] Search for similar activity across the environment.

---

## 10. Severity

- [ ] Determine whether compromise occurred.
- [ ] Determine affected assets.
- [ ] Determine privilege level.
- [ ] Determine potential impact.
- [ ] Determine whether persistence exists.
- [ ] Determine whether lateral movement occurred.
- [ ] Assign severity.
- [ ] Document severity reasoning.

---

## 11. Verdict

- [ ] True Positive
- [ ] False Positive
- [ ] Benign / Expected Activity
- [ ] Inconclusive

Document the evidence supporting the final verdict.

---

## 12. Response

### Containment

- [ ] Account restriction/reset
- [ ] Endpoint isolation
- [ ] Block malicious infrastructure
- [ ] Quarantine malicious files

### Eradication

- [ ] Remove malicious files
- [ ] Remove persistence
- [ ] Remove compromised credentials
- [ ] Address exploited vulnerabilities

### Recovery

- [ ] Restore affected systems
- [ ] Validate security controls
- [ ] Monitor affected assets

---

## 13. Documentation

- [ ] Investigation notes completed
- [ ] Timeline completed
- [ ] IOCs documented
- [ ] MITRE ATT&CK mapping completed
- [ ] Severity documented
- [ ] Verdict documented
- [ ] Response recommendations documented
- [ ] Lessons learned documented
- [ ] References documented

---

# Final Quality Check

Before publishing an investigation, ask:

> **Can another analyst reproduce my reasoning from the evidence I documented?**

If the answer is no, the investigation is not finished.
