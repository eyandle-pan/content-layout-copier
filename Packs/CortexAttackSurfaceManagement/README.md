The **Cortex Attack Surface Management** pack is supported by Cortex Xpanse Expander and the ASM module for Cortex XSIAM.

Cortex Xpanse Expander and the ASM module for Cortex XSIAM are both best in class External Attack Surface Management solutions that strive to proactively reduce the frequency and severity of security incidents caused by internet-exposed risks. These solutions deliver comprehensive attack surface visibility by combining thorough, ML enhanced asset attribution with continuous attack surface assessment. Discovered risks are prioritized using contextual information and exploitability data, and findings are actioned on through curated automated playbooks to investigate, remediate, and summarize every new alert.

## What does this pack do?
This pack contains all of the integrations, automations, and playbooks necessary to fully automate the investigation, remediation, verification, and reporting on ASM risks within Cortex Xpanse Expander and XSIAM.

- Enriches services, assets, and alerts based on out-of-the-box integrations with sources like CMDBs, Cloud Service Providers, VM solutions, and more.
- Uses ML assisted analysis to identify critical context useful for analyst decision making.
- Keeps human analysts in the loop to direct the desired remediation action depending on the type of risk and discovered context.
- Includes automated notification and ticket creation workflows for delegating remediation tasks to the appropriate service owners.
- Includes full automated remediation options for automatically removing risky services from the public internet.
- Supports validation rescanning to ensure that remediation efforts have been applied successfully.
- Includes PDF reporting capabilities for preserving and communicating the investigation summary.

### Playbooks
- [Cortex ASM - ASM Alert](#cortex-asm---asm-alert)
- [Cortex ASM - Detect Service](#cortex-asm---detect-service)
- [Cortex ASM - Enrichment](#cortex-asm---enrichment)
- [Cortex ASM - Remediation Guidance](#cortex-asm---remediation-guidance)


### Cortex ASM - ASM Alert
Playbook that enriches asset information for ASM alerts and provides means of remediation.
![Cortex ASM - ASM Alert](https://raw.githubusercontent.com/demisto/content/d6d88d2066ef1f0868e8e61c5f20a71766f3cae1/Packs/CortexAttackSurfaceManagement/doc_files/Cortex_ASM_-_ASM_Alert.png)

#### Cortex ASM - Detect Service
Playbook that looks at what ASM sub-type the alert is and directs it to different pre/post mitigation scans (such as NMAP).
![Cortex ASM - Detect Service](https://raw.githubusercontent.com/demisto/content/d6d88d2066ef1f0868e8e61c5f20a71766f3cae1/Packs/CortexAttackSurfaceManagement/doc_files/Cortex_ASM_-_Detect_Service.png)

#### Cortex ASM - Enrichment
Playbook that is used as a container folder for all enrichments of ASM alerts.
![Cortex ASM - Enrichment](https://raw.githubusercontent.com/demisto/content/d6d88d2066ef1f0868e8e61c5f20a71766f3cae1/Packs/CortexAttackSurfaceManagement/doc_files/Cortex_ASM_-_Enrichment.png)

#### Cortex ASM - Remediation Guidance
Playbook that pulls remediation guidance off of a list based on ASM RuleID to be used in service owner notifications (email or ticketing system).
![Cortex ASM - Remediation Guidance](https://raw.githubusercontent.com/demisto/content/d474d924dd0e7ef7067b15764623804a24c8e1c8/Packs/CortexAttackSurfaceManagement/doc_files/Cortex_ASM_-_Remediation_Guidance.png)

### Automation Scripts
This content pack includes the [generateASMReport](#generateasmreport) script: 


#### GenerateASMReport
This automation helps generate an ASM alert summary report with important information found via the playbook run.
![GenerateASMReport](https://raw.githubusercontent.com/demisto/content/d6d88d2066ef1f0868e8e61c5f20a71766f3cae1/Packs/CortexAttackSurfaceManagement/doc_files/GenerateASMReport.png)
