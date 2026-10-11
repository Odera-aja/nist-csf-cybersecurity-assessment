# Evidence Register: Current-State Assessment Basis

This document lists every fact about Nexora Industries' current cyber security posture that the NIST CSF assessment is based on. Each observation has an **Evidence ID** (E01–E44). The assessment workbook references these IDs in the **Evidence Ref** column, so every Pass/Fail rating can be traced back to its source.

## Sources

| Source | Description |
|---|---|
| Current-state description | Written description of Nexora's cyber security team and controls, covering governance, assets, BCP/DR, vulnerability management, risk, third parties, IAM, network, physical security, data security, policy, detection & response and awareness |
| NIST CSF v1.1 | Framework subcategories (ID, PR, DE, RS, RC) used as the control baseline |

## How evidence was applied

- **Pass:** the evidence shows the control is in place and operating.
- **Fail:** the evidence shows the control is missing, or only partially implemented.
- **Fail by absence:** where the description gives no evidence that a control exists, it is rated Fail ("no evidence = not in place"). These controls are marked *No evidence (absence)* in the workbook and should be validated in stakeholder interviews.
- **N/A:** the evidence shows the control does not apply (for example no software development, see E08).
- **To confirm:** there is no evidence either way and an assumption would be unsafe.

## Team & Reporting Lines

| Role | Reports to | Observation |
|---|---|---|
| Cyber security analyst (generalist) | IT Manager | Responds to incidents as they arise (E01) |
| Network engineer | Network Team Leader | Manages firewalls (E02) |
| Cyber security consultant | IT Manager | New role; no executive-level cyber reporting line (E03) |

## Evidence Register


### Team & governance

| ID | Observation | Supports controls |
|---|---|---|
| **E01** | The cyber security team consists of one generalist analyst who handles incidents as they arise and reports to the IT manager. | DE.DP-1, RS.RP-1 |
| **E02** | A network engineer manages the firewalls and reports to the Network Team Leader. | DE.DP-1 |
| **E03** | The newly hired cyber security consultant also reports to the IT manager; cyber has no executive-level reporting line. | ID.GV-4, RC.CO-3 |
| **E04** | The CEO has a clear business strategy. | ID.BE-3 |
| **E05** | Cyber security roles and responsibilities are not defined; they are informally assigned to the IT team. | ID.AM-6, ID.GV-2, PR.AT-5 |
| **E06** | There is no cyber security strategy. | ID.GV-4 |

### Asset management

| ID | Observation | Supports controls |
|---|---|---|
| **E07** | IT keeps a spreadsheet of laptops with serial number, model and warranty details. | ID.AM-1 |
| **E08** | The organisation uses Microsoft 365 and relies exclusively on SaaS applications (no in-house software development). | ID.AM-2, ID.AM-4, PR.DS-7, PR.IP-2, PR.PT-3 |
| **E09** | All data is hosted in Microsoft Azure / Microsoft 365; there are no on-premise servers. | PR.DS-1, PR.DS-4, PR.MA-1, PR.MA-2 |
| **E10** | All laptops are imaged with a Secure Operating Environment (SOE) running the latest Windows version. | PR.IP-1 |

### BCP / DR

| ID | Observation | Supports controls |
|---|---|---|
| **E11** | IT conducts regular disaster recovery testing. | ID.BE-4, ID.BE-5, PR.DS-4, PR.IP-10, RC.RP-1, RC.IM-1, RC.IM-2 |
| **E12** | IT has clear, documented business continuity plans. | ID.BE-4, ID.BE-5, PR.DS-4, PR.IP-9, RC.CO-1, RC.CO-2, RC.CO-3 |
| **E13** | Regular backups are taken and tested periodically. | PR.IP-4 |

### Vulnerability management

| ID | Observation | Supports controls |
|---|---|---|
| **E14** | A Qualys vulnerability scanner has been purchased but is only used ad hoc. | ID.RA-1, PR.IP-12, DE.CM-8 |
| **E15** | There is no formal vulnerability management program. | ID.RA-1, ID.RA-2, PR.IP-12, RS.MI-3 |
| **E16** | Qualys reports a large number of high and severe vulnerabilities. | ID.RA-1, PR.IP-12 |

### Risk management

| ID | Observation | Supports controls |
|---|---|---|
| **E17** | A risk team exists but only performs financial risk activities. | ID.RA-4, ID.RM-1 |
| **E18** | There is no technology or cyber risk process. | ID.GV-4, ID.RA-3, ID.RA-4, ID.RA-5, ID.RA-6, ID.RM-1, ID.RM-2 |

### Third-party risk

| ID | Observation | Supports controls |
|---|---|---|
| **E19** | No third-party risk management is performed. | ID.AM-4, ID.BE-1, ID.BE-5, PR.AT-3, DE.CM-6 |
| **E20** | Contracts are reviewed by procurement and finance only, not by IT/security. | ID.GV-2, PR.AT-3, DE.CM-6 |

### Identity & access

| ID | Observation | Supports controls |
|---|---|---|
| **E21** | Microsoft Active Directory is used to manage users and groups. | PR.AC-1 |
| **E22** | There is no privileged access management (PAM) solution. | PR.AC-1, PR.AT-2 |
| **E23** | The admin account password is shared among several senior IT staff. | PR.AC-1, PR.AC-4, PR.AT-2 |
| **E24** | Access to resources is granted upon request. | PR.AC-4 |
| **E25** | Two-factor authentication is not used for login. | PR.AC-1, PR.AC-3 |
| **E26** | Complex login passwords are enforced. | PR.AC-1 |
| **E27** | Employees use a VPN for remote access when required. | PR.AC-3, PR.DS-2, PR.PT-4 |

### Network security

| ID | Observation | Supports controls |
|---|---|---|
| **E28** | Palo Alto next-generation firewalls are in place, configured by the network team. | PR.AC-5, PR.PT-3, PR.PT-4 |
| **E29** | Firewalls are audited every year by the network team. | PR.PT-4 |
| **E30** | Firewalls receive regular updates. | PR.PT-4 |
| **E31** | IT maintains up-to-date network diagrams that include the cloud environment. | ID.AM-3 |
| **E32** | The network is segmented using VLANs. | PR.AC-5, PR.PT-4 |

### Physical security

| ID | Observation | Supports controls |
|---|---|---|
| **E33** | The facility is highly secure with state-of-the-art CCTV coverage; physical security is taken very seriously. | PR.AC-2, PR.IP-5 |
| **E34** | Extensive vetting is performed for all employees. | PR.IP-11 |
| **E35** | Research labs and physical facilities are monitored 24/7. | PR.AC-2, PR.IP-5, DE.CM-2, DE.CM-3 |

### Data security

| ID | Observation | Supports controls |
|---|---|---|
| **E36** | There is no Data Loss Prevention (DLP) solution. | PR.DS-1, PR.DS-2, PR.DS-5, PR.PT-2 |
| **E37** | The key critical application is a SaaS service provided by Horizon Labs (fictional third party). | ID.AM-4, ID.BE-1, ID.BE-4, ID.BE-5 |

### Policy

| ID | Observation | Supports controls |
|---|---|---|
| **E38** | Only one generic IT policy exists. | ID.GV-1, PR.IP-7 |
| **E39** | There is no formal information security policy. | ID.AM-6, ID.GV-1, PR.IP-7 |
| **E40** | There are no data governance policies and no information classification. | ID.AM-5, ID.GV-3, PR.DS-1, PR.DS-2, PR.DS-3, PR.IP-6 |

### Detection & response

| ID | Observation | Supports controls |
|---|---|---|
| **E41** | There is no detection or incident response capability. | PR.IP-9, PR.IP-10, DE.AE-2, DE.AE-4, DE.AE-5, DE.DP-2, DE.DP-3, DE.DP-4, DE.DP-5, RS.RP-1, RS.CO-1, RS.CO-2, RS.CO-3, RS.CO-4, RS.CO-5, RS.AN-2, RS.AN-3, RS.AN-4, RS.MI-1, RS.MI-2, RS.IM-1, RS.IM-2 |
| **E42** | IT responds to alerts from the anti-virus (Microsoft Defender). | DE.AE-2, DE.CM-4, DE.CM-5, RS.AN-1 |
| **E43** | No SIEM is in place. | PR.PT-1, DE.AE-1, DE.AE-3, DE.CM-1, DE.CM-3 |

### Awareness

| ID | Observation | Supports controls |
|---|---|---|
| **E44** | All employees complete a one-off induction web module with basic cyber security instructions. | PR.AT-1, PR.AT-4 |

## Controls rated without direct evidence

These controls are not addressed in the current-state description. They were rated conservatively and must be validated with stakeholders:

- `ID.BE-2`
- `ID.RM-3`
- `PR.IP-3`
- `PR.IP-8`
- `DE.CM-7`

## Traceability example

| Control | Result | Evidence | Reasoning |
|---|---|---|---|
| PR.AC-1 Identities & credentials | Fail | E21, E22, E23, E25, E26 | AD and complex passwords exist (E21, E26), but there is no MFA (E25), no PAM (E22) and a shared admin password (E23) |
| PR.AC-5 Network integrity | Pass | E28, E32 | NGFW in place and the network segmented with VLANs |
| ID.BE-5 Resilience requirements | Fail | E11, E12, E19, E37 | BCP/DR exist and are tested internally, but there is no due diligence on the critical SaaS provider (E19, E37) |

<sub>All observations are paraphrased from a fictional case-study scenario.</sub>
